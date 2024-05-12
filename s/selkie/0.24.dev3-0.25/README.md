# Comparing `tmp/selkie-0.24.dev3.tar.gz` & `tmp/selkie-0.25.tar.gz`

## Comparing `selkie-0.24.dev3.tar` & `selkie-0.25.tar`

### file list

```diff
@@ -1,38 +1,614 @@
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 selkie-0.24.dev3/dev/rom.ipynb
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 selkie-0.24.dev3/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 selkie-0.24.dev3/docs/make.bat
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 selkie-0.24.dev3/docs/source/conf.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 selkie-0.24.dev3/docs/source/index.rst
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 selkie-0.24.dev3/docs/source/corpus/index.rst
--rw-r--r--   0        0        0     7703 2020-02-02 00:00:00.000000 selkie-0.24.dev3/docs/source/corpus/rom.rst
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 selkie-0.24.dev3/docs/source/pyext/com.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 selkie-0.24.dev3/docs/source/pyext/data.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 selkie-0.24.dev3/docs/source/pyext/index.rst
--rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 selkie-0.24.dev3/docs/source/pyext/io.rst
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 selkie-0.24.dev3/docs/source/pyext/reflect.rst
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 selkie-0.24.dev3/docs/source/pyext/seq.rst
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 selkie-0.24.dev3/docs/source/pyext/string.rst
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 selkie-0.24.dev3/docs/source/pyext/xterm.rst
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/__init__.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/_config.py
--rw-r--r--   0        0        0    16710 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/com.py
--rw-r--r--   0        0        0    65205 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/io.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/reflect.py
--rw-r--r--   0        0        0    19232 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/rom.py
--rw-r--r--   0        0        0    14534 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/seq.py
--rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/string.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/xterm.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/data/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/data/examples/romtest.rom
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/data/roms/gothic-student.rom
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/data/roms/gothic.rom
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/data/roms/korean.rom
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/data/roms/otw-jones.rom
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/data/roms/otw-webkamigad.rom
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 selkie-0.24.dev3/src/selkie/data/roms/salish.rom
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 selkie-0.24.dev3/tests/Makefile
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 selkie-0.24.dev3/tests/run_tests.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 selkie-0.24.dev3/.gitignore
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 selkie-0.24.dev3/README.rst
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 selkie-0.24.dev3/pyproject.toml
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 selkie-0.24.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 selkie-0.25/.readthedocs.yaml
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 selkie-0.25/setup.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 selkie-0.25/utf8.txt
+-rw-r--r--   0        0        0     8890 2020-02-02 00:00:00.000000 selkie-0.25/dev/language_codes.ipynb
+-rw-r--r--   0        0        0    13413 2020-02-02 00:00:00.000000 selkie-0.25/dev/lazylist.ipynb
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 selkie-0.25/dev/rom.ipynb
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 selkie-0.25/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 selkie-0.25/docs/make.bat
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/conf.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/index.rst
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/requirements.txt
+-rw-r--r--   0        0        0    90260 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/app.fig1.jpeg
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/index.rst
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/mvmov.xml
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/corpus.rst
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/corpus_resources.rst
+-rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/export.rst
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/index.rst
+-rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/langdb.rst
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/language.rst
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/learn.rst
+-rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/lexicon.rst
+-rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/media.rst
+-rw-r--r--   0        0        0    11312 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/text.rst
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/token.rst
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/words.rst
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/index.rst
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/overview.rst
+-rw-r--r--   0        0        0    11526 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/content/elt.rst
+-rw-r--r--   0        0        0    10740 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/content/framework.rst
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/content/index.rst
+-rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/content/requests.rst
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/content/responses.rst
+-rw-r--r--   0        0        0    36559 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/db/database.rst
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/db/db_files.rst
+-rw-r--r--   0        0        0    16872 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/db/db_toplevel.rst
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/db/index.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/db/substrate.rst
+-rw-r--r--   0        0        0    27996 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/server/app_toplevel.rst
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/server/index.rst
+-rw-r--r--   0        0        0    23000 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/server/python_servers.rst
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/server/resources.rst
+-rw-r--r--   0        0        0    18025 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/server/sealapp.rst
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/server/server.rst
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/server/wsgi.rst
+-rw-r--r--   0        0        0    10962 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/js/PlainTextPanel.html
+-rw-r--r--   0        0        0    14838 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/js/XScript.html
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/pyext/config.rst
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/pyext/fs.rst
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/pyext/index.rst
+-rw-r--r--   0        0        0    43447 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/pyext/io.rst
+-rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/pyext/kvi.rst.ignore
+-rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/pyext/misc.rst
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/pyext/scripts.rst
+-rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/userguide/cgi.rst
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/userguide/index.rst
+-rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/userguide/intro.rst
+-rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/userguide/text.rst
+-rw-r--r--   0        0        0    31927 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/corpora.rst
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/data.rst
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/index.rst
+-rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/lexica.rst
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/wiktionary.rst
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/panlex/index.rst
+-rw-r--r--   0        0        0    28709 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/panlex/panlex2.rst
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/panlex/panlex_comline.rst
+-rw-r--r--   0        0        0    22026 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/panlex/panlex_intro.rst
+-rw-r--r--   0        0        0    11549 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/panlex/panlex_module.rst
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/index.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/conc.rst
+-rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/corpus.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/index.rst
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/rom/gothic-student.html
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/rom/gothic-student.rhtm
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/rom/gothic.html
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/rom/gothic.rhtm
+-rw-r--r--   0        0        0     8946 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/rom/index.rst
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/server/disk.rst
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/server/index.rst
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/server/intro.rst
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/server/store.rst
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/server/webserver.rst
+-rw-r--r--   0        0        0    17089 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/figs/fig9.jpg
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/intro/index.rst
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/intro/langdig.rst
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/intro/overview.rst
+-rw-r--r--   0        0        0    15174 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/bot.rst
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/chartparser.rst
+-rw-r--r--   0        0        0    20110 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dep.rst
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/expr.rst
+-rw-r--r--   0        0        0    31295 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/fsa.rst
+-rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/fst.rst
+-rw-r--r--   0        0        0    43843 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/glab.rst
+-rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/head.rst
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/index.rst
+-rw-r--r--   0        0        0    19125 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/interp.rst
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/interpreter.rst
+-rw-r--r--   0        0        0    24103 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/logic.rst
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/morph.rst
+-rw-r--r--   0        0        0    11912 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/parser.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/preproc.rst
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/pretts.rst
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/stemmer.rst
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/textgrid.rst
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/tok.rst
+-rw-r--r--   0        0        0    31625 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/tree.rst
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/eval.rst
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/features.rst
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/index.rst
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/mst.rst
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/nivre.rst
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/nnproj.rst
+-rw-r--r--   0        0        0    22915 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/parser.rst
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/ml/cluster.rst
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/ml/index.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/ml/mat.tex
+-rw-r--r--   0        0        0     6917 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/ml/prob.tex
+-rw-r--r--   0        0        0    12746 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/grammar/avs.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/grammar/eng.rst
+-rw-r--r--   0        0        0    13946 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/grammar/features.rst
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/grammar/gdev.rst
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/grammar/grammar.rst
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/grammar/index.rst
+-rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/com.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/data.rst
+-rw-r--r--   0        0        0    20329 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/formats.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/index.rst
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/io.rst
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/persist.rst
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/reflect.rst
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/seq.rst
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/string.rst
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/table.rst
+-rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/xml.rst
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/xterm.rst
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/utf8.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/__init__.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/abspath.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/auth.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/char.py
+-rw-r--r--   0        0        0    12649 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/dependencies.py
+-rw-r--r--   0        0        0    14840 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/doc.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/doctest.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/glab.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/manifest.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/panlex.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/__init__.py
+-rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/__main__.py
+-rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/config.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/core.py
+-rw-r--r--   0        0        0    20739 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/toplevel.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/__init__.py
+-rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/app-scraps.py.disabled
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/app_scraps.py.disabled
+-rw-r--r--   0        0        0    21962 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/auth.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/cgi.py
+-rw-r--r--   0        0        0    12806 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/client.py
+-rw-r--r--   0        0        0    16886 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/config.py
+-rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/core.py
+-rw-r--r--   0        0        0    11311 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/dualserver.py
+-rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/dualserver_full.py
+-rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/env.py
+-rw-r--r--   0        0        0    14359 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/handler.py
+-rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/handler_orig.py.ignore
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/html.py
+-rw-r--r--   0        0        0    14451 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/item.py
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/log.py
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/parse.py
+-rw-r--r--   0        0        0    11577 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/request.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/resources.py
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/response.py
+-rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/server.py
+-rw-r--r--   0        0        0    10167 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/server2_old.py
+-rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/server_old.py
+-rw-r--r--   0        0        0    14248 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/session.py.disabled
+-rw-r--r--   0        0        0    27457 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/toplevel.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/ui-scraps.py
+-rw-r--r--   0        0        0    47958 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/ui.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/ui_scraps.py.disabled
+-rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/weblib.py
+-rw-r--r--   0        0        0    10716 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/wsgi.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/__init__.py
+-rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/audio.py.todelete
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/core.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/course.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/drill.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/env.py
+-rw-r--r--   0        0        0    31570 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/export.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/export_file.py
+-rw-r--r--   0        0        0    15330 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/langdb.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/language.py
+-rw-r--r--   0        0        0    22626 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/lexicon.py
+-rw-r--r--   0        0        0     9639 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/media.py
+-rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/rom.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/sim.py
+-rw-r--r--   0        0        0     9117 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/text.py
+-rw-r--r--   0        0        0    35404 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/token-new.py.disabled
+-rw-r--r--   0        0        0    34350 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/token.py
+-rw-r--r--   0        0        0    11795 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/transcript.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/user.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/core.py
+-rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/dir.py
+-rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/disk.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/env.py
+-rw-r--r--   0        0        0    24305 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/file.py
+-rw-r--r--   0        0        0    15014 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/meta.py
+-rw-r--r--   0        0        0    15588 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/permissions.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/glab/__init__.py
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/glab/eval.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/glab/file.py
+-rw-r--r--   0        0        0    58024 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/glab/functions.py
+-rw-r--r--   0        0        0    17038 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/glab/lang.py
+-rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/glab/ui.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/seal/config.py
+-rw-r--r--   0        0        0    70509 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/seal/io.py
+-rw-r--r--   0        0        0    57270 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/seal/misc.py
+-rw-r--r--   0        0        0    18126 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/seal/rom.py
+-rw-r--r--   0        0        0    10090 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/seal/sh.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/seal/version.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/seal/xterm.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/__init__.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/audio.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/conc.py
+-rw-r--r--   0        0        0    16981 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/corpus.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/course.py
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/file.py
+-rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/igt.py
+-rw-r--r--   0        0        0    12708 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/language.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/lexicon.py
+-rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/media.py
+-rw-r--r--   0        0        0    13156 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/page.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/rom.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/text.py
+-rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/toc.py
+-rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/users.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/video.py
+-rw-r--r--   0        0        0    28573 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/__init__.py
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/drill.py
+-rw-r--r--   0        0        0    15440 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/langs.py
+-rw-r--r--   0        0        0    21939 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/lgc21.py
+-rw-r--r--   0        0        0    28476 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/lgc22.py
+-rw-r--r--   0        0        0    20075 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/rom.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/romfile.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/user.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/Makefile
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/__init__.py
+-rw-r--r--   0        0        0    10159 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/bionlp.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/brown.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/census.py
+-rw-r--r--   0        0        0    26282 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/dep.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/idp.py
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/make_seal_info
+-rw-r--r--   0        0        0    13736 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/panlex.py
+-rw-r--r--   0        0        0    26108 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/panlex_old.py
+-rw-r--r--   0        0        0    19693 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/panlex_scraps.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/perseus.py
+-rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/propbank.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/ptb-rest.py.disabled
+-rw-r--r--   0        0        0    12582 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/ptb.py
+-rw-r--r--   0        0        0    27553 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/udt.py
+-rw-r--r--   0        0        0    21353 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/wiktionary.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/wn.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/census/README
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/census/both
+-rw-r--r--   0        0        0  3107965 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/census/dist.all.last
+-rw-r--r--   0        0        0   149625 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/census/dist.female.first
+-rw-r--r--   0        0        0    42665 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/census/dist.male.first
+-rw-r--r--   0        0        0    10702 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/census/methodology.txt
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/README
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/README.seal
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/ar-padt.map
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/bg-btb.map
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/ca-cat3lb.map
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/cs-pdt.map
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/da-ddt.map
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/de-negra.map
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/de-tiger.map
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/el-gdt.map
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/en-brown.map
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/en-ptb.map
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/en-tweet.README
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/en-tweet.map
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/es-cast3lb.map
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/eu-eus3lb.map
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/fi-tdt.map
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/fr-paris.map
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/hu-szeged.map
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/it-isst.map
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/iw-mila.map
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/ja-kyoto.map
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/ja-verbmobil.map
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/ko-sejong.map
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/nl-alpino.map
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/pl-ipipan.map
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/pt-bosque.map
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/ru-rnc.map
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/sl-sdt.map
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/sv-talbanken.map
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/tu-metusbanci.map
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/universal_tags.py.ignore
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/zh-ctb6.map
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/zh-sinica.map
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/eng.g
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/eng.sents
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/main.decl
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/main.g
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/main.lex
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/num.decl
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/num.g
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/num.lex
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/EXAMPLES
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/Makefile
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/apptest.cfg
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/bad.html
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/ca.info
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/ca.pass
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/cfgfile
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/class1.arff
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/class2.test
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/class2.train
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/class3.test
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/class3.train
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/cnf.expr
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/coder1
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp1.ef
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp2.ef
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp2.ef.1
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp2.ef.2
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/crime.kb
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/curiosity.kb
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/depsent1
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/depsent2
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/depsent3_gold
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/depsent3_pred
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/deu.g
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/docs.mat
+-rw-r--r--   0        0        0     9239 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/dream
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/drill.txt
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/fg0
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/form.html
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/fsa1
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/fsa2
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/fsa3
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/fsa4
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/fst1
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g1
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g1.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g1a.g
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g2
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g3
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g4.g
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g4.lex
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g4.test
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g5.g
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g5.lex
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g5.test
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g6.g
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g6.lex
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g6.test
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g7.g
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g7.lex
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g7.test
+-rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g8.g
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g8.labels
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g8.sents
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g9.g
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g9.sents
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/intro.html
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/intro.tex
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/lex1
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/lex2
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/lex3
+-rw-r--r--   0        0        0   249612 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/libsvm-1.test
+-rw-r--r--   0        0        0   192782 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/libsvm-1.train
+-rw-r--r--   0        0        0   165698 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/libsvm-2.train
+-rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/libsvm-3.test
+-rw-r--r--   0        0        0   305582 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/libsvm-3.train
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/lisp1.lisp
+-rwxr-xr-x   0        0        0      749 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/make_repo_example
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/make_utf8.py.ignore
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/nivre-2007.ftrs
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/nivre.exp
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/normpointers.txt
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/northwind.TextGrid
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/notebook.gl
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/notebook2.gl
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/notebook3.gl
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/notebook_test.gl
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/notebook_test.output
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/par1.txt
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/ptb.abb
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/ptb.g
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/ptb.lex
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/ptb.test
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/romtest.rom
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/s1.snt
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sec_3
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sec_4
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sec_5
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sec_6
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sec_7
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sem.g
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sem.lex
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/server.info
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/server.pass
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg0
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg0.defs
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg0.g
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg0.lex
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg0a.g
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg1a.g
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg2.defs
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg2.g
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg2.lex
+-rw-r--r--   0        0        0    11651 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg2a.g
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg3.defs
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg3.g
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg3.lex
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/t1
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/t2
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tab1.tab
+-rwxr-xr-x   0        0        0      330 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/test.cgi
+-rw-r--r--   0        0        0    31700 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/test123.mp3
+-rwxr-xr-x   0        0        0   404992 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/test123.wav
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/testfiles
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/testinclude.gl
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/text1
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/text1.utf8
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tinygen.g
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tok1
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tree1
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tree2
+-rw-r--r--   0        0        0   796908 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tuebingen.m4a
+-rw-r--r--   0        0        0   409461 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tuebingen.mp3
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tuebingen.txt
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/upload.html
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/utf8.txt
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/xml1
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp22.lgc/toc
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp22.lgc/deu.lg/2.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp22.lgc/deu.lg/3.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp22.lgc/deu.lg/toc
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp23.lgc/corpus
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp23.lgc/deu/2.txt
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp23.lgc/deu/3.txt
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp23.lgc/deu/lang
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp25.lgc/langs
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp25.lgc/deu/toc
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp25.lgc/deu/txt/2
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp25.lgc/deu/txt/3
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corpus.cld/langs/eng/texts/1/orig
+-rw-r--r--   0        0        0    38333 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corpus.cld/langs/otw/lexicon
+-rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corpus.cld/langs/otw/texts/16/audio/clips
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corpus.cld/langs/otw/texts/16/audio/transcript
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/Database.hdr
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/index.tab
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/abney/arapesh/104.txt
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/arapesh/100.txt
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/arapesh/101.txt
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/arapesh/102.txt
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/arapesh/103.txt
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/arapesh/104.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/kutenai/18.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/kutenai/19.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/kutenai/20.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/kutenai/21.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/kutenai/22.txt
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/cards/index.hdr
+-rw-r--r--   0        0        0    20056 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/cards/index.tab
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/igt/117
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/index.hdr
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/index.tab
+-rw-r--r--   0        0        0    10116 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/ape/13.txt
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/deu/1.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/deu/11.lex
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/deu/2.snt
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/deu/2.spn
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/deu/3.snt
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/10.snt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/12.lex
+-rw-r--r--   0        0        0   204790 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/15.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/16.spn
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/4.txt
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/5.snt
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/6.tok
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/7.snt
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/8.txt
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/9.snt
+-rw-r--r--   0        0        0    12063 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/sat/14.txt
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/langs/index.hdr
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/langs/index.tab
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/index.hdr
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/index.tab
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/111/100
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/111/101
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/111/102
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/111/103
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/111/104
+-rw-r--r--   0        0        0    25355 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/111/info
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/99/18
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/99/19
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/99/20
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/99/21
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/99/22
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/users/index.hdr
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/users/index.tab
+-rw-r--r--   0        0        0    15532 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/iso/639-2.txt
+-rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/iso/639-5.txt
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/iso/639-3/iso-639-3-macrolanguages_20170131.tab
+-rw-r--r--   0        0        0   184065 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/iso/639-3/iso-639-3_20170202.tab
+-rw-r--r--   0        0        0   206914 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/iso/639-3/iso-639-3_Name_Index_20170217.tab
+-rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/iso/639-3/iso-639-3_Retirements_20170131.tab
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/roms/gothic-student.rom
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/roms/gothic.rom
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/roms/korean.rom
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/roms/otw-jones.rom
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/roms/otw-webkamigad.rom
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/roms/salish.rom
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/abbreviations
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/archive.gif
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/cog.png
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/entities.txt
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/external.gif
+-rw-r--r--   0        0        0    11795 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/fourletter.txt
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/headrules_main.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/headrules_np.txt
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/original_headrules_main.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/original_headrules_np.txt
+-rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/ptb_filenames
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/seal.info
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/standard.rmg
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/stemmer_stems
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/stemmer_words
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/__init__.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/eval.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/features.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/mst.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/nivre.py
+-rw-r--r--   0        0        0    11113 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/nnproj.py
+-rw-r--r--   0        0        0    15832 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/parser.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/tree.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/__init__.py
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/cluster.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/experiment.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/instance.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/libsvm.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/mat.py
+-rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/num.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/prob.py
+-rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/split.py
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/sym.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/editor/webserver.py
+-rw-r--r--   0        0        0    25338 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/avs.py
+-rw-r--r--   0        0        0    10713 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/bot.py
+-rw-r--r--   0        0        0    38502 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/com.py
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/conc.py
+-rw-r--r--   0        0        0    22515 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/dep.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/eng.py
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/expr.py
+-rw-r--r--   0        0        0    15836 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/features.py
+-rw-r--r--   0        0        0    21557 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/fsa.py
+-rw-r--r--   0        0        0    15430 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/fst.py
+-rw-r--r--   0        0        0    17385 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/gdev.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/gen.py
+-rw-r--r--   0        0        0    20833 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/grammar.py
+-rw-r--r--   0        0        0    12151 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/head.py
+-rw-r--r--   0        0        0    14416 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/interp.py
+-rw-r--r--   0        0        0    80152 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/io.py
+-rw-r--r--   0        0        0    23405 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/logic.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/map.py
+-rw-r--r--   0        0        0    15359 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/parser.py
+-rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/pretts.py
+-rw-r--r--   0        0        0    11121 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/seq.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/stemmer.py
+-rw-r--r--   0        0        0    11934 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/string.py
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/textgrid.py
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/tok.py
+-rw-r--r--   0        0        0    30483 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/tree.py
+-rw-r--r--   0        0        0    25353 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/avs.py
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/expr.py
+-rw-r--r--   0        0        0    15901 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/features.py
+-rw-r--r--   0        0        0    15805 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/gdev.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/glab.py
+-rw-r--r--   0        0        0    21099 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/grammar.py
+-rw-r--r--   0        0        0    15411 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/parser.py
+-rw-r--r--   0        0        0    30353 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/tree.py
+-rw-r--r--   0        0        0    16989 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/com.py
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/disk.py
+-rw-r--r--   0        0        0    17346 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/formats.py
+-rw-r--r--   0        0        0    46908 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/io.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/ipynb.py
+-rw-r--r--   0        0        0    15507 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/manifest.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/object.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/persist.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/reflect.py
+-rw-r--r--   0        0        0    15569 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/seq.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/store.py
+-rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/string.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/table.py
+-rw-r--r--   0        0        0    21059 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/xml.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/xterm.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 selkie-0.25/tests/Makefile
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 selkie-0.25/tests/checkdist.py
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 selkie-0.25/tests/run_tests.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 selkie-0.25/tests/test_bot.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 selkie-0.25/tests/test_rom.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 selkie-0.25/tests/test_rom_graph
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 selkie-0.25/.gitignore
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 selkie-0.25/README.rst
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 selkie-0.25/pyproject.toml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 selkie-0.25/PKG-INFO
```

