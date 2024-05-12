# Comparing `tmp/autoanki-1.1.9.tar.gz` & `tmp/autoanki-1.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoanki-1.1.9.tar", last modified: Mon Apr 15 21:47:26 2024, max compression
+gzip compressed data, was "autoanki-1.1.91.tar", last modified: Sun May 12 03:02:20 2024, max compression
```

## Comparing `autoanki-1.1.9.tar` & `autoanki-1.1.91.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.161110 autoanki-1.1.9/
--rw-r--r--   0 owner      (501) staff       (20)     1062 2024-04-04 21:53:37.000000 autoanki-1.1.9/LICENSE.txt
--rw-r--r--   0 owner      (501) staff       (20)      110 2024-04-15 18:10:25.000000 autoanki-1.1.9/MANIFEST.in
--rw-r--r--   0 owner      (501) staff       (20)     5558 2024-04-15 21:47:26.161024 autoanki-1.1.9/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)     5024 2024-04-15 21:45:41.000000 autoanki-1.1.9/README.md
--rw-r--r--   0 owner      (501) staff       (20)      223 2023-05-05 21:35:51.000000 autoanki-1.1.9/pyproject.toml
--rw-r--r--   0 owner      (501) staff       (20)      700 2024-04-15 21:47:26.162032 autoanki-1.1.9/setup.cfg
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.138400 autoanki-1.1.9/src/
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.140272 autoanki-1.1.9/src/autoanki/
--rw-r--r--   0 owner      (501) staff       (20)     6228 2024-04-15 21:29:46.000000 autoanki-1.1.9/src/autoanki/AutoAnki.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.141950 autoanki-1.1.9/src/autoanki/BookCleaner/
--rw-r--r--   0 owner      (501) staff       (20)     4435 2024-04-15 18:04:41.000000 autoanki-1.1.9/src/autoanki/BookCleaner/BookCleaner.py
--rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.1.9/src/autoanki/BookCleaner/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.143228 autoanki-1.1.9/src/autoanki/DatabaseManager/
--rw-r--r--   0 owner      (501) staff       (20)    13775 2024-04-15 20:45:52.000000 autoanki-1.1.9/src/autoanki/DatabaseManager/DatabaseManager.py
--rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.1.9/src/autoanki/DatabaseManager/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.1.9/src/autoanki/DatabaseManager/book_table.sql
--rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.1.9/src/autoanki/DatabaseManager/book_table_view.sql
--rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.1.9/src/autoanki/DatabaseManager/databases_init.sql
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.144090 autoanki-1.1.9/src/autoanki/DeckManager/
--rw-r--r--   0 owner      (501) staff       (20)     4692 2024-04-15 21:30:15.000000 autoanki-1.1.9/src/autoanki/DeckManager/DeckManager.py
--rw-r--r--   0 owner      (501) staff       (20)       67 2024-04-04 22:41:18.000000 autoanki-1.1.9/src/autoanki/DeckManager/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)     2654 2024-04-15 21:12:02.000000 autoanki-1.1.9/src/autoanki/DeckManager/template_decks.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.145512 autoanki-1.1.9/src/autoanki/Dictionary/
--rw-r--r--   0 owner      (501) staff       (20)     5791 2024-04-15 21:07:12.000000 autoanki-1.1.9/src/autoanki/Dictionary/CEDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)      286 2024-04-12 01:17:18.000000 autoanki-1.1.9/src/autoanki/Dictionary/Dictionary.py
--rw-r--r--   0 owner      (501) staff       (20)     5339 2024-04-15 18:03:31.000000 autoanki-1.1.9/src/autoanki/Dictionary/YellowBridgeDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)       40 2024-03-31 20:26:56.000000 autoanki-1.1.9/src/autoanki/Dictionary/__init__.py
--rw-rw-r--   0 owner      (501) staff       (20)  9650508 2024-04-10 22:45:58.000000 autoanki-1.1.9/src/autoanki/Dictionary/cedict_ts.u8
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.158726 autoanki-1.1.9/src/autoanki/Tokenizer/
--rw-r--r--   0 owner      (501) staff       (20)     6607 2024-04-15 21:23:30.000000 autoanki-1.1.9/src/autoanki/Tokenizer/ChineseTokenizer.py
--rw-r--r--   0 owner      (501) staff       (20)      223 2024-04-12 14:29:21.000000 autoanki-1.1.9/src/autoanki/Tokenizer/Tokenizer.py
--rw-r--r--   0 owner      (501) staff       (20)       48 2024-04-11 22:24:23.000000 autoanki-1.1.9/src/autoanki/Tokenizer/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.1.9/src/autoanki/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-15 21:47:26.160659 autoanki-1.1.9/src/autoanki.egg-info/
--rw-r--r--   0 owner      (501) staff       (20)     5558 2024-04-15 21:47:26.000000 autoanki-1.1.9/src/autoanki.egg-info/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)     1029 2024-04-15 21:47:26.000000 autoanki-1.1.9/src/autoanki.egg-info/SOURCES.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2024-04-15 21:47:26.000000 autoanki-1.1.9/src/autoanki.egg-info/dependency_links.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.1.9/src/autoanki.egg-info/not-zip-safe
--rw-r--r--   0 owner      (501) staff       (20)        9 2024-04-15 21:47:26.000000 autoanki-1.1.9/src/autoanki.egg-info/top_level.txt
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.297477 autoanki-1.1.91/
+-rw-r--r--   0 owner      (501) staff       (20)     1062 2024-04-04 21:53:37.000000 autoanki-1.1.91/LICENSE.txt
+-rw-r--r--   0 owner      (501) staff       (20)      134 2024-05-12 02:29:19.000000 autoanki-1.1.91/MANIFEST.in
+-rw-r--r--   0 owner      (501) staff       (20)     5559 2024-05-12 03:02:20.297403 autoanki-1.1.91/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)     5024 2024-04-15 21:45:41.000000 autoanki-1.1.91/README.md
+-rw-r--r--   0 owner      (501) staff       (20)      223 2023-05-05 21:35:51.000000 autoanki-1.1.91/pyproject.toml
+-rw-r--r--   0 owner      (501) staff       (20)      125 2024-04-14 18:52:00.000000 autoanki-1.1.91/requirements.txt
+-rw-r--r--   0 owner      (501) staff       (20)      701 2024-05-12 03:02:20.298227 autoanki-1.1.91/setup.cfg
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.274367 autoanki-1.1.91/src/
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.276563 autoanki-1.1.91/src/autoanki/
+-rw-r--r--   0 owner      (501) staff       (20)     6234 2024-05-08 02:45:14.000000 autoanki-1.1.91/src/autoanki/AutoAnki.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.278149 autoanki-1.1.91/src/autoanki/BookCleaner/
+-rw-r--r--   0 owner      (501) staff       (20)     4480 2024-05-08 01:47:01.000000 autoanki-1.1.91/src/autoanki/BookCleaner/BookCleaner.py
+-rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.1.91/src/autoanki/BookCleaner/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.279513 autoanki-1.1.91/src/autoanki/DatabaseManager/
+-rw-r--r--   0 owner      (501) staff       (20)    14271 2024-05-12 01:52:56.000000 autoanki-1.1.91/src/autoanki/DatabaseManager/DatabaseManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.1.91/src/autoanki/DatabaseManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.1.91/src/autoanki/DatabaseManager/book_table.sql
+-rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.1.91/src/autoanki/DatabaseManager/book_table_view.sql
+-rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.1.91/src/autoanki/DatabaseManager/databases_init.sql
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.280603 autoanki-1.1.91/src/autoanki/DeckManager/
+-rw-r--r--   0 owner      (501) staff       (20)     4745 2024-05-08 02:25:04.000000 autoanki-1.1.91/src/autoanki/DeckManager/DeckManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       67 2024-04-04 22:41:18.000000 autoanki-1.1.91/src/autoanki/DeckManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)     2654 2024-04-15 21:12:02.000000 autoanki-1.1.91/src/autoanki/DeckManager/template_decks.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.282433 autoanki-1.1.91/src/autoanki/Dictionary/
+-rw-r--r--   0 owner      (501) staff       (20)     6441 2024-05-08 02:44:04.000000 autoanki-1.1.91/src/autoanki/Dictionary/CEDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)      286 2024-04-12 01:17:18.000000 autoanki-1.1.91/src/autoanki/Dictionary/Dictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)     5339 2024-04-15 18:03:31.000000 autoanki-1.1.91/src/autoanki/Dictionary/YellowBridgeDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)       40 2024-03-31 20:26:56.000000 autoanki-1.1.91/src/autoanki/Dictionary/__init__.py
+-rw-rw-r--   0 owner      (501) staff       (20)  9650508 2024-04-10 22:45:58.000000 autoanki-1.1.91/src/autoanki/Dictionary/cedict_ts.u8
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.296725 autoanki-1.1.91/src/autoanki/Tokenizer/
+-rw-r--r--   0 owner      (501) staff       (20)     6669 2024-05-08 02:41:46.000000 autoanki-1.1.91/src/autoanki/Tokenizer/ChineseTokenizer.py
+-rw-r--r--   0 owner      (501) staff       (20)      223 2024-04-12 14:29:21.000000 autoanki-1.1.91/src/autoanki/Tokenizer/Tokenizer.py
+-rw-r--r--   0 owner      (501) staff       (20)       48 2024-04-11 22:24:23.000000 autoanki-1.1.91/src/autoanki/Tokenizer/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.1.91/src/autoanki/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.297073 autoanki-1.1.91/src/autoanki.egg-info/
+-rw-r--r--   0 owner      (501) staff       (20)     5559 2024-05-12 03:02:20.000000 autoanki-1.1.91/src/autoanki.egg-info/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)     1046 2024-05-12 03:02:20.000000 autoanki-1.1.91/src/autoanki.egg-info/SOURCES.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2024-05-12 03:02:20.000000 autoanki-1.1.91/src/autoanki.egg-info/dependency_links.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.1.91/src/autoanki.egg-info/not-zip-safe
+-rw-r--r--   0 owner      (501) staff       (20)        9 2024-05-12 03:02:20.000000 autoanki-1.1.91/src/autoanki.egg-info/top_level.txt
```

### Comparing `autoanki-1.1.9/LICENSE.txt` & `autoanki-1.1.91/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.9/PKG-INFO` & `autoanki-1.1.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.1.9
+Version: 1.1.91
 Summary: Automatically make Anki Decks for Chinese text
 Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
 Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autoanki-1.1.9/README.md` & `autoanki-1.1.91/README.md`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.9/setup.cfg` & `autoanki-1.1.91/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = autoanki
-version = 1.1.9
+version = 1.1.91
 author = Jarvis Coghlin
 author_email = jarviscoghlin@gmail.com
 description = Automatically make Anki Decks for Chinese text
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/timmy6figures/autoanki
 project_urls =
```

