# Comparing `tmp/jphrase-0.0.1.tar.gz` & `tmp/jphrase-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jphrase-0.0.1.tar", last modified: Sat May 11 14:25:59 2024, max compression
+gzip compressed data, was "jphrase-0.0.2.tar", last modified: Sun May 12 15:23:57 2024, max compression
```

## Comparing `jphrase-0.0.1.tar` & `jphrase-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-11 14:25:59.994780 jphrase-0.0.1/
--rw-r--r--   0 jiro       (501) staff       (20)     1069 2024-05-09 08:54:48.000000 jphrase-0.0.1/LICENSE
--rw-r--r--   0 jiro       (501) staff       (20)     7497 2024-05-11 14:25:59.993900 jphrase-0.0.1/PKG-INFO
--rw-r--r--   0 jiro       (501) staff       (20)     7054 2024-05-11 14:21:45.000000 jphrase-0.0.1/README.md
--rw-r--r--   0 jiro       (501) staff       (20)       38 2024-05-11 14:25:59.994833 jphrase-0.0.1/setup.cfg
--rw-r--r--   0 jiro       (501) staff       (20)      827 2024-05-11 13:51:45.000000 jphrase-0.0.1/setup.py
-drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-11 14:25:59.991541 jphrase-0.0.1/src/
-drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-11 14:25:59.992464 jphrase-0.0.1/src/jphrase/
--rw-r--r--   0 jiro       (501) staff       (20)       74 2024-05-09 14:29:27.000000 jphrase-0.0.1/src/jphrase/__init__.py
--rw-r--r--   0 jiro       (501) staff       (20)     6860 2024-05-11 14:03:55.000000 jphrase-0.0.1/src/jphrase/phrase_splitter.py
-drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-11 14:25:59.993623 jphrase-0.0.1/src/jphrase.egg-info/
--rw-r--r--   0 jiro       (501) staff       (20)     7497 2024-05-11 14:25:59.000000 jphrase-0.0.1/src/jphrase.egg-info/PKG-INFO
--rw-r--r--   0 jiro       (501) staff       (20)      251 2024-05-11 14:25:59.000000 jphrase-0.0.1/src/jphrase.egg-info/SOURCES.txt
--rw-r--r--   0 jiro       (501) staff       (20)        1 2024-05-11 14:25:59.000000 jphrase-0.0.1/src/jphrase.egg-info/dependency_links.txt
--rw-r--r--   0 jiro       (501) staff       (20)        8 2024-05-11 14:25:59.000000 jphrase-0.0.1/src/jphrase.egg-info/top_level.txt
-drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-11 14:25:59.993269 jphrase-0.0.1/tests/
--rw-r--r--   0 jiro       (501) staff       (20)     3340 2024-05-10 05:32:58.000000 jphrase-0.0.1/tests/test_phrase_splitter.py
+drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-12 15:23:57.850169 jphrase-0.0.2/
+-rw-r--r--   0 jiro       (501) staff       (20)     1069 2024-05-09 08:54:48.000000 jphrase-0.0.2/LICENSE
+-rw-r--r--   0 jiro       (501) staff       (20)     7500 2024-05-12 15:23:57.849900 jphrase-0.0.2/PKG-INFO
+-rw-r--r--   0 jiro       (501) staff       (20)     7057 2024-05-12 15:18:47.000000 jphrase-0.0.2/README.md
+-rw-r--r--   0 jiro       (501) staff       (20)       38 2024-05-12 15:23:57.850223 jphrase-0.0.2/setup.cfg
+-rw-r--r--   0 jiro       (501) staff       (20)      827 2024-05-12 15:18:47.000000 jphrase-0.0.2/setup.py
+drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-12 15:23:57.847506 jphrase-0.0.2/src/
+drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-12 15:23:57.848560 jphrase-0.0.2/src/jphrase/
+-rw-r--r--   0 jiro       (501) staff       (20)       74 2024-05-09 14:29:27.000000 jphrase-0.0.2/src/jphrase/__init__.py
+-rw-r--r--   0 jiro       (501) staff       (20)     7175 2024-05-12 15:18:47.000000 jphrase-0.0.2/src/jphrase/phrase_splitter.py
+drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-12 15:23:57.849612 jphrase-0.0.2/src/jphrase.egg-info/
+-rw-r--r--   0 jiro       (501) staff       (20)     7500 2024-05-12 15:23:57.000000 jphrase-0.0.2/src/jphrase.egg-info/PKG-INFO
+-rw-r--r--   0 jiro       (501) staff       (20)      251 2024-05-12 15:23:57.000000 jphrase-0.0.2/src/jphrase.egg-info/SOURCES.txt
+-rw-r--r--   0 jiro       (501) staff       (20)        1 2024-05-12 15:23:57.000000 jphrase-0.0.2/src/jphrase.egg-info/dependency_links.txt
+-rw-r--r--   0 jiro       (501) staff       (20)        8 2024-05-12 15:23:57.000000 jphrase-0.0.2/src/jphrase.egg-info/top_level.txt
+drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-12 15:23:57.849391 jphrase-0.0.2/tests/
+-rw-r--r--   0 jiro       (501) staff       (20)     3380 2024-05-12 15:18:47.000000 jphrase-0.0.2/tests/test_phrase_splitter.py
```

### Comparing `jphrase-0.0.1/LICENSE` & `jphrase-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jphrase-0.0.1/PKG-INFO` & `jphrase-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: jphrase
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Japanese phrase tokenizer
 Home-page: https://github.com/jiroshimaya/jphrase
 Author: shimajiroxyz
 Author-email: shimaya.jiro@irl.sys.es.osaka-u.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # jphrase
 jphraseは、日本語のテキストを文節に分割するためのライブラリです。