### Comparing `selkie-0.24.dev3/dev/rom.ipynb` & `selkie-0.25/dev/rom.ipynb`

 * *Files identical despite different names*

### Comparing `selkie-0.24.dev3/docs/Makefile` & `selkie-0.25/docs/Makefile`

 * *Files identical despite different names*

### Comparing `selkie-0.24.dev3/docs/make.bat` & `selkie-0.25/docs/make.bat`

 * *Files identical despite different names*

### Comparing `selkie-0.24.dev3/docs/source/conf.py` & `selkie-0.25/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 # -- Project information
 
 project = 'Selkie'
 copyright = '2022, University of Michigan'
 author = 'Steven Abney'
 
-release = '0.1'
-version = '0.1.0'
+# release: x.y, version: x.y.z
+release = '0.25'
+version = '0.25.0'
 
 # -- General configuration
 
 extensions = [
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
     'sphinx.ext.autodoc',
@@ -32,7 +33,8 @@
 
 # -- Options for HTML output
 
 html_theme = 'sphinx_rtd_theme'
 
 # -- Options for EPUB output
 epub_show_urls = 'footnote'
+
```

### Comparing `selkie-0.24.dev3/docs/source/corpus/rom.rst` & `selkie-0.25/docs/source/editor/corpus/rom/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 
-``selkie.rom`` — Romanizations
-==============================
+.. automodule:: selkie.corpus.rom
+
+Romanizations — ``selkie.corpus.rom``
+=====================================
 
 Definition
 ----------
 
 A **romanization** defines ASCII key sequences for entering
 non-ASCII characters.  It can be thought of as a keyboard for entering
 a non-roman script, or as an orthography.
@@ -31,40 +33,44 @@
 reverse mappings are not currently provided.
 
 The romanizations currently defined are: ``'gothic'``, ``'gothic-student'``,
 and ``'salish'``.
 They are enabled when seal.nlp.rom is imported.
 One uses them as one uses any decoder.  For example:
 
->>> import selkie.rom
+>>> import selkie.corpus.rom
 >>> s = b'c*a'.decode('salish')
->>> from selkie.string import unidescribe
+>>> from selkie.pyx.string import unidescribe
 >>> unidescribe(s)
 0 0x10d LATIN SMALL LETTER C WITH CARON
 1 0x61 LATIN SMALL LETTER A
 
 The string prints out as "ča."
 
 There is also a ``decode()`` function:
 
->>> from selkie.rom import decode
+>>> from selkie.corpus.rom import decode
 >>> s2 = decode("a'tho:", 'gothic-student')
 >>> unidescribe(s2)
 0 0xe1 LATIN SMALL LETTER A WITH ACUTE
 1 0xfe LATIN SMALL LETTER THORN
 2 0x6f LATIN SMALL LETTER O
 3 0x304 COMBINING MACRON
 
 To convert the output to an ascii string containing HTML entities of
 form ``&#dddd;`` for non-ascii characters:
 
->>> from selkie.rom import to_html
+>>> from selkie.corpus.rom import to_html
 >>> to_html(s2)
 b'&#225;&#254;o&#772;'
 
+To see the graph::
+
+   >>> student.print_graph() # doctest: +SKIP
+
 Decoder
 -------
 
 A Decoder applies a romanization.  It is similar to the reader
 for a codec, but it maps text to text, not bytes to text.
 
 The romanization behaves as a dict mapping strings to strings.  It is
@@ -151,27 +157,137 @@
 force all pending output to be produced by calling ``flush()``.
 
 Catalog
 -------
 
 To get a list of the defined romanizations:
 
->>> from selkie.rom import default_registry
->>> list(default_registry)
-['korean', 'otw-webkamigad', 'salish', 'gothic', 'gothic-student', 'otw-jones']
+>>> from selkie.corpus.rom import default_registry
+>>> default_registry.reset()
+>>> sorted(default_registry)
+['gothic', 'gothic-student', 'korean', 'otw-jones', 'otw-webkamigad', 'salish']
 
 To get the romanization itself, access the registry like a dict:
 
 >>> salish = default_registry['salish']
 
 The file in which the romanization resides is ``salish.filename``.
 Calling ``print(salish)`` prints its contents.  One can also use
 ``salish.items()`` to get an iteration over the pairs, and
 ``salish.print_graph()`` to see the finite-state graph.
 
+Gothic
+......
+
+Here are the contents of the 'gothic' romanization:
+
+.. list-table::
+
+   * - a
+     - 𐌰
+   * - b
+     - 𐌱
+   * - g
+     - 𐌲
+   * - d
+     - 𐌳
+   * - e
+     - 𐌴
+   * - q
+     - 𐌵
+   * - z
+     - 𐌶
+   * - h
+     - 𐌷
+   * - th
+     - 𐌸
+   * - i
+     - 𐌹
+   * - k
+     - 𐌺
+   * - l
+     - 𐌻
+   * - m
+     - 𐌼
+   * - n
+     - 𐌽
+   * - j
+     - 𐌾
+   * - u
+     - 𐌿
+   * - p
+     - 𐍀
+   * - 90
+     - 𐍁
+   * - r
+     - 𐍂
+   * - s
+     - 𐍃
+   * - t
+     - 𐍄
+   * - w
+     - 𐍅
+   * - f
+     - 𐍆
+   * - x
+     - 𐍇
+   * - hv
+     - 𐍈
+   * - o
+     - 𐍉
+   * - 900
+     - 𐍊
+
+Here are the contents of 'gothic-student':
+
+.. list-table::
+
+   * - A:
+     - Ā
+   * - E:
+     - Ē
+   * - O:
+     - Ō
+   * - U:
+     - Ū
+   * - A'
+     - Á
+   * - I'
+     - Í
+   * - U'
+     - Ú
+   * - A:'
+     - Ā́
+   * - I:'
+     - Ī́
+   * - U:'
+     - Ū́
+   * - a:
+     - ā
+   * - e:
+     - ē
+   * - o:
+     - ō
+   * - u:
+     - ū
+   * - a'
+     - á
+   * - i'
+     - í
+   * - u'
+     - ú
+   * - a:'
+     - ā́
+   * - i:'
+     - ī́
+   * - u:'
+     - ū́
+   * - th
+     - þ
+
 Defining a new romanization
 ---------------------------
 
 Here is an example of a romanization definition::
 
     a'	\(00e1)
     N	\(004b)
@@ -183,22 +299,18 @@
 
 If the preceding is the contents of ``romtest.rom`` in the current
 directory, it is immediately available as encoding ``romtest``.  If it resides in directory
 DIR, one may make it available by adding DIR to the default registry's
 path:
 
 >>> import selkie
->>> from os.path import join
->>> srcdir = selkie.__file__[:-len('/__init__.py')]
->>> examples = join(srcdir, 'data', 'examples')
->>> default_registry.path[0:1] = [examples]
+>>> default_registry.path.insert(0, selkie.data.path('examples'))
 >>> b"l-a'L-e ?u".decode('romtest')
 'ɬáƛe ˁu'
 
-
 API
 ---
 
 .. py:function:: load_rom(fn)
 
    Opens the file in binary mode.  Returns an iteration over (key,
    value) pairs.  The values are not expanded.
```

### Comparing `selkie-0.24.dev3/docs/source/pyext/string.rst` & `selkie-0.25/docs/source/pyx/io.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 
-``selkie.string`` — Strings
-===========================
+Input/output — ``selkie.pyx.io``
+================================
 
-.. automodule:: selkie.string
+.. automodule:: selkie.pyx.io
 
-General functionality
----------------------
+Filename suffixes
+-----------------
 
-.. autofunction:: unidescribe
-.. autofunction:: isword
-.. autofunction:: lines
+.. autofunction:: ispathlike
+.. autofunction:: strip_suffix
+.. autofunction:: split_suffix
+.. autofunction:: get_suffix
 
-Conversion to ASCII
--------------------
+Syntax
+------
 
-.. autofunction:: as_ascii
-.. autofunction:: from_ascii
-.. autofunction:: quoted
-.. autofunction:: deaccent
+.. autoclass:: Token
+.. autoclass:: Syntax
 
-Formatting dates/times and sizes
---------------------------------
+Special streams
+---------------
 
-.. autofunction:: dtstr
-.. autofunction:: sizestr
-.. autofunction:: elapsed_time_str
-.. autofunction:: timestr
+.. function:: pprint(*strs)
+.. autofunction:: tabular
 
-Expand environment variables
-----------------------------
-
-.. autofunction:: expand_envvars
+.. py:function:: redirect()
 
+   Example::
+   
+      with redirect() as s:
+          pprint('foo')
+          with pprint.indent():
+              pprint('bar')
+          return str(s)
 
+.. autoclass:: BackingSave
```

### Comparing `selkie-0.24.dev3/src/selkie/com.py` & `selkie-0.25/src/selkie/pyx/com.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 '''
 The selkie.com module contains functionality related to command-line processing,
 as well as system commands.
 '''
 
 import sys, subprocess
 from time import time
+from io import StringIO
 from .string import elapsed_time_str
 
 
 #--  file_size  ----------------------------------------------------------------
 
 def file_size (fn):
     '''
@@ -25,17 +26,19 @@
     return urllib.request.urlretrieve(url)[0]
 
 
 #--  System calls  -------------------------------------------------------------
 
 def system (*args, silent=False):
     '''
-    Runs a command line represented as separate words.
-    Returns True on success, False on failure.
-    Keyword argument silent=True suppresses any printout.
+    Execute a system command line.  Unless silent=True is specified,
+    the output is printed to stdout.  The return value is True if the
+    command executes successfully and False if not.  Example::
+
+        system('ls', '-l')
     '''
     return True if subprocess.run(args, capture_output=silent).returncode == 0 else False
 
 def backtick (*args):
     '''
     Runs a command line represented as separated words.
     Returns the printed output, as a string.
@@ -482,64 +485,69 @@
 class Progress (object):
     '''
     A progress monitor.
     '''
 
     ##  Constructor.
 
-    def __init__ (self, n=None):
+    def __init__ (self, n=None, file=sys.stderr):
 
         ##  How many ticks are expected in total.  It's OK if it's an underestimate.
         self.target = n
 
         ##  How many ticks have already taken place.
         self.count = 0
 
         ##  To keep track of elapsed time.
         self.timer = Timer()
 
         self.last_t = None
+        self.file = file
 
     def __enter__ (self):
         return self
 
     def done (self):
-        self.printout(end='\n')
+        self.printout(end='\n', file=self.file)
 
     def __exit__ (self, t, v, tb):
         self.done()
 
     ##  Increment by n ticks (default 1).  Prints/updates a progress message.
 
     def __iadd__ (self, n=1):
         self.count += n
         t = time()
         if self.last_t is None or t - self.last_t > 0.3:
             self.last_t = t
-            self.printout()
+            self.printout(file=self.file)
         return self
 
-    def printout (self, end=' '):
+    def printout (self, end=' ', file=sys.stderr):
         if self.target is None:
             print('\rProgress: %d' % self.count,
                   'Time elapsed: %s' % self.timer,
                   end=end,
-                  file=sys.stderr)
-            sys.stderr.flush()
+                  file=file)
+            file.flush()
 
         else:
             proportion_done = self.count/float(self.target)
             elapsed = self.timer.elapsed()
             est_total = elapsed/proportion_done
             print('\rProgress: %d/%d (%2.2f%%)' % (self.count, self.target, 100 * proportion_done),
                   'Time remaining: %s' % elapsed_time_str(elapsed, est_total),
                   end=end,
-                  file=sys.stderr)
-            sys.stderr.flush()
+                  file=file)
+            file.flush()
 
+    def __str__ (self):
+        with StringIO() as f:
+            self.printout(file=f)
+            return f.getvalue()
 
 
 #--  Manifest  -----------------------------------------------------------------
 #
 #  A manifest is a listing of the files in a directory tree.  The entries are of
 #  form:
 #
```

### Comparing `selkie-0.24.dev3/src/selkie/io.py` & `selkie-0.25/src/selkie/cld/seal/io.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,136 @@
-'''
-The io module contains input and output streams.
-'''
-
-try:
-    from fcntl import flock, LOCK_EX, LOCK_UN
-except:
-    flock = LOCK_EX = LOCK_UN = None
-
-import sys, os, re, urllib, urllib.request, urllib.parse, urllib.error, \
-    codecs, shutil, subprocess, stat, threading, datetime, random, \
-    json
+##  @package seal.core.io
+#   The io module contains input and output streams.
+
+
+import sys, os, re, urllib.request, urllib.parse, urllib.error, \
+    codecs, shutil, subprocess, stat, threading, datetime, random
 from glob import glob
 from io import StringIO, TextIOBase
-from os.path import exists, expanduser
-from pathlib import Path
-from collections import namedtuple
-from .seq import as_list, MapProxy, ListProxy
-from .string import as_ascii
+from fcntl import flock, LOCK_EX, LOCK_UN
+from .misc import as_list, as_ascii, file_size
 from .xterm import fg
 
+_open = __builtins__['open']
+
+
+##  Passes '-' through unchanged; otherwise dispatches to os.path.abspath().
+
+def abspath (fn):
+    if fn == '-':
+        return fn
+    else:
+        return os.path.abspath(os.path.expanduser(fn))
+
+
+#--  srepr  --------------------------------------------------------------------
+
+##  'Stable' repr, for use with doctest.
+#   E.g., prints out the keys of a dict or members of a set in sort order.
+
+def srepr (x):
+    if isinstance(x, dict):
+        pairs = ['%s: %s' % (repr(k), srepr(v))
+                 for (k,v) in sorted(x.items())]
+        return '{' + ', '.join(pairs) + '}'
+
+    elif isinstance(x, set):
+        elts = [srepr(e) for e in sorted(x)]
+        return '{' + ', '.join(elts) + '}'
+
+    else:
+        return repr(x)
+
+
+#--  Contents  -----------------------------------------------------------------
 
-def ispathlike (x):
-    return isinstance(x, str) or hasattr(x, '__fspath__')
+##  The contents of a file, as a string.
+
+def contents (filename, encoding=None):
+    return infile(filename, encoding).read()
+
+
+#--  Tee  ----------------------------------------------------------------------
+
+##  A tee.  Splits a stream into one going to a file and an identical copy going
+#   to stdout.
+
+class tee (object):
+
+    ##  Constructor.
+
+    def __init__ (self, filename):
+
+        ##  The filename being written.
+        self.filename = filename
+
+        ##  The output stream to the file.
+        self.stream = _open(filename, 'w')
+
+    ##  Writes the given string both to the output stream and to stdout.
+
+    def write (self, x):
+        self.stream.write(x)
+        sys.stdout.write(x)
+
+    ##  Closes the output stream.
+
+    def close (self):
+        self.stream.close()
+        self.stream = None
+    
+
+#--  NullStream  ---------------------------------------------------------------
+
+##  A fake stream.
+
+class NullStream (object):
+    
+    ##  No-op.
+
+    def write (self, s):
+        pass
+
+##  An instance of NullStream.
+null = NullStream()
+
+
+#--  Output List  --------------------------------------------------------------
+
+##  A specialization of list that behaves like an output stream.
+#   Specifically, it provides a write() method.  Writing to it appends lines;
+#   the final result is a list of lines.  The lines do not include carriage returns
+#   and newlines.
+
+class OutputList (list):
+
+    ##  Constructor.
+
+    def __init__ (self):
+
+        ##  A partial line, still waiting for the newline.
+        self.partial = None
+
+    ##  Write a string.  If the string ends in carriage return and/or newline,
+    #   it completes a line.  Append it to the list and clear the partial member.
+    #   Otherwise, concatenate it to the partial member and wait.
+    #   Caution: does not handled embedded newlines.
+
+    def write (self, s):
+        eol = False
+        if s and s[-1] in '\r\n':
+            eol = True
+            s = s.rstrip('\r\n')
+        if self.partial:
+            self.partial += s
+        else:
+            self.partial = s
+        if eol:
+            self.append(self.partial)
+            self.partial = None
 
 
 #--  Suffixes  -----------------------------------------------------------------
 
 ##  A suffix begins with the final period, provided that it occurs in the final
 #   pathname component.  Returns the pathname sans suffix.
 
@@ -51,57 +156,706 @@
     i = fn.rfind('.')
     if i > 0 and '/' not in fn[i+1:]:
         return fn[i+1:]
     else:
         return ''
 
 
+#--  Fn  -----------------------------------------------------------------------
 
-#--  Tokens  -------------------------------------------------------------------
+##  The only purpose of this object is so that we can distinguish by type
+#   between a filename and the contents of a file.
 
-##  A token.
+class Contents (object):
 
-class Token (str):
+    ##  Constructor.
 
-    ##  True if type is 'any' or equals the token's type.
-    def hastype (self, type):
-        if type == 'any': return self.type != 'eof'
-        else: return type == self.type
+    def __init__ (self, s):
 
-    ##  Raise an exception, indicating file, line, and offset.
-    def error (self, msg='syntax error'):
-        raise Exception('[%s line %d char %d] %s' % \
-            (self.filename, self.line, self.offset, msg))
+        ##  The string.
+        self.contents = s
 
