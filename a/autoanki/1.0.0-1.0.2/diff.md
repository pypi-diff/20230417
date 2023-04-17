# Comparing `tmp/autoanki-1.0.0.tar.gz` & `tmp/autoanki-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoanki-1.0.0.tar", last modified: Mon Apr 17 18:38:49 2023, max compression
+gzip compressed data, was "autoanki-1.0.2.tar", last modified: Mon Apr 17 18:53:29 2023, max compression
```

## Comparing `autoanki-1.0.0.tar` & `autoanki-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:38:49.538785 autoanki-1.0.0/
--rw-r--r--   0 owner      (501) staff       (20)        0 2023-04-17 16:36:34.000000 autoanki-1.0.0/LICENSE.txt
--rw-r--r--   0 owner      (501) staff       (20)        0 2023-04-17 16:36:34.000000 autoanki-1.0.0/MANIFEST.in
--rw-r--r--   0 owner      (501) staff       (20)     4342 2023-04-17 18:38:49.538848 autoanki-1.0.0/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)     3807 2023-04-17 18:17:51.000000 autoanki-1.0.0/README.md
--rw-r--r--   0 owner      (501) staff       (20)      103 2023-04-17 17:58:47.000000 autoanki-1.0.0/pyproject.toml
--rw-r--r--   0 owner      (501) staff       (20)      656 2023-04-17 18:38:49.539113 autoanki-1.0.0/setup.cfg
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:38:49.533922 autoanki-1.0.0/src/
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:38:49.535318 autoanki-1.0.0/src/autoanki/
--rw-r--r--   0 owner      (501) staff       (20)     5273 2023-04-17 18:14:09.000000 autoanki-1.0.0/src/autoanki/AutoAnki.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:38:49.536635 autoanki-1.0.0/src/autoanki/BookCleaner/
--rw-r--r--   0 owner      (501) staff       (20)     7268 2023-04-17 17:53:21.000000 autoanki-1.0.0/src/autoanki/BookCleaner/BookCleaner.py
--rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.0.0/src/autoanki/BookCleaner/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:38:49.537164 autoanki-1.0.0/src/autoanki/DatabaseManager/
--rw-r--r--   0 owner      (501) staff       (20)    13082 2023-04-17 17:53:21.000000 autoanki-1.0.0/src/autoanki/DatabaseManager/DatabaseManager.py
--rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.0.0/src/autoanki/DatabaseManager/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:38:49.537427 autoanki-1.0.0/src/autoanki/DeckManager/
--rw-r--r--   0 owner      (501) staff       (20)     6414 2023-04-17 18:17:51.000000 autoanki-1.0.0/src/autoanki/DeckManager/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:38:49.538522 autoanki-1.0.0/src/autoanki/Dictionary/
--rw-r--r--   0 owner      (501) staff       (20)      122 2023-04-17 18:22:48.000000 autoanki-1.0.0/src/autoanki/Dictionary/CC-CEDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)      232 2023-04-17 16:36:34.000000 autoanki-1.0.0/src/autoanki/Dictionary/Dictionary.py
--rw-r--r--   0 owner      (501) staff       (20)     5580 2023-04-17 17:53:21.000000 autoanki-1.0.0/src/autoanki/Dictionary/YellowBridgeDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)       58 2023-04-17 18:23:02.000000 autoanki-1.0.0/src/autoanki/Dictionary/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.0.0/src/autoanki/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:38:49.536246 autoanki-1.0.0/src/autoanki.egg-info/
--rw-r--r--   0 owner      (501) staff       (20)     4342 2023-04-17 18:38:49.000000 autoanki-1.0.0/src/autoanki.egg-info/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)      622 2023-04-17 18:38:49.000000 autoanki-1.0.0/src/autoanki.egg-info/SOURCES.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2023-04-17 18:38:49.000000 autoanki-1.0.0/src/autoanki.egg-info/dependency_links.txt
--rw-r--r--   0 owner      (501) staff       (20)        9 2023-04-17 18:38:49.000000 autoanki-1.0.0/src/autoanki.egg-info/top_level.txt
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:53:29.494090 autoanki-1.0.2/
+-rw-r--r--   0 owner      (501) staff       (20)        0 2023-04-17 16:36:34.000000 autoanki-1.0.2/LICENSE.txt
+-rw-r--r--   0 owner      (501) staff       (20)        0 2023-04-17 16:36:34.000000 autoanki-1.0.2/MANIFEST.in
+-rw-r--r--   0 owner      (501) staff       (20)     4339 2023-04-17 18:53:29.494196 autoanki-1.0.2/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)     3806 2023-04-17 18:46:28.000000 autoanki-1.0.2/README.md
+-rw-r--r--   0 owner      (501) staff       (20)      103 2023-04-17 17:58:47.000000 autoanki-1.0.2/pyproject.toml
+-rw-r--r--   0 owner      (501) staff       (20)      654 2023-04-17 18:53:29.494550 autoanki-1.0.2/setup.cfg
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:53:29.489435 autoanki-1.0.2/src/
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:53:29.490864 autoanki-1.0.2/src/autoanki/
+-rw-r--r--   0 owner      (501) staff       (20)     5273 2023-04-17 18:14:09.000000 autoanki-1.0.2/src/autoanki/AutoAnki.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:53:29.492040 autoanki-1.0.2/src/autoanki/BookCleaner/
+-rw-r--r--   0 owner      (501) staff       (20)     7268 2023-04-17 17:53:21.000000 autoanki-1.0.2/src/autoanki/BookCleaner/BookCleaner.py
+-rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.0.2/src/autoanki/BookCleaner/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:53:29.492574 autoanki-1.0.2/src/autoanki/DatabaseManager/
+-rw-r--r--   0 owner      (501) staff       (20)    13082 2023-04-17 17:53:21.000000 autoanki-1.0.2/src/autoanki/DatabaseManager/DatabaseManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.0.2/src/autoanki/DatabaseManager/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:53:29.492812 autoanki-1.0.2/src/autoanki/DeckManager/
+-rw-r--r--   0 owner      (501) staff       (20)     6413 2023-04-17 18:46:28.000000 autoanki-1.0.2/src/autoanki/DeckManager/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:53:29.493807 autoanki-1.0.2/src/autoanki/Dictionary/
+-rw-r--r--   0 owner      (501) staff       (20)      122 2023-04-17 18:22:48.000000 autoanki-1.0.2/src/autoanki/Dictionary/CC-CEDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)      232 2023-04-17 16:36:34.000000 autoanki-1.0.2/src/autoanki/Dictionary/Dictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)     5580 2023-04-17 17:53:21.000000 autoanki-1.0.2/src/autoanki/Dictionary/YellowBridgeDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)       58 2023-04-17 18:23:02.000000 autoanki-1.0.2/src/autoanki/Dictionary/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.0.2/src/autoanki/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-04-17 18:53:29.491596 autoanki-1.0.2/src/autoanki.egg-info/
+-rw-r--r--   0 owner      (501) staff       (20)     4339 2023-04-17 18:53:29.000000 autoanki-1.0.2/src/autoanki.egg-info/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)      622 2023-04-17 18:53:29.000000 autoanki-1.0.2/src/autoanki.egg-info/SOURCES.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2023-04-17 18:53:29.000000 autoanki-1.0.2/src/autoanki.egg-info/dependency_links.txt
+-rw-r--r--   0 owner      (501) staff       (20)        9 2023-04-17 18:53:29.000000 autoanki-1.0.2/src/autoanki.egg-info/top_level.txt
```

### Comparing `autoanki-1.0.0/PKG-INFO` & `autoanki-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.0.0
+Version: 1.0.2
 Summary: Automatically make Anki Decks for Chinese text