-形態素解析から得られた単語の品詞情報に基づき、ルールベースで文節を決定します、
+形態素解析から得られた単語の品詞情報に基づき、ルールベースで文節を決定します。
 
 # Basic Usage
 
 ```Python
-from jphrase import PHraseSplitter
+from jphrase import PhraseSplitter
 splitter = PhraseSplitter()
 print(splitter.split_text("今日はよく寝ました"))
 ```
 
 ```
 ['今日は', 'よく', '寝ました']
 ```
@@ -46,45 +46,45 @@
 ```
 pip install jphrase
 ```
 
 形態素解析ライブラリと辞書もインストールしてください。
 
 ```
-pip install mecab-python3 ipdaic
+pip install mecab-python3 ipadic
 ```
 
 mecab-python3以外の形態素解析ライブラリ、ipadic以外の辞書には現状非対応です。
 
 # Usage
 
-PhraseSplitterのインスタンスを作成し、split_textメソッドでで分割を実行してください。
+PhraseSplitterのインスタンスを作成し、split_textメソッドで分割を実行してください。
 
 ```Python
 from jphrase import PhraseSplitter
 splitter = PhraseSplitter()
 input_string = "今日はよく寝ていました"
 phrases = splitter.split_text(input_string)
 ```
 
 split_textにオプション引数を渡すことで、出力形式を調整できます。
 
 ```Python
-splitter = split_text(input_string, output_type = PharseSplitter.OUTPUT_SURFACE, consider_non_independent_nouns_and_verbs_as_breaks = True)
+phrases = splitter.split_text(input_string, output_type = PhraseSplitter.OUTPUT_SURFACE, consider_non_independent_nouns_and_verbs_as_breaks = True)
 ```
 
 output_type引数は、PhraseSplitterクラスのsplit_textメソッドの出力形式を指定するために使用されます。利用可能な出力形式は以下の通りです:
 
 1. `PhraseSplitter.OUTPUT_SURFACE`: 分割されたテキストを表層形のみで返します。各フレーズは文字列のリストとして返されます。
 2. `PhraseSplitter.OUTPUT_DETAILED`: 分割されたテキストを詳細な形態素情報と共に返します。各フレーズは辞書のリストとして返され、各辞書には形態素の表層形、品詞、読み、発音などの情報が含まれます。
 3. `PhraseSplitter.OUTPUT_CONCATENATED`: 分割されたテキストを連結された形で返します。各フレーズは表層形、読み、発音を含む辞書として返されます。
 
 output_type引数を指定しない場合、デフォルトの出力形式は`PhraseSplitter.OUTPUT_SURFACE`です。
 