-    ##  Print a warning, indicating file, line, and offset.
-    def warn (self, msg):
-        sys.stderr.write('WARNING: [%s line %d char %d] %s\n' % \
-                             (self.filename, self.line, self.offset, msg))
+
+##  A filename; a specialization of str.
+
+class Fn (str):
+
+    ##  Dot can be used to add a pathname component.
+
+    def __getattr__ (self, attr):
+        if os.path.isdir(self):
+            return Fn(os.path.join(self, attr))
+        else:
+            return Fn(self + '.' + attr)
+
+    ##  Plus can also be used to concatenate a string; no slash is inserted.
+
+    def __add__ (self, other):
+        return Fn(str.__add__(self, other))
+
+    ##  Divide can be used to add pathname components.
+
+    def __div__ (self, other):
+        return self.join(other)
+
+    ##  Double slash can also be used.
+
+    def __truediv__ (self, other):
+        return self.join(other)
+
+    ##  CAUTION: this overrides str.join, with a very different semantics.
+    #   Specifically, this does a pathname join.
+
+    def join (self, *cpts):
+        return Fn(os.path.join(self, *cpts))
+
+    ##  Whether the named file exists.
+
+    def exists (self):
+        return os.path.exists(self)
+
+    ##  True if the named file exists and is a directory.
+
+    def isdir (self):
+        return os.path.isdir(self)
+
+    ##  The parent, obtained by stripping off the last component and deleting
+    #   any trailing slashes.
+
+    def parent (self):
+        if self.endswith('/'):
+            name = self.rstrip('/')
+        else:
+            name = self
+        if name:
+            return Fn(os.path.dirname(name))
+
+    ##  Create the file.  Create any missing ancestor using os.makedirs(),
+    #   then touch the file.
+
+    def create (self, dir=False):
+        if self.endswith('/'): dir = True
+        if dir:
+            os.makedirs(self)
+        else:
+            dirname = os.path.dirname(self)
+            if not os.path.exists(dirname):
+                os.makedirs(dirname)
+            _open(self, 'w').close()
+
+    ##  List the named file.  No-op if the file does not exist.  Returns
+    #   a list of child file names, if it names an existing directory.
+    #   Returns the result of os.stat(), if it names an existing regular file.
+
+    def list (self):
+        if os.path.exists(self):
+            if os.path.isdir(self):
+                return [Fn(f) for f in os.listdir(self)]
+            else:
+                return os.stat(self)
+
+    ##  Dispatches to shutil.move().
+
+    def rename (self, newname):
+        shutil.move(self, newname)
+
+    ##  Makes a copy.  If this is a directory, it does a deep copy.
+
+    def copy (self, newname, symlinks=True):
+        if os.path.isdir(self):
+            shutil.copytree(self, newname, symlinks)
+        else:
+            shutil.copyfile(self, newname)
+
+    ##  Delete the file.
+
+    def delete (self):
+        if os.path.isdir(self):
+            os.rmdir(self)
+        else:
+            os.unlink(self)
+
+    ##  Return the file size.
+
+    def size (self):
+        return file_size(self)
+
+    ##  Return the modtime, in seconds since the epoch (midnight UTC, Jan 1, 1970).
+
+    def modtime (self):
+        return os.stat(self).st_mtime
+
+
+##  The Seal python directory: the inner 'seal' directory.
+__seal__ = os.path.dirname(os.path.dirname(os.path.dirname(__file__)))
+
+##  The Seal destination directory: the outer 'seal' directory.
+__dest__ = os.path.dirname(os.path.dirname(__seal__))
+
+##  The Seal destination directory.
+dest = Fn(__dest__)
+
+##  The Seal bin directory.
+bin = Fn(os.path.join(__dest__, 'bin'))
+
+##  The seal examples directory.
+ex = Fn(os.path.join(__seal__, 'data', 'examples'))
+
+##  The seal data directory.
+data = Fn(os.path.join(__seal__, 'data'))
+
+##  The root directory.
+root = Fn(os.path.sep)
+
+##  The tmp directory.
+tmp = root.tmp
+
+##  The current directory, as an Fn.
+here = Fn(os.path.curdir)
+
+##  The user's home directory, as an Fn.
+home = Fn(os.path.expanduser('~'))
+
+##  Nowhere (/dev/null).
+nowhere = Fn('/dev/null')
+
+##  Allocate a tmp filename.  It automatically gets deleted when
+#   the filename is deleted or garbage collected.
+#   That is, one may delete the file by calling del on the filename.
+
+def tmpfile ():
+    _TmpFn.count += 1
+    fn = _TmpFn('/tmp/seal_%d_%d' % (os.getpid(), _TmpFn.count))
+    fn._delete_on_gc = True
+    return fn
+
+
+##  Allocates a temporary filename prefix and arranges for any file whose
+#   name begins with that prefix to be
+#   deleted (if any such exist) when the C{TmpFile} object gets garbage
+#   collected.  The filename prefix is of form::
+#
+#       /tmp/seal_PID_N_
+#
+#   where PID is the pid of the python process and N is a
+#   sequence number that is advanced each time a temporary filename is
+#   allocated.
+
+class _TmpFn (Fn):
+
+    ##  So that we assign a unique number to each temp file.
+    count = 0
+
+    ##  When the TmpFn gets deleted, delete the file on disk.
+    def __del__ (self):
+        if self._delete_on_gc:
+            os.system("rm -f " + self + "*")
+
+    ##  Call this to prevent file deletion on garbage collection.
+    def no_delete (self):
+        self._delete_on_gc = False
+
+
+#--  infile and outfile  -------------------------------------------------------
+
+##  A readable representation; fn may be a filename, a StringIO, or a stream.
+
+def filename_string (fn):
+    if isinstance(fn, str):
+        return fn
+    elif isinstance(fn, StringIO):
+        return '<string input>'
+    else:
+        return '<open file>'
+
+##  Open a file for reading.  Filename may be '-', a string representing a
+#   filename, a StringIO, a stream, or anything that has a readline() method.
+
+def infile (filename, encoding=None):
+    if isinstance(filename, str):
+        if not encoding: encoding = 'utf8'
+        if filename == '-':
+            return sys.stdin
+        elif re.match(r'[A-Za-z]+:', filename):
+            bstream = urllib.request.urlopen(filename, 'r')
+            reader = codecs.getreader(encoding)
+            return reader(bstream)
+        else:
+            return _open(filename, 'r', encoding=encoding)
+    elif isinstance(filename, StringIO):
+        return filename
+    elif isinstance(filename, TextIOBase):
+        return filename
+    elif hasattr(filename, 'readline'):
+        return filename
+    else:
+        raise Exception('Cannot coerce to file: %s' % filename)
+
+##  Open a file for writing.  Fileid may be '-', a string representing
+#   a filename, or None.  If None, a StringIO is returned.
+
+def outfile (fileid=None, encoding=None):
+    if fileid is None:
+        return StringIO()
+    elif fileid == '-':
+        return sys.stdout
+    else:
+        if not encoding: encoding = 'utf8'
+        return _open(fileid, 'w', encoding=encoding)
+
+##  An infile containing bytes.
+
+def byte_infile (fn):
+    if fn == '-': return sys.stdin.buffer
+    else: return _open(fn, 'rb')
+
+##  An outfile writing bytes.
+
+def byte_outfile (fn):
+    if fn == '-': return sys.stdout.buffer
+    else: return _open(fn, 'wb')
+
+##  Close a file, but not if it is a StringIO or a std stream.
+
+def close (file):
+    if isinstance(file, StringIO):
+        value = file.getvalue()
+    else:
+        value = None
+    if file not in [sys.stdin, sys.stdout, sys.stderr]:
+        file.close()
+    return value
+
+
+#--  Load/save string  ---------------------------------------------------------
+
+##  Load a string from a file.
+
+def load_string (filename, encoding=None):
+    f = infile(filename, encoding)
+    return f.read()
+
+##  Save a string to a file.
+
+def save_string (s, filename=None, encoding=None):
+    f = outfile(filename, encoding)
+    f.write(s)
+    return close(f)
+
+
+#--  Lines  --------------------------------------------------------------------
+
+##  Load a list of lines from a file.  Newlines and carriage returns are not
+#   included in the lines.
+
+def load_lines (filename, encoding=None):
+    return list(iter_lines(filename, encoding))
+
+##  Iterate over a list of lines.
+
+def iter_lines (filename, encoding=None):
+    for line in infile(filename, encoding):
+        yield line.rstrip('\r\n')
+
+##  Save a list of lines to a file.
+
+def save_lines (lines, filename=None, encoding=None):
+    f = outfile(filename, encoding)
+    for line in lines:
+        f.write(line)
+        f.write('\n')
+    return close(f)
+
+
+#--  Records  ------------------------------------------------------------------
+
+##  Load tabular records from a file.
+
+def load_records (filename, header=None, separator='\t', encoding=None):
+    return list(iter_records(filename, header, separator, encoding))
+
+##  Iterate over tabular records.
+
+class iter_records (object):
+
+    ##  Constructor.
+
+    def __init__ (self, filename, header=None, separator='\t', encoding=None):
+        ##  Filename.
+        self.filename = filename_string(filename)
+        ##  File.
+        self.file = infile(filename, encoding)
+        ##  Number of lines processed so far.
+        self.linecount = 0
+        ##  Separator.
+        self.separator = separator
+        if header is not None:
+            line = self.__readline()
+            fileheader = line.rstrip('\r\n').split(separator)
+            if fileheader != header:
+                raise Exception("Bad header: got %s, expecting %s: %s" % \
+                    (fileheader, header, filename))
+
+    def __readline (self):
+        self.linecount += 1
+        return next(self.file)
+
+    ##  Returns self.
+
+    def __iter__ (self):
+        return self
+
+    ##  The iteration method.
+
+    def __next__ (self):
+        line = self.__readline()
+        return line.rstrip('\r\n').split(self.separator)
+
+    ##  Signal an error, adding the filename and line number.
+
+    def error (self, msg):
+        raise Exception("[%s line %d] %s" % (self.filename, self.linecount, msg))
+
+##  Save a list of records to a tabular file.
+
+def save_records (records, filename=None, header=None, separator='\t', encoding=None):
+    f = outfile(filename, encoding)
+    if header:
+        f.write(separator.join(header))
+        f.write('\n')
+    for record in records:
+        f.write(separator.join(record))
+        f.write('\n')
+    return close(f)
+
+
+#--  Dict  ---------------------------------------------------------------------
+
+##  Load a dict from a file.
+
+def load_dict (filename, encoding=None):
+    out = {}
+    for record in load_records(filename, encoding):
+        if len(record) != 2:
+            raise Exception(f'In {filename}: bad record: {repr(record)}')
+        (k,v) = record
+        out[k] = v
+    return out
+
+##  Save a dict to a file.  The output is tabular, with keys in the first column
+#   and values in the second column.
+
+def save_dict (d, filename=None, encoding=None):
+    return save_records(iter(d.items()), filename, encoding)
+
+    
+#--  NestedDict  ---------------------------------------------------------------
+
+##  Load a nested dict from a file.
+#   A nested dict permits keys containing dots.  The first part of the key
+#   becomes a key in the toplevel dict, and its value is a subdict.
+
+def load_nested_dict (fn, encoding=None):
+    out = {}
+    for line in infile(fn, encoding):
+        line = line.rstrip('\r\n')
+        if (not line) or line.startswith('#'): continue
+        i = 0
+        while True:
+            if i >= len(line):
+                raise Exception('No whitespace character in line')
+            if line[i].isspace():
+                break
+            i += 1
+        k = line[:i]
+        v = line[i+1:].strip()
+        d = out
+        subkeys = k.split('.')
+        if len(subkeys) > 1:
+            k = subkeys[-1]
+            for i in range(len(subkeys)-1):
+                sk = subkeys[i]
+                if sk in d:
+                    d = d[sk]
+                    if not isinstance(d, dict):
+                        raise Exception('Expecting dict: %s' % '.'.join(subkeys[:i+1]))
+                else:
+                    newd = {}
+                    d[sk] = newd
+                    d = newd
+        d[k] = v
+    return out
+
+##  Write a dict in nested dict format.
+
+def save_nested_dict (d, fn, encoding=None):
+    f = outfile(fn, encoding)
+    _write_nested_dict('', d, f)
+    return close(f)
+
+def _write_nested_dict (prefix, d, f):
+    for key in d:
+        if prefix: fullkey = prefix + '.' + key
+        else: fullkey = key
+        v = d[key]
+        if isinstance(v, dict):
+            _write_nested_dict(fullkey, v, f)
+        else:
+            f.write(fullkey)
+            f.write(' ')
+            v = str(v)
+            if '\n' in v:
+                raise Exception('Value contains newline: %s' % repr(v))
+            f.write(v)
+            f.write('\n')
+
+
+#--  Config file  --------------------------------------------------------------
+
+#
+#  [0][d1]
+#      (0, 'server', None)
+#  [0 4][d1 d2]
+#      (4, 'cld', None)
+#  [0 4 8][d1 d2 d3]
+#      (8, 'foo', '10')
+#      (8, 'bar', '2')
+#      (4, 'baz', '6')
+#
+
+
+##  Produces a nested dict, but instead of dotted keys, it uses indentation
+#   Keys and values are separated by '='.
+#   Hash starts a comment line.
+#   Empty lines are ignored.
+#
+#   Example:
+#
+#       server
+#           cld
+#               foo = 10
+#               bar = 2
+#           baz = 6
+
+def load_config (fn, encoding=None):
+    lines = list(_iter_config_lines(fn, encoding))
+    cfg = {}
+    indents = [0]
+    dicts = [cfg]
+
+    for i in range(len(lines)):
+        (ind, key, value) = lines[i]
+
+        # Pop as necessary
+        if ind > indents[-1]:
+            raise Exception('Bad indentation')
+        while ind < indents[-1]:
+            if len(indents) == 1:
+                raise Exception('Bad indentation in config file')
+            indents.pop()
+            dicts.pop()
+        if ind != indents[-1]:
+            raise Exception('Bad indentation in config file')            
+
+        # Start subdict
+        if value is None:
+            if i+1 >= len(lines):
+                raise Exception("No body for subdict '%s'" % key)
+            nextind = lines[i+1][0]
+            if nextind <= ind:
+                raise Exception("No body for subdict '%s'" % key)
+            d = {}
+            dicts[-1][key] = d
+            indents.append(nextind)
+            dicts.append(d)
+
+        # Set value
+        else:
+            dicts[-1][key] = value
+
+    return cfg
+
+def _iter_config_lines (fn, encoding):
+    for line in infile(fn, encoding):
+        line = line.rstrip('\r\n')
+        if (not line) or line.startswith('#'): continue
+        ind = 0
+        while ind < len(line) and line[ind].isspace():
+            if line[ind] != ' ':
+                raise Exception('Only spaces permitted in config file')
+            ind += 1
+        print('ind=', ind)
+        i = ind
+        while True:
+            if i >= len(line):
+                key = line.strip()
+                value = None
+                break
+            elif line[i] == '=':
+                key = line[ind:i].strip()
+                value = line[i+1:].strip()
+                break
+            else:
+                i += 1
+        yield (ind, key, value)
+
+
+#--  Paragraphs  ---------------------------------------------------------------
+
+##  Load a list of paragraphs from a file.  In the file, paragraphs are separated
+#   by empty lines.  In memory, paragraphs are represented as single strings with
+#   embedded newlines.
+
+def load_paragraphs (filename, encoding=None):
+    return list(iter_paragraphs(filename, encoding))
+
+##  Iterate over paragraphs.
+
+def iter_paragraphs (filename, encoding=None):
+    file = infile(filename, encoding)
+    par = []
+    try:
+        while True:
+            line = next(file)
+            if line == '\n':
+                yield ''.join(par)
+                par = []
+            else:
+                par.append(line)
+    except StopIteration:
+        if par:
+            yield ''.join(par)
+
+##  Write out a list of paragraphs to a file, inserting empty lines between them.
+
+def save_paragraphs (pars, filename=None, encoding=None):
+    file = outfile(filename, encoding)
+    first = True
+    for par in pars:
+        if first:
+            first = False
+        else:
+            file.write('\n')
+        file.write(par)
+    return close(file)
+
+
+#--  Blocks  -------------------------------------------------------------------
+
+##  Load a list of blocks from a file.  A block is a list of lines, sans newlines.
+#   In the file, blocks are separated by empty lines.
+
+def load_blocks (filename, encoding=None):
+    return list(iter_blocks(filename, encoding))
+
+##  Iterate over blocks.
+
+def iter_blocks (filename, encoding=None):
+    file = infile(filename, encoding)
+    block = []
+    try:
+        while True:
+            line = next(file).rstrip('\r\n')
+            if not line:
+                if block:
+                    yield block
+                    block = []
+            else:
+                block.append(line)
+    except StopIteration:
+        if block:
+            yield block
+
+##  Write a list of blocks to a file.
+
+def save_blocks (blocks, filename=None, encoding=None):
+    file = outfile(filename, encoding)
+    first = True
+    for block in blocks:
+        if first:
+            first = False
+        else:
+            file.write('\n')
+        for line in block:
+            file.write(line)
+            file.write('\n')
+    return close(file)
+
+
+#--  Record Blocks  ------------------------------------------------------------
+
+##  A record is a list of field values (strings).  A record block is a list of
+#   records.  A record-block file is a list of record blocks.
+#   In the file, fields are separated by tab and blocks are separated by empty lines.
+
+def load_record_blocks (filename, encoding=None):
+    return list(iter_record_blocks(filename, encoding))
+
+##  Iterate over record blocks.
+
+def iter_record_blocks (filename, encoding=None):
+    file = infile(filename, encoding)
+    block = []
+    try:
+        while True:
+            line = next(file).rstrip('\r\n')
+            if not line:
+                if block:
+                    yield block
+                    block = []
+            else:
+                block.append(line.split('\t'))
+    except StopIteration:
+        if block:
+            yield block
+
+##  Save a list of record blocks to a file.
+
+def save_record_blocks (blocks, filename=None, encoding=None):
+    file = outfile(filename, encoding)
+    first = True
+    for block in blocks:
+        if first:
+            first = False
+        else:
+            file.write('\n')
+        for record in block:
+            file.write('\t'.join(record))
+            file.write('\n')
+    return close(file)
+
+
+#--  Tokens  -------------------------------------------------------------------
+
+##  Quote characters: single and double quote.
+QuoteChars = '"\''
+
+##  Default special characters: parentheses, brackets, braces.
+DefaultSpecialChars = '()[]{}'
 
 
 ##  Represents the syntax of a little language.
 
 class Syntax (object):
 
-    QuoteChars = '"\''
-    DefaultSpecialChars = '()[]{}'
+    ##  Constructor.
 
     def __init__ (self,
-                  special=None,
+                  special=DefaultSpecialChars,
                   eol=False,
                   comments=True,
                   multi=None,
                   backslash=True,
                   stringtype='word',
                   mlstrings=False,
                   digits=False):
 
         ##  The special characters.  True means everything except alphanumerics
         #   and whitespace.
-        self.special = self.DefaultSpecialChars if special is None else special
+        self.special = None
 
         ##  Multi-character sequences that should be recognized as tokens.
         self.multi = None
 
         ##  The start characters for multi-character sequences.
         self.multi_start = None
 
@@ -155,353 +909,478 @@
         return s
 
     ##  String representation.
 
     def __repr__ (self):
         return '<Syntax %s %s>' % (self.special, self.eol)
 
-    
-    ##  Tokenize a file, returning a list.
-    
-    def load_tokens (self, filename, encoding=None):
-        return list(self.iter_tokens(filename, encoding))
-    
-    ##  Iterate over tokens of a string.
-    
-    def tokenize (self, s, encoding=None):
-        return self.iter_tokens(StringIO(s), encoding)
-    
-    ##  Iterator over tokens.
-    
-    def iter_tokens (self, filename, encoding=None):
-        return self.TokenIterator(self, filename, encoding)
+##  A Syntax instance.
+DefaultSyntax = Syntax()
 
