# Comparing `tmp/kitab-0.0.26.tar.gz` & `tmp/kitab-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitab-0.0.26.tar", last modified: Sun May 12 10:25:09 2024, max compression
+gzip compressed data, was "kitab-0.0.27.tar", last modified: Sun May 12 12:23:22 2024, max compression
```

## Comparing `kitab-0.0.26.tar` & `kitab-0.0.27.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.444533 kitab-0.0.26/
--rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.26/LICENSE
--rw-rw-rw-   0        0        0     6212 2024-05-12 10:25:09.434761 kitab-0.0.26/PKG-INFO
--rw-rw-rw-   0        0        0     5602 2024-05-12 10:23:37.000000 kitab-0.0.26/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.318653 kitab-0.0.26/kitab/
--rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.26/kitab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.383859 kitab-0.0.26/kitab/api/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.26/kitab/api/__init__.py
--rw-rw-rw-   0        0        0     8126 2024-05-12 10:22:02.000000 kitab-0.0.26/kitab/api/app.py
-drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.404101 kitab-0.0.26/kitab/db/
--rw-rw-rw-   0        0        0      416 2024-04-26 08:05:03.000000 kitab-0.0.26/kitab/db/__init__.py
--rw-rw-rw-   0        0        0      232 2024-05-07 05:22:41.000000 kitab-0.0.26/kitab/db/db_credentials.py
--rw-rw-rw-   0        0        0     1836 2024-04-25 20:34:46.000000 kitab-0.0.26/kitab/db/db_info.py
--rw-rw-rw-   0        0        0    20768 2024-05-10 10:10:49.000000 kitab-0.0.26/kitab/db/functions.py
--rw-rw-rw-   0        0        0     6825 2024-04-26 09:12:48.000000 kitab-0.0.26/kitab/db/get_data.py
--rw-rw-rw-   0        0        0    16160 2024-05-03 14:12:28.000000 kitab-0.0.26/kitab/db/sql_interactions.py
-drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.413947 kitab-0.0.26/kitab/logger/
--rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.26/kitab/logger/__init__.py
--rw-rw-rw-   0        0        0     1812 2024-04-25 18:53:05.000000 kitab-0.0.26/kitab/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.417577 kitab-0.0.26/kitab/recommendation_model/
--rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.26/kitab/recommendation_model/__init__.py
--rw-rw-rw-   0        0        0     5162 2024-05-03 14:37:05.000000 kitab-0.0.26/kitab/recommendation_model/models.py
--rw-rw-rw-   0        0        0     6366 2024-05-12 10:18:08.000000 kitab-0.0.26/kitab/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.434761 kitab-0.0.26/kitab.egg-info/
--rw-rw-rw-   0        0        0     6212 2024-05-12 10:25:09.000000 kitab-0.0.26/kitab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2024-05-12 10:25:09.000000 kitab-0.0.26/kitab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 10:25:09.000000 kitab-0.0.26/kitab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2024-05-12 10:25:09.000000 kitab-0.0.26/kitab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-12 10:25:09.000000 kitab-0.0.26/kitab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 10:25:09.445200 kitab-0.0.26/setup.cfg
--rw-rw-rw-   0        0        0     1053 2024-05-12 10:24:36.000000 kitab-0.0.26/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.429329 kitab-0.0.26/tests/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.26/tests/test_module1.py
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.26/tests/test_module2.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:23:22.282391 kitab-0.0.27/
+-rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.27/LICENSE
+-rw-rw-rw-   0        0        0     6212 2024-05-12 12:23:22.282391 kitab-0.0.27/PKG-INFO
+-rw-rw-rw-   0        0        0     5602 2024-05-12 10:23:37.000000 kitab-0.0.27/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 12:23:22.050553 kitab-0.0.27/kitab/
+-rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.27/kitab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:23:22.141923 kitab-0.0.27/kitab/api/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.27/kitab/api/__init__.py
+-rw-rw-rw-   0        0        0     8126 2024-05-12 10:22:02.000000 kitab-0.0.27/kitab/api/app.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:23:22.208655 kitab-0.0.27/kitab/db/
+-rw-rw-rw-   0        0        0      416 2024-04-26 08:05:03.000000 kitab-0.0.27/kitab/db/__init__.py
+-rw-rw-rw-   0        0        0      232 2024-05-07 05:22:41.000000 kitab-0.0.27/kitab/db/db_credentials.py
+-rw-rw-rw-   0        0        0     1836 2024-04-25 20:34:46.000000 kitab-0.0.27/kitab/db/db_info.py
+-rw-rw-rw-   0        0        0    21210 2024-05-12 12:17:28.000000 kitab-0.0.27/kitab/db/functions.py
+-rw-rw-rw-   0        0        0     6942 2024-05-12 12:18:45.000000 kitab-0.0.27/kitab/db/get_data.py
+-rw-rw-rw-   0        0        0    16160 2024-05-03 14:12:28.000000 kitab-0.0.27/kitab/db/sql_interactions.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:23:22.228370 kitab-0.0.27/kitab/logger/
+-rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.27/kitab/logger/__init__.py
+-rw-rw-rw-   0        0        0     1812 2024-04-25 18:53:05.000000 kitab-0.0.27/kitab/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:23:22.243301 kitab-0.0.27/kitab/recommendation_model/
+-rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.27/kitab/recommendation_model/__init__.py
+-rw-rw-rw-   0        0        0     5162 2024-05-12 12:19:06.000000 kitab-0.0.27/kitab/recommendation_model/models.py
+-rw-rw-rw-   0        0        0     6366 2024-05-12 10:18:08.000000 kitab-0.0.27/kitab/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:23:22.266197 kitab-0.0.27/kitab.egg-info/
+-rw-rw-rw-   0        0        0     6212 2024-05-12 12:23:21.000000 kitab-0.0.27/kitab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2024-05-12 12:23:21.000000 kitab-0.0.27/kitab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 12:23:21.000000 kitab-0.0.27/kitab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-05-12 12:23:21.000000 kitab-0.0.27/kitab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-12 12:23:21.000000 kitab-0.0.27/kitab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 12:23:22.282391 kitab-0.0.27/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2024-05-12 12:19:19.000000 kitab-0.0.27/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:23:22.265334 kitab-0.0.27/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.27/tests/test_module1.py
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.27/tests/test_module2.py
```

### Comparing `kitab-0.0.26/LICENSE` & `kitab-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `kitab-0.0.26/PKG-INFO` & `kitab-0.0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kitab
-Version: 0.0.26
+Version: 0.0.27
 Summary: A package for book recommendation.
 Author: Alexander Shahramanyan, Anna Charchyan, Yeva Manukyan, Lilith Asminian, Maria Petrosyan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `kitab-0.0.26/README.md` & `kitab-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `kitab-0.0.26/kitab/api/app.py` & `kitab-0.0.27/kitab/api/app.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.26/kitab/db/db_info.py` & `kitab-0.0.27/kitab/db/db_info.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.26/kitab/db/functions.py` & `kitab-0.0.27/kitab/db/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     """
     # Open connection to the database
     db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
     if verbose:
         logger.info("Database connection opened.")
     
     # Retrieve the book with the given title
-    books = db.get_table("book", conditions={"title": title})
+    books = db.get_table("book", conditions={"title": title}, verbose=verbose)
         
     if len(books) == 0:
         if verbose:
             logger.info("Book not found.")
         return None
     else:
         if verbose:
@@ -166,31 +166,31 @@
             logger.info("Book table populated.")
         
         # Add author(s) to the author table if doesn't exist
         authors = book["authors"]
         if len(authors) > 0:
             if verbose:
                 logger.info("Authors to be added.")
-            author_ids = _get_or_add_authors(db, authors)
+            author_ids = _get_or_add_authors(db, authors, verbose=verbose)
             
-            db.insert_records("bookauthor", [{"isbn": ISBN, "author_id": int(author_id)} for author_id in author_ids])
+            db.insert_records("bookauthor", [{"isbn": ISBN, "author_id": int(author_id)} for author_id in author_ids], verbose=verbose)
             if verbose:
                 logger.info("Author table populated.")
         else:
             if verbose:
                 logger.info("No authors to be added.")
         
         # Add genres to the genres table if doesn't exist
         genres = book["genres"]    
         if len(genres) > 0:
             if verbose:
                 logger.info("Genres to be added.")
-            genre_ids = _get_or_add_genres(db, genres)
+            genre_ids = _get_or_add_genres(db, genres, verbose=verbose)
             
-            db.insert_records("bookgenre", [{"isbn": ISBN, "genre_id": int(genre_id)} for genre_id in genre_ids])
+            db.insert_records("bookgenre", [{"isbn": ISBN, "genre_id": int(genre_id)} for genre_id in genre_ids], verbose=verbose)
             if verbose:
                 logger.info("Genre table populated.")
         else:
             if verbose:
                 logger.info("No genres to be added.")
 
         return True
@@ -235,59 +235,59 @@
             if key in ["ISBN", "title", "description", "available"]:
                 new_values[key] = new_book[key]
             if key == "ISBN":
                 latest_ISBN = new_book["ISBN"]
             if key == "description":
                 new_values["embedding"] = get_embedding(new_book["description"]).tolist()
 
-        db.update_records("book", new_values, condition)
+        db.update_records("book", new_values, condition, verbose=verbose)
         if verbose:
             logger.info("Book table updated.")
         
         ISBN = latest_ISBN
         
         # Get the tables
-        book_author = db.get_table("bookauthor", conditions={"isbn": ISBN})
-        book_genre = db.get_table("bookgenre", conditions={"isbn": ISBN})
+        book_author = db.get_table("bookauthor", conditions={"isbn": ISBN}, verbose=verbose)
+        book_genre = db.get_table("bookgenre", conditions={"isbn": ISBN}, verbose=verbose)
         
         # Add author(s) to the author table if doesn't exist
         if "authors" in new_book:
             if verbose:
                 logger.info("Authors to be updated.")
             
             authors = new_book["authors"]
-            new_author_ids = set(_get_or_add_authors(db, authors))
+            new_author_ids = set(_get_or_add_authors(db, authors, verbose=verbose))
             current_author_ids = set(book_author[book_author["isbn"] == ISBN]["author_id"].tolist())
             
             removed_authors = current_author_ids - new_author_ids
             added_authors = new_author_ids - current_author_ids
             
-            db.remove_records("bookauthor", [{"isbn": ISBN, "author_id": int(removed_author)} for removed_author in removed_authors])
-            db.insert_records("bookauthor", [{"isbn": ISBN, "author_id": int(added_author)} for added_author in added_authors])
+            db.remove_records("bookauthor", [{"isbn": ISBN, "author_id": int(removed_author)} for removed_author in removed_authors], verbose=verbose)
+            db.insert_records("bookauthor", [{"isbn": ISBN, "author_id": int(added_author)} for added_author in added_authors], verbose=verbose)
             
             if verbose:
                 logger.info("Author table updated.")
         else:
             if verbose:
                 logger.info("No authors to be updated.")
         
         # Add genres to the genres table if doesn't exist
         if "genres" in new_book:
             if verbose:
                 logger.info("Genres to be updated.")
             
             genres = new_book["genres"]    
-            new_genre_ids = set(_get_or_add_genres(db, genres))
+            new_genre_ids = set(_get_or_add_genres(db, genres, verbose=verbose))
             current_genre_ids = set(book_genre[book_genre["isbn"] == ISBN]["genre_id"].tolist())
         
             removed_genres = current_genre_ids - new_genre_ids
             added_genres = new_genre_ids - current_genre_ids
             
-            db.remove_records("bookgenre", [{"isbn": ISBN, "genre_id": int(removed_genre)} for removed_genre in removed_genres])
-            db.insert_records("bookgenre", [{"isbn": ISBN, "genre_id": int(added_genre)} for added_genre in added_genres])
+            db.remove_records("bookgenre", [{"isbn": ISBN, "genre_id": int(removed_genre)} for removed_genre in removed_genres], verbose=verbose)
+            db.insert_records("bookgenre", [{"isbn": ISBN, "genre_id": int(added_genre)} for added_genre in added_genres], verbose=verbose)
             
             if verbose:
                 logger.info("Genre table updated.")
         else:
             if verbose:
                 logger.info("No genres to be updated.")
             
@@ -314,17 +314,17 @@
     # Open connection to the database
     db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
     if verbose:
         logger.info("Database connection opened.")
     
     # Retrieve the table from the database
     if conditions:
-        table = db.get_table(table_name, conditions=conditions)
+        table = db.get_table(table_name, conditions=conditions, verbose=verbose)
     else:
-        table = db.get_table(table_name)
+        table = db.get_table(table_name, verbose=verbose)
         
     if verbose:
         logger.info(f"Table {table_name} retrieved.")
     
     # Return the table
     return table
 
@@ -340,15 +340,15 @@
         db (SqlHandler): The database handler.
         genres (list[str]): A list of genres.
         verbose (bool): Whether to print verbose output. Defaults to False.
 
     Returns:
         list[int]: A list of genre IDs.
     """
-    genre_table = db.get_table("genre")
+    genre_table = db.get_table("genre", verbose=verbose)
     
     genre_ids = []
     cur_index = max(genre_table["genre_id"] + 1)
     to_insert = []
     
     for genre in genres:
         if genre in genre_table["genre"].values:
@@ -356,15 +356,15 @@
         else:
             genre_id = cur_index
             cur_index += 1
             to_insert.append({"genre_id": genre_id, "genre": genre})
         genre_ids.append(genre_id)
     
     # Insert the records
-    db.insert_records("genre", to_insert)
+    db.insert_records("genre", to_insert, verbose=verbose)
     if verbose:
         logger.info("New genres added.")
     
     return genre_ids
 
 def _get_or_add_authors(db: SqlHandler, authors: list[str], verbose: bool = False) -> list[int]:
     """
@@ -381,15 +381,15 @@
         db (SqlHandler): The database handler.
         authors (list[str]): A list of authors.
         verbose (bool): Whether to print verbose output. Defaults to False.
 
     Returns:
         list[int]: A list of author IDs.
     """
-    author_table = db.get_table("author")
+    author_table = db.get_table("author", verbose=verbose)
     
     author_ids = []
     cur_index = max(author_table["author_id"]+1)
     to_insert = []
     
     for author in authors:
         if author in author_table["full_name"].values:
@@ -397,15 +397,15 @@
         else:
             author_id = cur_index
             cur_index += 1
             to_insert.append({"author_id": author_id, "full_name": author})
         author_ids.append(author_id)
     
     # Insert the records
-    db.insert_records("author", to_insert)
+    db.insert_records("author", to_insert, verbose=verbose)
     if verbose:
         logger.info("New authors added.")
     
     return author_ids
 
 def get_authors(ISBNs: list[str], verbose: bool = False) -> dict[str:list]:
     """
@@ -424,18 +424,18 @@
     """
     # Open connection to the database
     db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
     if verbose:
         logger.info("Database connection opened.")
     
     # Retrieve the authors of the books with the given ISBNs
-    authors = db.get_table("bookauthor", conditions={"isbn": ISBNs})
+    authors = db.get_table("bookauthor", conditions={"isbn": ISBNs}, verbose=verbose)
     author_ids = authors["author_id"].tolist()
     
-    author_table = db.get_table("author", conditions={"author_id": author_ids})
+    author_table = db.get_table("author", conditions={"author_id": author_ids}, verbose=verbose)
     
     # Initialize dictionary to store authors for each ISBN
     isbn_authors = {isbn: [] for isbn in ISBNs}
     
     # Populate dictionary with authors
     for _, row in authors.iterrows():
         isbn = row["isbn"]
@@ -463,18 +463,18 @@
     """
     # Open connection to the database
     db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
     if verbose:
         logger.info("Database connection opened.")
 
     # Retrieve the genres of the books with the given ISBNs
-    genres = db.get_table("bookgenre", conditions={"isbn": ISBNs})
+    genres = db.get_table("bookgenre", conditions={"isbn": ISBNs}, verbose=verbose)
     genre_ids = genres["genre_id"].tolist()
     
-    genre_table = db.get_table("genre", conditions={"genre_id": genre_ids})
+    genre_table = db.get_table("genre", conditions={"genre_id": genre_ids}, verbose=verbose)
     
     # Initialize dictionary to store genres for each ISBN
     isbn_genres = {isbn: [] for isbn in ISBNs}
     
     # Populate dictionary with genres
     for _, row in genres.iterrows():
         isbn = row["isbn"]
@@ -502,15 +502,15 @@
     """
     # Open connection to the database
     db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
     if verbose:
         logger.info("Database connection opened.")
     
     # Retrieve the history of books that have been recommended
-    history = db.get_table("history", conditions={"recommendation_ISBN": recommendation_isbn})
+    history = db.get_table("history", conditions={"recommendation_ISBN": recommendation_isbn}, verbose=verbose)
     
     # Return the history
     return history.drop(columns="log_id").to_dict(orient='records')
 
 
 def add_recommendation_log(description: str, recommendation_isbn: str, successful: bool, verbose: bool = False) -> bool:
     """
@@ -532,13 +532,13 @@
     try:
         # Open connection to the database
         db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
         if verbose:
             logger.info("Database connection opened.")
         
         # Insert the recommendation log into the history table
-        db.insert_records("history", [{"description": description, "recommendation_isbn": recommendation_isbn, "successful": successful}])
+        db.insert_records("history", [{"description": description, "recommendation_isbn": recommendation_isbn, "successful": successful}], verbose=verbose)
     
         return True
     except Exception as e:
         logger.error("Error adding recommendation log.")
         return False
```

