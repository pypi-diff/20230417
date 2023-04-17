# Comparing `tmp/tinote-0.3.1.tar.gz` & `tmp/tinote-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinote-0.3.1.tar", last modified: Sat Apr 15 14:52:21 2023, max compression
+gzip compressed data, was "tinote-0.3.2.tar", last modified: Mon Apr 17 20:34:48 2023, max compression
```

## Comparing `tinote-0.3.1.tar` & `tinote-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 14:52:21.297646 tinote-0.3.1/
--rw-rw-rw-   0        0        0     1830 2023-04-15 14:52:21.297646 tinote-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1165 2023-04-15 14:49:31.000000 tinote-0.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-15 14:52:21.297646 tinote-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1036 2023-04-15 14:52:09.000000 tinote-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 14:52:21.266299 tinote-0.3.1/tinote/
--rw-rw-rw-   0        0        0        0 2023-04-15 02:09:36.000000 tinote-0.3.1/tinote/__init__.py
--rw-rw-rw-   0        0        0     6022 2023-04-15 14:51:51.000000 tinote-0.3.1/tinote/main.py
-drwxrwxrwx   0        0        0        0 2023-04-15 14:52:21.282025 tinote-0.3.1/tinote.egg-info/
--rw-rw-rw-   0        0        0     1830 2023-04-15 14:52:21.000000 tinote-0.3.1/tinote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-04-15 14:52:21.000000 tinote-0.3.1/tinote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 14:52:21.000000 tinote-0.3.1/tinote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-15 14:52:21.000000 tinote-0.3.1/tinote.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-15 14:52:21.000000 tinote-0.3.1/tinote.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 20:34:48.933529 tinote-0.3.2/
+-rw-rw-rw-   0        0        0     1892 2023-04-17 20:34:48.932529 tinote-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1227 2023-04-17 20:34:20.000000 tinote-0.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 20:34:48.933529 tinote-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1036 2023-04-17 20:33:15.000000 tinote-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:34:48.916530 tinote-0.3.2/tinote/
+-rw-rw-rw-   0        0        0        0 2023-04-15 02:09:36.000000 tinote-0.3.2/tinote/__init__.py
+-rw-rw-rw-   0        0        0     6228 2023-04-17 20:32:18.000000 tinote-0.3.2/tinote/main.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:34:48.931529 tinote-0.3.2/tinote.egg-info/
+-rw-rw-rw-   0        0        0     1892 2023-04-17 20:34:48.000000 tinote-0.3.2/tinote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-04-17 20:34:48.000000 tinote-0.3.2/tinote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 20:34:48.000000 tinote-0.3.2/tinote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-17 20:34:48.000000 tinote-0.3.2/tinote.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 20:34:48.000000 tinote-0.3.2/tinote.egg-info/top_level.txt
```

### Comparing `tinote-0.3.1/PKG-INFO` & `tinote-0.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 0.3.1
+Version: 0.3.2
 Summary: A command-line note-taking tool
 Home-page: https://github.com/yourusername/tinote
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -29,21 +29,21 @@
 ```
 
 ## Usage
 
 Create a new note:
 
 ```bash
-ti "a note to remember" -c <optional category> -i <optional importance>
+ti add "a note to remember" -c <optional category> -i <optional importance>
 ```
 
-List all notes:
+List all notes (verbose list will include importance and timestamp):
 
 ```bash
-ti list
+ti list [-v]
 ```
 
 List notes with filters (category or importance):
 
 ```bash
 ti list -c <category> -i <importance>
 ```
```

### Comparing `tinote-0.3.1/README.md` & `tinote-0.3.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 ```
 
 ## Usage
 
 Create a new note:
 
 ```bash
-ti "a note to remember" -c <optional category> -i <optional importance>
+ti add "a note to remember" -c <optional category> -i <optional importance>
 ```
 
-List all notes:
+List all notes (verbose list will include importance and timestamp):
 
 ```bash
-ti list
+ti list [-v]
 ```
 
 List notes with filters (category or importance):
 
 ```bash
 ti list -c <category> -i <importance>
 ```