-    class TokenIterator (object):
-    
-        ##  Constructor.
-    
-        def __init__ (self, syntax, filename, encoding):
-    
-            ##  A Syntax instance.
-            self.syntax = syntax
-    
-            ##  Stack, for (possibly nested) temporary syntax changes.
-            self.stack = []
-    
-            ##  Filename string; set even for streams not associated with files.
-            self.filename = filename_string(filename)
-    
-            ##  The lines of the file.
-            self.lines = load_lines(filename, encoding)  # no newlines in lines
-    
-            ##  The current line.
-            self.line = None
-    
-            ##  Current line number.
-            self.linecount = 1
-    
-            ##  Current character offset on the line.
-            self.offset = 0
-    
-            ##  Previous linecount.
-            self.old_linecount = 1
-    
-            ##  Previous offset.
-            self.old_offset = 0
-    
-            self.__token = None
-    
-            if self.lines: self.line = self.lines[0]
-            else: self.line = ''
-    
-        ##  Returns self.
-    
-        def __iter__ (self):
-            return self
-    
-        ##  Whether we are at EOF.
-    
-        def __bool__ (self):
-            return self.token().type != 'eof'
-    
-        def __readline (self):
-            if self.linecount < len(self.lines):
-                self.line = self.lines[self.linecount]
-                self.linecount += 1
-            elif self.linecount == len(self.lines):
-                self.line = ''
-                self.linecount += 1
-            else:
-                raise Exception('Readline after EOF')
-            self.offset = 0
-    
-        def __at_eof (self):
-            return self.linecount > len(self.lines)
-    
-        def __empty_line (self):
-            for c in self.line:
-                if c in self.syntax.comments: return True
-                elif not c.isspace(): return False
-            return True
-    
-        def __is_special (self, c):
-            if self.syntax.special is True:
-                return not (c.isalnum() or c == '_')
+##  Convert s to a scanable string, assuming the default syntax.
+
+def scanable_string (s):
+    return DefaultSyntax.scanable_string(s)
+
+
+##  A token.
+
+class Token (str):
+
+    ##  True if type is 'any' or equals the token's type.
+    def hastype (self, type):
+        if type == 'any': return self.type != 'eof'
+        else: return type == self.type
+
+    ##  Raise an exception, indicating file, line, and offset.
+    def error (self, msg='syntax error'):
+        raise Exception('[%s line %d char %d] %s' % \
+            (self.filename, self.line, self.offset, msg))
+
+    ##  Print a warning, indicating file, line, and offset.
+    def warn (self, msg):
+        sys.stderr.write('WARNING: [%s line %d char %d] %s\n' % \
+                             (self.filename, self.line, self.offset, msg))
+
+
+##  Tokenize a file, returning a list.
+
+def load_tokens (filename, **kwargs):
+    return list(iter_tokens(filename, **kwargs))
+
+##  Iterate over tokens of a string.
+
+def tokenize (s, syntax=DefaultSyntax, encoding=None):
+    return iter_tokens(StringIO(s), syntax, encoding)
+
+##  Iterator over tokens.
+
+class iter_tokens (object):
+
+    ##  Constructor.
+
+    def __init__ (self, filename, syntax=DefaultSyntax, encoding=None):
+
+        ##  A Syntax instance.
+        self.syntax = syntax
+
+        ##  Stack, for (possibly nested) temporary syntax changes.
+        self.stack = []
+
+        ##  Filename string; set even for streams not associated with files.
+        self.filename = filename_string(filename)
+
+        ##  The lines of the file.
+        self.lines = load_lines(filename, encoding)  # no newlines in lines
+
+        ##  The current line.
+        self.line = None
+
+        ##  Current line number.
+        self.linecount = 1
+
+        ##  Current character offset on the line.
+        self.offset = 0
+
+        ##  Previous linecount.
+        self.old_linecount = 1
+
+        ##  Previous offset.
+        self.old_offset = 0
+
+        self.__token = None
+
+        if self.lines: self.line = self.lines[0]
+        else: self.line = ''
+
+    ##  Returns self.
+
+    def __iter__ (self):
+        return self
+
+    ##  Whether we are at EOF.
+
+    def __bool__ (self):
+        return self.token().type != 'eof'
+
+    def __readline (self):
+        if self.linecount < len(self.lines):
+            self.line = self.lines[self.linecount]
+            self.linecount += 1
+        elif self.linecount == len(self.lines):
+            self.line = ''
+            self.linecount += 1
+        else:
+            raise Exception('Readline after EOF')
+        self.offset = 0
+
+    def __at_eof (self):
+        return self.linecount > len(self.lines)
+
+    def __empty_line (self):
+        for c in self.line:
+            if c in self.syntax.comments: return True
+            elif not c.isspace(): return False
+        return True
+
+    def __is_special (self, c):
+        if self.syntax.special is True:
+            return not (c.isalnum() or c == '_')
+        else:
+            return c in self.syntax.special
+
+    ##  Advance, if necessary, then return the current token.
+
+    def token (self):
+        if self.__token is None: self.__advance()
+        return self.__token
+
+    def __skip_eol (self):
+        if self.offset >= len(self.line):
+            if self.syntax.eol and not self.__empty_line():
+                self.__set_token('\n', self.offset, string='\n')
+                self.__readline()
             else:
-                return c in self.syntax.special
-    
-        ##  Advance, if necessary, then return the current token.
-    
-        def token (self):
-            if self.__token is None: self.__advance()
-            return self.__token
-    
-        def __skip_eol (self):
-            if self.offset >= len(self.line):
-                if self.syntax.eol and not self.__empty_line():
-                    self.__set_token('\n', self.offset, string='\n')
+                while self.offset >= len(self.line):
+                    if self.__at_eof():
+                        self.__set_token('eof', self.offset)
+                        break
                     self.__readline()
-                else:
-                    while self.offset >= len(self.line):
-                        if self.__at_eof():
-                            self.__set_token('eof', self.offset)
-                            break
-                        self.__readline()
-    
-        def __advance (self):
-            self.old_linecount = self.linecount
-            self.old_offset = self.offset
-            self.__token = None
-            try:
-                while self.__token is None:
-                    self.__skip_eol()
-                    if self.__token is not None: return
-                    c = self.line[self.offset]
-    
-                    if c in self.syntax.multi_start and self.__scan_multi(): pass
-                    elif c in self.syntax.comments: self.offset = len(self.line)
-                    elif c == "'" or c == '"': self.__scan_quoted()
-                    elif c.isspace(): self.offset += 1
-                    elif self.__is_special(c): self.__scan_special()
-                    elif self.syntax.digits and self.__is_digit(c): self.__scan_digit()
-                    else: self.__scan_word()
-    
-            except StopIteration:
-                raise Exception('[%s line %d offset %d] Unexpected eof' % \
-                    (self.filename, self.linecount, self.offset))
-    
-        def __retreat (self):
-            self.__token = None
-            self.linecount = self.old_linecount
-            self.offset = self.old_offset
-            if self.linecount > 0:
-                self.line = self.lines[self.linecount-1]
-            else:
-                self.line = None
-    
-        def __set_token (self, type, start, line=None, string=None, quotes=None):
-            if line is None:
-                line = self.linecount
-            if string is None:
-                string = self.line[start:self.offset]
-            self.__token = Token(string)
-            self.__token.type = type
-            self.__token.filename = self.filename
-            self.__token.line = line
-            self.__token.offset = start
-            self.__token.quotes = quotes
-    
-        def __is_digit (self, c):
-            if c.isdigit(): return True
-            i = self.offset + 1
-            return c == '-' and i < len(self.line) and self.line[i].isdigit()
-    
-        def __scan_digit (self):
-            start = self.offset
-            if self.line[self.offset] == '-': self.offset += 1
-            while self.offset < len(self.line) and self.line[self.offset].isdigit():
-                self.offset += 1
-            self.__set_token('digit', start)
-    
-        def __scan_word (self):
-            start = self.offset
-            while self.offset < len(self.line):
+
+    def __advance (self):
+        self.old_linecount = self.linecount
+        self.old_offset = self.offset
+        self.__token = None
+        try:
+            while self.__token is None:
+                self.__skip_eol()
+                if self.__token is not None: return
                 c = self.line[self.offset]
-                if c.isspace() or self.__is_special(c): break
-                self.offset += 1
-            self.__set_token('word', start)
-    
-        def __error (self, start, msg):
-            raise Exception('[%s line %d char %d] %s' % \
-                (self.filename, self.linecount, start, msg))
-    
-        def __scan_quoted (self):
-            delim = self.line[self.offset]
+
+                if c in self.syntax.multi_start and self.__scan_multi(): pass
+                elif c in self.syntax.comments: self.offset = len(self.line)
+                elif c == "'" or c == '"': self.__scan_quoted()
+                elif c.isspace(): self.offset += 1
+                elif self.__is_special(c): self.__scan_special()
+                elif self.syntax.digits and self.__is_digit(c): self.__scan_digit()
+                else: self.__scan_word()
+
+        except StopIteration:
+            raise Exception('[%s line %d offset %d] Unexpected eof' % \
+                (self.filename, self.linecount, self.offset))
+
+    def __retreat (self):
+        self.__token = None
+        self.linecount = self.old_linecount
+        self.offset = self.old_offset
+        if self.linecount > 0:
+            self.line = self.lines[self.linecount-1]
+        else:
+            self.line = None
+
+    def __set_token (self, type, start, line=None, string=None, quotes=None):
+        if line is None:
+            line = self.linecount
+        if string is None:
+            string = self.line[start:self.offset]
+        self.__token = Token(string)
+        self.__token.type = type
+        self.__token.filename = self.filename
+        self.__token.line = line
+        self.__token.offset = start
+        self.__token.quotes = quotes
+
+    def __is_digit (self, c):
+        if c.isdigit(): return True
+        i = self.offset + 1
+        return c == '-' and i < len(self.line) and self.line[i].isdigit()
+
+    def __scan_digit (self):
+        start = self.offset
+        if self.line[self.offset] == '-': self.offset += 1
+        while self.offset < len(self.line) and self.line[self.offset].isdigit():
             self.offset += 1
-            start = self.offset
-            restart = self.offset
-            frags = []
-            while True:
-                while self.offset >= len(self.line):
-                    if self.syntax.mlstrings:
-                        if restart < len(self.line):
-                            frags.append(self.line[restart:])
-                        frags.append('\n')
-                        self.__readline()
-                        restart = self.offset
-                        if self.__at_eof():
-                            self.__error(start, 'Unterminated string at EOF')
-                    else:
-                        self.__error(start, 'End of line in string')
-                c = self.line[self.offset]
-                if c == delim:
-                    frags.append(self.line[restart:self.offset])
-                    self.offset += 1
-                    break
-                elif c == '\\' and self.syntax.backslash:
-                    frags.append(self.line[restart:self.offset])
-                    frags.append(self.__scan_escape_sequence())
+        self.__set_token('digit', start)
+
+    def __scan_word (self):
+        start = self.offset
+        while self.offset < len(self.line):
+            c = self.line[self.offset]
+            if c.isspace() or self.__is_special(c): break
+            self.offset += 1
+        self.__set_token('word', start)
+
+    def __error (self, start, msg):
+        raise Exception('[%s line %d char %d] %s' % \
+            (self.filename, self.linecount, start, msg))
+
+    def __scan_quoted (self):
+        delim = self.line[self.offset]
+        self.offset += 1
+        start = self.offset
+        restart = self.offset
+        frags = []
+        while True:
+            while self.offset >= len(self.line):
+                if self.syntax.mlstrings:
+                    if restart < len(self.line):
+                        frags.append(self.line[restart:])
+                    frags.append('\n')
+                    self.__readline()
                     restart = self.offset
+                    if self.__at_eof():
+                        self.__error(start, 'Unterminated string at EOF')
                 else:
-                    self.offset += 1
-            self.__set_token(self.syntax.stringtype, start, self.linecount, ''.join(frags), delim)
-    
-        def __scan_escape_sequence (self):
-            # self.line[self.offset] is backslash
-            self.offset += 1
-            if self.offset >= len(self.line): self.__error('Bad escape sequence')
+                    self.__error(start, 'End of line in string')
             c = self.line[self.offset]
-            self.offset += 1
-            if c == '\\' or c == '"' or c == "'": return c
-            elif c == 'a': return '\a'
-            elif c == 'b': return '\b'
-            elif c == 'f': return '\f'
-            elif c == 'n': return '\n'
-            elif c == 'r': return '\r'
-            elif c == 't': return '\t'
-            elif c == 'u':
-                i = self.offset
-                self.offset += 4
-                if self.offset > len(self.line): self.__error('Bad escape sequence')
-                return chr(int(self.line[i:self.offset], 16))
-            elif c == 'U':
-                self.__error('\\U escapes not implemented')
-            elif c == 'v': return '\v'
-            elif '0' <= c <= '7':
-                i = self.offset
+            if c == delim:
+                frags.append(self.line[restart:self.offset])
                 self.offset += 1
-                n = 1
-                while n < 3 and self.offset < len(self.line) and \
-                        '0' <= self.line[self.offset] <= '7':
-                    self.offset += 1
-                    n += 1
-                return chr(int(self.line[i:self.offset], 8))
-            elif c == 'x':
-                i = self.offset
+                break
+            elif c == '\\' and self.syntax.backslash:
+                frags.append(self.line[restart:self.offset])
+                frags.append(self.__scan_escape_sequence())
+                restart = self.offset
+            else:
                 self.offset += 1
-                if self.offset < len(self.line) and \
-                        ('0' <= self.line[self.offset] <= '9' or \
-                         'a' <= self.line[self.offset] <= 'f' or \
-                         'A' <= self.line[self.offset] <= 'F'):
-                    self.offset += 1
-                d = int(self.line[i:self.offset], 16)
-                if d < 0x100: return chr(d)
-                else: return chr(d)
-    
-        def __scan_special (self):
-            start = self.offset
+        self.__set_token(self.syntax.stringtype, start, self.linecount, ''.join(frags), delim)
+
+    def __scan_escape_sequence (self):
+        # self.line[self.offset] is backslash
+        self.offset += 1
+        if self.offset >= len(self.line): self.__error('Bad escape sequence')
+        c = self.line[self.offset]
+        self.offset += 1
+        if c == '\\' or c == '"' or c == "'": return c
+        elif c == 'a': return '\a'
+        elif c == 'b': return '\b'
+        elif c == 'f': return '\f'
+        elif c == 'n': return '\n'
+        elif c == 'r': return '\r'
+        elif c == 't': return '\t'
+        elif c == 'u':
+            i = self.offset
+            self.offset += 4
+            if self.offset > len(self.line): self.__error('Bad escape sequence')
+            return chr(int(self.line[i:self.offset], 16))
+        elif c == 'U':
+            self.__error('\\U escapes not implemented')
+        elif c == 'v': return '\v'
+        elif '0' <= c <= '7':
+            i = self.offset
             self.offset += 1
-            self.__set_token(self.line[start], start)
-    
-        def __looking_at (self, word):
-            for i in range(len(word)):
-                t = self.offset + i
-                if t >= len(self.line): return False
-                if self.line[t] != word[i]: return False
-            return True
-    
-        def __scan_multi (self):
-            for word in self.syntax.multi:
-                if self.__looking_at(word):
-                    start = self.offset
-                    self.offset += len(word)
-                    self.__set_token(self.line[start:self.offset], start)
-                    return True
-    
-        ##  Whether the next token is something other than EOF.
-        #   If type or string is provided, the value indicates whether the next
-        #   token has the given type and/or string.
-    
-        def has_next (self, type=None, string=None):
-            if string:
-                if type: raise Exception("Provide only one argument")
-                return self.token() == string
-            elif type:
-                return self.token().hastype(type)
-            else:
-                return self.token().type != 'eof'
-    
-        ##  Iterator method.
-    
-        def __next__ (self):
-            token = self.token()
-            if token.type == 'eof': raise StopIteration
-            self.__token = None
-            self.old_linecount = self.linecount
-            self.old_offset = self.offset
-            return token
-    
-        ##  If the next token matches the given type and/or string, return it
-        #   and advance.  Otherwise, return None.
-    
-        def accept (self, type=None, string=None):
-            token = self.token()
-            if type and not token.hastype(type):
-                return None
-            if string and not (token == string):
-                return None
-            return next(self)
-    
-        ##  If the next token has the given type and/or string, return it
-        #   and advance.  Otherwise, signal an error.  Returns None at EOF.
-    
-        def require (self, type=None, string=None):
-            token = self.token()
-            if type and not token.hastype(type):
-                token.error('Expecting ' + repr(type))
-            if string and not (token == string):
-                token.error('Expecting ' + repr(string))
-            if type == 'eof': return None
-            else: return next(self)
-    
-        ##  Signal an error, indicating filename and line number.
-    
-        def error (self, msg=None):
-            token = self.token()
-            token.error(msg)
-    
-        ##  Print a warning, showing filename and line number.
-    
-        def warn (self, msg=None):
-            token = self.token()
-            token.warn(msg)
-    
-        ##  Push the current syntax on the stack and switch to the given syntax.
-    
-        def push_syntax (self, syntax):
-            self.stack.append(self.syntax)
-            self.syntax = syntax
-            self.__retreat()
-    
-        ##  Restore the previous syntax from the stack.
-    
-        def pop_syntax (self):
-            if not self.stack: raise Exception('Empty stack')
-            self.syntax = self.stack.pop()
-            self.__retreat()
+            n = 1
+            while n < 3 and self.offset < len(self.line) and \
+                    '0' <= self.line[self.offset] <= '7':
+                self.offset += 1
+                n += 1
+            return chr(int(self.line[i:self.offset], 8))
+        elif c == 'x':
+            i = self.offset
+            self.offset += 1
+            if self.offset < len(self.line) and \
+                    ('0' <= self.line[self.offset] <= '9' or \
+                     'a' <= self.line[self.offset] <= 'f' or \
+                     'A' <= self.line[self.offset] <= 'F'):
+                self.offset += 1
+            d = int(self.line[i:self.offset], 16)
+            if d < 0x100: return chr(d)
+            else: return chr(d)
+
+    def __scan_special (self):
+        start = self.offset
+        self.offset += 1
+        self.__set_token(self.line[start], start)
+
+    def __looking_at (self, word):
+        for i in range(len(word)):
+            t = self.offset + i
+            if t >= len(self.line): return False
+            if self.line[t] != word[i]: return False
+        return True
+
+    def __scan_multi (self):
+        for word in self.syntax.multi:
+            if self.__looking_at(word):
+                start = self.offset
+                self.offset += len(word)
+                self.__set_token(self.line[start:self.offset], start)
+                return True
+
+    ##  Whether the next token is something other than EOF.
+    #   If type or string is provided, the value indicates whether the next
+    #   token has the given type and/or string.
+
+    def has_next (self, type=None, string=None):
+        if string:
+            if type: raise Exception("Provide only one argument")
+            return self.token() == string
+        elif type:
+            return self.token().hastype(type)
+        else:
+            return self.token().type != 'eof'
+
+    ##  Iterator method.
+
+    def __next__ (self):
+        token = self.token()
+        if token.type == 'eof': raise StopIteration
+        self.__token = None
+        self.old_linecount = self.linecount
+        self.old_offset = self.offset
+        return token
+
+    ##  If the next token matches the given type and/or string, return it
+    #   and advance.  Otherwise, return None.
+
+    def accept (self, type=None, string=None):
+        token = self.token()
+        if type and not token.hastype(type):
+            return None
+        if string and not (token == string):
+            return None
+        return next(self)
+
+    ##  If the next token has the given type and/or string, return it
+    #   and advance.  Otherwise, signal an error.  Returns None at EOF.
+
+    def require (self, type=None, string=None):
+        token = self.token()
+        if type and not token.hastype(type):
+            token.error('Expecting ' + repr(type))
+        if string and not (token == string):
+            token.error('Expecting ' + repr(string))
+        if type == 'eof': return None
+        else: return next(self)
+
+    ##  Signal an error, indicating filename and line number.
+
+    def error (self, msg=None):
+        token = self.token()
+        token.error(msg)
+
+    ##  Print a warning, showing filename and line number.
+
+    def warn (self, msg=None):
+        token = self.token()
+        token.warn(msg)
+
+    ##  Push the current syntax on the stack and switch to the given syntax.
+
+    def push_syntax (self, syntax):
+        self.stack.append(self.syntax)
+        self.syntax = syntax
+        self.__retreat()
+
+    ##  Restore the previous syntax from the stack.
+
+    def pop_syntax (self):
+        if not self.stack: raise Exception('Empty stack')
+        self.syntax = self.stack.pop()
+        self.__retreat()
+
+
+#--  Indenter  -----------------------------------------------------------------
+
+##  Indenter.
+#   The main facility a formatter provides is automatic indentation.
+#   There is a prevailing indentation level, and indentation spaces are
+#   automatically inserted after each newline that is written to the
+#   formatter.  The level of indentation is increased
+#   using begin_indent() and decreased
+#   using end_indent().  It is initially zero.
+#
+#   A formatter may be turned off, in which case writing commands are
+#   accepted but generate no output.  The formatter is initially on.
+
+class Indenter:
+
+    ##  Constructor.
+
+    def __init__ (self, filename=None, encoding=None):
+        self.__out = outfile(filename, encoding)
+
+        ##  Whether it is enabled.
+        self.enabled = True
+
+        self.__at_bol = True
+        self.__indent_level = 0
+        self.__indent_string = ""
+
+        ##  How many spaces to indent by each time.
+        self.indent_step = 3
+
+    ##  Flush any pending output.
+        
+    def flush (self):
+        if self.__out: self.__out.flush()
+
+    ##  Close the file.
+
+    def close (self):
+        if self.__out:
+            self.__out.close()
+            self.__out = None
+
+    ##  Turn the indenter on.
+
+    def on (self):
+        self.enabled = True
+
+    ##  Turn the indenter off.
+
+    def off (self):
+        self.enabled = False
+
+    ##  Write str(x) to the output, inserting indentation at the beginning
+    #   of each line.
+
+    def write (self, x):
+        string = str(x)
+        if self.enabled and string:
+            lines = string.split("\n")
+            self.__write(lines[0])
+            for i in range(1, len(lines)):
+                self.newline()
+                self.__write(lines[i])
+
+    def __write (self, string):
+        if string:
+            if self.__at_bol: self.__out.write(self.__indent_string)
+            self.__out.write(string)
+            self.__at_bol = False
+
+    ##  Equivalent to write('\n').
+
+    def newline (self):
+        self.__out.write("\n")
+        self.__at_bol = True
+
+    ##  Increase the indentation level by one.
+
+    def begin_indent (self):
+        self.__indent_level += 1
+        self.__indent_string = " " * (self.indent_step * self.__indent_level)
+
+    ##  Decrease the indentation level by one.
+
+    def end_indent (self):
+        self.__indent_level -= 1
+        if self.__indent_level < 0: raise Exception("No indentation to end")
+        self.__indent_string = " " * (self.indent_step * self.__indent_level)
+
+    ##  Set the indentation level to zero.
+
+    def reset (self):
+        self.__indent_level = 0
+
+    ##  If the internal stream is a StringIO, fetch its value.
+
+    def getvalue (self):
+        return self.__out.getvalue()
 
 
 #--  pprint  -------------------------------------------------------------------
 
 ##  A PPrinter instance.
 pprint = None
 