-Home-page: https://github.com/timmy6figures/auto-anki
+Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
-Project-URL: Bug Tracker, https://github.com/timmy6figures/auto-anki/issues
+Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -26,15 +26,15 @@
 AutoAnki was created to help Chinese learners get into more advanced texts. 
 It can be hard transitioning from graded readers to full books, and this tool was designed to help ease that process.
 
 ## Usage
 
 AutoAnki is both a library and a terminal tool. 
 To get started, run 
-```pip install auto-anki```
+```pip install autoanki```
 This should install all the requirements. Then, in a Python file do```from AutoAnki import AutoAnki, cli```
 
 To get started, first, create a database for AutoAnki to use 
 ```    
 db_path = "AutoAnki.db"
 if not AutoAnki.is_database(db_path):
     AutoAnki.create_autoanki_db(db_path)
```

### Comparing `autoanki-1.0.0/README.md` & `autoanki-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 AutoAnki was created to help Chinese learners get into more advanced texts. 
 It can be hard transitioning from graded readers to full books, and this tool was designed to help ease that process.
 
 ## Usage
 
 AutoAnki is both a library and a terminal tool. 
 To get started, run 
-```pip install auto-anki```
+```pip install autoanki```
 This should install all the requirements. Then, in a Python file do```from AutoAnki import AutoAnki, cli```
 
 To get started, first, create a database for AutoAnki to use 
 ```    
 db_path = "AutoAnki.db"
 if not AutoAnki.is_database(db_path):
     AutoAnki.create_autoanki_db(db_path)
```

