# Comparing `tmp/reader-toolbox-0.2.3.tar.gz` & `tmp/reader_toolbox-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reader-toolbox-0.2.3.tar", last modified: Wed May 31 14:33:38 2023, max compression
+gzip compressed data, was "reader_toolbox-0.9.tar", last modified: Sun May 12 15:15:41 2024, max compression
```

## Comparing `reader-toolbox-0.2.3.tar` & `reader_toolbox-0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-31 14:33:38.191029 reader-toolbox-0.2.3/
--rw-r--r--   0 eric       (501) staff       (20)    18092 2023-03-14 22:36:02.000000 reader-toolbox-0.2.3/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)     3174 2023-05-31 14:33:38.191115 reader-toolbox-0.2.3/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     2564 2023-03-14 22:36:02.000000 reader-toolbox-0.2.3/README.md
--rw-r--r--   0 eric       (501) staff       (20)       97 2023-03-14 22:36:03.000000 reader-toolbox-0.2.3/pyproject.toml
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-31 14:33:38.189328 reader-toolbox-0.2.3/rdr/
--rw-r--r--   0 eric       (501) staff       (20)   128860 2023-05-30 14:35:22.000000 reader-toolbox-0.2.3/rdr/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)    60186 2023-05-29 13:29:58.000000 reader-toolbox-0.2.3/rdr/rdr.py
--rw-r--r--   0 eric       (501) staff       (20)     4297 2023-03-14 22:36:03.000000 reader-toolbox-0.2.3/rdr/server.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-31 14:33:38.190836 reader-toolbox-0.2.3/reader_toolbox.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)     3174 2023-05-31 14:33:38.000000 reader-toolbox-0.2.3/reader_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      322 2023-05-31 14:33:38.000000 reader-toolbox-0.2.3/reader_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-05-31 14:33:38.000000 reader-toolbox-0.2.3/reader_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       36 2023-05-31 14:33:38.000000 reader-toolbox-0.2.3/reader_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 eric       (501) staff       (20)      236 2023-05-31 14:33:38.000000 reader-toolbox-0.2.3/reader_toolbox.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)        4 2023-05-31 14:33:38.000000 reader-toolbox-0.2.3/reader_toolbox.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)      645 2023-05-31 14:33:38.191559 reader-toolbox-0.2.3/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)      774 2023-03-14 23:00:04.000000 reader-toolbox-0.2.3/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-12 15:15:41.068383 reader_toolbox-0.9/
+-rw-r--r--   0 eric       (501) staff       (20)    18092 2023-03-14 22:36:02.000000 reader_toolbox-0.9/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)     3692 2024-05-12 15:15:41.068278 reader_toolbox-0.9/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     2564 2023-03-14 22:36:02.000000 reader_toolbox-0.9/README.md
+-rw-r--r--   0 eric       (501) staff       (20)       97 2023-03-14 22:36:03.000000 reader_toolbox-0.9/pyproject.toml
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-12 15:15:41.065945 reader_toolbox-0.9/rdr/
+-rw-r--r--   0 eric       (501) staff       (20)   141242 2024-05-12 15:12:04.000000 reader_toolbox-0.9/rdr/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)    61256 2024-01-22 13:35:12.000000 reader_toolbox-0.9/rdr/rdr.py
+-rw-r--r--   0 eric       (501) staff       (20)     4297 2023-03-14 22:36:03.000000 reader_toolbox-0.9/rdr/server.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-12 15:15:41.067810 reader_toolbox-0.9/reader_toolbox.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)     3692 2024-05-12 15:15:41.000000 reader_toolbox-0.9/reader_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)      322 2024-05-12 15:15:41.000000 reader_toolbox-0.9/reader_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2024-05-12 15:15:41.000000 reader_toolbox-0.9/reader_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       36 2024-05-12 15:15:41.000000 reader_toolbox-0.9/reader_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 eric       (501) staff       (20)      250 2024-05-12 15:15:41.000000 reader_toolbox-0.9/reader_toolbox.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)        4 2024-05-12 15:15:41.000000 reader_toolbox-0.9/reader_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 eric       (501) staff       (20)      643 2024-05-12 15:15:41.068859 reader_toolbox-0.9/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)      794 2024-05-12 15:12:35.000000 reader_toolbox-0.9/setup.py
```

### Comparing `reader-toolbox-0.2.3/LICENSE` & `reader_toolbox-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reader-toolbox-0.2.3/PKG-INFO` & `reader_toolbox-0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: reader-toolbox
-Version: 0.2.3
-Summary: A command-line interface for creating and interacting with Distant Reader data sets (a.k.a. study carrels)
-Home-page: https://github.com/ericleasemorgan/reader-toolbox
-Author: Eric Lease Morgan
-Author-email: emorgan@nd.edu
-Project-URL: Bug Tracker, https://github.com/ericleasemorgan/reader-toolbox/issues
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 
 # Distant Reader Toolbox
 
 A command-line interface for creating and interacting with [Distant Reader](https://distantreader.org) study carrels
```

### Comparing `reader-toolbox-0.2.3/README.md` & `reader_toolbox-0.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: reader-toolbox
+Version: 0.9
+Summary: A command-line interface for creating and interacting with Distant Reader data sets (a.k.a. study carrels)
+Home-page: https://github.com/ericleasemorgan/reader-toolbox
+Author: Eric Lease Morgan
+Author-email: emorgan@nd.edu
+Project-URL: Bug Tracker, https://github.com/ericleasemorgan/reader-toolbox/issues
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: catalogue>=1.0.0
+Requires-Dist: click>=7.1.2
+Requires-Dist: datasette>=0.55
+Requires-Dist: matplotlib>=3.4.2
+Requires-Dist: nltk>=3.6.2
+Requires-Dist: tika>=1.24
+Requires-Dist: pandas<=1.5.2
+Requires-Dist: requests>=2.26.0
+Requires-Dist: pytextrank>=3.2.2
+Requires-Dist: scikit-learn>=0.23.2
+Requires-Dist: scipy>=1.7.1
+Requires-Dist: srsly>=1.0.5
+Requires-Dist: textacy>=0.12.0
+Requires-Dist: pytextrank
+Requires-Dist: wordcloud
+Requires-Dist: networkx<=2.8.7
+Requires-Dist: gensim
+Requires-Dist: rdflib
+
 
 
 # Distant Reader Toolbox
 
 A command-line interface for creating and interacting with [Distant Reader](https://distantreader.org) study carrels
```

### Comparing `reader-toolbox-0.2.3/rdr/__init__.py` & `reader_toolbox-0.9/rdr/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,111 +32,228 @@
 CONFIGURATIONFILE    = '.rdrrc'
 READERLIBRARY        = 'reader-library'
 MALLETHOME           = 'mallet'
 TIKAHOME             = 'tika-server.jar'
 NOTEBOOKSHOME        = 'reader-notebooks'
 
 # remote library
-REMOTELIBRARY = 'https://distantreader.org'
-CARRELS       = 'stacks/carrels-legacy'
+REMOTELIBRARY = 'http://carrels.distantreader.org'
+CARRELS       = '/'
 
 # documentation
 DOCUMENTATION = 'https://reader-toolbox.readthedocs.io'
 
 # file system mappings
-AUTHORS              = 'reader.authors'
+AUTHORS              = 'carrel.authors'
 BIB                  = 'bib'
 BIBLIOGRAPHYHTML     = 'index.xhtml'
-BIBLIOGRAPHYJSON     = 'bibliography.json'
-BIBLIOGRAPHYTEXT     = 'bibliography.txt'
+BIBLIOGRAPHYJSON     = 'index.json'
+BIBLIOGRAPHYTEXT     = 'index.txt'
 BIGRAMSCLOUD         = 'bigrams-cloud.png'
 CACHE                = 'cache'
 CLUSTERCUBE          = 'cluster-cube.png'
 CLUSTERDENDROGRAM    = 'cluster-dendrogram.png'
-COLLOCATIONS         = 'reader.gml'
-CORPUS               = 'reader.txt'
-DATABASE             = 'reader.db'
+COLLOCATIONS         = 'carrel.gml'
+CORPUS               = 'carrel.txt'
+DATABASE             = 'carrel.db'
 ENTITIESANY          = 'entities-any.png'
 ENTITIESGPE          = 'entities-gpe.png'
 ENTITIESORG          = 'entities-org.png'
 ENTITIESPERSON       = 'entities-person.png'
 ETC                  = 'etc'
 FIGURES              = 'figures'
 HTM                  = 'htm'
-GML                  = 'reader.gml'
+GML                  = 'index.gml'
 INDEX                = 'index.htm'
-INDEXRDF                  = 'index.rdf'
+INDEXRDF             = 'index.rdf'
 KEYWORDSCLOUD        = 'keywords-cloud.png'
 LEXICON              = 'lexicon.txt'
 MANIFEST             = 'MANIFEST.xml'
 METADATA             = 'index.csv'
 POSADJ               = 'pos-adjective.png'
 POSADV               = 'pos-adverb.png'
 POSNOUN              = 'pos-noun.png'
 POSPRON              = 'pos-pronoun.png'
 POSPROPN             = 'pos-propernoun.png'
 POSVERB              = 'pos-verb.png'
 PROVENANCE           = 'index.tsv'
 READABILITYBOXPLOT   = 'readability-boxplot.png'
 READABILITYHISTOGRAM = 'readability-histogram.png'
-SENTENCES            = 'reader.sents'
+READMEFILE           = 'readme.txt'
+SENTENCES            = 'carrel.sents'
 SIZESBOXPLOT         = 'sizes-boxplot.png'
 SIZESHISTOGRAM       = 'sizes-histogram.png'
 STOPWORDS            = 'stopwords.txt'
 TXT                  = 'txt'
 UNIGRAMSCLOUD        = 'unigrams-cloud.png'
-VECTORS              = 'reader.vec'
+VECTORS              = 'carrel.vec'
 WRD                  = 'wrd'
-WRDS                 = 'reader.wrds'
+WRDS                 = 'carrel.wrds'
 ZIP                  = 'index.zip'
 
 # spacy langauge model
 MODELSMALL   = 'en_core_web_sm'
-MODELMEDIUM  = 'en_core_web_sm'
+MODELMEDIUM  = 'en_core_web_md'
 
 # mallet
 MALLETZIP = 'https://distantreader.org/apps/mallet.zip'
 MALLETBIN = 'bin/mallet'
 
 # tika server
 TIKADOWNLOAD = 'https://distantreader.org/apps/tika-server.jar'
 
 # xhtml template for bibliography (index.xhtml)
-XHTML = '''
-<!DOCTYPE html>
+XHTML = '''<!DOCTYPE html>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en">
 <head><title>Bibliography</title></head>
 <body style="margin:3%">
 <h1>Bibliography</h1>
 <p>This is an automatically generated bibliography describing the content of this study carrel.</p>
 <ol>##ITEMS##</ol>
 </body>
 </html>
 '''
 
+# readme.txt
+READMEWORDS = '''
+
+About Distant Reader Study Carrels
+==================================
+
+tl;dnr - Distant Reader study carrels are data sets, and they are designed to be read by computers as well as people.
+
+
+Introduction
+------------
+
+The Distant Reader takes a collection of texts as input, and it outputs data sets called "study carrels". This readme file elaborates on these ideas and thorugh the process addresses the question, "Why should I care?"
+
+
+Basic Layout
+------------
+
+
+Enhancements To The Basic Layout
+--------------------------------
+
+
+Desktop Applications
+--------------------
+
+There are quite a number of different desktop computer applications that can be used against study carrels, and they fall into a number of categories.
+
+
+Text Editors
+
+Text editors are not word processors. While text editors and word processors both work with text, the former are more about the manipulation of the text, and the later are more about graphic design. The overwhelming majority of data found in study carrels is in the form of plain text, and you will find the use of a descent text editor indispensible. Using a text editor, you can open and read just about any file found in a study carrel.
+
+A good text editor supports powerful find & replace functionality, supports regular expressions, has the ability to open mulit-megabyte files with ease, can turn on and off line wrapping, and the reads text files created by different computers. The following two text editors are recommended. Don't rely on Microsoft Word nor Google Docs, they are word processors.
+
+     BBEdit - https://www.barebones.com/products/bbedit/
+  NotePad++ - https://notepad-plus-plus.org/
+
+
+Word Cloud Applications
+
+The use of words clouds is often viewed as sophmoric. This is true becuase they are to often used to illustrate the frequency of all words in a text. On the other hand, if word clouds illustrate the frequencies of specific things -- keywords, parts-of-speech, or named entities -- then word clouds become much more complelling. After all, "A picture is worth a thousand words."
+
+A program called Wordle is an excellent word cloud program. It takes raw text as input. It also accepts delimited data as input. The resulting images are colorful, configurable, and exportable. Unfortunately, it is no longer supported; while it will run on most Macintosh comuters, it will no longer run (easily) on Windows computers. (I would pay a fee to have Wordle come back to life and brought up-to-date.) If Wordle does not work for you, then there are an abundance of Web-based word cloud application for use.
+
+  Wordle - https://web.archive.org/web/20191115162244/http://www.wordle.net/
+  
+
+Concordances
+
+Developed in the 13th Century, concordances are all but the oldest of text analysis techiques. They function like the rudimentary find function you see in many applications. Think control-f on steroids.
+
+Concordances locate a given word in a text, display the text surrounding the word, and help you understand what other words are used in the same context. After all, to paraphrase a linguist named John Firth, "One shall know a word by the company it keeps." The following is a link to a concordance application that is worth way more than what you pay for it, which is nothing.
+
+  AntConc - https://www.laurenceanthony.net/software/antconc/
+  
+
+Spreadsheet-Like Applications
+
+The overwhelming majority of the content found in study carrels is in the form of plain text, and most of this plain text is structured in the form of tab-delimited text files -- matrixes or sometimes called "data frames". These files are readable by any spreadsheet or database aplication. Microsoft Excel, Google Sheets, or Macintosh Numbers can import Reader study carrel delimited data, but these programs are more about numerical data and less about textual data.
+
+Thus, if you want to do analysis against Reader study carrel data, and if you do not want to write your own software, then the use of an analysis program called OpenRefine is highly recommended. OpenRefine eats delimited data for lunch. Once data is imported, OpenRefine supports powerful find & replace functions, counting & tabulating functions, faceting, sorting, exporting, etc. While text editors and concordances supplement traditional reading functions, OpenRefine supplements the process of understanding study carrels as data.
+
+  OpenRefine - https://openrefine.org/
+
+
+Topic Modeling Applications
+
+Topic modeling is a type of machine learning process called "clustering". Given an integer (I), a topic modeler will divide a corpus into I clusters, and each cluster is akin to a theme. Thus, after practicing with a topic modeler, you can address questions like: what are the things this corpus is about, to what degee are themes manifested across the corpus, and which documents are best reprsented by themes. After supplementing the corpus with metadata (authors, titles, dates, keywords, geners, etc.) Topic modeling becomes even more useful because you can address addtional questdions, such as: how did these themes ebb & flow over time, who wrote about what, and how is this style of writting different from that style of writing. 
+
+A venerable MALLET application is the grand-daddy of topic modeling tools, but is a command-line driven things. On the other hand, a program called Topic Modeling Tool, which is rooted in MALLET, brings topic modeling to the desktop. Like all the applications listed here, it requires practice to use well, but it works, it works quickly, and the data it outputs can be used in a myriad of ways.
+
+  Topic Modeling Tool - https://github.com/senderle/topic-modeling-tool
+  
+
+Network Analysis Applications
+
+Texts can be modeled in the form of networks -- nodes and edges. For example, there are authors (nodes), there are written works (additional nodes), and specific authors write specific works (edges). Similarly, there are works (nodes), there are keywords (additional nodes), and specific works are described with keywords (edges). Given these sorts of networks you can address -- and visualize -- all sorts of questions: who wrote what, what author wrote the most, what keywords dominate the collection, or what keywords are highly significant (central) to many works and therefore authors? 
+
+Network analysis is rooted in graph theory, and it is not a trivial process. On the other hand, a program called Gephi makes the process easier. Import one of any number of different graph formats or specifically shaped matrixes, apply any number layout options to visualize the graph, filter the graph, visualize again, apply clustering or calcuate graph characteristics, and visualize a third time. The process requires practice, some knowledge of graph theory, and an aesthetic sensibility. In the end, you will garnder a greater understanding of your carrel.
+
+  Gephi - https://gephi.org
+
+
+Command-Line (Shell) Interface
+------------------------------
+
+
+Reader Toolbox And Command-Line Interface
+------------------------------------------
+
+
+Reader Toolbox and the Python Application Programmer Interface
+--------------------------------------------------------------
+
+
+Write your own software
+-----------------------
+
+
+Summary
+-------
+
+
+--
+Eric Lease Morgan <emorgan@nd.edu>
+Navari Family Center for Digital Scholarship
+Hesburgh Libraries
+University of Notre Dame
+
+##DATE##
+
+
+'''
+
 # html template for summarize command
 TEMPLATE = '''
 <html>
 <head>
-<title>Index of ##CARREL##</title>
+<title>Simple summary of the Distant Reader study carrel named ##CARREL##</title>
 </head>
 <body style='margin: 7%'>
 
-	<h1>Index of ##CARREL##</h1>
+	<h1>Simple summary of the Distant Reader study carrel named ##CARREL##</h1>
+	
+	<p>Given a corpus of narrative text, the Distant Reader creates data sets -- affectionately called "study carrels" -- for the purposes of use &amp; understanding. By definition, data sets are designed to be computable, and this Web page is the result of one such computing process applied against the study carrel named <strong>##CARREL##</strong>. Here you will find a simple analysis of the carrel's extracted features. Use the features to characterize the content of the carrel, and use the features as a sort of back-of-the-book index as input for more in-depth use &amp; understanding. For more information, please see the <a href="./readme.txt">read me</a> file describing study carrels in greater detail.</p>
 
 	<h2>Basic characteristics</h2>
 
 		<table>
 		<tr><td>Creator</td><td>##CREATOR##</td></tr>
 		<tr><td>Date created</td><td>##DATECREATED##</td></tr>
 		<tr><td>Number of items</td><td>##ITEMS##</td></tr>
 		<tr><td>Number of words</td><td>##WORDS##</td></tr>
 		<tr><td>Average readability score</td><td>##FLESCH##</td></tr>
-		<tr><td>Bibliographics</td><td><a href="./etc/bibliography.txt">plain text</a>; <a href="./etc/bibliography.htm">HTML</a>; <a href="./etc/bibliography.json">JSON</a></td></tr>
-		<tr><td>Other files</td><td><a href="./etc/stopwords.txt">stopwords</a>; <a href="./etc/reader.txt">entire corpus</a></td></tr>
+		<tr><td>Bibliographics</td><td><a href="./index.txt">plain text</a>; <a href="./index.xhtml">HTML</a>; <a href="./index.json">JSON</a></td></tr>
+		<tr><td>Other files</td><td><a href="./etc/stopwords.txt">stopwords</a>; <a href="./etc/carrel.txt">entire corpus</a></td></tr>
 		</table>
 		
 		<h3>Sizes</h3>
 			<p style='text-align: center'>
 			<img src='./figures/sizes-boxplot.png' width='49%' /> <img src='./figures/sizes-histogram.png' width='49%' />
 			</p>
 
@@ -187,86 +304,18 @@
 			</table>
 
 		<h3>Keywords</h3>
 			<p style='text-align: center'>
 			<img src='./figures/keywords-cloud.png' width='66%' />
 			</p>
 
+	<h2>Next steps</h2>
+	
+		<p>For more information, please see the <a href="./readme.txt">read me</a> file describing study carrels in greater detail.</p>
 
-		<h3>Next steps</h3>
-
-		<p>
-		The next step is for you to ask yourself some sort of question, and apply it to this data set. There are quite a number of ways to do this.
-		</p>
-
-		<p>
-		The <a href="https://distantreader.org/">Distant Reader</a> and the <a href="https://reader-toolbox.readthedocs.io">Distant Reader Toolbox</a> take an almost arbitrary amount of text as input and output data sets -- affectionatly known as "study carrels". The contents of this page was created from a study carrel.
-		</p>
-
-		<p>
-		Each study carrel is constituted with the same set of folders and files. These folders and files contain "features" of the original documents such as parts-of-speech, named-entities, and statistically significant keywords. For example, all of the <a href="./cache/">original documents</a> have been saved in the cache folder, and all of the <a href="./txt/">plain-text versions of the original documents</a> have been saved in the txt directory. Since almost all of the files in a study carrel are either plain-text files or tab-delimited files, Distant Reader study carrels can be accessed and used by almost any text editor, word processor, spreadsheet, database, or analysis application. The following folders contain information of particular interest:
-		</p>
-
-		<ul>
-			<li><a href="./adr/">email addresses</a> (adr)</li>
-			<li><a href="./bib/">bibliographics</a> (bib)</li>
-			<li><a href="./cache/">original documents</a> (cache)</li>
-			<li><a href="./ent/">named-entities</a> (ent)</li>
-			<li><a href="./figures/">visualizations</a> (figures)</li>
-			<li><a href="./pos/">parts-of-speech</a> (pos)</li>
-			<li><a href="./txt/">plain-text versions of the cached documents</a> (txt)</li>
-			<li><a href="./urls/">universal resource locators</a> (urls)</li>
-			<li><a href="./wrd/">statistically significant keywords</a> (wrd)</li>
-		</ul>
-
-		<p>
-		There are a few files of note:
-		</p>
-
-		<ul>
-			<li><a href="./index.htm">this file</a> (index.htm)</li>
-			<li><a href="./etc/stopwords.txt">stopwords</a>, words of little interest (./etc/stopwords.txt)</li>
-			<li>a distillation of all the features in the form of an SQLite database (./etc/reader.db)</li>
-			<li><a href="./etc/reader.txt">the whole corpus as a single file</a> (./etc/reader.txt)</li>
-		</ul>
-
-		<p>
-		There are quite a number of graphical-user interface (GUI) applications you can apply to a carrel's content:
-		</p>
-
-		<ul>
-			<li>any text editor, and I recommend <a href="https://www.barebones.com/products/bbedit/">BBEdit</a> or <a href="https://notepad-plus-plus.org/">NotePad++</a></li>
-			<li><a href="https://web.archive.org/web/20191115162244/http://www.wordle.net/">Wordle</a> to create word clouds</li>
-			<li><a href="https://www.laurenceanthony.net/software/antconc/">AntConc</a> to do concordancing</li>
-			<li><a href="https://github.com/senderle/topic-modeling-tool">Topic Modeling Tool</a> for... topic modeling</li>
-			<li><a href="https://openrefine.org/">OpenRefine</a> to sort, filter, and normalize the tab-delimited files</li>
-			<li><a href="https://gephi.org">Gephi</a> to analyze and visualize network graphs</li>
-			<li>any SQLite client to query anything and everything</li>
-		</ul>
-
-		<p>
-		Finally, if you have Python installed, then you can install the Reader Toolbox (<code>pip install reader-toolbox</code>), and use the <code>rdr</code> command from the command line to do many of the things the GUI applications do and more. There is also a set of <a href="https://github.com/ericleasemorgan/reader-toolbox/tree/main/notebooks">Jupyter Notebooks</a> demonstrating how the Toolbox can be extended and used in conjunction with other Python modules (like Pandas, SQLite, WordNet, etc.).
-		</p>
-
-		<p>
-		For more information, please see the <a href="https://reader-toolbox.readthedocs.io">complete manual</a>.
-		</p>
-
-		<p>
-		<em>Happy reading!</em>
-		</p>
-
-		<hr />
-		
-		<p style='text-align:right'>
-		Eric Lease Morgan &lt;<a href="mailto:emorgan@nd.edu">emorgan@nd.edu</a>&gt;<br />
-		Navari Family Center for Digital Scholarship<br />
-		University of Notre Dame
-		</p>
-		
 </body>
 </html>
 '''
 
 # require
 import click
 
@@ -293,58 +342,62 @@
 	object = graph.query( sparql ).bindings[ 0 ][ 'object' ]
 	return object
 	
 
 # return the English label of a given object
 def rdfSearchForLabel ( graph, object ) :
 	sparql = 'SELECT ?label WHERE {<' + str( object ) + '> rdfs:label ?label . FILTER(LANG(?label) = "en")}'
-	label  = graph.query( sparql ).bindings[ 0 ][ 'label' ]
+	try : label  = graph.query( sparql ).bindings[ 0 ][ 'label' ]
+	except IndexError : label = 'nan'
 	return label
 
 	
 # given the name of a carrel, return GML
-def graph2gml( carrel, output='gml', save=False, erase=False ) :
+def graph2gml( carrel, output='gml', save=False, erase=False, localLibrary=None ) :
 
 	'''Given the name of a carrel, and an optional output type ('gml' or 'chart'), return GML or its visualization.'''
 	
 	# configure
 	FORMAT  = 'xml'
-	CARREL  = 'https://distantreader.org/carrel#'
+	CARREL  = 'http://carrels.distantreader.org/carrel#'
 	WDP     = 'http://www.wikidata.org/prop/direct/'
 	DCTITLE = 'http://purl.org/dc/terms/title'
 	OUTPUTS = [ 'gml', 'chart' ]
 	
 	# require
 	from rdflib.namespace import DCTERMS, RDFS
 	import networkx
 	import rdflib
 	import sys
+	from pathlib import Path
+	
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 	
 	# sanity check #0
 	if output not in OUTPUTS :
 	
 		click.echo( "Error: Unsupported value for output (" + str( output ) + "); exiting.", err=True )
 		exit()
 		
 	# sanity check #1
-	checkForCarrel( carrel )
+	checkForCarrel( carrel, localLibrary )
 	
 	# initialize
 	graph   = rdflib.Graph()
-	library = configuration( 'localLibrary' )
 
 	# sanity check #2
-	authors  = library/carrel/ETC/AUTHORS
-	keywords = library/carrel/ETC/WRDS
-	if not authors.exists()  : reconcile( carrel, 'authors' )
-	if not keywords.exists() : reconcile( carrel, 'keywords' )
+	authors  = localLibrary/carrel/ETC/AUTHORS
+	keywords = localLibrary/carrel/ETC/WRDS
+	if not authors.exists()  : reconcile( carrel, 'authors', localLibrary, erase=False )
+	if not keywords.exists() : reconcile( carrel, 'keywords', localLibrary, erase=False )
 
 	# more configuration and santity checks
-	rdf = library/carrel/INDEXRDF
-	if not rdf.exists() : carrel2graph( carrel )
+	rdf = localLibrary/carrel/INDEXRDF
+	if not rdf.exists() : carrel2graph( carrel, localLibrary )
 
 	# yet more initialization
 	graph  = graph.parse( rdf, format=FORMAT )
 	CARREL = rdflib.Namespace( CARREL )
 	WDP    = rdflib.Namespace( WDP )
 	nodes  = []
 	edges  = []
@@ -402,52 +455,129 @@
 
 	# GML output
 	if output == 'gml' :
 	
 		# save
 		if save == True :
 		
-			gml = library/carrel/ETC/GML
+			gml = localLibrary/carrel/GML
 			networkx.write_gml( graph, gml )
 
 		# send to STDOUT
 		else : networkx.write_gml( graph, sys.stdout.buffer )
 
 	# chart output
 	if output == 'chart' : click.echo( "Warning: The output value of chart is not implemented, yet.", err=True )
 
 
+# given the name of a carrel, output sentences
+def sentences( carrel, process='list', query='love', save=True ) :
+
+	# configure
+	PATTERN = '*.txt'
+	
+	# require
+	import rdr
+	import multiprocessing
+	from nltk.wsd import lesk
+
+	# configure
+	library   = configuration( 'localLibrary' )
+	filenames = library/carrel/rdr.TXT
+	sentences = library/carrel/( rdr.ETC )/( rdr.SENTENCES )
+
+	checkForCarrel( carrel )
+
+	if not sentences.exists() :
+	
+		# parallel process each plain text file in the given corpus
+		pool    = multiprocessing.Pool()
+		click.echo( 'Step #1 of 2: Reading sentences', err=True )
+		results = pool.starmap( rdr.extractSentences, [ [ filename ] for filename in filenames.glob( PATTERN ) ] )
+		pool.close()
+
+		# save the result
+		click.echo( 'Step #2 of 2: Saving sentences', err=True )
+		with open( sentences, 'w' ) as handle :
+
+			# get all sentences and process each one
+			for result in results :
+
+				# output
+				for sentence in result : handle.write( '%s\n' % sentence )
+
+		# done
+		click.echo( 'Done.', err=True )
+
+	if process == 'list' and save == False :
+		
+		# output each sentence
+		for sentence in Sentences( sentences ) : click.echo( sentence, nl=False )
+
+	if process == 'define' :
+	
+		# output each sentence
+		for sentence in Sentences( sentences ) : 
+		
+			# filter
+			if query in sentence :
+				
+				# disambiguate
+				synset = lesk( sentence.split(), query )
+	
+				# output, conditionally
+				if synset :
+	
+					# debug
+					click.echo( '       query: ' + query)
+					click.echo( '      synset: ' + synset.name() )
+					click.echo( '    sentence: ' + sentence, nl=False )
+					click.echo( '  definition: ' + synset.definition() )
+					click.echo()
+
+	if process == 'filter' :
+	
+		# output each sentence
+		for sentence in Sentences( sentences ) : 
+		
+			if query in sentence : click.echo( sentence, nl=False )
+
+
 # given the name of a carrel, create an RDF file describing it
-def carrel2graph( carrel ) :
+def carrel2graph( carrel, localLibrary=None ) :
 
 	'''Given the name of a carrel, create an RDF file (index.rdr) describing it.'''
 	
 	# configure
-	NAMESPACE = 'https://distantreader.org/carrel#'
+	NAMESPACE = 'http://carrels.distantreader.org/carrel#'
 	PREFIX    = 'carrel'
 	FORMAT    = 'xml'
-	GRAPHROOT = 'http://distantreader.org/stacks/carrels/'
+	GRAPHROOT = 'http://carrels.distantreader.org/'
 	CREATOR   = { 'name':"Eric Lease Morgan", 'qnumber':'https://www.wikidata.org/wiki/Q102275801' }
 	TEMPLATE  = '''PREFIX wd: <http://www.wikidata.org/entity/> CONSTRUCT { wd:##QNUMBER## ?p ?o } WHERE { SERVICE <https://query.wikidata.org/bigdata/namespace/wdq/sparql> { wd:##QNUMBER## ?p ?o }}'''
 	WIKIDATA  = 'http://www.wikidata.org/entity/'
 
 	# require
 	from rdflib           import Graph, URIRef, Literal, Namespace
 	from rdflib.namespace import RDF, DCTERMS, DCMITYPE, RDFS
 	import pandas as pd
 	import json
-
-	# sanity check
-	checkForCarrel( carrel )
+	import rdr
+	from pathlib import Path
 	
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
+	
+	# sanity check
+	checkForCarrel( carrel, localLibrary )
+
 	# initialize
 	studyCarrel = carrel
 	graph       = Graph()
 	CARREL      = Namespace( NAMESPACE )
-	library     = configuration( 'localLibrary' )
 	graph.bind( PREFIX, CARREL )
 
 	# denote a carrel and update the graph
 	carrel  = URIRef( GRAPHROOT + studyCarrel )
 	graph.add( ( carrel, RDF.type,        CARREL.carrel ) )
 	graph.add( ( carrel, RDF.type,        DCMITYPE.Dataset ) )
 	graph.add( ( carrel, RDF.type,        DCMITYPE.Collection ) )
@@ -455,29 +585,29 @@
 
 	# add the carrel's creator (me)
 	#qnumber = URIRef( CREATOR[ 'qnumber' ] )
 	#graph.add( ( carrel, DCTERMS.creator, qnumber ) )
 	#graph.add( ( qnumber, RDFS.label,     Literal( CREATOR[ 'name' ] ) ) )
 
 	# get provenance and extents...
-	dateCreated      = provenance( studyCarrel, 'dateCreated' )
-	process          = provenance( studyCarrel, 'process' )
-	totalSizeInItems = extents( studyCarrel,    'items' )
-	totalSizeInWords = extents( studyCarrel,    'words' )
-	averageFlesch    = extents( studyCarrel,    'flesch' )
+	dateCreated      = provenance( studyCarrel, 'dateCreated', localLibrary )
+	process          = provenance( studyCarrel, 'process', localLibrary )
+	totalSizeInItems = extents( studyCarrel,    'items', localLibrary )
+	totalSizeInWords = extents( studyCarrel,    'words', localLibrary )
+	averageFlesch    = extents( studyCarrel,    'flesch', localLibrary )
 
 	# ...and update the graph
 	graph.add( ( carrel, DCTERMS.created,            Literal( dateCreated ) ) )
 	graph.add( ( carrel, CARREL.hasCreationProcess,  Literal( process ) ) )
 	graph.add( ( carrel, CARREL.hasTotalSizeInItems, Literal( totalSizeInItems ) ) )
 	graph.add( ( carrel, CARREL.hasTotalSizeInWords, Literal( totalSizeInWords ) ) )
 	graph.add( ( carrel, CARREL.hasAverageFlesch,    Literal( averageFlesch ) ) )
 
 	# get the name of the keywords reconciliation file, and check
-	keywords = library/studyCarrel/ETC/WRDS
+	keywords = localLibrary/studyCarrel/ETC/WRDS
 	if not keywords.exists() :
 	
 		click.echo( "The keywords reconciliation file does not exist. Please create one. Exiting.", err=True )
 		exit()
 		
 	# reconciliation file exists
 	else :
@@ -494,15 +624,15 @@
 		# debug, create SPARQL query, search, get result, and update graph
 		click.echo( "Getting Wikidata for keyword " + qnumber + ' (#' + str( index + 1 ) + ' of ' + str( length) + ')', err=True )
 		sparql = TEMPLATE.replace( '##QNUMBER##', qnumber )
 		rdf    = graph.query( sparql ).serialize( format=FORMAT )
 		graph.parse( rdf, format=FORMAT )	
 
 	# get the name of the authors reconciliation file, and check
-	authors = library/studyCarrel/ETC/AUTHORS
+	authors = localLibrary/studyCarrel/ETC/AUTHORS
 	if not authors.exists() :
 	
 		click.echo( "The authors reconciliation file does not exist. Please create one. Exiting.", err=True )
 		exit()
 
 	# reconciliation file exists
 	else :
@@ -519,15 +649,15 @@
 		# debug, create SPARQL query, search, get result, and update graph
 		click.echo( "Getting Wikidata for author " + qnumber + ' (#' + str( index + 1 ) + ' of ' + str( length) + ')', err=True )
 		sparql = TEMPLATE.replace( '##QNUMBER##', qnumber )
 		rdf    = graph.query( sparql ).serialize( format=FORMAT )
 		graph.parse( rdf, format=FORMAT )	
 
 	# get and process each bibliographic item
-	bibliographics = json.loads( bibliography( studyCarrel, format='json' ) )
+	bibliographics = json.loads( bibliography( studyCarrel, localLibrary, format='json' ) )
 	length         = len( bibliographics )
 	for index, bibliographic in enumerate( bibliographics ) :
 		
 		# debug
 		click.echo( 'Adding item ' + str( index ) + ' of ' + str( length ) + '\r', nl=False, err=True )
 	
 		# get the item's id and update the graph
@@ -546,26 +676,27 @@
 				
 					# get the qnumber and update the graph, conditionally
 					qnumber = author[ 'qnumber' ]
 					if type( qnumber ) is str : graph.add( ( item, DCTERMS.creator, URIRef( WIKIDATA + qnumber ) ) )
 					else : graph.add( ( item, CARREL.hasAuthor, Literal( author[ 'author' ] ) ) )
 
 		# add title
-		graph.add( ( item, DCTERMS.title, Literal( bibliographic[ 'title' ] ) ) )
+		graph.add( ( item, DCTERMS.title, Literal( bibliographic[ 'id' ] ) ) )
 
 		# add date
 		graph.add( ( item, DCTERMS.date, Literal( bibliographic[ 'date' ] ) ) )
 
 		# add extents; using try is a hack for bogus data
 		try : graph.add( ( item, CARREL.hasFlesch, Literal( int( bibliographic[ 'flesch' ] ) ) ) )
 		except TypeError : continue
 		graph.add( ( item, CARREL.hasSizeInWords, Literal( int( bibliographic[ 'words' ] ) ) ) )
 
-		# add cache and plain text	
-		cache = URIRef( GRAPHROOT + studyCarrel + '/' + ( CACHE ) + '/' + idItem + bibliographic[ 'extension' ] )
+		# add cache and text
+		if bibliographic[ 'extension' ] : cache = URIRef( GRAPHROOT + studyCarrel + '/' + ( CACHE ) + '/' + idItem + bibliographic[ 'extension' ] )
+		else                            : cache = URIRef( GRAPHROOT + studyCarrel + '/' + ( CACHE ) + '/' + idItem )
 		text  = URIRef( GRAPHROOT + studyCarrel + '/' + ( TXT )   + '/' + idItem + '.txt' )
 		graph.add( ( item,  CARREL.hasCache,     cache ) )
 		graph.add( ( item,  CARREL.hasPlainText, text ) )
 		graph.add( ( cache, DCTERMS.type,        Literal( bibliographic[ 'mime' ] ) ) )
 		graph.add( ( text,  DCTERMS.type,        Literal( 'text/plain' ) ) )
 	
 		# process keywords, conditionally
@@ -580,130 +711,151 @@
 				
 					# get the qnumber and update the graph, conditionally
 					qnumber = keyword[ 'qnumber' ]
 					if type( qnumber ) is str : graph.add( ( item, DCTERMS.subject, URIRef( WIKIDATA + qnumber ) ) )
 					else : graph.add( ( item, CARREL.keyword, Literal( keyword[ 'keyword' ] ) ) )
 
 	# output and done
-	rdf = library/studyCarrel/INDEXRDF
+	rdf = localLibrary/studyCarrel/INDEXRDF
 	with open( rdf, 'w' ) as handle : handle.write( graph.serialize( format=FORMAT ) )
 
 
+
 # given a carrel and a type, (re-)create reconciliation file(s)
-def reconcile( carrel, type, erase=False ) :
+def reconcile( carrel, type, localLibrary=None, erase=False ) :
 
 	'''Given the name of a carrel and a type ('author' or 'keyword'), (re-)initialize a recoconciliation file'''
 
 	# configure
 	PATTERN  = '*'
 	AUTHORS  = [ 'id', 'author', 'qnumber' ]
 	KEYWORDS = [ 'id', 'keyword', 'qnumber' ]
 	TYPES    = [ 'authors', 'keywords' ]
 	
 	# require
 	from   glob import glob
+	from   pathlib import Path
 	import pandas as pd
 	import rdr
 	import sys
+	
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 
 	# sanity check #1
-	rdr.checkForCarrel( carrel )
-
+	checkForCarrel( carrel, localLibrary )
+	
 	# sanity check #2
 	if type not in TYPES :
 	
 		click.echo( "Error: Unknown value for type (" + str( type ) + "); exiting", err=True )
 		exit()
 	
 	# debug
 	click.echo( 'Reconciling ' + type + " of " + carrel, err=True )
 
 	# initialize
-	library  = rdr.configuration( 'localLibrary' )
-	authors  = library/carrel/( rdr.ETC )/( rdr.AUTHORS )
-	keywords = library/carrel/( rdr.ETC )/( rdr.WRDS )
+	authors  = localLibrary/carrel/( rdr.ETC )/( rdr.AUTHORS )
+	keywords = localLibrary/carrel/( rdr.ETC )/( rdr.WRDS )
+	with open( localLibrary/carrel/( rdr.ETC )/( rdr.STOPWORDS ) ) as handle : stopwords = handle.read().splitlines()	
 
 	# check whether or not we've already been here, and get files to reconcile, conditionally
 	if type == 'authors' :
 			
 		# check to see if the file ought to be overwritten
 		if authors.exists() and erase == False :
 	
 			click.echo( "Warning: Authors reconciliation exists and erase is false, thus, not overwriting; exiting.\n", err=True )
 			exit()
 	
 		# delete the existing reconcilation
 		else: authors.unlink( missing_ok=True )
 
 		# get the files to process
-		files = glob( str( library/carrel/( rdr.BIB )/PATTERN ) )
+		files = glob( str( localLibrary/carrel/( rdr.BIB )/PATTERN ) )
 
 	# check whether or we've already been here, and get files to reconcile, conditionally
 	if type == 'keywords' :
 			
 		# check to see if the file ought to be overwritten
 		if keywords.exists() and erase == False :
 	
 			click.echo( "Warning: Keywords reconciliation exists and erase is false, thus, not overwriting; exiting.\n", err=True )
 			exit()
 	
 		# delete the existing reconcilation
 		else: keywords.unlink( missing_ok=True )
 
 		# get the files to process
-		files   = glob( str( library/carrel/( rdr.WRD )/PATTERN ) )
+		files   = glob( str( localLibrary/carrel/( rdr.WRD )/PATTERN ) )
 
 	# create a dataframe of all records and process each; reconcile
+	# see: https://stackoverflow.com/questions/48023061/pandas-read-csv-eof-inside-string-starting-at-line
 	reconciliations = []
-	records         = pd.concat( ( pd.read_csv( file, sep='\t', dtype={ 'id': str } ) for file in files ) )
+	records         = pd.concat( ( pd.read_csv( file, quoting=3, sep='\t', dtype={ 'id': str } ) for file in files ) )
 	for index, record in records.iterrows() :
 	
+		
 		# reconcile; here is where we add qnumbers from a dictionary
-		if type == 'authors'  : reconciliation = [ record[ 'id' ], record[ 'author' ], '' ]
-		if type == 'keywords' : reconciliation = [ record[ 'id' ], record[ 'keyword' ], '' ]
+		if type == 'authors'  :
 		
-		# update
-		reconciliations.append( reconciliation )
+			reconciliation = [ record[ 'id' ], record[ 'author' ], '' ]
+			reconciliations.append( reconciliation )
+
+		if type == 'keywords' : 
+		
+			# check for stopwords
+			if record[ 'keyword' ] not in stopwords :
+			
+				reconciliation = [ record[ 'id' ], record[ 'keyword' ], '' ]
+				reconciliations.append( reconciliation )
 		
 	# create a dataframe of reconciliations, output, and done
 	if type == 'authors' :
 		reconciliations = pd.DataFrame( reconciliations, columns=AUTHORS )
 		with open( authors, 'w' ) as handle : handle.write( reconciliations.to_csv( sep='\t', index=False ) )
 
 	if type == 'keywords' :
 		reconciliations = pd.DataFrame( reconciliations, columns=KEYWORDS )
 		with open( keywords, 'w' ) as handle : handle.write( reconciliations.to_csv( sep='\t', index=False ) )
 
 
 # given the name of a carrel, create zip file (index.zip) in its root
-def carrel2zip( carrel ) :
+def carrel2zip( carrel, localLibrary=None ) :
 
 	'''Given then name of a carrel, create a zip file (index.zip)
 	in its root.'''
 
+	# configure
+	PERMISSION = 0o755
+
 	# I don't know were to require these, here or at the root?
-	from zipfile import ZipFile
+	from   pathlib import Path
+	from   zipfile import ZipFile
 	import os
-	import tempfile
+	import rdr
 	import shutil
+	import tempfile
 	
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
+
 	# sanity check
-	rdr.checkForCarrel( carrel )
+	rdr.checkForCarrel( carrel, localLibrary )
 	
 	# initialize
-	library = configuration( 'localLibrary' )
-	zip     = library/carrel/ZIP
+	zip     = localLibrary/carrel/ZIP
 	staging = tempfile.NamedTemporaryFile( delete=False ).name
 	
 	# debug
 	click.echo( "Creating archive (index.zip) file of " + carrel, err=True )
 	
 	# make sane
 	zip.unlink( missing_ok=True )
-	os.chdir( library )
+	os.chdir( localLibrary )
 	
 	# create an archive
 	with ZipFile( staging, 'w' ) as handle :
 
 		# find all files
 		for root, _, files in os.walk( carrel ) :
 
@@ -711,16 +863,18 @@
 			for file in files:
 			
 				# create full path name, debug, and do the work
 				file = os.path.join( root, file )
 				click.echo( file, err=True )
 				handle.write( file )
 
-	# put the archive into place
+	# put the archive into place and make it readable
 	shutil.move( staging, zip )
+	os.chmod( zip, PERMISSION )
+
 
 # given a sentence, parser, and lexicon return matching sentences
 def matchModal( sentence, parser, lexicon ) :
 		
 	'''Given a sentence, an NLTK RegexpParser object (a grammar), and a
 	lexicon (a set of strings), return the sentence if it matches the
 	object's grammar, otherwise return None.'''
@@ -918,22 +1072,28 @@
 	else : click.echo( '???' )
 	
 	# done
 	exit()
 
 
 # make sure a study carrel exists
-def checkForCarrel( carrel ) :
+def checkForCarrel( carrel, localLibrary=None ) :
 
 	'''Given the name of a study carrel, return True if it exists or False
 	if it does not, but really, if the carrel does not exist, then execution
 	is aborted.'''
 
+	# require
+	from pathlib import Path
+	
 	# initialize and do the work
-	directory = configuration( 'localLibrary' )/carrel
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
+	
+	directory = localLibrary/carrel
 	if not directory.is_dir() :
 		
 		# error
 		click.echo( ('''
   WARNING: The carrel, %s, does not seem to be in your local
   library. Are you sure you entered its name correctly? Try 'rdr
   catalog' to make sure.
@@ -982,28 +1142,32 @@
 		plt.show()
 
 	# done
 	return True
 
 
 # read and parse provenance data
-def provenance( carrel, field ) :
+def provenance( carrel, field, localLibrary=None ) :
 
 	'''Given the name of a study carrel and a provenance element (process,
 	originalID, dateCreated, timeCreated, creator, or input), return the
 	provenance value.'''
 	
+	# require
+	from pathlib import Path
+	
 	# initialize
-	locallibrary = configuration( 'localLibrary' )
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 	
 	# sanity check
-	checkForCarrel( carrel )
+	checkForCarrel( carrel, localLibrary )
 
 	# read provenance file
-	with open( locallibrary/carrel/PROVENANCE, encoding='utf-8'  ) as handle : provenance = handle.read().split( '\t' )
+	with open( localLibrary/carrel/PROVENANCE, encoding='utf-8'  ) as handle : provenance = handle.read().split( '\t' )
 	
 	# parse it
 	process     = provenance[ 0 ]
 	originalID  = provenance[ 1 ]
 	dateCreated = provenance[ 2 ]
 	timeCreated = provenance[ 3 ]
 	creator     = provenance[ 4 ]
@@ -1018,28 +1182,31 @@
 	elif field == 'input'       : value = input
 	
 	# done
 	return value
 	
 	
 # return various extents
-def extents( carrel, type ) :
+def extents( carrel, type, localLibrary=None ) :
 
 	'''Given the name of a study carrel and a type of extent (items, words,
 	or flesch) return the extent value.'''
 	
 	# require
 	import sqlite3
-
+	from pathlib import Path
+	
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
+	
 	# sanity check
-	checkForCarrel( carrel )
+	checkForCarrel( carrel, localLibrary )
 
 	# initialize
-	locallibrary           = configuration( 'localLibrary' )
-	connection             = sqlite3.connect( str( locallibrary/carrel/ETC/DATABASE )  )
+	connection             = sqlite3.connect( str( localLibrary/carrel/ETC/DATABASE )  )
 	connection.row_factory = sqlite3.Row
 
 	# get extents
 	sql = 'SELECT COUNT( id ) AS items, SUM( words ) AS words, AVG( flesch ) AS flesch FROM bib;'
 	rows = connection.execute( sql )
 	for row in rows :
 
@@ -1050,33 +1217,43 @@
 	if type == 'items'    : value = int( items )
 	elif type == 'words'  : value = int( words )
 	elif type == 'flesch' : value = int( flesch )
 	
 	return value
 
 
+# escape ampersands
+def escape( s ) :
+
+	from html import escape
+	if not s : return
+	return escape( s )
+
 # output a rudimentary bibliography
-def bibliography( carrel, format='text', save=False ) :
+def bibliography( carrel, localLibrary=None, format='text', save=False ) :
 
 	'''Given the name of a study carrel, and a format (text, html, or
 	json), create a rudimentary bibliography. If the value for save is
 	True, then the bibliography will be saved in the carrel's etc
 	directory/folder, otherwise the bibliography is returned.'''
 
 	# require
 	import sqlite3
 	from pathlib import Path
 	import json
 	
+	# initialize
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
+
 	# sanity check
-	checkForCarrel( carrel )
+	checkForCarrel( carrel, localLibrary )
 
 	# initialize
-	locallibrary           = configuration( 'localLibrary' )
-	connection             = sqlite3.connect( str( locallibrary/carrel/ETC/DATABASE )  )
+	connection             = sqlite3.connect( str( localLibrary/carrel/ETC/DATABASE )  )
 	connection.row_factory = sqlite3.Row
 
 	# query database
 	sql  = '''SELECT b.id, b.words, b.extension, b.flesch, b.author, b.title, b.date, GROUP_CONCAT( LOWER( w.keyword ), '; ') AS keywords, b.summary, b.mime
 			  FROM bib AS b, wrd AS w
 			  WHERE b.id = w.id
 			  GROUP BY b.id
@@ -1118,16 +1295,19 @@
 			
 			# build cache and plain text
 			#cache = str( locallibrary/carrel/CACHE/id ) + extension
 			#text  = str( locallibrary/carrel/TXT/id )   + '.txt'
 	
 			if format == 'text' :
 			
-				cache = str( locallibrary/carrel/CACHE/id ) + extension
-				text  = str( locallibrary/carrel/TXT/id )   + '.txt'
+				#cache = str( localLibrary/carrel/CACHE/id ) + extension
+				#text  = str( localLibrary/carrel/TXT/id )   + '.txt'
+				
+				cache = id + extension
+				text  = id + '.txt'
 				
 				# build the bibliography
 				bibliography = bibliography + ( '        item: #%s of %s\n' % ( str( item + 1 ), total ) )
 				bibliography = bibliography + ( '          id: %s\n' % id )
 				bibliography = bibliography + ( '      author: %s\n' % author )
 				bibliography = bibliography + ( '       title: %s\n' % title )
 				bibliography = bibliography + ( '        date: %s\n' % date )
@@ -1141,33 +1321,33 @@
 	
 			else :
 			
 				cache = './' + CACHE + '/' + id + extension
 				text  = './' + TXT + '/' + id + '.txt'
 				
 				item = '<ul>'
-				item = item + '<li>' + ( 'author: %s'    % author )   + '</li>'
-				item = item + '<li>' + ( 'title: %s'     % title )    + '</li>'
-				item = item + '<li>' + ( 'date: %s'      % date )     + '</li>'
-				item = item + '<li>' + ( 'words: %s'     % words )    + '</li>'
-				item = item + '<li>' + ( 'flesch: %s'    % flesch )   + '</li>'
-				item = item + '<li>' + ( 'summary: %s'   % summary )  + '</li>'
-				item = item + '<li>' + ( 'keywords: %s'  % keywords ) + '</li>'
-				item = item + '<li>' + ( 'versions: <a href="' + cache + '">original</a>; <a href="' + text + '">plain text</a>' ) + '</li>'
+				item = item + '<li>' + ( '<strong>author</strong>: %s'    % escape( author ) )   + '</li>'
+				item = item + '<li>' + ( '<strong>title</strong>: %s'     % escape( title ) )    + '</li>'
+				item = item + '<li>' + ( '<strong>date</strong>: %s'      % date )     + '</li>'
+				item = item + '<li>' + ( '<strong>words</strong>: %s'     % escape( words ) )    + '</li>'
+				item = item + '<li>' + ( '<strong>flesch</strong>: %s'    % flesch )   + '</li>'
+				item = item + '<li>' + ( '<strong>summary</strong>: %s'   % escape( summary ) )  + '</li>'
+				item = item + '<li>' + ( '<strong>keywords</strong>: %s'  % escape( keywords ) ) + '</li>'
+				item = item + '<li>' + ( '<strong>versions</strong>: <a href="' + escape( cache ) + '">original</a>; <a href="' + escape( text ) + '">plain text</a>' ) + '</li>'
 				item = item + '</ul>'
 				
 				items = items + "<li>" + id + item + "</li>"
 				
 	if format == 'html' : bibliography = template.replace( '##ITEMS##', items )
 	
 	if save :
 
-		if format == 'text' : file = locallibrary/carrel/ETC/BIBLIOGRAPHYTEXT
-		if format == 'html' : file = locallibrary/carrel/BIBLIOGRAPHYHTML
-		if format == 'json' : file = locallibrary/carrel/ETC/BIBLIOGRAPHYJSON
+		if format == 'text' : file = localLibrary/carrel/BIBLIOGRAPHYTEXT
+		if format == 'html' : file = localLibrary/carrel/BIBLIOGRAPHYHTML
+		if format == 'json' : file = localLibrary/carrel/BIBLIOGRAPHYJSON
 		
 		with open( file, 'w', encoding='utf-8' ) as handle : handle.write( bibliography )
 		
 	else : return bibliography
 	
 
 # get email addresses
@@ -1357,15 +1537,15 @@
 			for row in rows : items.append( "\t".join( [ row[ 'domain' ], str( row[ 'count' ] ) ] ) )
 			
 	# clean up and done
 	connection.close()
 	return '\n'.join( items )
 
 
-def keywords( carrel, count=False, wordcloud=False, save=False ) :
+def keywords( carrel, localLibrary=None, count=False, wordcloud=False, save=False ) :
 
 	'''Given the name of a study carrel, return a new-line delimited
 	list of keywords denoted by the build process. If count it True,
 	then the list of keywords is counted, tabulated, and sorted in
 	descending order by frequency. If count is True and wordcloud is
 	True, then a visualization of the frequencies is returned. If count
 	is True, wordcloud is True, and save is True, then the visualization
@@ -1374,24 +1554,27 @@
 
 	Admittedly, this function, like many of the functions, is convoluted;
 	this function ought to return more standard data structures, not
 	line-delimited lists containing tab-delimited values. My bad. '''
 
 	# require
 	import sqlite3
-
+	from pathlib import Path
+	
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
+	
 	# sanity check
-	checkForCarrel( carrel )
+	checkForCarrel( carrel, localLibrary )
 
 	# initialize
-	locallibrary           = configuration( 'localLibrary' )
-	connection             = sqlite3.connect( str( locallibrary/carrel/ETC/DATABASE )  )
+	connection             = sqlite3.connect( str( localLibrary/carrel/ETC/DATABASE )  )
 	connection.row_factory = sqlite3.Row
 	items                  = []
-	stopwords              = open( str( locallibrary/carrel/ETC/STOPWORDS ), encoding='utf-8' ).read().split()
+	stopwords              = open( str( localLibrary/carrel/ETC/STOPWORDS ), encoding='utf-8' ).read().splitlines()
 
 	# dump a sorted list of all keywords
 	if not count :
 
 		# articulate sql, search, and output
 		sql  = 'SELECT DISTINCT( LOWER( keyword ) ) AS keyword FROM wrd ORDER BY LOWER( keyword );'
 		rows = connection.execute( sql )
@@ -1427,15 +1610,15 @@
 				
 					# make sure the value is not in the stopwords
 					if row[ 'keyword' ] not in stopwords : frequencies[ row[ 'keyword' ] ] = row[ 'count' ]
 			
 			if not save : cloud( frequencies )
 			else :
 			
-				file = locallibrary/carrel/FIGURES/KEYWORDSCLOUD
+				file = localLibrary/carrel/FIGURES/KEYWORDSCLOUD
 				cloud( frequencies, file=file )
 
 	# clean up and done; the result might be empty, which is sort of bogus
 	connection.close()
 	return '\n'.join( items )
 
 
@@ -1477,15 +1660,15 @@
 		snippets.append( snippet )	
 	
 	# done
 	return( snippets )
 
 
 # get sizes (measured in words) of documents
-def sizes( carrel, sort='words', output='list', save=False ) :
+def sizes( carrel, localLibrary=None, sort='words', output='list', save=False ) :
 
 	'''Given a the name of study carrel, output a newline-delimited list of
 	study carrel item identifiers and the number of words (size) of the
 	given item. Each item/number of words combination is a tab-delimited
 	value. The value of sort can be "words" or anything else. If it is
 	anything else, then the output is sorted by item identifier. The value
 	of "output" can be list, histogram, or boxplot. If the value is
@@ -1505,21 +1688,24 @@
 	ID      = 'SELECT id, words FROM bib ORDER BY id ASC'
 	COLUMNS = [ 'sizes in words' ]
 	
 	# require
 	import matplotlib.pyplot as plt
 	import pandas as pd
 	import sqlite3
-
+	from pathlib import Path
+	
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
+	
 	# sanity check
-	checkForCarrel( carrel )
+	checkForCarrel( carrel, localLibrary )
 
 	# initialize
-	locallibrary           = configuration( 'localLibrary' )
-	connection             = sqlite3.connect( str( locallibrary/carrel/ETC/DATABASE )  )
+	connection             = sqlite3.connect( str( localLibrary/carrel/ETC/DATABASE )  )
 	connection.row_factory = sqlite3.Row
 	items                  = []
 	
 	# find all rows
 	if sort == 'words' : rows = connection.execute( WORDS )
 	else               : rows = connection.execute( ID )
 		
@@ -1548,30 +1734,30 @@
 		# initialize the plot
 		figure, axis = plt.subplots()
 		
 		# plot
 		if output == 'histogram' : 
 		
 			df.hist( ax=axis )
-			if save : plt.savefig( locallibrary/carrel/FIGURES/SIZESHISTOGRAM )
+			if save : plt.savefig( localLibrary/carrel/FIGURES/SIZESHISTOGRAM )
 			else    : plt.show()
 
 		else :
 		
 			df.boxplot( ax=axis )		
-			if save : plt.savefig( locallibrary/carrel/FIGURES/SIZESBOXPLOT )
+			if save : plt.savefig( localLibrary/carrel/FIGURES/SIZESBOXPLOT )
 			else    : plt.show()
 		
 	# clean up
 	connection.close()
 	return '\n'.join( items )
 
 
 # get readability scores
-def flesch( carrel, sort='score', output='list', save=False) :
+def flesch( carrel, localLibrary=None, sort='score', output='list', save=False) :
 
 	'''Given the name of study carrel, output a newline-delimited list of
 	study carrel item identifiers and the readability (Flesch) score of each
 	item. Each item/score combination is a tab-delimited value. The value of
 	sort can be "score" or anything else. If it is anything else, then the
 	output is sorted by item identifier. The value of "output" can be list,
 	histogram, or boxplot. If the value is histogram or boxplot, then the
@@ -1591,21 +1777,24 @@
 	ID      = 'SELECT id, flesch FROM bib ORDER BY id ASC'
 	COLUMNS = [ 'readability' ]
 	
 	# require
 	import matplotlib.pyplot as plt
 	import pandas as pd
 	import sqlite3
+	from pathlib import Path
+	
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 
 	# sanity check
-	checkForCarrel( carrel )
+	checkForCarrel( carrel, localLibrary )
 
 	# initialize
-	locallibrary           = configuration( 'localLibrary' )
-	connection             = sqlite3.connect( str( locallibrary/carrel/ETC/DATABASE )  )
+	connection             = sqlite3.connect( str( localLibrary/carrel/ETC/DATABASE )  )
 	connection.row_factory = sqlite3.Row
 	items                  = []
 	
 	# find all rows
 	if sort == 'score' : rows = connection.execute( SCORE )
 	else               : rows = connection.execute( ID )
 		
@@ -1632,30 +1821,30 @@
 		# initialize the plot
 		figure, axis = plt.subplots()
 
 		# plot
 		if output == 'histogram' : 
 		
 			df.hist( ax=axis )
-			if save : plt.savefig( locallibrary/carrel/FIGURES/READABILITYHISTOGRAM )
+			if save : plt.savefig( localLibrary/carrel/FIGURES/READABILITYHISTOGRAM )
 			else    : plt.show()
 
 		else :
 		
 			df.boxplot( ax=axis )		
-			if save : plt.savefig( locallibrary/carrel/FIGURES/READABILITYBOXPLOT )
+			if save : plt.savefig( localLibrary/carrel/FIGURES/READABILITYBOXPLOT )
 			else    : plt.show()
 
 	# clean up
 	connection.close()
 	return '\n'.join( items )
 
 
 # compute ngrams
-def ngrams( carrel, size=1, query=None, count=False, location='local', wordcloud=False, save=False ) :
+def ngrams( carrel, localLibrary=None, size=1, query=None, count=False, location='local', wordcloud=False, save=False ) :
 
 	'''Given the name of a study carrel, output a newline-delimited list of
 	ngrams in the carrel. The value of size denotes the number of ngrams to
 	output on each line. If the value of size is 1 or 2, then stopwords are
 	removed from the output. The output can be filtered using the query
 	parameter, which supports regular expressions. If the value of count is
 	True, then each item in the resulting list of ngrams is counted and
@@ -1673,23 +1862,26 @@
 	# configure
 	LIMIT = 200
 	
 	# require
 	from re       import search
 	from requests import get
 	import nltk
+	from pathlib import Path
+	
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 
 	# branch according to location; local
 	if location == 'local' :
 	
 		# sanity check
-		checkForCarrel( carrel )
+		checkForCarrel( carrel, localLibrary )
 		
 		# read local data
-		localLibrary = configuration( 'localLibrary' )
 		stopwords    = open( str( localLibrary/carrel/ETC/STOPWORDS ), encoding='utf-8' ).read().split()
 		text         = open( str( localLibrary/carrel/ETC/CORPUS ), encoding='utf-8' ).read()
 	
 	# remote
 	elif location == 'remote' :
 	
 		# read remote data; needs error checking
@@ -1812,15 +2004,15 @@
 	
 		# output raw data, and hope sort, uniq, grep, and less are used
 		for ngram in ngrams : results.append( "\t".join( list( ngram ) ) )
 		return '\n'.join( results )
 
 
 # process parts-of-speech
-def pos( carrel, select='parts', like='any', count=False, normalize=True, wordcloud=False, save=False ) :
+def pos( carrel, localLibrary=None, select='parts', like='any', count=False, normalize=True, wordcloud=False, save=False ) :
 
 	'''Given the name of a study carrel, return various
 	incarnations of parts-of-speech (pos) values.
 
 	If the value of select is "parts" (the default), then a
 	newline-delimited list of pos values are returned for each
 	and every word in the carrel. If the value of select is
@@ -1844,21 +2036,24 @@
 	If count is True, wordcloud is True, and save is True, then
 	the resulting wordcloud is saved in the carrel's etc
 	directory, but only for a limited number of values for like
 	(NOUN, VERB, PRON, ADJ, PROPN, and ADV).'''
 	
 	# require
 	import sqlite3
+	from pathlib import Path
+	
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 
 	# sanity check
-	checkForCarrel( carrel )
+	checkForCarrel( carrel, localLibrary )
 
 	# initialize
-	locallibrary           = configuration( 'localLibrary' )
-	connection             = sqlite3.connect( str( locallibrary/carrel/ETC/DATABASE )  )
+	connection             = sqlite3.connect( str( localLibrary/carrel/ETC/DATABASE )  )
 	connection.row_factory = sqlite3.Row
 	items                  = []
 	
 	# branch accordingly; parts-of-speech
 	if select == 'parts' :
 	
 		# initialize like
@@ -1942,15 +2137,15 @@
 				# simply output
 				if not save : cloud( frequencies )
 			
 				# save to the corresponding figures directory
 				else :
 			
 					# configure
-					localLibrary = configuration( 'localLibrary' )
+					#localLibrary = configuration( 'localLibrary' )
 
 					# nouns
 					if like == 'NOUN%' :
 				
 						# configure and save
 						file = localLibrary/carrel/FIGURES/POSNOUN
 						cloud( frequencies, file=file )
@@ -1998,15 +2193,15 @@
 		
 	# clean up and done
 	connection.close()
 	return '\n'.join( items )
 
 
 # process named entities
-def entities( carrel, select='type', like='any', count=False, wordcloud=False, save=False ) :
+def entities( carrel, localLibrary=None, select='type', like='any', count=False, wordcloud=False, save=False ) :
 
 	'''Given the name of a study carrel, return various
 	incarnations of named-entity values.
 
 	If the value of select is "type" (the default), then a
 	newline-delimited list of entity values are returned for each
 	and every word in the carrel. If the value of select is
@@ -2027,20 +2222,23 @@
 	If count is True, wordcloud is True, and save is True, then
 	the resulting wordcloud is saved in the carrel's etc
 	directory, but only for a limited number of values for like
 	(any, PERSON, ORG, and GPE).'''
 
 	# require
 	import sqlite3
+	from pathlib import Path
+
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 
 	# sanity check
-	checkForCarrel( carrel )
+	checkForCarrel( carrel, localLibrary )
 
 	# initialize
-	localLibrary           = configuration( 'localLibrary' )
 	connection             = sqlite3.connect( str( localLibrary/carrel/ETC/DATABASE )  )
 	connection.row_factory = sqlite3.Row
 	items                  = []
 	
 	# branch accordingly; types of entities
 	if select == 'type' :
 	
@@ -2140,15 +2338,15 @@
 				
 	# clean up
 	connection.close()
 	return '\n'.join( items )
 
 
 # do feature reduction and visualize
-def cluster( carrel, type='dendrogram', save=False ) :
+def cluster( carrel, localLibrary=None, type='dendrogram', save=False ) :
 
 	'''Given the name of a study carrel, use PCA to reduce the
 	carrel's content to two or three dimensions and then
 	visualize the result. If the value of type is "dendrogram",
 	then reducd to two dimensions, and if the value of type is
 	"cube", then reduce to three dimensions. If the value of save
 	is True, then save the resulting image in the carrel's
@@ -2162,24 +2360,27 @@
 	# require
 	from os                              import path, system, listdir
 	from scipy.cluster.hierarchy         import ward, dendrogram
 	from sklearn.feature_extraction.text import TfidfVectorizer
 	from sklearn.manifold                import MDS
 	from sklearn.metrics.pairwise        import cosine_similarity
 	import matplotlib.pyplot             as     plt
+	from pathlib import Path
 	
 	# ignore warnings; probably not the greatest idea
 	import warnings
 	warnings.filterwarnings("ignore")
 
+	# initialize
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
+	
 	# sanity check
-	checkForCarrel( carrel )
+	checkForCarrel( carrel, localLibrary )
 
-	# initialize
-	localLibrary = configuration( 'localLibrary' )
 	stopwords    = open( str( localLibrary/carrel/ETC/STOPWORDS ), encoding='utf-8' ).read().split()
 	directory    = localLibrary/carrel/TXT
 	filenames    = [ path.join( directory, filename ) for filename in listdir( directory ) ]
 	vectorizer   = TfidfVectorizer( input='filename', max_df=MAXIMUM, min_df=MINIMUM, stop_words=stopwords )
 	matrix       = vectorizer.fit_transform( filenames ).toarray()
 	distance     = 1 - cosine_similarity( matrix )
 	keys         = [ path.basename( filename ).replace( EXTENSION, '' ) for filename in filenames ] 
@@ -2538,18 +2739,18 @@
 	# done
 	return( results )
 
 
 # make sure the carrel has been indexed
 def checkForSemanticIndex( carrel ) :
 
-	# configure
-	VECTORS = 'reader.vec'
+	# configure; not quite right
+	VECTORS = 'carrel.vec'
 	PATTERN = '*.txt'
-	TOKENS  = 'reader.tok'
+	TOKENS  = 'carrel.tok'
 	
 	# require
 	from multiprocessing import Pool
 	from pathlib         import Path
 	import gensim
 	import sys
 
@@ -2594,15 +2795,15 @@
 
 # implement semantic (word2vec) indexing
 def word2vec( carrel, type='similarity', query='love', topn=10 ) :
 
 	'''types = similarity|distance|analogy|scatter'''
 
 	# configure
-	VECTORS  = 'reader.vec'
+	VECTORS  = 'carrel.vec'
 	
 	# require
 	import sys
 	import gensim
 
 	# initialize
 	localLibrary = configuration( 'localLibrary' )
@@ -2695,32 +2896,39 @@
 		try :
 		
 			positive = [ words[ 0 ], words[ 2 ] ]
 			negative = words[ 1 ]
 			items    = []
 			
 			similarities = model.most_similar( positive=positive, negative=negative, topn=topn )
-			for similarity in similarities : print( similarity )
+			#for similarity in similarities : print( similarity )
+			return( similarities )
 			
 		# error
 		except KeyError as word : sys.stderr.write( ( 'A word in your query -- %s -- is not in the index. Please remove it.\n' % word ) )
 
 
 # make sure the carrel has been indexed; sqlite++
 def _checkForIndex( carrel ) :
 
 	# configure
 	SANITYCHECK    = "SELECT * FROM sqlite_master WHERE type='table' AND name='fulltext';"
 	DROPFULLTEXT   = 'DROP TABLE IF EXISTS fulltext;'
 	CREATEFULLTEXT = 'CREATE TABLE fulltext ( id TEXT, fulltext TEXT );\n'
 	TEMPLATE       = "INSERT INTO fulltext ( id, fulltext ) VALUES ( '##ID##', '##FULLTEXT##' );\n"
 	DROPINDX       = 'DROP TABLE IF EXISTS indx;'
+
+	# these are what we want
 	CREATEINDX     = 'CREATE VIRTUAL TABLE indx USING FTS5( id, author, title, date, summary, keyword, words, sentence, flesch, cache, txt, fulltext );'
 	INDEX          = 'INSERT INTO indx SELECT b.id, b.author, b.title, b.date, b.summary, group_concat( LOWER( w.keyword ), "; " ), b.words, b.sentence, b.flesch, b.id || b.extension, b.id || ".txt", f.fulltext FROM bib AS b, fulltext AS f, wrd AS w WHERE b.id IS f.id AND b.id IS w.id GROUP BY w.id;';
 
+	# these work when "database is full"; no full text
+	#CREATEINDX     = 'CREATE VIRTUAL TABLE indx USING FTS5( id, author, title, date, summary, keyword, words, sentence, flesch, cache, txt );'
+	#INDEX          = 'INSERT INTO indx SELECT b.id, b.author, b.title, b.date, b.summary, group_concat( LOWER( w.keyword ), "; " ), b.words, b.sentence, b.flesch, b.id || b.extension, b.id || ".txt" FROM bib AS b, fulltext AS f, wrd AS w WHERE b.id IS f.id AND b.id IS w.id GROUP BY w.id;';
+
 	# require
 	import os
 	import re
 	import sqlite3
 	import tempfile
 	import sys
 	
@@ -2911,21 +3119,23 @@
 
 # get an inventory of available study carrels
 def catalog( location='local', human=True ) :
 
 	'''location = local|remote'''
 
 	# configure
-	TSV    = 'stacks/carrels-legacy/catalog.tsv'
-	RECORD = "      item: ##ITEM##\n      name: ##NAME##\n      date: ##DATE##\n  keywords: ##KEYWORDS##\n     items: ##ITEMS##\n     words: ##WORDS##\n     score: ##SCORE##\n     bytes: ##BYTES##\n\n"
-	HEADER = "\nThe catalog includes ##COUNT## items, and each is listed below:\n\n"
+	INDEX    = 'index.csv'
+	RECORD   = "         item: ##ITEM##\n   identifier: ##IDENTIFIER##\n        title: ##TITLE##\n         type: ##TYPE##\n       source: ##SOURCE##\n        items: ##ITEMS##\n        words: ##WORDS##\n  readability: ##SCORE##\n     keywords: ##KEYWORDS##\n         read: ##READ##\n       browse: ##BROWSE##\n     download: ##DOWNLOAD##\n\n"
+	HEADER   = "\nThe catalog includes ##COUNT## items, and each is listed below:\n\n"
 
 	# require
 	from requests import get
-		
+	from pandas   import read_csv
+	from io       import StringIO
+	
 	# branch accordingly; local
 	if location == 'local' :
 		
 		# initialize
 		localLibrary = configuration( 'localLibrary' )
 		items        = []
 		
@@ -2942,73 +3152,65 @@
 		# create person-amenable output
 		if human :
 		
 			# create a rudimentary catalog
 			catalog = ''
 			count   = 0
 						
-			records = get( REMOTELIBRARY + '/' + TSV ).text 
-			for item, record in enumerate( records.split( '\n' ) ) :
-			
-				# delimit and sanity check
-				fields = record.split( '\t' )
-				if len( fields ) != 7 : break
-			
-				# parse
-				name     = fields[ 0 ]
-				date     = fields[ 1 ]
-				keywords = fields[ 2 ]
-				items    = fields[ 3 ]
-				words    = fields[ 4 ]
-				score    = fields[ 5 ]
-				bytes    = fields[ 6 ]
-			
+			# get all the remote records and process each; convoluted
+			carrels = read_csv( StringIO( get( REMOTELIBRARY + '/' + INDEX ).text ) )
+			for item, carrel in carrels.iterrows() :
+										
 				# increment
 				count += 1
 				item  += 1
 				
 				# update
-				record   = RECORD.replace( '##ITEM##', str( item ) )
-				record   = record.replace( '##NAME##', name )
-				record   = record.replace( '##DATE##', date )
-				record   = record.replace( '##KEYWORDS##', keywords )
-				record   = record.replace( '##ITEMS##', items )
-				record   = record.replace( '##WORDS##', words )
-				record   = record.replace( '##SCORE##', score )
-				record   = record.replace( '##BYTES##', bytes )
+				record   = RECORD.replace( '##ITEM##',       str( item ) )
+				record   = record.replace( '##IDENTIFIER##', carrel[ 'id' ] )
+				record   = record.replace( '##TITLE##',      carrel[ 'title' ] )
+				record   = record.replace( '##KEYWORDS##',      carrel[ 'keywords' ] )
+				record   = record.replace( '##ITEMS##',      str( carrel[ 'items' ] ) )
+				record   = record.replace( '##WORDS##',      str( carrel[ 'words' ] ) )
+				record   = record.replace( '##SCORE##',      str( carrel[ 'flesch' ] ) )
+				record   = record.replace( '##TYPE##',      str( carrel[ 'type' ] ) )
+				record   = record.replace( '##SOURCE##',      str( carrel[ 'source' ] ) )
+				record   = record.replace( '##READ##',      str( carrel[ 'read' ] ) )
+				record   = record.replace( '##BROWSE##',      str( carrel[ 'browse' ] ) )
+				record   = record.replace( '##DOWNLOAD##',      str( carrel[ 'download' ] ) )
 				catalog += record
 				
 			# add the header and output
 			header  = HEADER.replace( '##COUNT##', str( count ) )
 			catalog = header + catalog
 			return( catalog )
 				
 		# get the raw data and hope the results get piped to utilities like sort, grep, cut, less, etc.
-		else : return( get( REMOTELIBRARY + '/' + TSV ).text  )
+		else : return( get( REMOTELIBRARY + '/' + INDEX ).text  )
 
 	
 # locally cache a carrel from the public library
 def download( carrel ) :
 			
 	# configure
-	ZIPFILE = 'study-carrel.zip'
-	CARRELS = 'stacks/carrels-legacy'
+	ZIPFILE = 'index.zip'
+	CARRELS = ''
 
 	# require
 	from requests import get
 	from tempfile import TemporaryFile
 	from zipfile  import ZipFile
 	import sys
 	
 	# initialize
 	localLibrary  = configuration( 'localLibrary' )
 
 	# get the remote zip file; needs error checking
 	sys.stderr.write( "\n  INFO: Downloading remote study carrel...\n" )
-	response = get( REMOTELIBRARY + '/' + CARRELS + '/' + carrel + '/' + ZIPFILE )
+	response = get( REMOTELIBRARY + '/' + carrel + '/' + ZIPFILE )
 	
 	# initialize a temporary file and write to it
 	sys.stderr.write( "  INFO: Saving study carrel...\n" )
 	handle = TemporaryFile()
 	handle.write( response.content )
 	
 	# unzip the temporary file and close it, which also deletes it
@@ -3018,28 +3220,31 @@
 
 	# done
 	sys.stderr.write( ( '''  INFO: Done.\n''' ) )
 	return
 
 
 # open the html root of a study carrel
-def read( carrel, location='local' ) :
+def read( carrel, location='local', localLibrary=None, ) :
 
 	# require
 	from webbrowser import open
 	import sys
+	from pathlib import Path
 	
 	if location == 'local' :
 	
+		if localLibrary : localLibrary = Path( localLibrary )
+		else            : localLibrary = configuration( 'localLibrary' )
+		
 		# sanity check
-		checkForCarrel( carrel )
+		checkForCarrel( carrel, localLibrary )
 
-		localLibrary  = configuration( 'localLibrary' )
+		#localLibrary  = configuration( 'localLibrary' )
 		url = 'file://' + str( localLibrary/carrel/INDEX )
-		sys.stderr.write( url + '\n' )
 		open( url )
 		
 	elif location == 'remote' :
 	
 		url = REMOTELIBRARY + '/' + CARRELS + '/' + carrel
 		open( url )
 
@@ -3101,15 +3306,18 @@
 	except requests.ConnectionError : pass
 	
 	# done
 	return( running )
 	
 	
 # create carrel skeleton
-def _initialize( carrel, directory ) :
+def _initialize( carrel, directory, localLibrary=None ) :
+	
+	# require
+	from datetime import datetime
 	
 	# configure
 	ADR      = 'adr'
 	BIB      = 'bib'
 	CACHE    = 'cache'
 	ENT      = 'ent'
 	ETC      = 'etc'
@@ -3123,15 +3331,16 @@
 	# require
 	from   datetime import datetime
 	from   getpass  import getuser
 	from   pathlib  import Path
 	import shutil
 	
 	# create the library, the carrel, and the carrel's sub-directories
-	localLibrary = configuration( 'localLibrary' )
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 	Path.mkdir( localLibrary,                exist_ok=True )
 	Path.mkdir( localLibrary/carrel,         exist_ok=True )
 	Path.mkdir( localLibrary/carrel/ADR,     exist_ok=True )
 	Path.mkdir( localLibrary/carrel/BIB,     exist_ok=True )
 	Path.mkdir( localLibrary/carrel/CACHE,   exist_ok=True )
 	Path.mkdir( localLibrary/carrel/ENT,     exist_ok=True )
 	Path.mkdir( localLibrary/carrel/ETC,     exist_ok=True )
@@ -3169,17 +3378,22 @@
 			destination = localLibrary/carrel/CACHE/( source.name )
 			shutil.copyfile( source, destination )
 
 	# add stop words; there is probably a better way
 	output = localLibrary/carrel/ETC/STOPWORDS
 	with open( output, 'w', encoding='utf-8' ) as handle : handle.write( WORDS )
 
+	# add readme
+	output      = localLibrary/carrel/READMEFILE
+	readmewords = READMEWORDS.replace( '##DATE##', datetime.today().strftime("%B %-d, %Y") )
+	with open( output, 'w', encoding='utf-8' ) as handle : handle.write( readmewords )
+
 
 # given a file, create some bibliographics and save plain text
-def _file2bib( carrel, file, metadata=None ) :
+def _file2bib( carrel, file, metadata=None, localLibrary=None ) :
 		
 	# configure
 	BIB          = 'bib'
 	TXT          = 'txt'
 	CACHE        = 'cache'
 	COUNT        = 24
 	EXTENSION    = '.txt'
@@ -3191,25 +3405,26 @@
 	from   pathlib              import Path
 	from   textacy              import text_stats
 	from   tika                 import detector
 	from   tika                 import parser
 	import os
 	import spacy
 	import pytextrank
-
+	
 	# _initialize
 	authorFound  = False
 	dateFound    = False
 	titleFound   = False
 	title        = _name2key( file )
 	extension    = os.path.splitext( os.path.basename( file ) )[ 1 ]
 	key          = _name2key( file )
 	pages        = ''
 	summary      = ''
-	localLibrary = configuration( 'localLibrary' )
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 
 	# debug 
 	if VERBOSE : click.echo( ( '\t%s' % key ), err=True )
 
 	# get the text, and if not, then return; the whole point is to have content to read!
 	parsed = parser.from_file( file )
 	text   = parsed[ 'content' ]	
@@ -3311,14 +3526,15 @@
 		click.echo( '     flesch: ' + str( flesch ),    err=True )
 		click.echo( '      cache: ' + str( cache ),     err=True )
 		click.echo( '        txt: ' + str( txt ),       err=True )
 		click.echo( '',                                 err=True )
 	
 	# open output
 	output = localLibrary/carrel/BIB/( key + BIBEXTENSION )
+	
 	with open( output, 'w', encoding='utf-8' ) as handle :
 	
 		try :
 		
 			# output the header and the data
 			handle.write( '\t'.join( HEADER ) + '\n' )
 			handle.write( '\t'.join( [ str( key ), author, str( title ), str( date ), pages, extension, mimetype, str( words ), str( sentences ), str( flesch ), summary, str( cache ), str( txt ) ] ) + '\n' )
@@ -3422,27 +3638,28 @@
 	summary = re.sub( '^\s', '',  summary )
 	summary = re.sub( '\s$', '',  summary )
 
 	# done
 	return summary
 
 # create bag of words
-def _txt2bow( carrel ) :
+def _txt2bow( carrel, localLibrary=None ) :
 
-	# configure
+	# configure; not quite right
 	PATTERN = '*.txt'
-	BOW     = 'reader.txt'
+	BOW     = 'carrel.txt'
 	TXT     = 'txt'
 	ETC     = 'etc'
 	
 	# require
 	from pathlib import Path
 
 	# _initialize
-	localLibrary = configuration( 'localLibrary' )
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 
 	# process each text file in the given directory
 	txt = localLibrary/carrel/TXT
 	bow = ''
 	for file in txt.glob( PATTERN ) :
 	
 		# create/increment the bag of words
@@ -3474,28 +3691,30 @@
 	text = re.sub( '\t', ' ',  text )
 
 	# done
 	return text
 
 
 # extract email addresses
-def _txt2adr( carrel, file ) :
+def _txt2adr( carrel, file, localLibrary ) :
 	
 	# configure
 	ADR       = 'adr'
 	EXTENSION = '.adr'
 	HEADER    = [ 'id', 'address' ]
 	PATTERN   = '''(?:[a-z0-9!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*|"(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21\x23-\x5b\x5d-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])*")@(?:(?:[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?|\[(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?|[a-z0-9-]*[a-z0-9]:(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21-\x5a\x53-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])+)\])'''
 
 	# require
 	import re
+	from pathlib import Path
 	
 	# _initialize
 	key          = _name2key( file )
-	localLibrary = configuration( 'localLibrary' )
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 
 	# debug 
 	if VERBOSE : click.echo( ( '\t%s' % key ), err=True )
 
 	# slurp up the file
 	with open ( file, encoding='utf-8' ) as handle : text = _normalize( handle.read() )
 	
@@ -3521,27 +3740,29 @@
 				address = re.sub( '}',  '', address )
 				
 				# output
 				handle.write( '\t'.join( [ key, address ] ) + '\n' )
 
 
 # extract named entities
-def _txt2ent( carrel, file ) :
+def _txt2ent( carrel, file, localLibrary=None ) :
 
 	# configure
 	EXTENSION = '.ent'
 	ENT       = 'ent'
 	HEADER    = [ 'id', 'sid', 'eid', 'entity', 'type' ]
 
 	# require
 	import spacy
-
+	from pathlib import Path
+	
 	# _initialize
 	key          = _name2key( file )
-	localLibrary = configuration( 'localLibrary' )
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 	
 	# debug 
 	if VERBOSE : click.echo( ( '\t%s' % key ), err=True )
 
 	# slurp up the file
 	with open( file, encoding='utf-8' ) as handle : text = _normalize( handle.read() )
 
@@ -3566,27 +3787,29 @@
 				# parse and output
 				value = entity.text
 				type  = entity.label_
 				handle.write( '\t'.join( [ key, str( s + 1 ), str( e + 1 ), value, type ] ) + '\n' )
 
 
 # extract parts-of-speech
-def _txt2pos( carrel, file ) :
+def _txt2pos( carrel, file, localLibrary=None ) :
 
 	# configure
 	EXTENSION = '.pos'
 	POS       = 'pos'
 	HEADER    = [ 'id', 'sid', 'tid', 'token', 'lemma', 'pos' ]
 
 	# require
 	import spacy
-
+	from pathlib import Path
+	
 	# _initialize
 	key          = _name2key( file )
-	localLibrary = configuration( 'localLibrary' )
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 	
 	# debug 
 	if VERBOSE : click.echo( ( '\t%s' % key ), err=True )
 
 	# slurp up the file
 	with open( file, encoding='utf-8' ) as handle : text = _normalize( handle.read() )
 
@@ -3615,28 +3838,30 @@
 					feature = str( token.text )
 					lemma   = str( token.lemma_.lower() )
 					pos     = token.pos_
 					handle.write( '\t'.join( [  key, str( s + 1 ), str( t + 1 ), feature, lemma, pos ] ) + '\n' )
 
 
 # given a file, extract domains and urls
-def _txt2url( carrel, file ) :
+def _txt2url( carrel, file, localLibrary ) :
 
 	# configure
 	EXTENSION = '.url'
 	URLS      = 'urls'
 	HEADER    = [ 'id', 'domain', 'url']
 	PATTERN   = '(https?:\/\/(?:www\.|(?!www))[a-zA-Z0-9][a-zA-Z0-9-]+[a-zA-Z0-9]\.[^\s]{2,}|www\.[a-zA-Z0-9][a-zA-Z0-9-]+[a-zA-Z0-9]\.[^\s]{2,}|https?:\/\/(?:www\.|(?!www))[a-zA-Z0-9]+\.[^\s]{2,}|www\.[a-zA-Z0-9]+\.[^\s]{2,})'
 
 	# require
 	import re
+	from pathlib import Path
 	
 	# _initialize
 	key          = _name2key( file )
-	localLibrary = configuration( 'localLibrary' )
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 	
 	# debug 
 	if VERBOSE : click.echo( ( '\t%s' % key ), err=True )
 
 	# slurp up the file
 	with open( file, encoding='utf-8' ) as handle : text = _normalize( handle.read() )
 
@@ -3665,47 +3890,50 @@
 				domain = re.sub( '\W$',     '', domain )
 	
 				# output
 				handle.write( '\t'.join( [ key, domain, url ] ) + '\n' )
 
 
 # given a file, output keywords
-def _txt2wrd( carrel, file ) :
+def _txt2wrd( carrel, file, localLibrary=None ) :
 
 	# configure
 	EXTENSION  = '.wrd'
 	WRD        = 'wrd'
-	NGRAMS     = 1
-	TOPN       = 0.005
+	NGRAMS     = ( 1, 2 )
+	TOPN       = 0.05
 	HEADER     = [ 'id', 'keyword' ]
 	NORMALIZE  = 'lower'
 	WINDOWSIZE = 5
-	
+	POS        = ( 'NOUN', 'PROPN', 'ADJ' )
+
 	# require
-	from  textacy.extract.keyterms.yake import yake
-	import spacy
+	from   pathlib                  import Path
+	from   textacy.extract.keyterms import yake
 	import os
+	import spacy
 	
 	# _initialize
 	key          = _name2key( file )
-	localLibrary = configuration( 'localLibrary' )
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 	
 	# debug 
 	if VERBOSE : click.echo( ( '\t%s' % key ), err=True )
 
 	# slurp up the file
 	with open( file, encoding='utf-8' ) as handle : text = _normalize( handle.read() )
 
 	# model the text and get the keywords
 	nlp            = spacy.load( MODELMEDIUM )
 	nlp.max_length = os.path.getsize( file ) + 1 
 	doc            = nlp( text )
 
 	# do the extraction
-	try    : records = ( yake( doc, ngrams=( 1, 2 ), window_size=WINDOWSIZE, topn=TOPN, normalize=NORMALIZE ) )
+	try    : records = ( yake( doc, ngrams=NGRAMS, window_size=WINDOWSIZE, topn=TOPN, normalize=NORMALIZE, include_pos=POS ) )
 	except : records = []
 	
 	# check for records
 	if len( records ) > 0 :
 	
 		# open output
 		output = localLibrary/carrel/WRD/( key + EXTENSION )
@@ -3789,15 +4017,15 @@
 		# update
 		found = True
 		
 	# fill the database, conditionally
 	if found : features.to_sql( table, connection, if_exists='replace', index=False )
 
 
-def build( carrel, directory, erase=False, start=False ) :
+def build( carrel, directory, erase=False, start=False, localLibrary=None ) :
 
 	"""Create <carrel> from files in <directory>
 
 	Use this command to build a data set ("study carrel") based on the files
 	saved in a directory. Once the data set is created the other Toolbox
 	commands can be applied to the result. The files can be of any type
 	(PDF, Microsoft Word, HTML, etc.), and they can be of any kind (books,
@@ -3819,29 +4047,31 @@
 	SCHEMA    = '''-- parts-of-speech\ncreate table pos (\n    id    TEXT,\n    sid   INT,\n    tid   INT,\n    token TEXT,\n    lemma TEXT,\n    pos   TEXT\n);\n\n-- name entitites\ncreate table ent (\n    id     TEXT,\n    sid    INT,\n    eid    INT,\n    entity TEXT,\n    type   TEXT\n);\n\n-- keywords\ncreate table wrd (\n    id      TEXT,\n    keyword TEXT\n);\n\n-- email addresses\ncreate table adr (\n    id      TEXT,\n    address TEXT\n);\n\n-- questions\ncreate table questions (\n    id       TEXT,\n    question TEXT\n);\n\n-- urls\ncreate table url (\n    id     TEXT,\n    domain TEXT,\n    url    TEXT\n);\n\n-- bibliographics, such as they are\ncreate table bib (\n    id        TEXT,\n    words     INT,\n    sentence  INT,\n    flesch    INT,\n    summary   TEXT,\n    title     TEXT,\n    author    TEXT,\n    date      TEXT,\n    txt       TEXT,\n    cache     TEXT,\n    pages     INT,\n    extension TEXT,\n    mime      TEXT,\n    genre     TEXT\n);'''
 	POS       = 'pos'
 	ENT       = 'ent'
 	WRD       = 'wrd'
 	ADR       = 'adr'
 	URL       = 'urls'
 	BIB       = 'bib'
-	POOLSMALL = 48
-	POOLBIG   = 54
+	POOLSMALL = 8
+	POOLBIG   = 8
 	
 	# require
 	from   multiprocessing import Pool
+	from   pathlib         import Path
 	import os
 	import shutil
 	import sqlite3
 	import pandas as pd
 	import spacy
 	
 	# _initialize
-	localLibrary = configuration( 'localLibrary' )
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
 	pool         = Pool( POOLSMALL )
-
+	
 	# make sure we have Tika Server
 	_checkForTika( str( configuration( 'tikaHome' ) ) )
 	
 	# start tika; the toolbox's secret sauce
 	if start :
 	
 		# debug
@@ -3888,15 +4118,15 @@
 			click.echo( ( '''
   WARNING: Carrel exists; specify a name other than "%s" or add -e
   to erase it.''' % carrel ), err=True )
 			exit()
 
 	# build skeleton
 	click.echo( '(Step #1 of 9) Initializing %s with %s and stop words' % ( carrel, directory ), err=True )
-	_initialize( carrel, directory )
+	_initialize( carrel, directory, localLibrary )
 		
 	# create a list of filenames to process
 	filenames = []
 	cache     = localLibrary/carrel/CACHE
 	for filename in os.listdir( cache ) :
 	
 		# update list, conditionally
@@ -3910,70 +4140,70 @@
 	if ( localLibrary/carrel/METADATA ).exists() :
 	
 		try : metadata = pd.read_csv( localLibrary/carrel/METADATA, index_col='file' )
 		except ValueError :
 			click.echo( ( '\n  Error: The metadata file (metadata.csv) does not have a\n  column named "file". Remove metadata.csv from the original\n  input directory:\n\n    %s\n\n  Alternatively, edit the metadata file accordingly. Exiting.\n' % directory ), err=True )
 			exit()
 
-		pool.starmap( _file2bib, [ [ carrel, filename, metadata ] for filename in filenames ] )
+		pool.starmap( _file2bib, [ [ carrel, filename, metadata, localLibrary ] for filename in filenames ] )
 		
 	# no metadata file; just do the work
-	else : pool.starmap( _file2bib, [ [ carrel, filename ] for filename in filenames ] )
+	else : pool.starmap( _file2bib, [ [ carrel, filename, None, localLibrary ] for filename in filenames ] )
 		
 	# clean up
 	pool.close()
 	pool = Pool( POOLBIG )
 
 	# bag of words
 	click.echo( '(Step #3 of 9) Creating bag-of-words', err=True )
-	_txt2bow( carrel )
+	_txt2bow( carrel, localLibrary )
 	
 	# output hint
 	click.echo( ( "\n  Hint: Now that the bag-of-words has been created, you can begin\n  to use many of the other Reader Toolbox commands while the\n  building process continues. This is especially true for larger\n  carrels. Open a new terminal window and try:\n\n    rdr cluster %s\n    rdr ngrams %s -c | more\n    rdr concordance %s\n    rdr collocations %s\n" % ( carrel, carrel, carrel, carrel ) ), err=True )
 	
 	# re-create a list of filenames to process
 	filenames = []
 	txt       = localLibrary/carrel/TXT
 	for filename in os.listdir( txt ) : filenames.append( os.path.join( txt, filename ) )
 
 	# extract email addresses
 	click.echo( '(Step #4 of 9) Extracting (email) addresses', err=True )
-	pool.starmap( _txt2adr, [ [ carrel, filename ] for filename in filenames ] )
+	pool.starmap( _txt2adr, [ [ carrel, filename, localLibrary ] for filename in filenames ] )
 	
 	# clean up
 	pool.close()
 	pool = Pool( POOLBIG )
 
 	# extract named entities
 	click.echo( '(Step #5 of 9) Extracting (named) entities', err=True )
-	pool.starmap( _txt2ent, [ [ carrel, filename ] for filename in filenames ] )
+	pool.starmap( _txt2ent, [ [ carrel, filename, localLibrary ] for filename in filenames ] )
 	
 	# clean up
 	pool.close()
 	pool = Pool( POOLBIG )
 
 	# extract parts-of-speech
 	click.echo( '(Step #6 of 9) Extracting parts-of-speech', err=True )
-	pool.starmap( _txt2pos, [ [ carrel, filename ] for filename in filenames ] )
+	pool.starmap( _txt2pos, [ [ carrel, filename, localLibrary ] for filename in filenames ] )
 
 	# clean up
 	pool.close()
 	pool = Pool( POOLBIG )
 
 	# extract urls
 	click.echo( '(Step #7 of 9) Extracting URLs', err=True )
-	pool.starmap( _txt2url, [ [ carrel, filename ] for filename in filenames ] )
+	pool.starmap( _txt2url, [ [ carrel, filename, localLibrary ] for filename in filenames ] )
 
 	# clean up
 	pool.close()
 	pool = Pool( POOLBIG )
 
 	# extract keywords
 	click.echo( '(Step #8 of 9) Extracting (key) words', err=True )
-	pool.starmap( _txt2wrd, [ [ carrel, filename ] for filename in filenames ] )
+	pool.starmap( _txt2wrd, [ [ carrel, filename, localLibrary ] for filename in filenames ] )
 
 	# clean up
 	pool.close()
 
 	# create database
 	click.echo( '(Step #9 of 9) Creating and filling database (reducing)', err=True )
 	database   = str( localLibrary/carrel/ETC/DATABASE )
@@ -3986,85 +4216,89 @@
 	_tsv2db( localLibrary/carrel/ADR, '*.adr', 'adr', connection )
 	_tsv2db( localLibrary/carrel/URL, '*.url', 'url', connection )
 	_tsv2db( localLibrary/carrel/WRD, '*.wrd', 'wrd', connection )
 	_tsv2db( localLibrary/carrel/ENT, '*.ent', 'ent', connection )
 	_tsv2db( localLibrary/carrel/POS, '*.pos', 'pos', connection )
 
 	# output another hint
-	# out hint
 	click.echo( ( '\n  Another hint: The build process is done, and now you ought to\n  be able to use any Toolbox command. For example:\n\n    rdr info %s\n    rdr bib %s | more\n    rdr tm %s\n' % ( carrel, carrel, carrel ) ), err=True )
 
-def summarize( carrel, look=False ) :
+def summarize( carrel, look=False, localLibrary=None ) :
 
 	'''Summarize <carrel>
 
 	The use of this command will generate a set of reports and save them in
 	specific locations in <carrel>'s file system. If you specify the -l
 	(look) option, then <carrel>'s index.htm file will be opened in your Web
 	browser. You can subsequently use rdr read <carrel> to open the
 	index.htm file.'''
 
+	from pathlib import Path
+	
+	if localLibrary : localLibrary = Path( localLibrary )
+	else            : localLibrary = configuration( 'localLibrary' )
+	
 	# sanity check
-	checkForCarrel( carrel )
+	checkForCarrel( carrel, localLibrary )
 	
 	# save bibliography
 	click.echo( "Creating bibliography", err=True )
-	bibliography( carrel, 'text', save=True )
-	bibliography( carrel, 'html', save=True )
-	bibliography( carrel, 'json', save=True )
+	bibliography( carrel, localLibrary, 'text', save=True )
+	bibliography( carrel, localLibrary, 'html', save=True  )
+	bibliography( carrel, localLibrary, 'json', save=True  )
 			
 	# save sizes	
 	click.echo( "Graphing sizes", err=True )
-	sizes( carrel, output='boxplot',   save=True )
-	sizes( carrel, output='histogram', save=True )
+	sizes( carrel, localLibrary, output='boxplot',   save=True )
+	sizes( carrel, localLibrary, output='histogram', save=True )
 		
 	# save readability	
 	click.echo( "Graphing readability", err=True )
-	flesch( carrel, output='boxplot',   save=True )
-	flesch( carrel, output='histogram', save=True )
+	flesch( carrel, localLibrary, output='boxplot',   save=True )
+	flesch( carrel, localLibrary, output='histogram', save=True )
 	
 	# save cluster	
 	click.echo( "Graphing clusters", err=True )
-	cluster( carrel, type='cube',       save=True )
+	cluster( carrel, localLibrary, type='cube', save=True )
 	#ctx.invoke( cluster.cluster, carrel=carrel, type='dendrogram', save=True )
 	
 	# save ngrams	
 	click.echo( "Graphing ngrams", err=True )
-	ngrams( carrel, count=True, size=1, wordcloud=True, save=True )
-	ngrams( carrel, count=True, size=2, wordcloud=True, save=True )
+	ngrams( carrel, localLibrary, count=True, size=1, wordcloud=True, save=True )
+	ngrams( carrel, localLibrary, count=True, size=2, wordcloud=True, save=True )
 	
 	# save entities	
 	click.echo( "Graphing entities", err=True )
-	entities( carrel, count=True, select='entity', like='any',    wordcloud=True, save=True )
-	entities( carrel, count=True, select='entity', like='PERSON', wordcloud=True, save=True )
-	entities( carrel, count=True, select='entity', like='GPE',    wordcloud=True, save=True )
-	entities( carrel, count=True, select='entity', like='ORG',    wordcloud=True, save=True )
+	entities( carrel, localLibrary, count=True, select='entity', like='any',    wordcloud=True, save=True )
+	entities( carrel, localLibrary, count=True, select='entity', like='PERSON', wordcloud=True, save=True )
+	entities( carrel, localLibrary, count=True, select='entity', like='GPE',    wordcloud=True, save=True )
+	entities( carrel, localLibrary, count=True, select='entity', like='ORG',    wordcloud=True, save=True )
 	
 	# save pos	
 	click.echo( "Graphing parts-of-speach", err=True )
-	pos( carrel, count=True, select='lemmas', like='NOUN',  wordcloud=True, save=True )
-	pos( carrel, count=True, select='lemmas', like='VERB',  wordcloud=True, save=True )
-	pos( carrel, count=True, select='lemmas', like='ADJ',   wordcloud=True, save=True )
-	pos( carrel, count=True, select='lemmas', like='ADV',   wordcloud=True, save=True )
-	pos( carrel, count=True, select='lemmas', like='PRON',  wordcloud=True, save=True )
-	pos( carrel, count=True, select='lemmas', like='PROPN', wordcloud=True, save=True )
+	pos( carrel, localLibrary, count=True, select='lemmas', like='NOUN',  wordcloud=True, save=True )
+	pos( carrel, localLibrary, count=True, select='lemmas', like='VERB',  wordcloud=True, save=True )
+	pos( carrel, localLibrary, count=True, select='lemmas', like='ADJ',   wordcloud=True, save=True )
+	pos( carrel, localLibrary, count=True, select='lemmas', like='ADV',   wordcloud=True, save=True )
+	pos( carrel, localLibrary, count=True, select='lemmas', like='PRON',  wordcloud=True, save=True )
+	pos( carrel, localLibrary, count=True, select='lemmas', like='PROPN', wordcloud=True, save=True )
 	
 	# save keywords	
 	click.echo( "Graphing keywords", err=True )
-	keywords( carrel, count=True, wordcloud=True, save=True )
+	keywords( carrel, localLibrary, count=True, wordcloud=True, save=True )
 	
 	# create html
 	click.echo( "Building HTML page", err=True )
 	html = TEMPLATE.replace( '##CARREL##', carrel )
-	html = html.replace( '##ITEMS##', str( extents( carrel, 'items' ) ) )
-	html = html.replace( '##WORDS##', str( extents( carrel, 'words' ) ) )
-	html = html.replace( '##FLESCH##', str( extents( carrel, 'flesch' ) ) )
-	html = html.replace( '##DATECREATED##', str( provenance( carrel, 'dateCreated' ) ) )
-	html = html.replace( '##CREATOR##', str( provenance( carrel, 'creator' ) ) )
+	html = html.replace( '##ITEMS##', str( extents( carrel, 'items', localLibrary ) ) )
+	html = html.replace( '##WORDS##', str( extents( carrel, 'words', localLibrary ) ) )
+	html = html.replace( '##FLESCH##', str( extents( carrel, 'flesch', localLibrary ) ) )
+	html = html.replace( '##DATECREATED##', str( provenance( carrel, 'dateCreated', localLibrary ) ) )
+	html = html.replace( '##CREATOR##', str( provenance( carrel, 'creator', localLibrary ) ) )
 	
 	# save html
-	locallibrary = configuration( 'localLibrary' )
-	with open( locallibrary/carrel/INDEX, 'w', encoding='utf-8' ) as handle : handle.write( html )
+	#locallibrary = configuration( 'localLibrary' )
+	with open( localLibrary/carrel/INDEX, 'w', encoding='utf-8' ) as handle : handle.write( html )
 	
 	# read, 
-	if look : read( carrel )
+	if look : read( carrel, localLibrary )
```

### Comparing `reader-toolbox-0.2.3/rdr/rdr.py` & `reader_toolbox-0.9/rdr/rdr.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,16 +174,19 @@
 	# process each id; update with more meaningful labels
 	for index, id in enumerate( ids ) :
 
 		column = str( id )
 		label  = labels[ index ]
 		topics.rename( columns = { column:label }, inplace=True )
 
-	# _pivot and return
+	# _pivot, sort, and return; improves the output SOO much
+	# see: https://stackoverflow.com/questions/60758625/sort-pandas-dataframe-by-sum-of-columns
 	topics = topics.pivot_table( list( topics.columns ), index=field )
+	sums   = topics.sum()
+	topics = topics[ sums.sort_values( ascending=False ).index[ : ] ]
 	return( topics )
 
 
 # define; launch
 def _launch( directory, jupyter ) :
 
 	# require
@@ -318,15 +321,15 @@
 	See also:
 	
 	\b
 	  rdr info --help
 	  rdr search --help"""
 
 	if save : bibliography( carrel, format, save )
-	else    : click.echo( bibliography( carrel, format ) )
+	else    : click.echo( bibliography( carrel, None, format ) )
 
 
 # download
 @click.command( options_metavar='[<options>]' )
 @click.argument( 'carrel', metavar='<carrel>' )
 def cmdDownload( carrel ) :
 
@@ -370,14 +373,28 @@
 	# do the work and give a hint
 	carrel2zip( carrel )
 	click.echo('''\n  Done. An archive file (index.zip) has been created and saved
   in the root of the ''' + carrel + ''' study carrel. Share the file
   with your friends and colleagues.\n''', err=True )
 
 
+# do cool stuff with sentences
+@click.command( options_metavar='[<options>]' )
+@click.argument( 'carrel', metavar='<carrel>' )
+@click.option('-q', '--query', default='love', type=click.STRING, help="filter results to include the given regular expression")
+@click.option('-p', '--process', default='list', type=click.Choice( [ 'list', 'filter', 'define' ] ), help="type of work to do" )
+@click.option('-v', '--save', is_flag=True, help='write output to default location')
+def cmdSentences( carrel, process, query='love', save=False ) :
+
+	'''Given <carrel> save, output, and process sentences'''
+	
+	# do the work
+	sentences( carrel, process, query, save )
+
+
 # reconcile, create RDF, and graph
 @click.command( options_metavar='[<options>]' )
 @click.argument( 'carrel', metavar='<carrel>' )
 @click.option('-v', '--save', is_flag=True, help='write output to default location')
 @click.option('-o', '--output', default='gml', help='gml for custom visualization (recommended); chart for graphic', type=click.Choice( [ 'gml', 'chart' ] ) )
 def cmdRDFGraph( carrel, output, save ) :
 
@@ -531,15 +548,15 @@
 	This is useful for determining how holistic <carrel> is. A carrel with many clusters is less holistic and probably means the number of latent topics (think "subjects") is high. On the other hand, you may observe clusters falling into distinct groups surrounding authors, titles, or sources. In other words, use this subcommand to learn the degree <carrel> is a hodgepodge of items or a collection of related items. 
 	
 	Example: rdr cluster homer
 	
 	See also: rdr tm --help"""
 
 	# do the work
-	cluster( carrel, type, save )
+	cluster( carrel, type=type, save=save )
 
 
 # named entities
 @click.command( options_metavar='<options>' )
 @click.argument( 'carrel', metavar='<carrel>' )
 @click.option('-s', '--select',    default='type', type=click.Choice( [ 'type', 'entity' ] ), help='the type of output')
 @click.option('-l', '--like',      default='any', help='the type of enity')
@@ -559,16 +576,16 @@
 	  rdr ent -c homer
 	  rdr ent -s entity -c homer
 	  rdr ent -s entity -l PERSON -c homer
 	  
 	See also: rdr pos --help"""
 
 	# do the work
-	if not wordcloud : click.echo( entities( carrel, select, like, count ) )
-	else             : entities( carrel, select, like, count, wordcloud, save )
+	if not wordcloud : click.echo( entities( carrel, None, select, like, count ) )
+	else             : entities( carrel, None, select, like, count, wordcloud, save )
 
 
 # parts-of-speech
 @click.command( options_metavar='<options>' )
 @click.option('-s', '--select',    default='parts', type=click.Choice( [ 'parts', 'words', 'lemmas' ] ), help='the type of output')
 @click.option('-l', '--like',      default='any', help='the part-of-speech')
 @click.option('-c', '--count',     is_flag=True, help='count and tabulate the result')
@@ -594,16 +611,16 @@
 	See also:
 	
 	\b
 	  rdr ngrams --help
 	  rdr ent --help"""
 
 	# do the work and done
-	if not wordcloud : click.echo( pos( carrel, select, like, count, normalize ) )
-	else             : pos( carrel, select, like, count, normalize, wordcloud, save )
+	if not wordcloud : click.echo( pos( carrel, None, select, like, count, normalize ) )
+	else             : pos( carrel, None, select, like, count, normalize, wordcloud, save )
 
 
 # ngrams
 @click.command( options_metavar='<options>' )
 @click.option('-q', '--query',     type=click.STRING, help="filter results to include the given regular expression")
 @click.option('-c', '--count',     is_flag=True, help='count and tabulate the result')
 @click.option('-l', '--location',  default='local', type=click.Choice( [ 'local', 'remote' ] ), help='where is the study carrel')
@@ -625,16 +642,16 @@
 	  rdr ngrams -s 2 -c homer
 	  rdr ngrams -s 2 -c -q love homer
 	  rdr ngrams -s 2 -c -q love homer | more
 	  rdr ngrams -s 2 -c -q love -l remote sonnets | more
 
 	See also: rdr concordance --help"""
 
-	if not save : click.echo( ngrams( carrel, size, query, count, location, wordcloud ) )
-	else        : ngrams( carrel, size, query, count, location, wordcloud, save )
+	if not save : click.echo( ngrams( carrel, None, size, query, count, location, wordcloud ) )
+	else        : ngrams( carrel, None, size, query, count, location, wordcloud, save )
 
 
 # readability
 @click.command( options_metavar='<options>' )
 @click.argument( 'carrel', metavar='<carrel>' )
 @click.option('-s', '--sort', default='score', type=click.Choice( [ 'id', 'score' ] ), help='order result')
 @click.option('-o', '--output', default='list', type=click.Choice( [ 'list', 'histogram', 'boxplot' ] ), help='type of output')
@@ -644,30 +661,30 @@
 	"""Report on the readability (Flesch score) of items in <carrel>
 	
 	It is possible to denote how difficult a text is to read by measuring things like number of words, density of the vocabulary, the length of a document, etc. Such calculations have been done against <carrel>, and this subcommand will output the results. If the returned values are wide-ranging, then this will tell you one thing about <carrel>. For example, some of the documents are either difficult to read, very long, or poorly transcribed ("OCR'ed"). If the measurements are homogeneous, then your carrel is more sane than not.
 	
 	Example: rdr readability homer -o boxplot"""
 
 	# do the work
-	if not save : click.echo( flesch( carrel, sort, output ) )
-	else        : flesch( carrel, sort, output, save )
+	if not save : click.echo( flesch( carrel, None, sort, output ) )
+	else        : flesch( carrel, None, sort, output, save )
 
 
 # sizes
 @click.command( options_metavar='<options>' )
 @click.argument( 'carrel', metavar='<carrel>' )
 @click.option('-s', '--sort', default='words', type=click.Choice( [ 'id', 'words' ] ), help='order result')
 @click.option('-o', '--output', default='list', type=click.Choice( [ 'list', 'histogram', 'boxplot' ] ), help='type of output')
 @click.option('-v', '--save', is_flag=True, help='save result in default location')
 def cmdSizes( carrel, sort, output, save ) :
 
 	"""Report on the sizes (in words) of items in <carrel>"""
 
 	# do the work
-	click.echo( sizes( carrel, sort, output, save ) )
+	click.echo( sizes( carrel, None, sort, output, save ) )
 
 
 # concordance
 @click.command( options_metavar='[<options>]' )
 @click.option('-w', '--width', default=40, help='number of characters on each side of <query>')
 @click.option('-q', '--query', default='love', help='a word, phrase, or regular expression')
 @click.argument( 'carrel', metavar='<carrel>' )
@@ -710,16 +727,16 @@
 	See also:
 	
 	\b
 	  rdr concordance --help
 	  rdr search --help"""
 
 	# do the work and conditionally output
-	if not wordcloud : click.echo( keywords( carrel, count ) )
-	else             : keywords( carrel, count, wordcloud, save )
+	if not wordcloud : click.echo( keywords( carrel, None, count ) )
+	else             : keywords( carrel, None, count, wordcloud, save )
 
 
 # urls
 @click.command( options_metavar='<options>' )
 @click.option('-s', '--select', default='url', type=click.Choice( [ 'url', 'domain' ] ), help='full URLs or just domain')
 @click.option('-l', '--like',   type=click.STRING, help="filter results using the expression")
 @click.option('-c', '--count', is_flag=True, help='count and tabulate the result')
@@ -1270,16 +1287,15 @@
 
 @click.command( options_metavar='<options>' )
 @click.option('-p', '--process', default='model', type=click.Choice( [ 'model', 'read' ] ), help="type of work to do" )
 @click.option('-t', '--topics', default=8, help="number of topics to generate" )
 @click.option('-w', '--words', default=8, help="number of words used to describe topic" )
 @click.option('-i', '--iterations', default=2400, help="number of times to cacluate" )
 @click.option('-o', '--output', default='summary', type=click.Choice( [ 'summary', 'chart', 'topdocs', 'csv' ] ), help="type of report" )
-@click.option('-f', '--field', type=click.Choice( [ 'author', 'title', 'date', 'track', 'category', 'type', 'year', 'journal', 'topic', 
-'pub_place' ] ), help="field for pivoting" )
+@click.option('-f', '--field', type=click.Choice( [ 'use', 'author', 'title', 'date', 'track', 'category', 'type', 'year', 'journal', 'topic', 'college', 'discipline', 'degree', 'pub_place' , 'region' ] ), help="field for pivoting" )
 @click.option('-y', '--type', default='pie', type=click.Choice( [ 'pie', 'bar', 'barh', 'line', 'scatter' ] ), help="type of chart" )
 @click.argument( 'carrel', metavar='<carrel>' )
 def cmdTm( carrel, process, topics, words, iterations, output, field, type ) :
 
 	"""Apply topic modeling against <carrel>
 	
 	Topic modeling is the process of enumerating latent themes from a corpus, and it is yet another way to describe a corpus's aboutness. It is suggested you start out small when it comes to the values for -t and -w. Repeat the modeling process and gradually increase the values. Increase the value of -i as the size of your carrel increases. Remember, there is no such thing as the correct value of -t. After all, exactly how many things are the sum of Shakespeare's works about?
@@ -1504,15 +1520,15 @@
 @click.option('-s', '--start', is_flag=True, help='start Tika')
 def cmdBuild( carrel, directory, erase, start ) :
 
 	"""Create <carrel> from files in <directory>
 
 Use this command to build a data set ("study carrel") based on the files saved in a directory. Once the data set is created the other Toolbox commands can be applied to the result. The files can be of any type (PDF, Microsoft Word, HTML, etc.), and they can be of any kind (books, articles, reports, etc.), and they can be of any number (1, 2, 12, a few dozen, hundreds, etc.). The Toolbox is designed to read about a dozen journal articles in the form of PDF files. This command requires a Java tool called Tika, and it is used to convert the input files into plain text as well as extract authors, titles, and dates. If the Toolbox has not been configured and/or Tika is not installed, then the Toolbox will try to install it on your behalf. If the given directory contains a file named 'metadata.csv', then this command will use the file as the source of author, title, and date metadata values. This is often very helpful because sans metadata it is very difficult to make comparison between documents. Please see the full-blown documentation for details."""
 
-	build( carrel, directory, erase, start )
+	build( carrel, directory, erase, start, None )
 
 @click.command()
 def cmdServer() :
 
 	'''Experimental Web interface to your Distant Reader study carrels'''
 	
 	# configure; code for rdr
@@ -1557,10 +1573,11 @@
 rdr.add_command( cmdSizes,         name='sizes' )
 rdr.add_command( cmdSql,           name='sql' )
 rdr.add_command( cmdSummarize,     name='summarize' )
 rdr.add_command( cmdTm,            name='tm' )
 rdr.add_command( cmdUrl,           name='url' )
 rdr.add_command( cmdWrd,           name='wrd' )
 rdr.add_command( cmdZip,           name='zip' )
+rdr.add_command( cmdSentences,     name='sentences' )
 
 # do the work
 if __name__ == '__main__' : rdr()
```

### Comparing `reader-toolbox-0.2.3/rdr/server.py` & `reader_toolbox-0.9/rdr/server.py`

 * *Files identical despite different names*

### Comparing `reader-toolbox-0.2.3/reader_toolbox.egg-info/PKG-INFO` & `reader_toolbox-0.9/reader_toolbox.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,38 @@
 Metadata-Version: 2.1
 Name: reader-toolbox
-Version: 0.2.3
+Version: 0.9
 Summary: A command-line interface for creating and interacting with Distant Reader data sets (a.k.a. study carrels)
 Home-page: https://github.com/ericleasemorgan/reader-toolbox
 Author: Eric Lease Morgan
 Author-email: emorgan@nd.edu
 Project-URL: Bug Tracker, https://github.com/ericleasemorgan/reader-toolbox/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: catalogue>=1.0.0
+Requires-Dist: click>=7.1.2
+Requires-Dist: datasette>=0.55
+Requires-Dist: matplotlib>=3.4.2
+Requires-Dist: nltk>=3.6.2
+Requires-Dist: tika>=1.24
+Requires-Dist: pandas<=1.5.2
+Requires-Dist: requests>=2.26.0
+Requires-Dist: pytextrank>=3.2.2
+Requires-Dist: scikit-learn>=0.23.2
+Requires-Dist: scipy>=1.7.1
+Requires-Dist: srsly>=1.0.5
+Requires-Dist: textacy>=0.12.0
+Requires-Dist: pytextrank
+Requires-Dist: wordcloud
+Requires-Dist: networkx<=2.8.7
+Requires-Dist: gensim
+Requires-Dist: rdflib
 
 
 
 # Distant Reader Toolbox
 
 A command-line interface for creating and interacting with [Distant Reader](https://distantreader.org) study carrels
```

### Comparing `reader-toolbox-0.2.3/setup.cfg` & `reader_toolbox-0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = reader-toolbox
-version = 0.2.3
+version = 0.9
 author = Eric Lease Morgan
 author_email = emorgan@nd.edu
 description = A command-line interface for creating and interacting with Distant Reader data sets (a.k.a. study carrels)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ericleasemorgan/reader-toolbox
 project_urls = Bug Tracker = https://github.com/ericleasemorgan/reader-toolbox/issues
```

### Comparing `reader-toolbox-0.2.3/setup.py` & `reader_toolbox-0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,10 +2,10 @@
 
 # 	install_requires=[ 'catalogue>=1.0.0', 'click>=7.1.2', 'datasette>=0.55', 'matplotlib>=3.4.2', 'nltk>=3.6.2', 'tika>=1.24', 'pandas>=1.3.2', 'requests>=2.26.0', 'pytextrank>=3.2.2', 'scikit-learn>=0.23.2', 'scipy>=1.7.1', 'srsly>=1.0.5', 'textacy>=0.12.0' ],
 
 setup(
     name='reader-toolbox',
     packages=find_packages(),
     include_package_data=True,
-	install_requires=[ 'catalogue>=1.0.0', 'click>=7.1.2', 'datasette>=0.55', 'matplotlib>=3.4.2', 'nltk>=3.6.2', 'tika>=1.24', 'pandas>=1.3.2', 'requests>=2.26.0', 'pytextrank>=3.2.2', 'scikit-learn>=0.23.2', 'scipy>=1.7.1', 'srsly>=1.0.5', 'textacy>=0.12.0', 'pytextrank', 'wordcloud', 'networkx<=2.8.7' ],
+	install_requires=[ 'catalogue>=1.0.0', 'click>=7.1.2', 'datasette>=0.55', 'matplotlib>=3.4.2', 'nltk>=3.6.2', 'tika>=1.24', 'pandas<=1.5.2', 'requests>=2.26.0', 'pytextrank>=3.2.2', 'scikit-learn>=0.23.2', 'scipy>=1.7.1', 'srsly>=1.0.5', 'textacy>=0.12.0', 'pytextrank', 'wordcloud', 'networkx<=2.8.7', 'gensim', 'rdflib' ],
     entry_points={ 'console_scripts': [ 'rdr = rdr.rdr:rdr' ] }
 )
```