```

### Comparing `tinote-0.3.1/setup.py` & `tinote-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tinote",
-    version="0.3.1",
+    version="0.3.2",
     packages=find_packages(),
     install_requires=[
         # Add your package dependencies here
     ],
     entry_points={
         "console_scripts": [
             "ti = tinote.main:main"
```

### Comparing `tinote-0.3.1/tinote/main.py` & `tinote-0.3.2/tinote/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,39 +46,39 @@
 
 def format_note(note_text):
     lines = note_text.split("*")
     formatted_lines = [lines[0]] + [f"\t* {line.strip()}" for line in lines[1:]]
     return "\n".join(formatted_lines)
 
 
-def list_notes(category=None, importance=None):
+def list_notes(category=None, importance=None, verbose=None):
     notes, _ = load_notes()
     if not notes:
         print("No notes found.")
         return
 
     if category or importance is not None:
         filtered_notes = [note for note in notes if (not category or note["category"] == category) and (importance is None or note["importance"] == importance)]
         if not filtered_notes:
             print("No notes found matching the given filters.")
             return
 
         for note in filtered_notes:
             checkbox = "[x]" if note["checked"] else "[ ]"
             formatted_note = format_note(note["note"])
-            print(f"{note['id']}. {checkbox} {formatted_note} (Category: {note['category']}, Importance: {note['importance']}, Timestamp: {note['timestamp']})")
+            print(f"{note['id']}. {checkbox} {formatted_note}" + (f" (Category: {note['category']}, Importance: {note['importance']}, Timestamp: {note['timestamp']})" if verbose else ""))
     else:
         grouped_notes = {category: [note for note in notes if note["category"] == category] for category in set(note["category"] for note in notes)}
 
         for category, category_notes in grouped_notes.items():
             print(f"Category: {category or 'Uncategorized'}")
             for note in category_notes:
                 checkbox = "[x]" if note["checked"] else "[ ]"
                 formatted_note = format_note(note["note"])
-                print(f"  {note['id']}. {checkbox} {formatted_note} (Importance: {note['importance']}, Timestamp: {note['timestamp']})")
+                print(f"  {note['id']}. {checkbox} {formatted_note}" + (f" (Importance: {note['importance']}, Timestamp: {note['timestamp']})" if verbose else ""))
             print()
 
 
 def mark_note(note_id, checked=True):
     notes, max_id = load_notes()
 
     for note in notes:
@@ -128,14 +128,15 @@
     add_parser.add_argument("-c", "--category", type=str, default=None, help="Optional category for the note.")
     add_parser.add_argument("-i", "--importance", type=int, default=None, help="Optional importance level for the note (integer).")
 
     # Add subparser for 'list' command
     list_parser = subparsers.add_parser("list", help="List all notes.")
     list_parser.add_argument("-c", "--category", type=str, default=None, help="List notes from a specific category.")
     list_parser.add_argument("-i", "--importance", type=int, default=None, help="List notes with a specific importance level.")
+    list_parser.add_argument("-v", "--verbose", action="store_true", help="Show importance and timestamp with each note.")
 
     mark_parser = subparsers.add_parser("mark", help="Mark a note as checked or unchecked.")
     mark_parser.add_argument("id", type=int, help="The ID of the note to mark.")
     mark_parser.add_argument("-u", "--uncheck", action="store_true", help="Unmark the note instead of marking it.")
 
     delete_parser = subparsers.add_parser("delete", help="Delete a note.")
     delete_parser.add_argument("id", type=int, help="The ID of the note to delete.")
@@ -144,15 +145,15 @@
     clear_parser.add_argument('-c', '--category', type=str, help='Category of notes to clear (optional)')
 
     args = parser.parse_args()
 
     if args.subcommand == "add":
         create_note(args.note, args.category, args.importance)
     elif args.subcommand == "list":
-        list_notes(args.category, args.importance)
+        list_notes(args.category, args.importance, args.verbose)
     elif args.subcommand == "mark":
         mark_note(args.id, not args.uncheck)
     elif args.subcommand == "delete":
         delete_note(args.id)
     elif args.subcommand == 'clear':
         clear_notes(args.category)
     else:
```

### Comparing `tinote-0.3.1/tinote.egg-info/PKG-INFO` & `tinote-0.3.2/tinote.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 0.3.1
+Version: 0.3.2
 Summary: A command-line note-taking tool
 Home-page: https://github.com/yourusername/tinote
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -29,21 +29,21 @@
 ```
 
 ## Usage
 
 Create a new note:
 
 ```bash
-ti "a note to remember" -c <optional category> -i <optional importance>
+ti add "a note to remember" -c <optional category> -i <optional importance>
 ```
 
-List all notes:
+List all notes (verbose list will include importance and timestamp):
 
 ```bash
-ti list
+ti list [-v]
 ```
 
 List notes with filters (category or importance):
 
 ```bash
 ti list -c <category> -i <importance>
 ```
```