### Comparing `autoanki-1.1.9/src/autoanki/AutoAnki.py` & `autoanki-1.1.91/src/autoanki/AutoAnki.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 MAGENTA = "\u001b[35m"
 CYAN = "\u001b[36m"
 WHITE = "\u001b[37m"
 RESET = "\u001b[0m"
 logging.basicConfig(
     # filename='HISTORY.log',
     level=logging.WARNING,
-    format=f'{GREEN}%(asctime)s{RESET} {RED}%(levelname)8s{RESET} {YELLOW}%(name)16s{RESET}: %(message)s',
+    format=f'{GREEN}%(asctime)s{RESET} {RED}%(levelname)8s{RESET} {YELLOW}%(name)-16s{RESET}: %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S',
 )
 
+
 class AutoAnki:
 
     def __init__(self, database_filepath='autoanki.db', debug_level=20, force=False, dictionary=None):
         """
         Creates an instance of autoanki.
         This creates a book cleaner, database connection, dictioary connection, and deck maker
         :param database_filepath: The filepath for the database
@@ -62,17 +63,17 @@
         :param book_path: The filepath to the directory that contains the files to add. e.g. lost_prince.txt
         :param book_name: The name of the book being added e.g. "Lost Prince"
         :return:
         """
         self.logger.debug(f"autoanki: Adding book from [{book_path}]")
 
         # Clean the book