-consider_non_independent_nouns_and_verbs_as_breaks引数は、非自立な名詞や動詞を文節の区切りとして扱うかどうかを制御します。この引数がTrueに設定されている場合、非自立な名刺や動詞の前で新しい文節が始まります。Falseの場合、非自立な名詞や動詞は前の文節に含まれ続けます。
+consider_non_independent_nouns_and_verbs_as_breaks引数は、非自立な名詞や動詞を文節の区切りとして扱うかどうかを制御します。この引数がTrueに設定されている場合、非自立な名詞や動詞の前で新しい文節が始まります。Falseの場合、非自立な名詞や動詞は前の文節に含まれ続けます。
 
 またこれらのオプション引数はPhraseSplitterのインスタンス作成時にも指定することができ、指定した場合は、split_text実行時のデフォルト値として扱われます。
 
 # Testing
 
 ```Python
 python tests/test_phrase_splitter.py
@@ -103,19 +103,21 @@
 ただし以下の条件に該当する場合は文節の境界とはみなさないようにします。
 
 |種類|例|判断方法|
 |---|---|---|
 |接尾辞|「痛さ」の「さ」など|品詞が「名詞」かつ品詞細分類に「接尾」が含まれている|
 |接頭詞の直後の単語|「お美しい」の「美しい」など（「お」が接頭詞）|直前の単語の品詞が「接頭詞」である|
 |サ変接続名詞の直後のサ変接続動詞|「勉強する」の「する」など|品詞が「動詞」、かつ、活用型が「サ変・スル」、かつ、直前の単語の品詞細分類に「サ変接続」が含まれている（注１）|
-|非自立な名詞（注２）|動詞や形容詞などの直後の「もの」「こと」や、「やったのか？」の(「もの・こと」という意味の）「の」など|品詞が「名詞」かつ品詞細分類に「非自立」が含まれている|
+|非自立な名詞（注２）|動詞や形容詞などの直後の「もの」「こと」や、「やったのか？」の「もの・こと」という意味の「の」など|品詞が「名詞」かつ品詞細分類に「非自立」が含まれている|
 |非自立な動詞（注２）|「やっている」の「いる」など|品詞が「動詞」かつ品詞細分類に「非自立」が含まれている|
 
 注１：辞書によっては、記号が「サ変接続」になって、その周辺の処理の精度が悪くなることがあるので注意。
+
 注２：jphraseではオプションによって非自立な名詞，動詞を文節の境界とするかどうか選択可能。これらは文法的には文節の境界とするのが正しいが、実際に結果を眺めた際に、分割が細かすぎると感じられるケースもあったため、そのようにした。
 
 また上記以外に、主に記号と連続するケースなどにおいて、より細かな例外処理が存在します。詳細はソースコードを参照してください。
 
 # Licensing
 
 jphraseはMITライセンスの下で公開されています。
 ただし、jphraseを使用する際に必要となる追加のライブラリや辞書は、それぞれのライセンス条項に従ってください。
+
```

### Comparing `jphrase-0.0.1/README.md` & `jphrase-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # jphrase
 jphraseは、日本語のテキストを文節に分割するためのライブラリです。
-形態素解析から得られた単語の品詞情報に基づき、ルールベースで文節を決定します、
+形態素解析から得られた単語の品詞情報に基づき、ルールベースで文節を決定します。
 
 # Basic Usage
 
 ```Python
-from jphrase import PHraseSplitter
+from jphrase import PhraseSplitter
 splitter = PhraseSplitter()
 print(splitter.split_text("今日はよく寝ました"))
 ```
 
 ```
 ['今日は', 'よく', '寝ました']
 ```
@@ -32,45 +32,45 @@
 ```
 pip install jphrase
 ```
 
 形態素解析ライブラリと辞書もインストールしてください。
 
 ```
-pip install mecab-python3 ipdaic
+pip install mecab-python3 ipadic
 ```
 
 mecab-python3以外の形態素解析ライブラリ、ipadic以外の辞書には現状非対応です。
 
 # Usage
 