@@ -687,48 +1566,50 @@
 
 
 pprint = PPrinter()
 
 
 #--  tabular  ------------------------------------------------------------------
 
-def __getcell (row, j, tostring):
-    if len(row) > j: return tostring(row[j])
+def __getcell (row, j):
+    if len(row) > j: return as_ascii(row[j])
     else: return ''
 
-def __compute_width (rows, j, tostring):
-    return max(len(__getcell(r,j,tostring)) for r in rows)
+def __compute_width (rows, j):
+    return max(len(__getcell(r,j)) for r in rows)
+
+
+##  Produces a string representation of a table with aligned columns,
+#   suitable for printing.
 
-def colalign (rows, header=None, indent='', tostring=str, hlines=True):
+def tabular (rows, header=None, indent=''):
     tmp = []
     if header: tmp.append(header)
-    tmp.extend(rows)
+    for row in rows: tmp.append(row)
     rows = tmp
+    out = ''
     ncols = max(len(r) for r in rows)
-    widths = [__compute_width(rows,j,tostring) for j in range(ncols)]
-    for i in range(len(rows)):
-        line = indent
+    widths = [__compute_width(rows,j) for j in range(ncols)]
+    first = True
+    for row in rows:
+        if first: first = False
+        else: out += '\n'
+        if indent: out += indent
         for j in range(ncols):
-            if j: line += ' '
-            line += '%-*s' % (widths[j], __getcell(rows[i], j, tostring))
-        rows[i] = line
-    if hlines:
-        linewidth = sum(widths) + ncols - 1
-        hline = '-' * linewidth
-        if header:
-            rows[1:1] = [hline]
-        rows[-1:-1] = [hline]
-    return rows
+            if j: out += ' '
+            out += '%-*s' % (widths[j], __getcell(row, j))
+    return out
 
-##  Produces a string representation of a table with aligned columns,
-#   suitable for printing.
 
-def tabular (rows, header=None, indent='', tostring=str, hlines=True):
-    return '\n'.join(colalign(rows, header, indent, tostring, hlines))
+#--  wget  ---------------------------------------------------------------------
 
+##  Simple interface to urlretrieve().
+
+def wget (url):
+    return urllib.request.urlretrieve(url)[0]
 
 
 #--  OutputRedirected  ---------------------------------------------------------
 
 ##  Does the actual output redirection.
 class _Redirect (object):
 
@@ -812,1426 +1693,769 @@
 #           f.write(...)
 #           out = f.output
 #
 
 redirect = _Redirect()
 
 
-#--  BackingSave  --------------------------------------------------------------
+#--  Location  -----------------------------------------------------------------
 
-##  Handles locking (only).
+##  Affects some Location methods.
+DryRun = False
 
-class BackingAdmin (object):
 
-    ##  Constructor.
+##  Generalizes over local files and remote files represented by URL.
 
-    def __init__ (self, fn):
-
-        ##  The filename.
-        self.filename = fn
-
-        ##  The lock, when locked.
-        self.lock = None
-
-    ##  Lock the file.
-
-    def __enter__ (self):
-        self.lock = open(fn + '.lock', 'w')
-        flock(self.lock, LOCK_EX)
-        return self
-
-    ##  Release the lock.
-
-    def __exit__ (self, type, value, tb):
-        self.lock.close()
-    
-    ##  Replace the file with the backup version.
-
-    def undo (self):
-        bakfn = self.filename + '.bak'
-        if not os.path.exists(bakfn):
-            raise Exception('No undo information available: %s' % fn)
-        if os.path.exists(self.filename):
-            os.replace(self.filename, self.filename + '.redo')
-        os.replace(bakfn, self.filename)
-
-    ##  Restore the old version after an undo.
-
-    def redo (self):
-        redofn = self.filename + '.redo'
-        if not os.path.exists(redofn):
-            raise Exception('No redo information available')
-        bakfn = self.filename + '.bak'
-        if os.path.exists(self.filename):
-            if os.path.exists(bakfn):
-                os.unlink(bakfn)
-            os.replace(self.filename, bakfn)
-        os.replace(redofn, self.filename)
-
-
-##  Handles backup and locking.
+class Location (object):
 
-class BackingSave (object):
-
-    ##  Constructor.
-
-    def __init__ (self, fn, binary=False, makedirs=False):
-
-        ##  Filename.
-        self.filename = fn
+    ##  Constructor.  The filename may contain a * wildcard.  It will be
+    #   expanded out as the filename of an existing file.
 
-        ##  The file.
-        self.file = None
-
-        ##  Whether to create missing directories.
-        self.makedirs = makedirs
-
-        ##  Whether it is a binary file.
-        self.binary = binary
+    def __init__ (self, fn=None, user=None, host=None, pathname=None):
 
-        ##  Write to a temp file, only touch the protected file if all writes
-        #   complete successfully.
-        self.tmp = fn + '.tmp'
+        ##  May include ~ and *
+        self.orig_pathname = pathname
 
-        ##  The lock, while locked.
-        self.lock = None
+        if fn is None:
 
-    ##  Enter.  Create any missing directories.  Lock the file.
-    #   Open the temp file.  Return the temp file.
+            ##  The specified user name, None for a local file.
+            self.user = user
 
-    def __enter__ (self):
-        dir = os.path.dirname(self.filename)
-        # if filename contains no slash, dir is ''
-        if dir and not os.path.exists(dir):
-            if self.makedirs:
-                os.makedirs(dir)
-            else:
-                raise Exception('Directory does not exist: %s' % dir)
-        self.lock = open(self.filename + '.lock', 'w')
-        flock(self.lock, LOCK_EX)
-        if self.binary: mode = 'wb'
-        else: mode = 'w'
-        self.file = open(self.tmp, mode)
-        return self.file
+            ##  The specified host, None for a local file.
+            self.host = host
 
-    ##  Close the temp file.  If no error occurred, move the current
-    #   file to backup and move the temp file into its place.
-    #   If an error occurred, just delete the temp file.
-    #   Release the lock.
+            ##  The pathname, converted to absolute form.
+            self.pathname = pathname
 
-    def __exit__ (self, type, value, traceback):
-        self.file.close()
-        if type is None:
-            bak = self.filename + '.bak'
-            if os.path.exists(bak):
-                os.unlink(bak)
-            if os.path.exists(self.filename):
-                shutil.move(self.filename, bak)
-            shutil.move(self.tmp, self.filename)
         else:
-            if os.path.exists(self.tmp):
-                os.unlink(self.tmp)
-        self.lock.close()
+            if user or host or pathname:
+                raise Exception('Specify either fn or user-host-pathname')
 
+            i = fn.find('@')
+            j = fn.find(':')
+    
+            # No colon: local file
+            if j < 0:
+                if i >= 0:
+                    raise Exception('At-sign but no colon: ' + fn)
+                self.user = None
+                self.host = None
+                self.pathname = fn
+    
+            # Remote file
+            else:
+    
+                # User not specified: use current user
+                if i < 0:
+                    self.user = getpass.getuser()
+                    self.host = fn[:j]
+                else:
+                    self.user = fn[:i]
+                    self.host = fn[i+1:j]
+                self.pathname = fn[j+1:]
+
+        if self.host is None:
+            if self.pathname.startswith('~'):
+                fn = os.path.expanduser(self.pathname)
+            else:
+                fn = os.path.abspath(self.pathname)
+            self.pathname = instantiate_pathname(fn)
 
-#===============================================================================
-#  Formatted Files
-#
-
-#--  BaseFile  -----------------------------------------------------------------
-
-# Anything that File() should pass through unchanged
-
-class BaseFile (object):
-
-    def __iter__ (self): raise NotImplementedError
-    def store (self, contents, mode='w'): raise NotImplementedError
+    ##  String representation.
 
-    def append (self, contents):
-        self.store(contents, 'a')
+    def __repr__ (self):
+        if self.user is None: u = ''
+        elif isinstance(self.user, str): u = self.user + '@'
+        else: u = '<BAD USER>@'
+        if self.host is None: h = ''
+        elif isinstance(self.host, str): h = self.host + ':'
+        else: h = '<BAD HOST>:'
+        if self.pathname is None: p = '<NO PATHNAME>'
+        elif isinstance(self.pathname, str): p = self.pathname
+        else: p = '<BAD PATHNAME>'
+        return u + h + p
 
-    def writer (self):
-        return Writer(self)
+    ##  Join a component to create a new Location.
 
-    def __str__ (self):
-        bol = True
-        with StringIO() as f:
-            for elt in self:
-                if not bol:
-                    f.write('\n')
-                    bol = True
-                s = str(elt)
-                f.write(s)
-                if s and s[-1] != '\n':
-                    bol = False
-            return f.getvalue()
+    def join (self, cpt):
+        return Location(user=self.user, host=self.host, pathname=os.path.join(self.pathname, cpt))
 
+    ##  Slash is a synonym for join().
 
-# This collects all items into a list, then passes the entire list
-# the File's store() method.
-#
-# The alternative would be to run store() in a separate thread, but
-# that would reduce space needs at the cost of increased time overhead.
+    def __truediv__ (self, cpt):
+        return self.join(cpt)
 
-class Writer (object):
+    ##  Creates a new Location by concatenating the given string to the pathname.
+    #   Unlike join(), does not insert a slash.
 
-    def __init__ (self, f, mode='w'):
-        self._file = f
-        self._mode = mode
-        self._contents = []
+    def __add__ (self, suffix):
+        return Location(user=self.user, host=self.host, pathname=self.pathname+suffix)
 
-    def __enter__ (self):
-        return self
+    ##  Whether this Location is for a remote file.  Boolean not of is_local().
 
-    def __call__ (self, elt):
-        self._contents.append(elt)
+    def is_remote (self):
+        return bool(self.host)
 
-    def __exit__ (self, t, v, tb):
-        self._file.store(self._contents, self._mode)
+    ##  Whether this Location is for a local file.
 
+    def is_local (self):
+        return not self.host
 
-#--  File  ---------------------------------------------------------------------
-#
-#  A stream is just an iterator.
-#
-#  A source is just a stream.
-#
-#  A sink is a function that accepts a stream as input and consumes it.
-#
-#  A filter is a function that takes a stream as input and returns a stream.
+    ##  Raise an exception unless this Location is a local file.
 
-def File (filename=None, encoding='utf8', binary=False, contents=None, format=None):
-    f = _file1(filename, encoding, binary, contents)
-    if format is not None:
-        return FormattedFile(format, f)
-    else:
-        return f
+    def require_local (self):
+        if self.is_remote(): raise Exception('Not a local file: %s' % self)
 
-def _file1 (filename, encoding, binary, contents):
-    if not (filename is None or contents is None):
-        raise Exception('Cannot specify both filename and contents')
+    ##  Signals an error if not local.
+    #   Return is not guaranteed to be an *existing* file.
 
-    if filename is None:
-        if contents is None:
-            raise Exception('Must specify either filename or contents')
-        if binary:
-            raise Exception('Not implemented')
-        return FileFromString(contents)
+    def to_filename (self):
+        self.require_local()
+        return self.pathname
 
-    elif filename == '-':
-        return StdStream()
+    ##  Open the file.
 
-    elif isinstance(filename, str):
-        if re.match(r'[A-Za-z]+:', filename):
-            return URLStream(filename)
+    def open (self, mode='r', encoding=None, makedirs=False):
+        fn = self.to_filename()
+        if makedirs:
+            if not mode.startswith('w'):
+                raise Exception('Makedirs=True but mode is not w')
+            dir = os.path.dirname(fn)
+            if not os.path.exists(dir):
+                os.makedirs(dir)
+        return _open(fn, mode, encoding=encoding)
 
-        elif binary:
-            return BinaryFile(filename)
+    ##  Read the file.  Set encoding to 'bytes' to read a binary file.
 
+    def read (self, encoding=None):
+        if encoding == 'bytes':
+            mode = 'rb'
+            encoding = None
         else:
-            return RegularFile(filename, encoding)
-
-    elif isinstance(filename, BaseFile):
-        return filename
-
-    else:
-        raise Exception(f'Cannot coerce to file: {repr(filename)}')
+            mode = 'r'
+        with self.open(mode, encoding) as f:
+            return f.read()
 
+    ##  Returns a TabularFile.
 
-class FileFromString (BaseFile):
+    def tabular (self, mode='r', encoding=None, separator='\t'):
+        return TabularFile(self, mode, encoding, separator)
 
-    def __init__ (self, contents=''):
-        BaseFile.__init__(self)
-        self._contents = contents
-
-    def __iter__ (self):
-        with StringIO(self._contents) as f:
-            for line in f:
-                yield line
-
-    def store (self, lines, mode='w'):
-        with StringIO() as f:
-            if mode == 'a':
-                f.write(self._contents)
-            for line in lines:
-                f.write(line)
-            self._contents = f.getvalue()
+    ##  Calls load_dict() on the file.
 
-    def __str__ (self):
-        return self._contents
+    def dict (self):
+        return load_dict(str(self))
 
+    ##  Like dirname(), but returns a Location.
 
-class StdStream (BaseFile):
-
-    def __iter__ (self):
-        for line in sys.stdin:
-            yield line
-
-    def store (self, lines, mode='w'):
-        for line in lines:
-            sys.stdout.write(line)
-
-
-class URLStream (BaseFile):
-
-    def __init__ (self, url):
-        BaseFile.__init__(self)
-        self.url = url
+    def parent (self):
+        if (not self.pathname) or self.pathname == '/':
+            return None
+        else:
+            return Location(user=self.user, host=self.host,
+                            pathname=os.path.dirname(self.pathname))
 
-    def __iter__ (self):
-        bstream = urllib.request.urlopen(self.url, 'r')
-        reader = codecs.getreader(encoding)
-        with reader(bstream) as f:
-            for line in f:
-                yield line
+    ##  Like basename().  Returns a string.
 
-    def store (self, lines, mode='w'):
-        raise Exception('Cannot write to URLs')
-    
+    def name (self):
+        return os.path.basename(self.pathname)
 
-class RegularFile (BaseFile):
+    ##  Returns (parent, name) pair.  The parent is a Location, the name
+    #   is a string.
+
+    def split (self):
+        (dirname, name) = os.path.split(self.pathname)
+        return (Location(user=self.user, host=self.host, pathname=dirname),
+                name)
+
+    ##  Whether the file exists.
+
+    def exists (self):
+        return os.path.exists(self.to_filename())
+
+    ##  Whether the file is '/'.
+
+    def is_root (self):
+        return self.pathname == '/'
+
+    ##  Mac-specific.  If the filename begins with '/Volumes', check whether
+    #   the subdirectory within /Volumes exists.
+
+    def is_mounted (self):
+        if self.is_remote(): raise Exception('Not a local file')
+        f0 = self
+        f1 = f2 = None
+        while not f0.is_root():
+            f2 = f1
+            f1 = f0
+            f0 = f0.parent()
+            if f0 is None: return True
+        if f1.pathname == '/Volumes':
+            return f2 is not None and f2.exists()
+        else:
+            return True
 
-    def __init__ (self, fn, encoding):
-        BaseFile.__init__(self)
-        self.filename = expanduser(fn)
-        self.encoding = encoding
+    ##  Whether the file is a symbolic link.
 
-    def __iter__ (self):
-        if exists(self.filename):
-            with open(self.filename, 'r', encoding=self.encoding) as f:
-                for line in f:
-                    yield line
-
-    def store (self, lines, mode='w'):
-        with open(self.filename, mode, encoding=self.encoding) as f:
-            for line in lines:
-                f.write(line)
+    def islink (self):
+        os.path.islink(self.to_filename())
 
+    ##  Whether the file is a directory.
 
-class BinaryFile (BaseFile):
+    def isdir (self):
+        return os.path.isdir(self.to_filename())
 
-    def __init__ (self, fn):
-        BaseFile.__init__(self)
-        self.filename = fn
+    ##  Return an iteration over file names in this directory.
+    #   Raises an exception if this is a regular file.
 
-    def __iter__ (self):
-        with open(fn, 'rb') as f:
-            for line in f:
-                yield line
+    def listdir (self):
+        dir = self.to_filename()
+        if not os.path.exists(dir):
+            return iter([])
+        elif not os.path.isdir(dir):
+            raise Exception('Not a directory: %s' % self)
+        else:
+            return iter(os.listdir(dir))
 
-    def store (self, lines, mode='w'):
-        with open(fn, mode + 'b') as f:
-            for line in lines:
-                f.write(line)
+    ##  Like listdir(), but iterates over (name, loc) pairs.
 
+    def items (self):
+        for name in self.listdir():
+            yield (name, self.join(name))
 
-#--  Buffered  -----------------------------------------------------------------
+    ##  Returns the size of the file, in bytes.
 
-class Buffered (object):
+    def size (self):
+        return os.stat(self.to_filename()).st_size
 
-    def __init__ (self, stream):
-        self.stream = iter(stream)
-        self.buffer = []
+    ##  Returns the modification time of the file, in seconds since the epoch.
 
-    def __iter__ (self):
-        return self
-    
-    def __next__ (self):
-        if self.buffer:
-            return self.buffer.pop()
-        else:
-            return next(self.stream)
+    def modtime (self):
+        return os.stat(self.to_filename()).st_mtime
 
-    def pushback (self, item):
-        self.buffer.append(item)
+    ##  Returns the current user's relation to the file: 'owner', 'group', or 'other'.
 
-    def peek (self):
-        try:
-            item = self.__next__()
-            self.pushback(item)
-            return item
-        except StopIteration:
-            return StopIteration
+    def my_relation (self):
+        return self._my_relation1(os.stat(self.to_filename()))
 
+    def _my_relation1 (self, s):
+        if s.st_uid == os.getuid(): return 'owner'
+        elif s.st_gid in os.getgroups(): return 'group'
+        else: return 'other'
 
-#--  Format  ---------------------------------------------------------------
+    def _Xable (self, forwhom, u, g, o):
+        s = os.stat(self.to_filename())
+        m = s.st_mode
+        if forwhom == 'me': forwhom = self._my_relation1(s)
+        if forwhom == 'owner': return m & u
+        elif forwhom == 'group': return m & g
+        elif forwhom == 'other': return m & o
+        else: raise Exception('Bad forwhom: %s' % forwhom)
 