-        if not self.book_cleaner.clean(book_path):
+        # if not self.book_cleaner.clean(book_path):
             # self.logger.warning("autoanki: Unable to clean book [" + book_name + "].")
-            return
+            # return
 
         # Add the book to the database
         if not self.database_manager.add_book(book_path, book_name):
             self.logger.warning("Unable to add [" + book_name + "] to database.")
             return
 
         self.logger.info("autoanki: Added [" + book_path + "].")
```

### Comparing `autoanki-1.1.9/src/autoanki/BookCleaner/BookCleaner.py` & `autoanki-1.1.91/src/autoanki/BookCleaner/BookCleaner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import logging
 import os
 
+# TODO: I think that the entire book cleaner file is not needed. 
+#   Words should not be written back to a file. This is slow
 CLEANED_FILES_DIRECTORY = 'cleaned_files'
 CLEANED_FILES_SUFFIX = '_cleaned'
 # Sentences That should not be added to the completed file.
 GARBAGE_SENTENCES = ['',
                      "",
+                     ".",
                      "。",
                      "\n"]
 
 
 class BookCleaner:
 
     def __init__(self, debug_level, force=False):
         """ Internal tool used to sanatize input
         Use `clean(bookpath)` to sanatize files and remove junk data
-        `force` Ignore confirmations on if you want to clean >50 files
+        Args:
+            `force`: Ignore confirmations on if you want to clean >50 files
         """
         self.logger = logging.getLogger('autoanki.bookcleaner')
         self.logger.setLevel(debug_level)
         self.file_list = []
         self.bookpath = ""
         self.force = force
 