-PhraseSplitterのインスタンスを作成し、split_textメソッドでで分割を実行してください。
+PhraseSplitterのインスタンスを作成し、split_textメソッドで分割を実行してください。
 
 ```Python
 from jphrase import PhraseSplitter
 splitter = PhraseSplitter()
 input_string = "今日はよく寝ていました"
 phrases = splitter.split_text(input_string)
 ```
 
 split_textにオプション引数を渡すことで、出力形式を調整できます。
 
 ```Python
-splitter = split_text(input_string, output_type = PharseSplitter.OUTPUT_SURFACE, consider_non_independent_nouns_and_verbs_as_breaks = True)
+phrases = splitter.split_text(input_string, output_type = PhraseSplitter.OUTPUT_SURFACE, consider_non_independent_nouns_and_verbs_as_breaks = True)
 ```
 
 output_type引数は、PhraseSplitterクラスのsplit_textメソッドの出力形式を指定するために使用されます。利用可能な出力形式は以下の通りです:
 
 1. `PhraseSplitter.OUTPUT_SURFACE`: 分割されたテキストを表層形のみで返します。各フレーズは文字列のリストとして返されます。
 2. `PhraseSplitter.OUTPUT_DETAILED`: 分割されたテキストを詳細な形態素情報と共に返します。各フレーズは辞書のリストとして返され、各辞書には形態素の表層形、品詞、読み、発音などの情報が含まれます。
 3. `PhraseSplitter.OUTPUT_CONCATENATED`: 分割されたテキストを連結された形で返します。各フレーズは表層形、読み、発音を含む辞書として返されます。
 
 output_type引数を指定しない場合、デフォルトの出力形式は`PhraseSplitter.OUTPUT_SURFACE`です。
 
-consider_non_independent_nouns_and_verbs_as_breaks引数は、非自立な名詞や動詞を文節の区切りとして扱うかどうかを制御します。この引数がTrueに設定されている場合、非自立な名刺や動詞の前で新しい文節が始まります。Falseの場合、非自立な名詞や動詞は前の文節に含まれ続けます。
+consider_non_independent_nouns_and_verbs_as_breaks引数は、非自立な名詞や動詞を文節の区切りとして扱うかどうかを制御します。この引数がTrueに設定されている場合、非自立な名詞や動詞の前で新しい文節が始まります。Falseの場合、非自立な名詞や動詞は前の文節に含まれ続けます。
 
 またこれらのオプション引数はPhraseSplitterのインスタンス作成時にも指定することができ、指定した場合は、split_text実行時のデフォルト値として扱われます。
 
 # Testing
 
 ```Python
 python tests/test_phrase_splitter.py
@@ -89,19 +89,21 @@
 ただし以下の条件に該当する場合は文節の境界とはみなさないようにします。
 
 |種類|例|判断方法|
 |---|---|---|
 |接尾辞|「痛さ」の「さ」など|品詞が「名詞」かつ品詞細分類に「接尾」が含まれている|
 |接頭詞の直後の単語|「お美しい」の「美しい」など（「お」が接頭詞）|直前の単語の品詞が「接頭詞」である|
 |サ変接続名詞の直後のサ変接続動詞|「勉強する」の「する」など|品詞が「動詞」、かつ、活用型が「サ変・スル」、かつ、直前の単語の品詞細分類に「サ変接続」が含まれている（注１）|
-|非自立な名詞（注２）|動詞や形容詞などの直後の「もの」「こと」や、「やったのか？」の(「もの・こと」という意味の）「の」など|品詞が「名詞」かつ品詞細分類に「非自立」が含まれている|
+|非自立な名詞（注２）|動詞や形容詞などの直後の「もの」「こと」や、「やったのか？」の「もの・こと」という意味の「の」など|品詞が「名詞」かつ品詞細分類に「非自立」が含まれている|
 |非自立な動詞（注２）|「やっている」の「いる」など|品詞が「動詞」かつ品詞細分類に「非自立」が含まれている|
 
 注１：辞書によっては、記号が「サ変接続」になって、その周辺の処理の精度が悪くなることがあるので注意。
+
 注２：jphraseではオプションによって非自立な名詞，動詞を文節の境界とするかどうか選択可能。これらは文法的には文節の境界とするのが正しいが、実際に結果を眺めた際に、分割が細かすぎると感じられるケースもあったため、そのようにした。
 
 また上記以外に、主に記号と連続するケースなどにおいて、より細かな例外処理が存在します。詳細はソースコードを参照してください。
 
 # Licensing
 
 jphraseはMITライセンスの下で公開されています。
 ただし、jphraseを使用する際に必要となる追加のライブラリや辞書は、それぞれのライセンス条項に従ってください。
+
```

### Comparing `jphrase-0.0.1/setup.py` & `jphrase-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="jphrase",  # PyPIに登録するパッケージ名
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(where='src'),  # パッケージはsrcディレクトリ内にある
     package_dir={'': 'src'},  # パッケージのルートディレクトリをsrcに設定
     install_requires=[],
     author="shimajiroxyz",
     author_email="shimaya.jiro@irl.sys.es.osaka-u.ac.jp",
     description="A Japanese phrase tokenizer",
     long_description=open('README.md').read(),