-class Format (object):
+    ##  Whether the file is readable.
 
-    def __init__ (self, read, render):
-        self.read = read
-        self.render = render
+    def readable (self, forwhom='me'):
+        return self._Xable(forwhom, stat.S_IRUSR, stat.S_IRGRP, stat.S_IROTH)
 
-    def __call__ (self, filename=None, encoding='utf8', binary=False, contents=None):
-        return FormattedFile(self, _file1(filename, encoding, binary, contents))
+    ##  Whether it is writable.
 
+    def writable (self, forwhom='me'):
+        return self._Xable(forwhom, stat.S_IWUSR, stat.S_IWGRP, stat.S_IWOTH)
 
-class FormattedFile (BaseFile):
+    ##  Whether it is executable.
 
-    def __init__ (self, fmt, f):
-        BaseFile.__init__(self)
-        self._format = fmt
-        self._file = f
+    def executable (self, forwhom='me'):
+        return self._Xable(forwhom, stat.S_IXUSR, stat.S_IXGRP, stat.S_IXOTH)
 
-    def format (self):
-        return self._format
+    ##  The permissions value: an int representing a 3-digit octal number.
 
-    def base (self):
-        return self._file
+    def permissions (self):
+        return stat.filemode(os.stat(self.to_filename()).st_mode)
 
-    def __iter__ (self):
-        return self._format.read(iter(self._file))
+    ##  The MD5 hash of the file.
 
-    def store (self, contents, mode='w'):
-        self._file.store(self._format.render(contents), mode)
+    def md5 (self, silent=False):
+        if not silent: print('Computing md5 hash for', self, '...', end='')
+        sys.stdout.flush()
+        s = subprocess.getoutput('openssl md5 < ' + self.to_filename())
+        if s.startswith('(stdin)= '):
+            s = s[9:]
+        if not silent: print(' ok')
+        return s
 
+    ##  Whether the file has dir as an ancestor.
 
-# class LoadableFormat (Format):
-# 
-#     pass
+    def is_under (self, dir):
+        return (self.host == dir.host and
+                self.user == dir.user and
+                self.pathname.startswith(dir.pathname))
+
+    ##  Execute the file using os.system().
+
+    def __call__ (self):
+        return os.system(self.to_filename()) == 0
+
+
+    #--  Modifications  --------------------
+
+    def _actionmask (self, s, action, forwhom):
+        w = 0
+        if isinstance(forwhom, str): forwhom = [forwhom]
+        for name in forwhom:
+            if name == 'me': name = self._my_relation1(s)
+            if name == 'all': w |= (stat.S_IRWXU | stat.S_IRWXG | stat.S_IRWXO)
+            elif name == 'owner': w |= stat.S_IRWXU
+            elif name == 'group': w |= stat.S_IRWXG
+            elif name == 'other': w |= stat.S_IRWXO
+            else: raise Exception('Bad name: %s' % name)
+        a = 0
+        if 'r' in action:
+            a |= (stat.S_IRUSR | stat.S_IRGRP | stat.S_IROTH)
+        if 'w' in action:
+            a |= (stat.S_IWUSR | stat.S_IWGRP | stat.S_IWOTH)
+        if 'x' in action:
+            a |= (stat.S_IXUSR | stat.S_IXGRP | stat.S_IXOTH)
+        return w & a
+
+    ##  Change permissions to allow the given action: 'r', 'w', 'x'.
+    #   @arg forwhom - may be 'me', 'owner', 'group', 'other', or 'all'.
+
+    def permit (self, action, forwhom='me', recurse=False, silent=False):
+        return self._chmod('permit', action, forwhom, recurse, silent)
+
+    ##  Change permissions to disallow the given action.
+
+    def deny (self, action, forwhom='all', recurse=False, silent=False):
+        return self._chmod('deny', action, forwhom, recurse, silent)
+
+    def _chmod (self, change, action, forwhom, recurse, silent):
+        if not silent: pprint(change.title(), self, action, forwhom)
+        fn = self.to_filename()
+        s = os.stat(fn, follow_symlinks=False)
+        mask = self._actionmask(s, action, forwhom)
+
+        # specifying 'me' on a recursive call chooses owner/group/other
+        # based on ownership of top file; may be wrong if lower files have
+        # different owners
+
+        if recurse and self.isdir():
+            for (dir, subdirs, files) in os.walk(fn):
+                self._chmod1(change, dir, mask)
+                for name in files:
+                    fn = os.path.join(dir, name)
+                    self._chmod1(change, fn, mask)
+        else:
+            self._chmod1(change, fn, mask, s)
         
+    def _chmod1 (self, change, fn, mask, s=None):
+        if s is None: s = os.stat(fn, follow_symlinks=False)
+        if change == 'permit': mode = (s.st_mode | mask)
+        elif change == 'deny': mode = (s.st_mode & ~mask)
+        else: raise Exception('Bad change: %s' % change)
+        os.chmod(fn, mode, follow_symlinks=False)
+
+    ##  Create any missing directories above this file.
+
+    def assure_parent (self):
+        dir = os.path.dirname(self.to_filename())
+        if not os.path.exists(dir):
+            os.makedirs(dir)
+
+    ##  Create this directory, including any missing directories above it.
+    #   Prints out a message.  Can get just the message and not the action
+    #   by setting DryRun = True.
+
+    def make_directory (self, silent=False):
+        global DryRun
+        if not self.exists():
+            if not silent: pprint('Make Directory', self)
+            fn = self.to_filename()
+            if DryRun: return
+            os.makedirs(fn)
+
+    ##  Copy this file to the target.  Can be disabled by DryRun.
+
+    def copy_to (self, tgt, silent=False):
+        global DryRun
+        if not silent: pprint('Copy File', self, tgt)
+        if self.is_remote() and tgt.is_remote():
+            raise Exception('Not implemented: copying remote to remote')
+        if DryRun: return
+        if self.is_remote():
+            server = _intern_server(self.host, self.user)
+            server.get(self.pathname, local=tgt.to_filename())
+        elif tgt.is_remote():
+            server = _intern_server(tgt.host, tgt.user)
+            server.put(self.to_filename(), remote=tgt.pathname)
+        else:
+            shutil.copyfile(self.to_filename(), tgt.to_filename())
 
+    ##  Copy the source file to this one.  Can be disabled by DryRun.
 
-Lines = Format(lambda x: x, lambda x: x)
+    def copy_from (self, src, silent=False):
+        src.copy_to(self, silent)
+    
+    ##  Rename this file.  Can be disabled by DryRun.
 
+    def move_to (self, tgt, silent=False):
+        global DryRun
+        if not silent: pprint('Move File', self, tgt)
+        if self.is_remote() or tgt.is_remote():
+            raise Exception('Only local moves are possible')
+        if DryRun: return
+        shutil.move(self.to_filename(), tgt.to_filename())
+
+    ##  Delete this file.  Can be disabled by DryRun.
+
+    def delete_file (self, silent=False):
+        if not silent: pprint('Delete File', self)
+        if DryRun: return
+        if self.is_remote():
+            server = _intern_server(self.host, self.user)
+            server('rm ' + self.pathname)
+        else:
+            os.unlink(self.to_filename())
+    
+    ##  Delete this directory, if it is empty, error otherwise.  Can be disabled
+    #   by DryRun.
 
-#--  Records  ------------------------------------------------------------------
+    def delete_empty_directory (self, silent=False):
+        if not silent: pprint('Delete Empty Directory', self)
+        if DryRun: return
+        if self.is_remote():
+            server = _intern_server(self.host, self.user)
+            server('rmdir ' + self.pathname)
+        else:
+            os.unlink(self.to_filename())
+    
+    ##  Delete the directory hierarchy rooted here.
+    #   Use with caution!
+    
+    def delete_hierarchy (self, silent=False):
+        if self.is_remote():
+            raise Exception('Not implemented: remote delete hierarchy')
+        if not silent: pprint('Delete Hierarchy', self)
+        top = self.to_filename()
+    
+        if DryRun: return
+    
+        if os.path.islink(top):
+            os.unlink(top)
+    
+        elif os.path.isdir(top):
+            for (dir, subdirs, files) in os.walk(top, topdown=False):
+                for name in files:
+                    fn = os.path.join(dir, name)
+                    os.unlink(fn)
+                # symbolic links to dirs show up here
+                for name in subdirs:
+                    fn = os.path.join(dir, name)
+                    if os.path.islink(fn):
+                        os.unlink(fn)
+                os.rmdir(dir)
 
-def lines_to_records (lines):
-    for line in lines:
-        line = line.rstrip('\r\n')
-        if line:
-            yield line.split('\t')
         else:
-            yield []
+            os.unlink(top)
 
-def records_to_lines (recs):
-    for rec in recs:
-        yield '\t'.join(rec) + '\r\n'
+    ##  Same as delete_hierarchy(), but no error if the directory has already
+    #   been deleted.  Also, refuses to delete the root directory.
 
-Tabular = Records = Format(lines_to_records, records_to_lines)
+    def clear (self, silent=False):
+        if self.is_local() and self.exists():
+            if not self.pathname or self.pathname == '/':
+                raise Exception('Attempt to delete root')
+            if self.isdir():
+                self.delete_hierarchy(silent)
+            else:
+                self.delete_file(silent)
 
+    ##  Same as clear(), but will even change the file permissions to override
+    #   the lack of write permission.  Use with extreme caution.
 
-#--  Simples  ------------------------------------------------------------------
-#
-# Works with any object that consists of a mix of strings, pairs whose first
-# element is a string, list-like objects, and dict-like objects.  A dict-like
-# object is anything that has an items() method, and a list-like object is
-# anything that has an __iter__() method but is not dict-like.
-#
-# When loading, the original objects are not reconstructed.  The value consists
-# of strings, pairs, lists and dicts.
+    def nuke (self, silent=False):
+        self.permit('w', 'me', recurse=True, silent=silent)
+        self.parent().permit('w', 'me', silent=silent)
+        self.clear(silent=silent)
 
-def lines_to_simples (lines):
-    return _lines_to_simples(iter(lines))
 
-def _lines_to_simples (lines, terminator=None):
-    try:
-        while True:
-            yield lines_to_simple(lines, terminator)
-    except StopIteration:
-        pass
+##  Expand out a wildcard (*) by looking for an existing file matching the pattern.
 
-def lines_to_simple (lines, terminator=None):
-    line = next(lines)
-    j = -1 if line.endswith('\n') else len(line)
-    if terminator and line == terminator:
-        raise StopIteration
-    elif line.startswith('|'):
-        return line[1:j]
-    elif line.startswith(':'):
-        key = line[1:j]
-        value = lines_to_simple(lines)
-        return (key, value)
-    elif line.startswith('{'):
-        return _make_dict(_lines_to_simples(lines, '}\n'))
-    elif line.startswith('['):
-        return list(_lines_to_simples(lines, ']\n'))
-    else:
-        raise Exception(f'Unexpected line: {repr(line)}')
+def instantiate_pathname (orig):
 
-def _make_dict (items):
-    d = {}
-    for item in items:
-        if not (isinstance(item, tuple) and len(item) == 2):
-            raise Exception(f'Expecting pairs: {repr(item)}')
-        (k,v) = item
-        d[k] = v
-    return d
+    # if the * is in a directory name, we want the unique directory, even
+    #     if the full pathname does not exist
+    # from the end, in case there are multiple wildcards
         
-def simples_to_lines (objs):
-    for obj in objs:
-        for line in simple_to_lines(obj):
-            yield line
-
-def simple_to_lines (obj):
-    if isinstance(obj, str):
-        yield '|' + obj + '\n'
-    elif isinstance(obj, dict):
-        yield '{\n'
-        for (k,v) in obj.items():
-            yield ':' + str(k) + '\n'
-            for line in simple_to_lines(v):
-                yield line
-        yield '}\n'
-    elif isinstance(obj, tuple) and len(obj) == 2 and isinstance(obj[0], str):
-        yield ':' + obj[0] + '\n'
-        for line in simple_to_lines(obj[1]):
-            yield line
-    elif isinstance(obj, list):
-        yield '[\n'
-        for elt in obj:
-            for line in simple_to_lines(elt):
-                yield line
-        yield ']\n'
+    i = orig.rfind('*')
+    if i < 0:
+        return orig
     else:
-        raise Exception(f'Not a simple: {repr(obj)}')
-            
-Simples = Format(lines_to_simples, simples_to_lines)
-
-
-#--  Blocks  -------------------------------------------------------------------
-
-def lines_to_blocks (lines):
-    return _records_to_blocks(lines_to_records(lines))
-
-def _records_to_blocks (records):
-    block = []
-    for r in records:
-        if r:
-           block.append(r)
-        elif block:
-            yield block
-            block = []
-    if block:
-        yield block
-
-def blocks_to_lines (blocks):
-    first = True
-    for block in blocks:
-        if first:
-            first = False
-        else:
-            yield '\n'
-        for record in block:
-            yield '\t'.join(record) + '\n'
-    
-Blocks = Format(lines_to_blocks, blocks_to_lines)
-
-
-#--  Dicts  --------------------------------------------------------------------
-
-def lines_to_dicts (lines):
-    d = {}
-    for line in lines:
-        line = line.rstrip('\r\n')
-        if line:
-            i = _first_space(line)
-            if i is None:
-                raise Exception(f'Missing value: {repr(line)}')
-            key = line[:i]
-            value = line[i+1:]
-            if key in d:
-                raise Exception(f'Duplicate key: {key}')
-            d[key] = value
+        j = orig.find('/', i+1)
+        if j > 0:
+            suffix = orig[j:]
+            fn = orig[:j]
         else:
-            yield d
-            d = {}
-    if d:
-        yield d
+            suffix = ''
+            fn = orig
+        alts = glob(fn)
+        if len(alts) != 1:
+            return orig
+        return alts[0] + suffix
+
+##  Returns the first pathname component.
+
+def first_component (fn):
+    i = fn.find('/')
+    if i < 0: return fn
+    else: return fn[:i]
+
+def _make_writable (self, fn):
+    if not os.path.islink(fn):
+        mode = os.lstat(fn).st_mode
+        os.chmod(fn, mode | 0o200)
 
-def _first_space (line):
-    for i in range(len(line)):
-        if line[i].isspace():
-            return i
+            
+##  Shorthand for Location.
+def L (s): return Location(s)
 
-def dicts_to_lines (dicts):
-    first = True
-    for d in dicts:
-        if first: first = False
-        else: yield '\n'
-        for (k,v) in d.items():
-            if not _spacefree(k):
-                raise Exception(f'Bad key: {repr(key)}')
-            yield k + ' ' + v
-        
-def _spacefree (key):
-    for i in range(len(key)):
-        if key[i].isspace():
-            return False
-    return True
+##  The Seal destination directory, as a Location.
+Dest = L(__dest__)
 
-Dicts = Format(lines_to_dicts, dicts_to_lines)
+##  The Seal python directory, as a Location.
+Seal = L(__seal__)
 
+##  The Seal bin directory, a Location.
+Bin = Dest/'bin'
 
-#--  ILines  -------------------------------------------------------------------
+##  The Seal examples directory, a Location.
+Examples = L(ex)
 
-def lines_to_ilines (lines):
-    for line in lines:
-        line = line.rstrip('\r\n')
-        i = 0
-        while i < len(line) and line[i] == ' ':
-            i += 1
-        yield (i, line[i:])
+##  The Seal data directory, a Location.
+Data = L(data)
 
-def ilines_to_lines (ilines):
-    for (ind, line) in ilines:
-        yield '  ' * ind + line + '\n'
+##  The /tmp directory, as a Location.
+Tmp = L('/tmp')
 
-ILines = Format(lines_to_ilines, ilines_to_lines)
 
+#--  TabularFile  --------------------------------------------------------------
 
-#--  NestedLists  --------------------------------------------------------------
-#
-# A block at indentation level i consists of a mix of lines at indentation i+1
-# and subblocks at indentation i+1.
-#
-# The toplevel elements are the elements of the (nonexistent) block at level -1.
+##  A tabular file.
 
-def lines_to_nested_lists (lines):
-    stream = Buffered(lines_to_ilines(lines))
-    lst = list(ilines_to_nested_list(stream, 0))
-    if lst:
-        yield lst
-
-def ilines_to_nested_list (ilines, indent):
-    for (ind, line) in ilines:
-        if ind < indent:
-            ilines.pushback((ind, line))
-            break
-        elif ind == indent:
-            yield line
-        else:
-            ilines.pushback((ind, line))
-            lst = list(ilines_to_nested_list(ilines, ind))
-            if lst:
-                yield lst
-        
-def nested_lists_to_lines (lst):
-    return ilines_to_lines(_nested_list_to_ilines(lst, 0))
-
-def _nested_list_to_ilines (lines, ind):
-    for line in lines:
-        if isinstance(line, str):
-            yield (ind, line)
-        else:
-            for iline in _nested_list_to_ilines(line, ind + 2):
-                yield iline
+class TabularFile (object):
 
-NestedLists = Format(lines_to_nested_lists, nested_lists_to_lines)
+    ##  Constructor.
+    #   Separator of None means any whitespace on read, single space on write.
 
+    def __init__ (self, loc, mode='r', encoding=None, separator='\t'):
 
-#--  Containers  ---------------------------------------------------------------
-
-def lines_to_containers (lines):
-    return nested_lists_to_containers(lines_to_nested_lists(lines))
-
-def nested_lists_to_containers (lists):
-    for lst in lists:
-        yield nested_list_to_container(list(lst))
-
-def nested_list_to_container (lst):
-    out = None
-    i = 0
-    while i < len(lst):
-        if isinstance(lst[i], list):
-            raise Exception('Embedded dict without a key')
-        elif i+1 < len(lst) and isinstance(lst[i+1], list):
-            out = _insert_item(lst[i], nested_list_to_container(lst[i+1]), dict, out)
-            i += 2
-        else:
-            line = lst[i].strip()
-            k = _first_space(line)
-            if k is None:
-                out = _insert_item(None, line, list, out)
-            else:
-                out = _insert_item(line[:k], line[k+1:].strip(), dict, out)
-            i += 1
-    return out
+        ##  Location.
+        self.location = loc
 
-def _insert_item (key, value, typ, out):
-    if out is None:
-        out = typ()
-    elif not isinstance(out, typ):
-        raise Exception(f'Inconsistent with {type(out)}: {key} {value}')
-    if key is None:
-        out.append(value)
-    elif key in out:
-        raise Exception(f'Duplicate key: {key}')
-    else:
-        out[key] = value
-    return out
+        ##  Mode.
+        self.mode = mode
 
-def containers_to_lines (conts):
-    for cont in conts:
-        for line in container_to_lines(cont):
-            yield line
-
-def container_to_lines (cont):
-    return ilines_to_lines(container_to_ilines(cont, 0))
-
-def container_to_ilines (cont, indent):
-    if isinstance(cont, dict):
-        for (k, v) in cont.items():
-            if isinstance(v, str):
-                yield (indent, k + ' ' + v)
-            elif isinstance(v, dict):
-                yield (indent, k)
-                for iline in container_to_ilines(v, indent+2):
-                    yield iline
-            else:
-                raise Exception(f'Unexpected value type: {repr(v)}')
-    elif isinstance(cont, list):
-        for v in cont:
-            if isinstance(v, str):
-                yield (indent, v)
-            else:
-                raise Exception('Lists may only contain strings')
+        ##  Character encoding.
+        self.encoding = encoding
 
+        ##  Field separator.
+        self.separator = separator
 
-Containers = Format(lines_to_containers, containers_to_lines)
+        ##  Stream.
+        self.file = None
 
