# Comparing `tmp/tinote-1.0.0.tar.gz` & `tmp/tinote-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinote-1.0.0.tar", last modified: Mon Apr 17 21:12:13 2023, max compression
+gzip compressed data, was "tinote-1.0.1.tar", last modified: Mon Apr 17 21:21:14 2023, max compression
```

## Comparing `tinote-1.0.0.tar` & `tinote-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 21:12:13.465038 tinote-1.0.0/
--rw-rw-rw-   0        0        0     2093 2023-04-17 21:12:13.465038 tinote-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1428 2023-04-17 21:11:26.000000 tinote-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 21:12:13.465038 tinote-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1036 2023-04-17 21:11:43.000000 tinote-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:12:13.452038 tinote-1.0.0/tinote/
--rw-rw-rw-   0        0        0        0 2023-04-15 02:09:36.000000 tinote-1.0.0/tinote/__init__.py
--rw-rw-rw-   0        0        0     9237 2023-04-17 21:10:07.000000 tinote-1.0.0/tinote/main.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:12:13.463038 tinote-1.0.0/tinote.egg-info/
--rw-rw-rw-   0        0        0     2093 2023-04-17 21:12:13.000000 tinote-1.0.0/tinote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-04-17 21:12:13.000000 tinote-1.0.0/tinote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 21:12:13.000000 tinote-1.0.0/tinote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-17 21:12:13.000000 tinote-1.0.0/tinote.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 21:12:13.000000 tinote-1.0.0/tinote.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 21:21:14.133456 tinote-1.0.1/
+-rw-rw-rw-   0        0        0     2191 2023-04-17 21:21:14.132462 tinote-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1422 2023-04-17 21:21:01.000000 tinote-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 21:21:14.133456 tinote-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2023-04-17 21:21:01.000000 tinote-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:21:14.113456 tinote-1.0.1/tinote/
+-rw-rw-rw-   0        0        0        0 2023-04-15 02:09:36.000000 tinote-1.0.1/tinote/__init__.py
+-rw-rw-rw-   0        0        0     9933 2023-04-17 21:19:37.000000 tinote-1.0.1/tinote/main.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:21:14.130456 tinote-1.0.1/tinote.egg-info/
+-rw-rw-rw-   0        0        0     2191 2023-04-17 21:21:14.000000 tinote-1.0.1/tinote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-04-17 21:21:14.000000 tinote-1.0.1/tinote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 21:21:14.000000 tinote-1.0.1/tinote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-17 21:21:14.000000 tinote-1.0.1/tinote.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 21:21:14.000000 tinote-1.0.1/tinote.egg-info/top_level.txt
```

### Comparing `tinote-1.0.0/PKG-INFO` & `tinote-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 1.0.0
+Version: 1.0.1
 Summary: A command-line note-taking tool
 Home-page: https://github.com/yourusername/tinote
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Tinote
 
 Tinote is a lightweight command-line note-taking tool, designed for quick and easy note management. Keep track of your thoughts, ideas, or reminders directly from the terminal.
 
@@ -29,15 +31,15 @@
 ```
 
 ## Usage
 
 Create a new note (if no category is provided, the last category will be used):
 
 ```bash
-ti add "a note to remember" -c <optional category> -i <optional importance>
+ti add "a note to remember" <optional category> <optional importance>
 ```
 
 List all notes (verbose list will include importance and timestamp):
 
 ```bash
 ti list [-v]
 ```
```

### Comparing `tinote-1.0.0/README.md` & `tinote-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ```
 
 ## Usage
 
 Create a new note (if no category is provided, the last category will be used):
 
 ```bash
-ti add "a note to remember" -c <optional category> -i <optional importance>
+ti add "a note to remember" <optional category> <optional importance>
 ```
 
 List all notes (verbose list will include importance and timestamp):
 
 ```bash
 ti list [-v]
 ```
```

### Comparing `tinote-1.0.0/setup.py` & `tinote-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tinote",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
     install_requires=[
         # Add your package dependencies here
     ],
     entry_points={
         "console_scripts": [
             "ti = tinote.main:main"
@@ -23,10 +23,12 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     python_requires=">=3.6",
 )
```

### Comparing `tinote-1.0.0/tinote/main.py` & `tinote-1.0.1/tinote/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -182,16 +182,23 @@
 def main():
     parser = argparse.ArgumentParser(description="A command-line tool for taking quick notes.", prog="ti")
     subparsers = parser.add_subparsers(dest="subcommand")
 
     # Add subparser for 'add' command
     add_parser = subparsers.add_parser("add", help="Add a new note.")
     add_parser.add_argument("note", type=str, help="The content of the note.")
-    add_parser.add_argument("-c", "--category", type=str, default=None, help="Optional category for the note. If none is provided, the last category will be used.")
-    add_parser.add_argument("-i", "--importance", type=int, default=None, help="Optional importance level for the note (integer).")
+    add_parser.add_argument("category", type=str, nargs="?", default=None,
+                            help="Optional category for the note. If none is provided, the last category will be used.")
+    add_parser.add_argument("importance", type=int, nargs="?", default=None,
+                            help="Optional importance level for the note (integer).")
+    add_parser.add_argument("-c", "--category", type=str, default=None,
+                            help="Optional category for the note. If none is provided, the last category will be used.",
+                            dest="category_keyword")
+    add_parser.add_argument("-i", "--importance", type=int, default=None,
+                            help="Optional importance level for the note (integer).", dest="importance_keyword")
 
     sub_parser = subparsers.add_parser('sub', help='Add a sub-note to a note')
     sub_parser.add_argument('parent_id', type=int, help='Parent note ID')
     sub_parser.add_argument('note', type=str, help='Sub-note text')
     sub_parser.add_argument("-i", "--importance", type=int, default=None, help="Optional importance level for the note (integer).")
 
     # Add subparser for 'list' command
@@ -209,15 +216,17 @@
 
     clear_parser = subparsers.add_parser('clear', help='Clear all notes or notes in the specified category')
     clear_parser.add_argument('-c', '--category', type=str, help='Category of notes to clear (optional)')
 
     args = parser.parse_args()
 
     if args.subcommand == "add":
-        create_note(args.note, args.category, args.importance)
+        category = args.category_keyword if args.category_keyword is not None else args.category
+        importance = args.importance_keyword if args.importance_keyword is not None else args.importance
+        create_note(args.note, category, importance)
     elif args.subcommand == "list":
         list_notes(args.category, args.importance, args.verbose)
     elif args.subcommand == "mark":
         mark_note(args.id, not args.uncheck)
     elif args.subcommand == "delete":
         delete_note(args.id)
     elif args.subcommand == 'clear':
```

### Comparing `tinote-1.0.0/tinote.egg-info/PKG-INFO` & `tinote-1.0.1/tinote.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 1.0.0
+Version: 1.0.1
 Summary: A command-line note-taking tool
 Home-page: https://github.com/yourusername/tinote
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Tinote
 
 Tinote is a lightweight command-line note-taking tool, designed for quick and easy note management. Keep track of your thoughts, ideas, or reminders directly from the terminal.
 
@@ -29,15 +31,15 @@
 ```
 
 ## Usage
 
 Create a new note (if no category is provided, the last category will be used):
 
 ```bash
-ti add "a note to remember" -c <optional category> -i <optional importance>
+ti add "a note to remember" <optional category> <optional importance>
 ```
 
 List all notes (verbose list will include importance and timestamp):
 
 ```bash
 ti list [-v]
 ```
```