### Comparing `kitab-0.0.26/kitab/db/get_data.py` & `kitab-0.0.27/kitab/db/get_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         verbose (bool): Whether to display logs. Default is False.
 
     Returns:
         None
     """
     try:
         # Getting the full data
-        data = get_full_data(folder_path)
+        data = get_full_data(folder_path, verbose=verbose)
         
         data.fillna({"genre": ""}, inplace=True)
         data = data[REQUIRED_COLUMNS + ["embedding", "available"]]
         
         data.dropna(subset = ["isbn", "description"], inplace=True)
 
         book_table = data[["isbn", "title", "description", "embedding", "available"]]
@@ -145,41 +145,41 @@
             sql_handler.cursor.execute(command)
             
         if verbose:
             logger.info("Tables created successfully.")
 
         # Inserting data
         # Book table
-        sql_handler.insert_many(book_table, "book")
+        sql_handler.insert_many(book_table, "book", verbose=verbose)
         
         if verbose:
             logger.info("Book data inserted successfully.")
 
         # Author table
-        sql_handler.insert_many(author_table, "author")
+        sql_handler.insert_many(author_table, "author", verbose=verbose)
         
         if verbose:
             logger.info("Author data inserted successfully.")
 
         # Genre table
-        sql_handler.insert_many(genre_table, "genre")
+        sql_handler.insert_many(genre_table, "genre", verbose=verbose)
         
         if verbose:
             logger.info("Genre data inserted successfully.")
 
         # BookAuthor table
-        sql_handler.insert_many(book_author, "bookauthor")
+        sql_handler.insert_many(book_author, "bookauthor", verbose=verbose)
         
         if verbose:
             logger.info("Book-Author mapping inserted successfully.")
 
         # BookGenre table
-        sql_handler.insert_many(book_genre, "bookgenre")
+        sql_handler.insert_many(book_genre, "bookgenre", verbose=verbose)
         
         if verbose:
             logger.info("Book-Genre mapping inserted successfully.")
         
         # Close the connection
-        sql_handler.close_cnxn()
+        sql_handler.close_cnxn(verbose=verbose)
 
     except psycopg2.Error as e:
         logger.error("Unable to connect to the PostgreSQL server.")
```

### Comparing `kitab-0.0.26/kitab/db/sql_interactions.py` & `kitab-0.0.27/kitab/db/sql_interactions.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.26/kitab/logger/logger.py` & `kitab-0.0.27/kitab/logger/logger.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.26/kitab/recommendation_model/models.py` & `kitab-0.0.27/kitab/recommendation_model/models.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.26/kitab/utils.py` & `kitab-0.0.27/kitab/utils.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.26/kitab.egg-info/PKG-INFO` & `kitab-0.0.27/kitab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kitab
-Version: 0.0.26
+Version: 0.0.27
 Summary: A package for book recommendation.
 Author: Alexander Shahramanyan, Anna Charchyan, Yeva Manukyan, Lilith Asminian, Maria Petrosyan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `kitab-0.0.26/kitab.egg-info/SOURCES.txt` & `kitab-0.0.27/kitab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kitab-0.0.26/setup.py` & `kitab-0.0.27/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Add install requirements
 setup(
     author="Alexander Shahramanyan, Anna Charchyan, Yeva Manukyan, Lilith Asminian, Maria Petrosyan",
     description="A package for book recommendation.",
     name="kitab",
     packages=find_packages(include=["kitab", "kitab.*"]),
-    version="0.0.26",
+    version="0.0.27",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=['pandas', 'sentence-transformers>=2.6', 'psycopg2-binary', 'pgvector', 'python-dotenv', 'tqdm'],
     python_requires=">=3.9",
```