@@ -30,14 +34,15 @@
             `bookpath: filepath of files to be cleaned`
         Return: 
             `str: list of cleaned file(s)`
         """
         if not os.path.exists(bookpath):
             self.logger.warning("Cannot find path [" + str(bookpath) + "]")
             return None
+        self.logger.info("Bookpath: " + bookpath)
 
         # If the bookpath is a single file, clean and return it
         if os.path.isfile(bookpath):
             cleaned_files = [self._clean_file(bookpath, cleaned_files_root=None)]
             return cleaned_files
         else:
             dirty_files = []
@@ -61,34 +66,32 @@
         # Create directory for files
         cleaned_files_root = os.path.join(bookpath, CLEANED_FILES_DIRECTORY)
         if not os.path.exists(cleaned_files_root):
             os.mkdir(cleaned_files_root)
 
         for file in dirty_files:
             cleaned_filepath = self._clean_file(file, cleaned_files_root=cleaned_files_root)
-            cleaned_files.append(cleaned_filepath)
+            if cleaned_filepath:
+                cleaned_files.append(cleaned_filepath)
 
         return cleaned_files
 
-    def _clean_file(self, filepath, cleaned_files_root):
+    def _clean_file(self, filepath: str, cleaned_files_root: str):
         """
-        Takes a txt file and cleans it up, putting every sentence on a new line
-        :param filepath: The txt file to clean
-        :param cleaned_files_root: The root
-        :return:
+        Takes a txt file and cleans it up, filtering junk and putting every sentence on a new line
+        Args:
+            `filepath`: The txt file to clean
+            `cleaned_files_root`: The root
         """
-        # Set the directory where the cleaned file will go
-        if not cleaned_files_root:
-            # root/test1.txt -> root/hello_cleaned.txt
-            new_filepath = os.path.splitext(filepath)[0] + CLEANED_FILES_SUFFIX + os.path.splitext(filepath)[1]
-        else:
-            # TODO I'm suspicious that this works every time
-            new_filepath = os.path.join(cleaned_files_root, '/'.join(filepath.split('/')[2:]))
-        # self.logger.debug(f"Old filepath: [{filepath}]")
-        # self.logger.debug(f"New filepath: [{new_filepath}]")
+
+        # TODO: This will not work for books with nested files that share the same name
+        filename = os.path.basename(filepath)
+        new_filepath = os.path.join(cleaned_files_root, filename)
+        self.logger.debug("Filepath:     " + filepath)
+        self.logger.debug("New filepath: " + new_filepath)
 
         # Clean page file of characters that may cause issues.
         page_file = open(filepath, encoding='utf-8')
         try: 
             page_sentences = page_file.read().split("。")
         except:
             self.logger.error(f"Critical error cleaning file: [{filepath}]")
```

### Comparing `autoanki-1.1.9/src/autoanki/DatabaseManager/DatabaseManager.py` & `autoanki-1.1.91/src/autoanki/DatabaseManager/DatabaseManager.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 from autoanki.BookCleaner.BookCleaner import CLEANED_FILES_DIRECTORY
 from autoanki.Tokenizer.ChineseTokenizer import ChineseTokenizer
 
 
 class DatabaseManager:
 
     def __init__(self, database_path, debug_level):
-        # TODO Documentation
+        """Interfaces with an SQLLite database containing information on words, definitions, and more
+
+        """
         self.logger = logging.getLogger('autoanki.dbmngr')
         self.logger.setLevel(debug_level)
 
         # Init database
         if not os.path.exists(database_path):
             self.logger.warning("The database [", database_path, "] does not exist.")
             raise Exception("Cannot create DatabaseManager with invalid database path.")
@@ -34,25 +36,31 @@
 
         self.books = []
 
     @staticmethod
     def convert_to_tablename(name: str) -> str:
         """
         Converts a string to a sql-valid table name.