-# 
-# #--  NestedDict  ---------------------------------------------------------------
-# 
-# def first_space (line):
-#     for (i, c) in enumerate(line):
-#         if c.isspace():
-#             return i
-#     return -1
-# 
-# # It would be more readable if this transformed the output of lines_to_nested_items,
-# # but maybe this way is more efficient
-# 
-# def lines_to_nested_dicts (lines):
-#     yield nested_items_to_nested_dict(lines_to_nested_items(lines))
-# 
-# def nested_items_to_nested_dict (items):
-#     if isinstance(items, str):
-#         return items
-#     elif isinstance(items, list):
-#         d = {}
-#         for (k1, v1) in nested_items_to_nested_dicts(v):
-#             if k1 in d:
-#                 raise Exception(f'Duplicate key: {repr(k1)}')
-#             d[k1] = v1
-#         return d
-# 
-# # Warning: if you convert multiple dicts to lines and then convert them
-# # back to dicts, you will get a single dict containing all items
-# 
-# def nested_dicts_to_lines (dicts):
-#     for d in dicts:
-#         for line in nested_dict_to_lines(d):
-#             yield line
-# 
-# def nested_dict_to_lines (d):
-#     return nested_items_to_lines(nested_dict_to_nested_items(d))
-# 
-# def nested_dict_to_nested_items (d):
-#     for (k, v) in d.items():
-#         if isinstance(v, str):
-#             yield (k, v)
-#         elif isinstance(v, dict):
-#             yield (k, list(nested_dict_to_nested_items(v)))
-#         else:
-#             raise Exception(f'Unexpected value type: {repr(v)}')
-# 
-# NestedDicts = Format(lines_to_nested_dicts, nested_dicts_to_lines)
-
-
-#--  Single  -------------------------------------------------------------------
-
-class Single (object):
-
-    def __init__ (self, f):
-        self._file = f
-
-    def load (self):
-        for elt in self._file:
-            return elt
-
-    def save (self, obj):
-        self._file.store([obj])
-
-
-def Simple (f):
-    return Single(Simples(f))
-
-
-#--  Container  ----------------------------------------------------------------
-
-class Container (object):
-
-    def __init__ (self, f):
-        self._file = Containers(f)
-        self._editing = False
-        self._contents = None
-        self.load()
-        if self._contents is None:
-            raise Exception('Implementation error: loading failed to set _contents')
-
-    # Returns the first element without checking whether there are more
-
-    def load (self):
-        isempty = True
-        for elt in self._file:
-            self._contents = elt
-            isempty = False
-            break
-        if isempty:
-            self._contents = {}
-
-    def save (self):
-        if not self._editing:
-            self._file.store([self._contents])
-
-    def edit (self):
-        return BatchEdit(self)
-
-    def __setitem__ (self, key, value):
-        self._contents[key] = value
-        self.save()
-
-    def __delitem__ (self, key):
-        del self._contents[key]
-        self.save()
-
-    def __getitem__ (self, att):
-        return self._contents[att]
-
-    def append (self, value):
-        self._contents.append(value)
-        self.save()
+    ##  Enter.
 
-    def __repr__ (self):
-        return repr(self._contents)
+    def __enter__ (self):
+        self.file = self.location.open(self.mode)
+        return self
 
+    ##  Exit.
 
-class BatchEdit (object):
+    def __exit__ (self, t, v, tr):
+        self.file.close()
+        self.file = None
 
-    def __init__ (self, tgt):
-        self._tgt = tgt
+    ##  Returns self.
 
-    def __enter__ (self):
-        self._tgt._editing = True
+    def __iter__ (self):
         return self
 
-    def __exit__ (self, t, v, tb):
-        self._tgt._editing = False
-        if not t:
-            self._tgt.save()
-
-
-# 
-# class Cell (object):
-# 
-#     def __init__ (self, array, i=0):
-#         if isinstance(array, BaseFile):
-#             array = Array(array)
-# 
-#         self._array = array
-#         self._i = i
-# 
-#     def get (self):
-#         return self._array[self._i]
-# 
-#     def set(self, value):
-#         self._array[self._i] = value
-# 
-#     def save (self):
-#         self._array.save()
-# 
-#     def __enter__ (self):
-#         return self
-# 
-#     def __exit__ (self, t, v, tb):
-#         if not t:
-#             self._array.save()
-# 
-
-# class SingletonFile (object):
-# 
-#     def load (self): raise NotImplementedError
-#     def save (self, contents): raise NotImplementedError
-# 
-#     def __iter__ (self):
-#         yield self.load()
-# 
-#     def store (self, contents):
-#         self.save(contents)
-# 
-# 
-# class LoadableFile (SingletonFile):
-# 
-#     def __init__ (self, fmt, f):
-#         SingletonFile.__init__(self)
-#         self._format = fmt
-#         self._file = f
-# 
-#     def load (self):
-#         return self._format.read(self._file)
-# 
-#     def save (self, contents):
-#         self._file.store(self._format.render(contents))
+    ##  Iterator method.
 
+    def __next__ (self):
+        return next(self.file).rstrip('\r\n').split(self.separator)
 
-#--  Tokens  -------------------------------------------------------------------
+    ##  Like print().
 
-# class Tokenizer (object):
-# 
-#     ##  Constructor.  Filename only for printing error messages; need not be genuine filename.
-# 
-#     def __init__ (self, filename, lines, syntax=DefaultSyntax):
-# 
-#         ##  A Syntax instance.
-#         self.syntax = syntax
-# 
-#         ##  Stack, for (possibly nested) temporary syntax changes.
-#         self.stack = []
-# 
-#         ##  Filename string; set even for streams not associated with files.
-#         self.filename = filename
-# 
-#         ##  The lines of the file.
-#         self.lines = lines
-# 
-#         ##  The current line.
-#         self.line = None
-# 
-#         ##  Current line number.
-#         self.linecount = 1
-# 
-#         ##  Current character offset on the line.
-#         self.offset = 0
-# 
-#         ##  Previous linecount.
-#         self.old_linecount = 1
-# 
-#         ##  Previous offset.
-#         self.old_offset = 0
-# 
-#         self.__token = None
-# 
-#         if self.lines: self.line = self.lines[0]
-#         else: self.line = ''
-# 
-#     ##  Returns self.
-# 
-#     def __iter__ (self):
-#         return self
-# 
-#     ##  Whether we are at EOF.
-# 
-#     def __bool__ (self):
-#         return self.token().type != 'eof'
-# 
-#     def __readline (self):
-#         if self.linecount < len(self.lines):
-#             self.line = self.lines[self.linecount]
-#             self.linecount += 1
-#         elif self.linecount == len(self.lines):
-#             self.line = ''
-#             self.linecount += 1
-#         else:
-#             raise Exception('Readline after EOF')
-#         self.offset = 0
-# 
-#     def __at_eof (self):
-#         return self.linecount > len(self.lines)
-# 
-#     def __empty_line (self):
-#         for c in self.line:
-#             if c in self.syntax.comments: return True
-#             elif not c.isspace(): return False
-#         return True
-# 
-#     def __is_special (self, c):
-#         if self.syntax.special is True:
-#             return not (c.isalnum() or c == '_')
-#         else:
-#             return c in self.syntax.special
-# 
-#     ##  Advance, if necessary, then return the current token.
-# 
-#     def token (self):
-#         if self.__token is None: self.__advance()
-#         return self.__token
-# 
-#     def __skip_eol (self):
-#         if self.offset >= len(self.line):
-#             if self.syntax.eol and not self.__empty_line():
-#                 self.__set_token('\n', self.offset, string='\n')
-#                 self.__readline()
-#             else:
-#                 while self.offset >= len(self.line):
-#                     if self.__at_eof():
-#                         self.__set_token('eof', self.offset)
-#                         break
-#                     self.__readline()
-# 
-#     def __advance (self):
-#         self.old_linecount = self.linecount
-#         self.old_offset = self.offset
-#         self.__token = None
-#         try:
-#             while self.__token is None:
-#                 self.__skip_eol()
-#                 if self.__token is not None: return
-#                 c = self.line[self.offset]
-# 
-#                 if c in self.syntax.multi_start and self.__scan_multi(): pass
-#                 elif c in self.syntax.comments: self.offset = len(self.line)
-#                 elif c == "'" or c == '"': self.__scan_quoted()
-#                 elif c.isspace(): self.offset += 1
-#                 elif self.__is_special(c): self.__scan_special()
-#                 elif self.syntax.digits and self.__is_digit(c): self.__scan_digit()
-#                 else: self.__scan_word()
-# 
-#         except StopIteration:
-#             raise Exception('[%s line %d offset %d] Unexpected eof' % \
-#                 (self.filename, self.linecount, self.offset))
-# 
-#     def __retreat (self):
-#         self.__token = None
-#         self.linecount = self.old_linecount
-#         self.offset = self.old_offset
-#         if self.linecount > 0:
-#             self.line = self.lines[self.linecount-1]
-#         else:
-#             self.line = None
-# 
-#     def __set_token (self, type, start, line=None, string=None, quotes=None):
-#         if line is None:
-#             line = self.linecount
-#         if string is None:
-#             string = self.line[start:self.offset]
-#         self.__token = Token(string)
-#         self.__token.type = type
-#         self.__token.filename = self.filename
-#         self.__token.line = line
-#         self.__token.offset = start
-#         self.__token.quotes = quotes
-# 
-#     def __is_digit (self, c):
-#         if c.isdigit(): return True
-#         i = self.offset + 1
-#         return c == '-' and i < len(self.line) and self.line[i].isdigit()
-# 
-#     def __scan_digit (self):
-#         start = self.offset
-#         if self.line[self.offset] == '-': self.offset += 1
-#         while self.offset < len(self.line) and self.line[self.offset].isdigit():
-#             self.offset += 1
-#         self.__set_token('digit', start)
-# 
-#     def __scan_word (self):
-#         start = self.offset
-#         while self.offset < len(self.line):
-#             c = self.line[self.offset]
-#             if c.isspace() or self.__is_special(c): break
-#             self.offset += 1
-#         self.__set_token('word', start)
-# 
-#     def __error (self, start, msg):
-#         raise Exception('[%s line %d char %d] %s' % \
-#             (self.filename, self.linecount, start, msg))
-# 
-#     def __scan_quoted (self):
-#         delim = self.line[self.offset]
-#         self.offset += 1
-#         start = self.offset
-#         restart = self.offset
-#         frags = []
-#         while True:
-#             while self.offset >= len(self.line):
-#                 if self.syntax.mlstrings:
-#                     if restart < len(self.line):
-#                         frags.append(self.line[restart:])
-#                     frags.append('\n')
-#                     self.__readline()
-#                     restart = self.offset
-#                     if self.__at_eof():
-#                         self.__error(start, 'Unterminated string at EOF')
-#                 else:
-#                     self.__error(start, 'End of line in string')
-#             c = self.line[self.offset]
-#             if c == delim:
-#                 frags.append(self.line[restart:self.offset])
-#                 self.offset += 1
-#                 break
-#             elif c == '\\' and self.syntax.backslash:
-#                 frags.append(self.line[restart:self.offset])
-#                 frags.append(self.__scan_escape_sequence())
-#                 restart = self.offset
-#             else:
-#                 self.offset += 1
-#         self.__set_token(self.syntax.stringtype, start, self.linecount, ''.join(frags), delim)
-# 
-#     def __scan_escape_sequence (self):
-#         # self.line[self.offset] is backslash
-#         self.offset += 1
-#         if self.offset >= len(self.line): self.__error('Bad escape sequence')
-#         c = self.line[self.offset]
-#         self.offset += 1
-#         if c == '\\' or c == '"' or c == "'": return c
-#         elif c == 'a': return '\a'
-#         elif c == 'b': return '\b'
-#         elif c == 'f': return '\f'
-#         elif c == 'n': return '\n'
-#         elif c == 'r': return '\r'
-#         elif c == 't': return '\t'
-#         elif c == 'u':
-#             i = self.offset
-#             self.offset += 4
-#             if self.offset > len(self.line): self.__error('Bad escape sequence')
-#             return chr(int(self.line[i:self.offset], 16))
-#         elif c == 'U':
-#             self.__error('\\U escapes not implemented')
-#         elif c == 'v': return '\v'
-#         elif '0' <= c <= '7':
-#             i = self.offset
-#             self.offset += 1
-#             n = 1
-#             while n < 3 and self.offset < len(self.line) and \
-#                     '0' <= self.line[self.offset] <= '7':
-#                 self.offset += 1
-#                 n += 1
-#             return chr(int(self.line[i:self.offset], 8))
-#         elif c == 'x':
-#             i = self.offset
-#             self.offset += 1
-#             if self.offset < len(self.line) and \
-#                     ('0' <= self.line[self.offset] <= '9' or \
-#                      'a' <= self.line[self.offset] <= 'f' or \
-#                      'A' <= self.line[self.offset] <= 'F'):
-#                 self.offset += 1
-#             d = int(self.line[i:self.offset], 16)
-#             if d < 0x100: return chr(d)
-#             else: return chr(d)
-# 
-#     def __scan_special (self):
-#         start = self.offset
-#         self.offset += 1
-#         self.__set_token(self.line[start], start)
-# 
-#     def __looking_at (self, word):
-#         for i in range(len(word)):
-#             t = self.offset + i
-#             if t >= len(self.line): return False
-#             if self.line[t] != word[i]: return False
-#         return True
-# 
-#     def __scan_multi (self):
-#         for word in self.syntax.multi:
-#             if self.__looking_at(word):
-#                 start = self.offset
-#                 self.offset += len(word)
-#                 self.__set_token(self.line[start:self.offset], start)
-#                 return True
-# 
-#     ##  Whether the next token is something other than EOF.
-#     #   If type or string is provided, the value indicates whether the next
-#     #   token has the given type and/or string.
-# 
-#     def has_next (self, type=None, string=None):
-#         if string:
-#             if type: raise Exception("Provide only one argument")
-#             return self.token() == string
-#         elif type:
-#             return self.token().hastype(type)
-#         else:
-#             return self.token().type != 'eof'
-# 
-#     ##  Iterator method.
-# 
-#     def __next__ (self):
-#         token = self.token()
-#         if token.type == 'eof': raise StopIteration
-#         self.__token = None
-#         self.old_linecount = self.linecount
-#         self.old_offset = self.offset
-#         return token
-# 
-#     ##  If the next token matches the given type and/or string, return it
-#     #   and advance.  Otherwise, return None.
-# 
-#     def accept (self, type=None, string=None):
-#         token = self.token()
-#         if type and not token.hastype(type):
-#             return None
-#         if string and not (token == string):
-#             return None
-#         return next(self)
-# 
-#     ##  If the next token has the given type and/or string, return it
-#     #   and advance.  Otherwise, signal an error.  Returns None at EOF.
-# 
-#     def require (self, type=None, string=None):
-#         token = self.token()
-#         if type and not token.hastype(type):
-#             token.error('Expecting ' + repr(type))
-#         if string and not (token == string):
-#             token.error('Expecting ' + repr(string))
-#         if type == 'eof': return None
-#         else: return next(self)
-# 
-#     ##  Signal an error, indicating filename and line number.
-# 
-#     def error (self, msg=None):
-#         token = self.token()
-#         token.error(msg)
-# 
-#     ##  Print a warning, showing filename and line number.
-# 
-#     def warn (self, msg=None):
-#         token = self.token()
-#         token.warn(msg)
-# 
-#     ##  Push the current syntax on the stack and switch to the given syntax.
-# 
-#     def push_syntax (self, syntax):
-#         self.stack.append(self.syntax)
-#         self.syntax = syntax
-#         self.__retreat()
-# 
-#     ##  Restore the previous syntax from the stack.
-# 
-#     def pop_syntax (self):
-#         if not self.stack: raise Exception('Empty stack')
-#         self.syntax = self.stack.pop()
-#         self.__retreat()
+    def write (self, *args):
+        sep = self.separator or ' '
+        last = len(args) - 1
+        for (i, arg) in enumerate(args):
+            self.file.write(str(arg))
+            if i == last: self.file.write('\n')
+            else: self.file.write(sep)
 
 
+#--  Open  ---------------------------------------------------------------------
 
-#--  pprint  -------------------------------------------------------------------
+##  Wraps around stdin or stdout.
 
-##  A PPrinter instance.
-pprint = None
+class PseudoFile (object):
 
+    ##  Constructor.
 
-##  Indentation for a PPrinter.
+    def __init__ (self, file):
+        ##  File.
+        self.file = file
 
-class PPrintIndent (object):
+    ##  Write to the file.
 
-    ##  Constructor.
+    def write (self, s):
+        self.file.write(s)
 
-    def __init__ (self, pprinter, n):
+    ##  Returns self.
 
-        ##  The pprinter.
-        self.pprinter = pprinter
+    def __iter__ (self):
+        return self
 
-        ##  The number of spaces indented by.
-        self.n = n
+    ##  Iterator method.
+
+    def __next__ (self):
+        return self.file.__next__()
 
     ##  Enter.
 
     def __enter__ (self):
-        self.pprinter._indent += self.n
+        return self
 
     ##  Exit.
 
-    def __exit__ (self, t, v, tb):
-        self.pprinter._indent -= self.n
-        
-
-##  A color for a PPrinter.
-
-class PPrintColor (object):
-
-    ##  Constructor.
-
-    def __init__ (self, pprinter, color):
-
-        ##  The pprinter.
-        self.pprinter = pprinter
-
-        ##  The color.
-        self.color = color
-
-        ##  Saves the previous color.
-        self.prevcolor = None
-
-    def _set_color (self, color):
-        self.pprinter._color = color
-        sys.stdout.write(fg[color])
-        sys.stdout.flush()
+    def __exit__ (self, t, v, tr):
+        pass
 
-    ##  Enter.
 
-    def __enter__ (self):
-        self.prevcolor = self.pprinter._color or 'default'
-        self._set_color(self.color)
+##  Accepts '-' as filename, representing stdin/stdout.
 
-    ##  Exit.
+def open (fn, mode='r'):
+    if fn == '-':
+        if mode.startswith('r'): return PseudoFile(sys.stdin)
+        else: return PseudoFile(sys.stdout)
+    else:
+        return _open(fn, mode)
 
-    def __exit__ (self, t, v, tb):
-        self._set_color(self.prevcolor)
 
+#--  BackingSave  --------------------------------------------------------------
 
-##  A pretty-printer.
+##  Handles locking (only).
 
-class PPrinter (object):
+class BackingAdmin (object):
 
     ##  Constructor.
 
-    def __init__ (self, file=None):
-        self._color = None
-        self._indent = 0
-        self._atbol = True
-        self._brflag = False
-        self._file = file
-    
-    ##  String representation.
-
-    def __repr__ (self):
-        return '<PPrinter %s>' % repr(self._file)
-
-    ##  The protected file.
+    def __init__ (self, fn):
 
-    def file (self):
-        if self._file is None: return sys.stdout
-        else: return self._file
+        ##  The filename.
+        self.filename = fn
 
-    ##  Returns an indentation.  Calling this in a with-statement causes the
-    #   indentation to be active within the body.
+        ##  The lock, when locked.
+        self.lock = None
 
-    def indent (self, n=2):
-        return PPrintIndent(self, n)
+    ##  Lock the file.
 
-    ##  Start an indentation.  One should usually do "with pp.indent()" instead.
+    def __enter__ (self):
+        self.lock = open(fn + '.lock', 'w')
+        flock(self.lock, LOCK_EX)
+        return self
 
-    def start_indent (self, n=2):
-        self._indent += n
-    
-    ##  End an indentation.
+    ##  Release the lock.
 
-    def end_indent (self, n=2):
-        self._indent -= n
-        if self._indent < 0: self._indent = 0
+    def __exit__ (self, type, value, tb):
+        self.lock.close()
     
-    ##  Freshline.
-
-    def br (self):
-        self._brflag = True
+    ##  Replace the file with the backup version.
 
-    ##  Returns a color.  Calling this in a with-statement causes the color
-    #   to be used in the body.
+    def undo (self):
+        bakfn = self.filename + '.bak'
+        if not os.path.exists(bakfn):
+            raise Exception('No undo information available: %s' % fn)
+        if os.path.exists(self.filename):
+            os.replace(self.filename, self.filename + '.redo')
+        os.replace(bakfn, self.filename)
 
-    def color (self, c):
-        return PPrintColor(self, c)
+    ##  Restore the old version after an undo.
 