```

### Comparing `jphrase-0.0.1/src/jphrase/phrase_splitter.py` & `jphrase-0.0.2/src/jphrase/phrase_splitter.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,41 +49,43 @@
 
         if not current_phrase:
             return False
         if all(_token['pos'] == '記号' for _token in current_phrase):
             return False
                     
         phrase_break_pos_tags = ['名詞', '動詞', '接頭詞', '副詞', '感動詞', '形容詞', '形容動詞', '連体詞']
+        open_bra = '「『（【｛〈《〘〚)]}'
+        close_bra = '」』）】｝〉》〙〗)]}'
         
         pos_info = token['pos']
         pos_detail = ','.join([token['pos_detail_1'], token['pos_detail_2'], token['pos_detail_3']])
 
         previous_token = current_phrase[-1]
         previous_pos_info = previous_token['pos']
         previous_pos_detail = ','.join([previous_token['pos_detail_1'], previous_token['pos_detail_2'], previous_token['pos_detail_3']])
 
 
-        if pos_info == '記号':
+        if pos_info == '記号' and token['surface_form'] not in open_bra:
             return False
         
-        is_phrase_break_pos = pos_info in phrase_break_pos_tags
+        is_phrase_break_pos = pos_info in phrase_break_pos_tags or token['surface_form'] in open_bra
         if not consider_non_independent_nouns_and_verbs_as_breaks and '非自立' in pos_detail:
             is_phrase_break_pos = False
 
         if is_phrase_break_pos:
-            if previous_pos_info == '接頭詞':
+            if previous_pos_info == '接頭詞' or previous_token['surface_form'] in open_bra:
                 return False
             elif '接尾' in pos_detail:
                 return False
             elif token['conjugated_type'] == 'サ変・スル' and 'サ変接続' in previous_pos_detail:
                 return False
                         
             return True
         else:
-            if previous_pos_info == '記号' and previous_token['surface_form'] not in '」』）】｝〉》〙〗)]}':
+            if previous_pos_info == '記号' and previous_token['surface_form'] not in close_bra:
                 return True
             
             return False
                 
         return True
             
         
@@ -130,8 +132,10 @@
             self.OUTPUT_CONCATENATED: self.__split_text_into_concatenated_phrases
         }
         if output_type in split_methods:
             return split_methods[output_type](text, consider_non_independent_nouns_and_verbs_as_breaks)
         else:
             valid_types = ', '.join(split_methods.keys())
             raise ValueError(f"Invalid output type specified. Choose {valid_types}.")
-
+        
+if __name__=='__main__':
+    print(PhraseSplitter().split_text('「て。」や「に」などの'))
```

### Comparing `jphrase-0.0.1/src/jphrase.egg-info/PKG-INFO` & `jphrase-0.0.2/src/jphrase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: jphrase
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Japanese phrase tokenizer
 Home-page: https://github.com/jiroshimaya/jphrase
 Author: shimajiroxyz
 Author-email: shimaya.jiro@irl.sys.es.osaka-u.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # jphrase
 jphraseは、日本語のテキストを文節に分割するためのライブラリです。
-形態素解析から得られた単語の品詞情報に基づき、ルールベースで文節を決定します、
+形態素解析から得られた単語の品詞情報に基づき、ルールベースで文節を決定します。
 
 # Basic Usage
 
 ```Python
-from jphrase import PHraseSplitter
+from jphrase import PhraseSplitter
 splitter = PhraseSplitter()
 print(splitter.split_text("今日はよく寝ました"))
 ```
 
 ```
 ['今日は', 'よく', '寝ました']
 ```
@@ -46,45 +46,45 @@
 ```
 pip install jphrase
 ```
 
 形態素解析ライブラリと辞書もインストールしてください。
 
 ```
-pip install mecab-python3 ipdaic
+pip install mecab-python3 ipadic
 ```
 
 mecab-python3以外の形態素解析ライブラリ、ipadic以外の辞書には現状非対応です。
 
 # Usage
 