-        `param name` The name to convert
-        `return` A tablename valid for an sql table
+        Args:
+            `name`: The name to convert
+        Return:
+            A valid sql table name
         """
         value = unicodedata.normalize('NFKC', name)
         # value.replace("：",":")
         value = value.replace("：", "__")
         value = re.sub(r'[^\w\s-]', '', value.lower())
         return re.sub(r'[-\s]+', '_', value).strip('-_')
 
     @staticmethod
     def is_database(database_name:str):
+        """ Verifies integrity of AutoAnki database
+        Args:
+            `database_name`: Filepath of database
+        """
         if not database_name.endswith(".db"):
             return False
         if not os.path.exists(database_name):
             return False
         try:
             connection = sqlite3.connect(database_name)
             cursor = connection.cursor()
@@ -60,18 +68,18 @@
             cursor.execute("SELECT word FROM dictionary")
             connection.close()
         except sqlite3.OperationalError:
             return False
         return True
 
     @staticmethod
-    def create_database(database_path):
-        """
-        Creates an autoanki database file, including all tables needed for autoanki
-        `database_path` The path to the database to create
+    def create_database(database_path: str):
+        """ Creates autoanki database file, including all tables needed
+        Args:
+            `database_path`: The path to the database to create
         """
         logger = logging.getLogger('autoanki.dbmngr')
         logger.info("Creating database [" + database_path + "]")
         # TODO Fix this logger
         path = os.path.join(os.path.dirname(__file__), 'databases_init.sql')
         try:
             with open(path, 'r') as sql_file:
@@ -81,18 +89,19 @@
             cursor.executescript(sql_script)
             connection.commit()
         except FileNotFoundError:
             logger.warning("Could not create database: Missing SQL files")
             return False
 
     def _create_book_table(self, book_name, table_name) -> bool:
-        """
-        Creates a new entry in the book_list table
-        `table_name` The name of the new entry to create
-        `return` False if error
+        """ Creates a new entry in the book_list table
+        Args:
+            `table_name`: The name of the new entry to create
+        Return:
+            False if error
         """
         self.cursor.execute("SELECT table_name FROM book_list")
         book_list = self.cursor.fetchall()
 
         if (table_name,) in book_list:
             self.logger.warning("The book is already in database. Not adding")
             return False
@@ -109,20 +118,20 @@
         book_table_file = book_table_file.replace("BOOK_NAME", table_name)
         fd.close()
         # Create the new table
         self.cursor.execute(book_table_file)
         self.connection.commit()
         return True
 
-    def add_file_to_database(self, filepath, table_name):
-        """
-        Adds every word in a file to both the dictionary table and the book's table
-        `filepath` The path to the file
-        `table_name` The name of the table to add the words to.
-            This should be the same for every wile in a given book
+    def add_file_to_database(self, filepath: str, table_name: str):
+        """ Adds every word in a file to both the dictionary table and the book's table
+        Args:
+            `filepath`: The path to the file
+            `table_name`: The name of the table to add the words to.
+                This should be the same for every wile in a given book
         """
         self.logger.info(f"Adding [{filepath}] to database...")
         word_appearances = {}
         with open(filepath,'r',encoding='utf-8') as f:
             line = " "
             while line:
                 line = f.readline().strip(" ")