### Comparing `autoanki-1.0.0/setup.cfg` & `autoanki-1.0.2/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = autoanki
-version = 1.0.0
+version = 1.0.2
 author = Jarvis Coghlin
 author_email = jarviscoghlin@gmail.com
 description = Automatically make Anki Decks for Chinese text
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/timmy6figures/auto-anki
+url = https://github.com/timmy6figures/autoanki
 project_urls = 
-	Bug Tracker = https://github.com/timmy6figures/auto-anki/issues
+	Bug Tracker = https://github.com/timmy6figures/autoanki/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir =
```

### Comparing `autoanki-1.0.0/src/autoanki/AutoAnki.py` & `autoanki-1.0.2/src/autoanki/AutoAnki.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.0.0/src/autoanki/BookCleaner/BookCleaner.py` & `autoanki-1.0.2/src/autoanki/BookCleaner/BookCleaner.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.0.0/src/autoanki/DatabaseManager/DatabaseManager.py` & `autoanki-1.0.2/src/autoanki/DatabaseManager/DatabaseManager.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.0.0/src/autoanki/DeckManager/__init__.py` & `autoanki-1.0.2/src/autoanki/DeckManager/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     This class makes extensive use of genanki, so understanding how genanki works
         is pretty significant for understanding this.
     """
 
     def __init__(self):
         self.deck = genanki.Deck(
             2020000110,
-            "auto-ankiTesting"
+            "autoankiTesting"
         )
         self.include_pinyin_numbers = False
         self.include_number_of_strokes = False
 
         self.book_list = []
 
     def generate_deck_file(self, words, deck_name: str, filename: str):
```

### Comparing `autoanki-1.0.0/src/autoanki/Dictionary/YellowBridgeDictionary.py` & `autoanki-1.0.2/src/autoanki/Dictionary/YellowBridgeDictionary.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.0.0/src/autoanki.egg-info/PKG-INFO` & `autoanki-1.0.2/src/autoanki.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.0.0
+Version: 1.0.2
 Summary: Automatically make Anki Decks for Chinese text
-Home-page: https://github.com/timmy6figures/auto-anki
+Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
-Project-URL: Bug Tracker, https://github.com/timmy6figures/auto-anki/issues
+Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -26,15 +26,15 @@
 AutoAnki was created to help Chinese learners get into more advanced texts. 
 It can be hard transitioning from graded readers to full books, and this tool was designed to help ease that process.
 
 ## Usage
 
 AutoAnki is both a library and a terminal tool. 
 To get started, run 
-```pip install auto-anki```
+```pip install autoanki```
 This should install all the requirements. Then, in a Python file do```from AutoAnki import AutoAnki, cli```
 
 To get started, first, create a database for AutoAnki to use 
 ```    
 db_path = "AutoAnki.db"
 if not AutoAnki.is_database(db_path):
     AutoAnki.create_autoanki_db(db_path)
```

### Comparing `autoanki-1.0.0/src/autoanki.egg-info/SOURCES.txt` & `autoanki-1.0.2/src/autoanki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