-PhraseSplitterのインスタンスを作成し、split_textメソッドでで分割を実行してください。
+PhraseSplitterのインスタンスを作成し、split_textメソッドで分割を実行してください。
 
 ```Python
 from jphrase import PhraseSplitter
 splitter = PhraseSplitter()
 input_string = "今日はよく寝ていました"
 phrases = splitter.split_text(input_string)
 ```
 
 split_textにオプション引数を渡すことで、出力形式を調整できます。
 
 ```Python
-splitter = split_text(input_string, output_type = PharseSplitter.OUTPUT_SURFACE, consider_non_independent_nouns_and_verbs_as_breaks = True)
+phrases = splitter.split_text(input_string, output_type = PhraseSplitter.OUTPUT_SURFACE, consider_non_independent_nouns_and_verbs_as_breaks = True)
 ```
 
 output_type引数は、PhraseSplitterクラスのsplit_textメソッドの出力形式を指定するために使用されます。利用可能な出力形式は以下の通りです:
 
 1. `PhraseSplitter.OUTPUT_SURFACE`: 分割されたテキストを表層形のみで返します。各フレーズは文字列のリストとして返されます。
 2. `PhraseSplitter.OUTPUT_DETAILED`: 分割されたテキストを詳細な形態素情報と共に返します。各フレーズは辞書のリストとして返され、各辞書には形態素の表層形、品詞、読み、発音などの情報が含まれます。
 3. `PhraseSplitter.OUTPUT_CONCATENATED`: 分割されたテキストを連結された形で返します。各フレーズは表層形、読み、発音を含む辞書として返されます。
 
 output_type引数を指定しない場合、デフォルトの出力形式は`PhraseSplitter.OUTPUT_SURFACE`です。
 
-consider_non_independent_nouns_and_verbs_as_breaks引数は、非自立な名詞や動詞を文節の区切りとして扱うかどうかを制御します。この引数がTrueに設定されている場合、非自立な名刺や動詞の前で新しい文節が始まります。Falseの場合、非自立な名詞や動詞は前の文節に含まれ続けます。
+consider_non_independent_nouns_and_verbs_as_breaks引数は、非自立な名詞や動詞を文節の区切りとして扱うかどうかを制御します。この引数がTrueに設定されている場合、非自立な名詞や動詞の前で新しい文節が始まります。Falseの場合、非自立な名詞や動詞は前の文節に含まれ続けます。
 
 またこれらのオプション引数はPhraseSplitterのインスタンス作成時にも指定することができ、指定した場合は、split_text実行時のデフォルト値として扱われます。
 
 # Testing
 
 ```Python
 python tests/test_phrase_splitter.py
@@ -103,19 +103,21 @@
 ただし以下の条件に該当する場合は文節の境界とはみなさないようにします。
 
 |種類|例|判断方法|
 |---|---|---|
 |接尾辞|「痛さ」の「さ」など|品詞が「名詞」かつ品詞細分類に「接尾」が含まれている|
 |接頭詞の直後の単語|「お美しい」の「美しい」など（「お」が接頭詞）|直前の単語の品詞が「接頭詞」である|
 |サ変接続名詞の直後のサ変接続動詞|「勉強する」の「する」など|品詞が「動詞」、かつ、活用型が「サ変・スル」、かつ、直前の単語の品詞細分類に「サ変接続」が含まれている（注１）|
-|非自立な名詞（注２）|動詞や形容詞などの直後の「もの」「こと」や、「やったのか？」の(「もの・こと」という意味の）「の」など|品詞が「名詞」かつ品詞細分類に「非自立」が含まれている|
+|非自立な名詞（注２）|動詞や形容詞などの直後の「もの」「こと」や、「やったのか？」の「もの・こと」という意味の「の」など|品詞が「名詞」かつ品詞細分類に「非自立」が含まれている|
 |非自立な動詞（注２）|「やっている」の「いる」など|品詞が「動詞」かつ品詞細分類に「非自立」が含まれている|
 
 注１：辞書によっては、記号が「サ変接続」になって、その周辺の処理の精度が悪くなることがあるので注意。
+
 注２：jphraseではオプションによって非自立な名詞，動詞を文節の境界とするかどうか選択可能。これらは文法的には文節の境界とするのが正しいが、実際に結果を眺めた際に、分割が細かすぎると感じられるケースもあったため、そのようにした。
 
 また上記以外に、主に記号と連続するケースなどにおいて、より細かな例外処理が存在します。詳細はソースコードを参照してください。
 
 # Licensing
 
 jphraseはMITライセンスの下で公開されています。
 ただし、jphraseを使用する際に必要となる追加のライブラリや辞書は、それぞれのライセンス条項に従ってください。
+
```