-    ##  Like print().  Handles embedded newlines correctly.
+    def redo (self):
+        redofn = self.filename + '.redo'
+        if not os.path.exists(redofn):
+            raise Exception('No redo information available')
+        bakfn = self.filename + '.bak'
+        if os.path.exists(self.filename):
+            if os.path.exists(bakfn):
+                os.unlink(bakfn)
+            os.replace(self.filename, bakfn)
+        os.replace(redofn, self.filename)
 
-    def __call__ (self, *args, end=None, color=None):
-        if color is None:
-            self._call1(args, end)
-        else:
-            with self.color(color):
-                self._call1(args, end)
-                
-    def _call1 (self, args, end):
-        if end is None and (len(args) == 0 or not hasattr(args[-1], '__pprint__')):
-            end = '\n'
-        first = True
-        for arg in args:
-            if first: first = False
-            else: self.file().write(' ')
-            self._printarg(arg)
-        if end:
-            self._printarg(end)
 
-    def _printarg (self, arg):
-        if hasattr(arg, '__pprint__'):
-            arg.__pprint__()
-        else:
-            self.write(str(arg))
+##  Handles backup and locking.
 
-    ##  Write a string.
+class BackingSave (object):
 
-    def write (self, s):
-        f = self.file()
-        i = 0
-        n = len(s)
-        while i < n:
-            j = s.find('\n', i)
-            if j < 0: j = n
-            # it is possible that s[0] == '\n'
-            if i < j:
-                if self._brflag and not self._atbol:
-                    f.write('\n')
-                    self._atbol = True
-                if self._atbol:
-                    f.write(' ' * self._indent)
-                f.write(s[i:j].replace('\x1b', '\\x1b'))
-                self._atbol = False
-            # if j < n then s[j] == '\n'
-            if j < n:
-                f.write('\n')
-                j += 1
-                self._atbol = True
-            i = j
-    
-    ##  Emit a newline, unless the last character printed was a newline.
+    ##  Constructor.
 
-    def freshline (self):
-        if not self._atbol:
-            self.write('\n')
+    def __init__ (self, fn, binary=False, makedirs=False):
 
-    ##  Print and immediately flush.
+        ##  Filename.
+        self.filename = fn
 
-    def now (self, *args, end=''):
-        self.__call__(*args, end)
-        self.file().flush()
-    
-    ##  Flush the output.
+        ##  The file.
+        self.file = None
 
-    def flush (self):
-        self.file().flush()
+        ##  Whether to create missing directories.
+        self.makedirs = makedirs
 
+        ##  Whether it is a binary file.
+        self.binary = binary
 
-pprint = PPrinter()
+        ##  Write to a temp file, only touch the protected file if all writes
+        #   complete successfully.
+        self.tmp = fn + '.tmp'
 
+        ##  The lock, while locked.
+        self.lock = None
 
-#--  redirect  -----------------------------------------------------------------
-#
-# with redirect() as f:
-#     pprint('foo')
-#     with pprint.indent():
-#         pprint('bar')
-#     return str(f)
-#
+    ##  Enter.  Create any missing directories.  Lock the file.
+    #   Open the temp file.  Return the temp file.
 
-class redirect (object):
+    def __enter__ (self):
+        dir = os.path.dirname(self.filename)
+        # if filename contains no slash, dir is ''
+        if dir and not os.path.exists(dir):
+            if self.makedirs:
+                os.makedirs(dir)
+            else:
+                raise Exception('Directory does not exist: %s' % dir)
+        self.lock = open(self.filename + '.lock', 'w')
+        flock(self.lock, LOCK_EX)
+        if self.binary: mode = 'wb'
+        else: mode = 'w'
+        self.file = open(self.tmp, mode)
+        return self.file
 
-    def __init__ (self, filename=None, mode='w', stderr=False):
-        self.filename = filename
-        self.mode = mode
-        self._redirect_stderr = stderr
-        self._file = None
-        self._old_stdout = None
-        self._old_stderr = None
+    ##  Close the temp file.  If no error occurred, move the current
+    #   file to backup and move the temp file into its place.
+    #   If an error occurred, just delete the temp file.
+    #   Release the lock.
 
-    def __enter__ (self):
-        if self.filename is None:
-            self._file = StringIO()
+    def __exit__ (self, type, value, traceback):
+        self.file.close()
+        if type is None:
+            bak = self.filename + '.bak'
+            if os.path.exists(bak):
+                os.unlink(bak)
+            if os.path.exists(self.filename):
+                shutil.move(self.filename, bak)
+            shutil.move(self.tmp, self.filename)
         else:
-            self._file = open(self.filename, self.mode)
-        self._file.__enter__()
-        self._old_stdout = sys.stdout
-        sys.stdout = self._file
-        if self._redirect_stderr:
-            self._old_stderr = sys.stderr
-            sys.stderr = self._file
-        return self
+            if os.path.exists(self.tmp):
+                os.unlink(self.tmp)
+        self.lock.close()
 
-    def __str__ (self):
-        if self.filename is None and self._file is not None:
-            return self._file.getvalue()
-        else:
-            return f'redirect({self.filename}, {self.mode})'
-            
-    def __exit__ (self, t, v, tb):
-        sys.stdout = self._old_stdout
-        if self._redirect_stderr:
-            sys.stderr = self._old_stderr
-        return self._file.__exit__(t, v, tb)
```

### Comparing `selkie-0.24.dev3/src/selkie/reflect.py` & `selkie-0.25/src/selkie/pyx/reflect.py`

 * *Files identical despite different names*

### Comparing `selkie-0.24.dev3/src/selkie/rom.py` & `selkie-0.25/src/selkie/corpus/rom.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,43 +62,23 @@
 #   value.
 #
 
 import os, codecs
 from os.path import exists
 from io import StringIO
 from codecs import CodecInfo
-from .io import ispathlike, Format
-from .com import shift
-from .data import path as datapath
-from . import config
+from ..pyx.io import ispathlike
+from ..pyx.formats import Format
+from ..pyx.com import shift
+from ..data import path as datapath
+from .. import config
 
 default_registry = None
 
 
-#--  Romanization file  --------------------------------------------------------
-
-def load_romfile (fn):
-    with open(fn, 'rb') as f:
-        return read_romfile(f)
-
-# Since this is returned from inside 'with open', it should not be a generator
-# that requires the file to be open
-
-def read_romfile (f):
-    return list(_read_romfile_1(f))
-
-def _read_romfile_1 (f):
-    for line in f:
-        line = line.rstrip(b'\r\n')
-        if line.startswith(b'#') or not line:
-            continue
-        (key, value) = line.split(b'\t')
-        yield (key, value)
-
-
 #--  Romanization  -------------------------------------------------------------
 
 ##  State in the romanization dictionary.
 
 class State (dict):
 
     ##  Constructor.
@@ -110,14 +90,37 @@
         self.value = None
 
 
 ##  A romanization.
 
 class Romanization (object):
 
+    ##  Signals an error if type is not 'rom'.
+
+    def check_type (self, type):
+        if type != 'rom':
+            raise Exception('Fails type check: %s %s' % (type, self))
+
+    ##  Read one from file.
+
+    def __read__ (self, f):
+        self._table = table = {}
+        for line in f:
+            (k,v) = line.rstrip('\r\n').split('\t')
+            table[k] = v
+        self._make_rom()
+
+    def _make_rom (self):
+        self._rom = rom = make_romanization(self.parent(), self.name())
+        decode = Decoder()
+        for (key, value) in self._table.items():
+            key = key.encode('ascii')
+            value = decode(value.encode('ascii'))
+            rom[key] = value
+
     ##  Constructor.
 
     def __init__ (self, name=None, fn=None):
 
         ##  Its name.
         self.name = name
 
@@ -165,30 +168,30 @@
 
     def __str__ (self):
         with open(self.filename) as f:
             return f.read()
 
     ##  Print out the state graph.
 
-    def print_graph (self):
+    def print_graph (self, file=None):
         todo = [self.start]
         stateno = {id(self.start): 1}
         while todo:
             q = todo[0]
             del todo[0]
-            print(stateno[id(q)])
+            print(stateno[id(q)], file=file)
             for c in sorted(q):
                 next = q[c]
                 j = id(next)
                 if j not in stateno:
                     stateno[j] = len(stateno)+1
                     todo.append(next)
-                print("   %d ('%s')" % (c, chr(c)), stateno[j])
+                print("   %d ('%s')" % (c, chr(c)), stateno[j], file=file)
             if q.value:
-                print('    value=', repr(q.value))
+                print('    value=', repr(q.value), file=file)
 
     ##  Match an input.  Returns a pair (j, value).
 
     def match (self, input, i=0):
         q = self.start
         value = None
         j = None
@@ -483,27 +486,40 @@
 #   Romanization and Decoder only use the methods get() and __getitem__().
 #   They are expected to return Romanizations.
 
 class Registry (object):
 
     ##  Constructor.
 
-    def __init__ (self, path):
+    def __init__ (self, path=None):
         # backwards compatibility
-        if isinstance(path, str):
-            path = [path]
-
-        for d in path:
-            assert ispathlike(d)
-
-        ##  A list of directory filenames to search for rom files.
-        self.path = path
-
-        ##  Cache romanizations that have been loaded.
-        #   A 'default' romanization is always available.
+        if path is not None:
+            if isinstance(path, str):
+                path = [path]
+            else:
+                path = list(path)
+            for d in path:
+                assert ispathlike(d)
+
+        self.orig_path = path
+        self.path = None
+        self.cache = {}
+
+        self.reset()
+
+    def reset (self):
+        if self.orig_path is None:
+            self.path = ['.']
+            try:
+                self.path.extend(config['data']['rompath'])
+            except:
+                pass
+            self.path.append(datapath('roms'))
+        else:
+            self.path = list(self.orig_path)
         self.cache = {'default': Romanization('default')}
 
     ##  Convert a name to a '.rom' filename that exists in one of the
     #   path directories.  Returns None if no existing rom file is found.
 
     def find_filename (self, name):
         for d in self.path:
@@ -552,27 +568,14 @@
     def __iter__ (self):
         for d in self.path:
             if os.path.exists(d):
                 for name in os.listdir(d):
                     if name.endswith('.rom'):
                         yield name[:-4]
 
-
-def _create_default_registry ():
-    path = ['.']
-    try:
-        path = config['data']['rompath']
-    except:
-        pass
-    path.append(datapath('roms'))
-    return Registry(path)
-    
-##  The seal registry.
-default_registry = _create_default_registry()
-
 ##  Backwards compatibility.
 
 def require_rom (name):
     global default_registry
     return default_registry[name]
 
 ##  Backwards compatibility.
@@ -602,19 +605,40 @@
     else:
         rom = default_registry.get(name)
         if rom:
             return CodecInfo(None,
                              rom.std_decoder,
                              name=name)
 
-codecs.register(find_codec)
+
+#--  Romanization file  --------------------------------------------------------
+
+def load_romfile (fn):
+    with open(fn, 'rb') as f:
+        return read_romfile(f)
+
+# Since this is returned from inside 'with open', it should not be a generator
+# that requires the file to be open
+
+def read_romfile (f):
+    return list(_read_romfile_1(f))
+
+def _read_romfile_1 (f):
+    for line in f:
+        line = line.rstrip(b'\r\n')
+        if line.startswith(b'#') or not line:
+            continue
+        (key, value) = line.split(b'\t')
+        yield (key, value)
 
 
-#--  RomFormat  ----------------------------------------------------------------
+#--  Initialize  ---------------------------------------------------------------
 
+default_registry = Registry()
+codecs.register(find_codec)
 RomFormat = Format(read_romfile, None)
 
 
 #--  Main  ---------------------------------------------------------------------
 
 ##  Main function.
 #   Argument: [INFILE].
```

### Comparing `selkie-0.24.dev3/src/selkie/seq.py` & `selkie-0.25/src/selkie/pyx/seq.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 from math import inf
 from itertools import islice
+from collections.abc import Sequence
 
 
 #--  Lists  --------------------------------------------------------------------
 
 def as_list (x):
     '''
     Converts x to a list.
@@ -340,22 +341,94 @@
             for i in range(n):
                 self.__buffer[i] = self.__buffer[self.__head + i]
             self.__head = 0
             self.__tail = n
         return elt
 
 
+
+#--  Index  --------------------------------------------------------------------
+
+class Index (dict):
+    '''
+    A specialization of dict in which keys are associated with lists of values
+    instead of single values. Setting a value actually appends it to the list
+    values. The method ``add()`` is available as a synonym. The method
+    ``count(key)`` returns the number of values for the given key, and
+    ``delete(key,val)`` deletes one of the values, leaving the others in place.
+    '''
+    ##  Constructor.
+
+    def __init__ (self, *pairs):
+        dict.__init__(self)
+        if len(pairs) == 1 and hasattr(pairs[0], '__next__'):
+            pairs = pairs[0]
+        for (k,v) in pairs:
+            self.add(k,v)
+
+    ##  Add a value.
+
+    def __setitem__ (self, key, value):
+        if key in self:
+            dict.__getitem__(self, key).append(value)
+        else:
+            dict.__setitem__(self, key, [value])
+
+    ##  Add a value.
+
+    def add (self, key, value):
+        self.__setitem__(key, value)
+
+    ##  Fetch a list of values.  Returns the empty list if the key is missing.
+
+    def __getitem__ (self, key):
+        if key in self:
+            return dict.__getitem__(self, key)
+        else:
+            return []
+
+    ##  Iterate over all values.
+
+    def itervalues (self):
+        for vlist in dict.values(self):
+            for v in vlist:
+                yield v
+
+    ##  Returns a list containing all values.
+
+    def values (self):
+        return list(self.itervalues())
+
+    ##  Returns the number of values for the given key.
+
+    def count (self, key):
+        return len(self[key])
+
+    ##  Deletes the given value.
+
+    def delete (self, key, value):
+        values = dict.__getitem__(self, key)
+        values.remove(value)
+        if not values: dict.__delitem__(self, key)
+
+    ##  String representation.
+
+    def __str__ (self):
+        lines = ['%s -> %s' % (k, str(self[k])) for k in sorted(self.keys())]
+        return '\n'.join(lines)
+
+
 #--  Iterables  ----------------------------------------------------------------
 
 def nth (iter, n):
     '''
     Returns the n-th item of iterable g, counting from 0, and counting from the
     current position of the iterator's "read head."  For example:
 
-    >>> from selkie.seq import nth
+    >>> from selkie.pyx.seq import nth
     >>> import itertools
     >>> c = itertools.count(0)
     >>> nth(c, 3)
     3
     >>> nth(c, 3)
     7
 
@@ -368,17 +441,17 @@
 
     >>> c = itertools.count(0)
     >>> next(itertools.islice(c, 3, 4))
     3
 
     One use of nth is to jump to problematic cases in a large
     iteration.  An idiom for finding such cases in the first place is the
-    following:
+    following::
 
-        for i, x in enumerate(myiteration):
+        for (i, x) in enumerate(myiteration):
             if isproblematic(x):
                 return i
 
     '''
     try:
         count = 0
         while count < n:
@@ -445,113 +518,59 @@
         if item in dict:
             dict[item] += 1
         else:
             dict[item] = 1
     return dict
 
 
-#--  ListProxy, MapProxy  ------------------------------------------------------
+#--  ListWrapper, MapWrapper  --------------------------------------------------
 
-class ListProxy (object):
+class LazyList (Sequence):
     '''
-    A mixin class. The implementing class should have a ``__list__()`` method
-    that returns the object contents as a list. Provides implementations of the
-    following methods:
-
-     * ``__iter__()``
-     * ``__contains__(v)``
-     * ``__getitem__(i)``
-     * ``__len__()``
-     * ``__repr__()``
-    
-    '''
-
-    def __iter__ (self):
-        return self.__list__().__iter__()
-        
-    def __contains__ (self, k):
-        return self.__list__().__contains__(k)
-
-    def __getitem__ (self, k):
-        return self.__list__().__getitem__(k)
-
-    def __len__ (self):
-        return self.__list__().__len__()
-
-    def __repr__ (self):
-        return self.__list__().__repr__()
-
-
-class MapProxy (object):
+    An abstract class. Its ``__init__()`` method requires an iterable. Elements
+    will be fetched from the iterable only on demand, so one should be cautious about
+    changing the underlying element source during the lifetime of the LazyList.
     '''
-    A mixin class. The implementing class should have a ``__map__()`` method
-    that returns the object contents as a map. Provides implementations of
-    the following methods:
-
-     * ``__iter__()``
-     * ``__len__()``
-     * ``__contains__(k)``
-     * ``__getitem__(k)``
-     * ``get(k)``
-     * ``keys()``
-     * ``values()``
-     * ``items()``
-     * ``__repr__()``
 
-    '''
+    def __init__ (self, iterable):
+        self.__expanded = []
+        self.__iter = iter(iterable)
 
     def __iter__ (self):
-        return iter(self.__map__())
-        
-    def __len__ (self):
-        return len(self.__map__())
-
-    def __contains__ (self, k):
-        return k in self.__map__()
-
-    def __getitem__ (self, k):
-        return self.__map__()[k]
-
-    def get (self, k, dflt=None):
-        return self.__map__().get(k, dflt)
-
-    def keys (self):
-        return self.__map__().keys()
+        return LazyListIterator(self)
 
-    def values (self):
-        return self.__map__().values()
+    def _fully_expanded (self):
+        return self.__iter is None
     
-    def items (self):
-        return self.__map__().items()
-
-    def __repr__ (self):
-        return self.__map__().__repr__()
-
-
-class LazyList (ListProxy):
-    '''
-    A mixin class. Its ``__init__()`` method requires a function that
-    returns an iteration. The function should return the same iteration
-    each time it is called. This mixin provides a ``__list__()`` method,
-    plus all methods provided by ListProxy.
-    '''
+    def _advance (self):
+        if self._fully_expanded():
+            raise IndexError('list index out of range')
+        try:
+            self.__expanded.append(next(self.__iter))
+        except StopIteration:
+            self.__iter = None
 
-    def __init__ (self, iterf):
-        self.__expanded = None
-        self.__iterf = iterf
-
-    def __list__ (self):
-        if self.__expanded is None:
-            self.__expanded = list(self.__iterf())
-        return self.__expanded
+    def __getitem__ (self, i):
+        while len(self.__expanded) <= i:
+            self._advance()
+        return self.__expanded[i]
 
-    def __iter__ (self):
-        if self.__expanded is None:
-            return self.__iterf()
-        else:
-            return iter(self.__expanded)
+    def __len__ (self):
+        while not self._fully_expanded():
+            self._advance()
+        return self.__expanded.__len__()
 
     def __repr__ (self):
-        if self.__expanded is None:
-            return '[...]'
-        else:
+        if self._fully_expanded():
             return repr(self.__expanded)
+        else:
+            with StringIO() as f:
+                f.write('[')
+                first = True
+                for item in self.__expanded:
+                    if first: first = False
+                    else: f.write(', ')
+                    f.write(repr(item))
+                if not self._fully_expanded():
+                    f.write(', ...')
+                f.write(']')
+                return f.getvalue()
```

### Comparing `selkie-0.24.dev3/src/selkie/string.py` & `selkie-0.25/src/selkie/pyx/string.py`

 * *Files identical despite different names*

### Comparing `selkie-0.24.dev3/src/selkie/xterm.py` & `selkie-0.25/src/selkie/pyx/xterm.py`

 * *Files identical despite different names*

### Comparing `selkie-0.24.dev3/src/selkie/data/roms/korean.rom` & `selkie-0.25/src/selkie/data/roms/korean.rom`

 * *Files identical despite different names*

### Comparing `selkie-0.24.dev3/src/selkie/data/roms/salish.rom` & `selkie-0.25/src/selkie/data/roms/salish.rom`

 * *Files identical despite different names*

### Comparing `selkie-0.24.dev3/.gitignore` & `selkie-0.25/.gitignore`

 * *Files identical despite different names*

### Comparing `selkie-0.24.dev3/PKG-INFO` & `selkie-0.25/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: selkie
-Version: 0.24.dev3
+Version: 0.25
 Summary: Natural language processing and digital language description
 Project-URL: Homepage, https://github.com/abney/selkie
 Project-URL: Bug Tracker, https://github.com/abney/selkie/issues
 Author-email: Steven Abney <abney@umich.edu>
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