@@ -184,54 +193,57 @@
                                     f"VALUES (?,?)", [dictionary_word_id, word_appearances[word]])
                 self.connection.commit()
 
         # self.logger.debug("Done adding file to database")
 
     def insert_word(self, word):
         # TODO Doing this breaks the `number_of_appearances`. This is a temporary fix
+        # TODO This is really ineficcient
+        #   Either contain an internal dict of words in the dictionary, 
+        #   or wrap this with a try catch
         self.cursor.execute("SELECT word FROM dictionary WHERE word = ?", [word])
         all_rows = self.cursor.fetchall()
         if len(all_rows) == 0:
             # self.logger.info("  Inserting")
             self.cursor.execute(f"INSERT INTO dictionary (word) VALUES (?)", [word])
             self.connection.commit()
 
     def remove_word(self, word:str):
+        # TODO: Make more stringent constraints on removing words. This should be extremely rare
         if '*' in word:
             self.logger.info(f"Not executing: [{word}]. Star in command")
             return
         self.cursor.execute(f"DELETE FROM dictionary WHERE word=(?)", [word])
         self.connection.commit()
 
     def add_book(self, bookpath: str, book_name: str):
-        """
-        Adds a file to the autoanki database. This involves the following steps:\n
-        1 - Add book to the book_list table
+        """ Adds a file to the autoanki database. 
+        This involves the following steps:\n
+        1 - Add book to the `book_list` table
         2 - Add all the files in "bookpath" to the definitions table and book table
         3 - Add book to book_list property
 
         If given a directory, it will recursively search for all files in the directory and add them.
 
         if not already there, adding the
-        :param bookpath: The filepath to the book. This is file, or a directory of files
-        :param book_name: The name of the book. This will show up in the Anki deck
-        :return: None
+        Args:
+            `bookpath`: The filepath to the book. This is file, or a directory of files
+            `book_name: The name of the book. This will show up in the Anki deck
         """
         self.logger.info("Adding book...")
-
-        # Gets a 'table name' clean version of the book name
+        # Get a 'table name' clean version of the book name
         book_tablename = self.convert_to_tablename(book_name)
 
         # Add the name of the book to the book_list table
         success = self._create_book_table(book_name, book_tablename)
         if not success:
             self.logger.error("Failed to create book table")
             return
 
-        self.logger.debug(bookpath)
+        self.logger.debug("Bookpath: " + bookpath)
         if os.path.isdir(bookpath):
             self.logger.debug("Directory found:")
             result = [y for x in os.walk(bookpath + '/' + CLEANED_FILES_DIRECTORY) for y in glob(os.path.join(x[0], '*.txt'))]
             for path in result:
                 self.logger.debug(path)
                 self.add_file_to_database(path, book_tablename)
 
@@ -244,18 +256,15 @@
             self.logger.warning(f"Incorrect bookpath: [{bookpath}]")
             return False
 
         self.logger.info("Done adding book.")
         return True
 
     def print_info(self):
-        """
-        Print basic information about the database
-        :return:
-        """
+        """ Print basic information about the database """
         self.cursor.execute("SELECT word FROM dictionary")
         all_rows = self.cursor.fetchall()
         self.cursor.execute("SELECT word FROM dictionary WHERE definition IS NULL")
         unfinished_rows = self.cursor.fetchall()
         format_string_int = "{:<30} | {:>8}"
         format_string_dec = "{:<30} | {:>8.2}"
         print("------------------------")
@@ -264,16 +273,15 @@
         print(format_string_int.format("Number of books:", len(self.books)))
         print(format_string_dec.format("Database size (MB):", Path(self.database_path).stat().st_size / (1024 * 1024)))
         print("Dictionary Table:")
         print(format_string_int.format("Number of rows:", len(all_rows)))
         print(format_string_int.format("Number of unfinished rows:", len(unfinished_rows)))
 
     def update_definition(self, params: list):
-        f"""
-        Complete a definition for one word in the dictionary table\n
+        f""" Complete a definition for one word in the dictionary table\n
         traditional_script = params[0]\n
         word_type = params[1]\n
         pinyin = params[2]\n
         pinyin_numbers = params[3]\n
         sub_components = params[4]\n
         hsk_level = params[5]\n
         top_level = params[6]\n
```