### Comparing `jphrase-0.0.1/tests/test_phrase_splitter.py` & `jphrase-0.0.2/tests/test_phrase_splitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,55 +6,55 @@
         self.splitter = PhraseSplitter()
         self.base_cases = [
             ["痛さを", ["痛さを"]] #接尾辞
             , ["ご丁寧に", ["ご丁寧に"]] # 接頭辞
             , ["勉強する", ["勉強する"]] #サ変接続名詞+サ変
             , ["abcする", ["abc", "する"]] #Unknown名詞+サ変
             , ["違うする", ["違う", "する"]] #名詞以外+サ変
-            , ["「あなたは、『どこ』？」", ["「あなたは、『", "どこ』？」"]] # 記号
+            , ["「あなたは、『どこ』？」", ["「あなたは、", "『どこ』？」"]] # 記号
             , ["はが", ["はが"]] # 助詞から始まる文節
             , ["て、に、を、はなどの", ["て、","に、","を、","はなどの"]] # 記号直後の助詞
-            , ["「て。」や「に」などの", ["「て。」や「","に」などの"]] # 閉じカッコ直後の助詞
+            , ["「て。」や「に」などの", ["「て。」や","「に」などの"]] # 閉じカッコ直後の助詞
         ]
 
     def test_split_text_surface_true(self):
         
         specific_cases = [
             ["寝ているところなんです", ["寝て", "いる", "ところな","んです"]] # 非自立動詞
             , ["寝ている、ところ", ["寝て","いる、", "ところ"]] # 非自立名詞
             , ["寝ている」ところ", ["寝て","いる」", "ところ"]] # 非自立名詞
             ]
         for input_string, expected in self.base_cases + specific_cases:
-            result = self.splitter.split_text(input_string, output_type=PhraseSplitter.OUTPUT_SURFACE, consider_non_independent_nouns_as_breaks=True)
+            result = self.splitter.split_text(input_string, output_type=PhraseSplitter.OUTPUT_SURFACE, consider_non_independent_nouns_and_verbs_as_breaks=True)
             self.assertEqual(result, expected)
 
     def test_split_text_surface_false(self):
         specific_cases = [
             ["寝ているところなんです", ["寝ているところなんです"]] # 非自立動詞
             , ["寝ている、ところ", ["寝ている、", "ところ"]] # 非自立名詞
             , ["寝ている」ところ", ["寝ている」ところ"]] # 非自立名詞
             ]
         for input_string, expected in self.base_cases + specific_cases:
-            result = self.splitter.split_text(input_string, output_type=PhraseSplitter.OUTPUT_SURFACE, consider_non_independent_nouns_as_breaks=False)
+            result = self.splitter.split_text(input_string, output_type=PhraseSplitter.OUTPUT_SURFACE, consider_non_independent_nouns_and_verbs_as_breaks=False)
             self.assertEqual(result, expected)
 
     def test_split_text_detailed_true(self):
         specific_cases = [
             ["寝ている", [['寝', 'て'], ['いる']]]
             ]
         for input_string, expected in specific_cases:
-            detailed_phrases = self.splitter.split_text(input_string, PhraseSplitter.OUTPUT_DETAILED, consider_non_independent_nouns_as_breaks=True)
+            detailed_phrases = self.splitter.split_text(input_string, PhraseSplitter.OUTPUT_DETAILED, consider_non_independent_nouns_and_verbs_as_breaks=True)
             surface_forms_only = [[token['surface_form'] for token in phrase] for phrase in detailed_phrases]
             result = surface_forms_only
             self.assertEqual(result, expected)
 
     def test_split_text_concatenated_true(self):
         specific_cases = [
             ["今日は", [{'surface_form': '今日は', 'reading': 'キョウハ', 'pronunciation': 'キョーワ'}]]
             ]
         for input_string, expected in specific_cases:
-            result = self.splitter.split_text(input_string, output_type=PhraseSplitter.OUTPUT_CONCATENATED, consider_non_independent_nouns_as_breaks=True)
+            result = self.splitter.split_text(input_string, output_type=PhraseSplitter.OUTPUT_CONCATENATED, consider_non_independent_nouns_and_verbs_as_breaks=True)
             self.assertEqual(result, expected)
 
 
 if __name__ == '__main__':
     unittest.main()
```