### Comparing `autoanki-1.1.9/src/autoanki/DatabaseManager/databases_init.sql` & `autoanki-1.1.91/src/autoanki/DatabaseManager/databases_init.sql`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.9/src/autoanki/DeckManager/DeckManager.py` & `autoanki-1.1.91/src/autoanki/DeckManager/DeckManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
             "autoankiTesting"
         )
         self.include_pinyin_numbers = False
         self.include_number_of_strokes = False
         self.include_traditional = include_traditional 
         self.include_part_of_speech = include_part_of_speech
 
+        self.word_frequency_filter = None
+
         self.book_list = []
 
     def settings(self,
                  include_traditional,
                  include_part_of_speech,
                  word_frequency_filter
                  ):
@@ -113,15 +115,15 @@
                 pinyin = "Not found"
             if not definition:
                 definition = "Not found"
 
             note = genanki.Note(
                 model=template_decks.CHINESE_CARD_MODEL,
                 tags=['autoanki'],
-                fields=[word, word_traditional, pinyin, definition],
+                fields=[word, formatted_word_traditional, pinyin, definition],
                 # sort_field can be used to sort when the cards appear.
                 # By default they are shown in the order they are addeed, so this is not currently used
                 sort_field=1,
 
             )
             self.deck.add_note(note)
             num_of_valid_cards_added += 1
```

### Comparing `autoanki-1.1.9/src/autoanki/DeckManager/template_decks.py` & `autoanki-1.1.91/src/autoanki/DeckManager/template_decks.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.9/src/autoanki/Dictionary/CEDictionary.py` & `autoanki-1.1.91/src/autoanki/Dictionary/CEDictionary.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from os import path
 import logging
 
 import pinyin
 import jieba
+logging.getLogger("jieba").setLevel(logging.WARNING)
 import jieba.posseg as pseg
 import chinese_converter
 from wordfreq import word_frequency
 
 from autoanki.Dictionary.Dictionary import Dictionary
 
 PATH_TO_FILE = path.join(path.dirname(__file__), 'cedict_ts.u8')
 
-
 # Use the lookup table here: https://github.com/fxsjy/jieba
 NOUN = ['n', 'nt', 'nrt', 'ORG', 'nr', 'PER', 'ns', 'nw', 'nz', 'f', 's', 'an', 'zg', 'j']
 TIME = ['t', 'TIME', 'tg', 'g']
 ADPOSITION = ['p']
-PRONOUN = ['r']
+PRONOUN = ['r', 'rz', 'rg']
 QUANTIFIER = ['q', 'm']
 VERB = ['v', 'vd', 'vn', 'e', 'vg', 'h']
-ADVERB = ['ad', 'd', 'aq']
+ADVERB = ['ad', 'd', 'aq', 'df']
 OTHER = ['vn', 'xc', 'x']
-ADJECTIVE = ['a', 'b', 'ng']
+ADJECTIVE = ['a', 'b', 'ng', 'ag']
 CONJUNCTION = ['c']
 PARTICLE = ['y', 'u', 'uj', 'uz', 'ul', 'uv', 'ud', 'ug']
 PUNCTUATION = ['w']
 IDIOM = ['i', 'l']
 SUFFIX = ['k']
 OTHER = ['z', 'o', 'x']
 
@@ -43,15 +43,18 @@
         self.logger.info("Loading Chinese Dictionary (CEDictionary)")
         self.dict = self._parse_file()
         self.logger.debug("Done!")
         
         pass
 
     def _parse_file(self) -> dict[str, dict]:
-        self.logger.debug("Parsing file...")
+        """Parse dictionary file on load
+        `return` A dictionary of the information, the key being the Chinese word
+        """
+        self.logger.debug("Parsing CE-DICT file...")
         if not path.isfile(PATH_TO_FILE):
             self.logger.critical("Could not open dictionary file")
 
         # TODO Some entries use a dot in the midde
         #   e.g. 哈利·波特
         #   this does not currently match
         definitions = {}
@@ -86,14 +89,20 @@
                     definitions[current_word]['frequency'] = str(word_frequency(current_word, 'zh'))
 
                 definitions[current_word]['definition'] += '<br>' + definition 
                 last_word = current_word
 
         for key, _ in definitions.items():
             definitions[key]['definition'].strip('\n')
+            definitions[key]['definition'] = definitions[key]['definition'].lstrip('<br>')
+            definitions[key]['definition'] = definitions[key]['definition'].lstrip('/')
+
+            definitions[key]['definition'] = definitions[key]['definition'].rstrip('\n')
+            definitions[key]['definition'] = definitions[key]['definition'].rstrip('/')
+            # self.logger.info('[' + definitions[key]['definition'] + ']')
         return definitions
 
 
     def find_word(self, word: str) -> None | list[str]:
         """
         Find a word in the dictionary. This can be simplified, or traditional
         `return` Paramaters that get passed to the database
```

### Comparing `autoanki-1.1.9/src/autoanki/Dictionary/YellowBridgeDictionary.py` & `autoanki-1.1.91/src/autoanki/Dictionary/YellowBridgeDictionary.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.9/src/autoanki/Dictionary/cedict_ts.u8` & `autoanki-1.1.91/src/autoanki/Dictionary/cedict_ts.u8`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.9/src/autoanki/Tokenizer/ChineseTokenizer.py` & `autoanki-1.1.91/src/autoanki/Tokenizer/ChineseTokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import logging
+
 import jieba
+logging.getLogger("jieba").setLevel(logging.WARNING)
 import chinese_converter
 from string import punctuation
-import logging
 
 from autoanki.Dictionary.CEDictionary import CEDictionary
 
 # TODO Is there a way to do this in a smarter way? Maybe check if the characters are in a certian UTF-8 block?
 PUNCTUATION = """
 +,;:'()[]{}&*^%$#@!◇♦•·■◎∞=™©×
 """
-CHINESE_PUNC = "！？｡。．.…、＂＃＄％＆＇（）＊＋，－／：；＜＝＞＠［＼］＾＿｀｛｜｝～｟｠｢｣､、〃《》「」『』【】〔〕〖〗〘〙〚〛〜〝〞〟〰〾〿–—‘’‛“”„‟…‧﹏  ① ② ⑽ "
+CHINESE_PUNC = "！？｡。．.…、＂＃＄％＆＇（）＊＋，－／：；＜＝＞＠［＼］＾＿｀｛｜｝～｟｠｢｣､、〃《》「」『』【】〔〕〖〗〘〙〚〛〜〝〞〟〰〾〿–—‘’‛“”„‟…‧﹏  ① ② ③ ④ ⑽ "
 
 # TODO: This can be extened and implemented
 OTHER = "ｗ９ｌｉｔｂｎｅｐｈⅠ Ⅱ Ⅲ Ⅳ "
 
 # TODO Remove straight numbers and english words
 
 class ChineseTokenizer():
```

### Comparing `autoanki-1.1.9/src/autoanki.egg-info/PKG-INFO` & `autoanki-1.1.91/src/autoanki.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.1.9
+Version: 1.1.91
 Summary: Automatically make Anki Decks for Chinese text
 Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
 Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autoanki-1.1.9/src/autoanki.egg-info/SOURCES.txt` & `autoanki-1.1.91/src/autoanki.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
+requirements.txt
 setup.cfg
 src/autoanki/AutoAnki.py
 src/autoanki/__init__.py
 src/autoanki.egg-info/PKG-INFO
 src/autoanki.egg-info/SOURCES.txt
 src/autoanki.egg-info/dependency_links.txt
 src/autoanki.egg-info/not-zip-safe
```

