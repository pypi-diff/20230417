# Comparing `tmp/tinote-0.3.2.tar.gz` & `tmp/tinote-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinote-0.3.2.tar", last modified: Mon Apr 17 20:34:48 2023, max compression
+gzip compressed data, was "tinote-1.0.0.tar", last modified: Mon Apr 17 21:12:13 2023, max compression
```

## Comparing `tinote-0.3.2.tar` & `tinote-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 20:34:48.933529 tinote-0.3.2/
--rw-rw-rw-   0        0        0     1892 2023-04-17 20:34:48.932529 tinote-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1227 2023-04-17 20:34:20.000000 tinote-0.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 20:34:48.933529 tinote-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1036 2023-04-17 20:33:15.000000 tinote-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 20:34:48.916530 tinote-0.3.2/tinote/
--rw-rw-rw-   0        0        0        0 2023-04-15 02:09:36.000000 tinote-0.3.2/tinote/__init__.py
--rw-rw-rw-   0        0        0     6228 2023-04-17 20:32:18.000000 tinote-0.3.2/tinote/main.py
-drwxrwxrwx   0        0        0        0 2023-04-17 20:34:48.931529 tinote-0.3.2/tinote.egg-info/
--rw-rw-rw-   0        0        0     1892 2023-04-17 20:34:48.000000 tinote-0.3.2/tinote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-04-17 20:34:48.000000 tinote-0.3.2/tinote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 20:34:48.000000 tinote-0.3.2/tinote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-17 20:34:48.000000 tinote-0.3.2/tinote.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 20:34:48.000000 tinote-0.3.2/tinote.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 21:12:13.465038 tinote-1.0.0/
+-rw-rw-rw-   0        0        0     2093 2023-04-17 21:12:13.465038 tinote-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1428 2023-04-17 21:11:26.000000 tinote-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 21:12:13.465038 tinote-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1036 2023-04-17 21:11:43.000000 tinote-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:12:13.452038 tinote-1.0.0/tinote/
+-rw-rw-rw-   0        0        0        0 2023-04-15 02:09:36.000000 tinote-1.0.0/tinote/__init__.py
+-rw-rw-rw-   0        0        0     9237 2023-04-17 21:10:07.000000 tinote-1.0.0/tinote/main.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:12:13.463038 tinote-1.0.0/tinote.egg-info/
+-rw-rw-rw-   0        0        0     2093 2023-04-17 21:12:13.000000 tinote-1.0.0/tinote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-04-17 21:12:13.000000 tinote-1.0.0/tinote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 21:12:13.000000 tinote-1.0.0/tinote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-17 21:12:13.000000 tinote-1.0.0/tinote.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 21:12:13.000000 tinote-1.0.0/tinote.egg-info/top_level.txt
```

### Comparing `tinote-0.3.2/PKG-INFO` & `tinote-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 0.3.2
+Version: 1.0.0
 Summary: A command-line note-taking tool
 Home-page: https://github.com/yourusername/tinote
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 
 ```bash
 pip install tinote
 ```
 
 ## Usage
 
-Create a new note:
+Create a new note (if no category is provided, the last category will be used):
 
 ```bash
 ti add "a note to remember" -c <optional category> -i <optional importance>
 ```
 
 List all notes (verbose list will include importance and timestamp):
 
@@ -44,14 +44,20 @@
 
 List notes with filters (category or importance):
 
 ```bash
 ti list -c <category> -i <importance>
 ```
 
+Add a sub-note to a note (currently only supports one level)
+
+```bash
+ti sub <parent_id> "Text of your sub-note" -i <importance>
+```
+
 Mark a note as checked/unchecked:
 
 ```bash
 ti mark <note_id>
 ```
 
 Delete a note:
```

### Comparing `tinote-0.3.2/README.md` & `tinote-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ```bash
 pip install tinote
 ```
 
 ## Usage
 
-Create a new note:
+Create a new note (if no category is provided, the last category will be used):
 
 ```bash
 ti add "a note to remember" -c <optional category> -i <optional importance>
 ```
 
 List all notes (verbose list will include importance and timestamp):
 
@@ -26,14 +26,20 @@
 
 List notes with filters (category or importance):
 
 ```bash
 ti list -c <category> -i <importance>
 ```
 
+Add a sub-note to a note (currently only supports one level)
+
+```bash
+ti sub <parent_id> "Text of your sub-note" -i <importance>
+```
+
 Mark a note as checked/unchecked:
 
 ```bash
 ti mark <note_id>
 ```
 
 Delete a note:
```

### Comparing `tinote-0.3.2/setup.py` & `tinote-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tinote",
-    version="0.3.2",
+    version="1.0.0",
     packages=find_packages(),
     install_requires=[
         # Add your package dependencies here
     ],
     entry_points={
         "console_scripts": [
             "ti = tinote.main:main"
```

### Comparing `tinote-0.3.2/tinote/main.py` & `tinote-1.0.0/tinote/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,136 +2,202 @@
 import argparse
 import os
 from datetime import datetime
 
 NOTES_FILE = os.path.expanduser("~/.ti_notes.json")
 
 
-def save_notes(notes, max_id):
+def save_notes(notes, max_id, last_category):
     with open(NOTES_FILE, "w") as f:
-        json.dump({"notes": notes, "max_id": max_id}, f, indent=2)
+        json.dump({"notes": notes, "max_id": max_id, "last_category": last_category}, f, indent=2)
 
 
 def load_notes():
     if not os.path.exists(NOTES_FILE):
-        return [], 0  # Return max_id as 0 for an empty file
+        return [], 0, "unknown"  # Return max_id as 0 for an empty file
 
     with open(NOTES_FILE, "r") as f:
         content = f.read().strip()
         if not content:
-            return [], 0  # Return max_id as 0 for an empty file
+            return [], 0, "unknown"  # Return max_id as 0 for an empty file
 
         data = json.loads(content)
-        notes, max_id = data.get("notes", []), data.get("max_id", 0)
-        return notes, max_id
+        notes, max_id, last_category = data.get("notes", []), data.get("max_id", 0), data.get("last_category", "unknown")
+        return notes, max_id, last_category
 
 
 def create_note(note, category, importance):
-    notes, max_id = load_notes()
+    notes, max_id, last_category = load_notes()
+    category = last_category if category is None else category
+
     new_id = max_id + 1
 
     new_note = {
         "id": new_id,  # Use the new ID
         "note": note,
         "category": category,
         "importance": importance,
         "timestamp": datetime.now().isoformat(),
+        "subs": [],
         "checked": False,
     }
 
     notes.append(new_note)
-    save_notes(notes, new_id)  # Update max_id
+    save_notes(notes, new_id, category)  # Update max_id
 
     print("Note added successfully.")
 
 
-def format_note(note_text):
+def create_sub_note(note, parent_id, importance):
+    notes, max_id, last_category = load_notes()
+
+    for n in notes:
+        if n["id"] == parent_id:
+            parent_note = n
+            break
+    else:
+        print("Parent does not exist.")
+        return
+
+    new_id = max_id + 1
+
+    new_note = {
+        "id": new_id,  # Use the new ID
+        "parent": parent_id,
+        "note": note,
+        "category": parent_note["category"],
+        "importance": importance,
+        "timestamp": datetime.now().isoformat(),
+        "checked": False,
+    }
+
+    try:
+        parent_note["subs"].append(new_note)
+    except KeyError:
+        parent_note["subs"] = [new_note]
+
+    save_notes(notes, new_id, last_category)
+
+    print("Sub-note added successfully.")
+
+
+def format_note(note_text, sub=False):
+    bullet_indent = "\t\t" if sub else "\t"
     lines = note_text.split("*")
-    formatted_lines = [lines[0]] + [f"\t* {line.strip()}" for line in lines[1:]]
+    formatted_lines = [lines[0]] + [f"{bullet_indent}* {line.strip()}" for line in lines[1:]]
     return "\n".join(formatted_lines)
 
 
 def list_notes(category=None, importance=None, verbose=None):
-    notes, _ = load_notes()
+    notes, _, _ = load_notes()
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
             print(f"{note['id']}. {checkbox} {formatted_note}" + (f" (Category: {note['category']}, Importance: {note['importance']}, Timestamp: {note['timestamp']})" if verbose else ""))
+
+            for sub in note["subs"]:
+                checkbox = "[x]" if sub["checked"] else "[ ]"
+                formatted_note = format_note(sub["note"], True)
+                print(f"\t{sub['id']}. {checkbox} {formatted_note}" + (f" (Category: {sub['category']}, Importance: {sub['importance']}, Timestamp: {sub['timestamp']})" if verbose else ""))
     else:
         grouped_notes = {category: [note for note in notes if note["category"] == category] for category in set(note["category"] for note in notes)}
 
         for category, category_notes in grouped_notes.items():
             print(f"Category: {category or 'Uncategorized'}")
             for note in category_notes:
                 checkbox = "[x]" if note["checked"] else "[ ]"
                 formatted_note = format_note(note["note"])
                 print(f"  {note['id']}. {checkbox} {formatted_note}" + (f" (Importance: {note['importance']}, Timestamp: {note['timestamp']})" if verbose else ""))
+
+                for sub in note["subs"]:
+                    checkbox = "[x]" if sub["checked"] else "[ ]"
+                    formatted_note = format_note(sub["note"], True)
+                    print(f"\t{sub['id']}. {checkbox} {formatted_note}" + (f" (Importance: {sub['importance']}, Timestamp: {sub['timestamp']})" if verbose else ""))
             print()
 
 
 def mark_note(note_id, checked=True):
-    notes, max_id = load_notes()
+    notes, max_id, last_category = load_notes()
 
     for note in notes:
         if note["id"] == note_id:
             note["checked"] = checked
-            save_notes(notes, max_id)
+            save_notes(notes, max_id, last_category)
             print(f"Note {'marked' if checked else 'unmarked'} successfully.")
-            break
+            return
+
+        for index, sub in enumerate(note["subs"]):
+            if sub["id"] == note_id:
+                sub["checked"] = checked
+                save_notes(notes, max_id, last_category)
+                print(f"Note {'marked' if checked else 'unmarked'} successfully.")
+                return
     else:
         print("Invalid note ID.")
 
 
 def delete_note(note_id):
-    notes, max_id = load_notes()
+    notes, max_id, last_category = load_notes()
 
     for index, note in enumerate(notes):
         if note["id"] == note_id:
             del notes[index]
-            save_notes(notes, max_id)
+            save_notes(notes, max_id, last_category)
             print("Note deleted successfully.")
-            break
+            return
+
+        for sub_index, sub in enumerate(note["subs"]):
+            if sub["id"] == note_id:
+                del note["subs"][sub_index]
+                save_notes(notes, max_id, last_category)
+                print("Note deleted successfully.")
+                return
     else:
         print("Invalid note ID.")
 
 
 def clear_notes(category=None):
-    notes, max_id = load_notes()
+    notes, max_id, last_category = load_notes()
     if category:
         notes = [note for note in notes if note['category'] != category]
     else:
         notes = []
 
-    save_notes(notes, max_id)
+    save_notes(notes, max_id, last_category)
     if category:
         print(f"Successfully cleared all notes in category '{category}'.")
     else:
         print("Successfully cleared all notes.")
 
 
 def main():
     parser = argparse.ArgumentParser(description="A command-line tool for taking quick notes.", prog="ti")
     subparsers = parser.add_subparsers(dest="subcommand")
 
     # Add subparser for 'add' command
     add_parser = subparsers.add_parser("add", help="Add a new note.")
     add_parser.add_argument("note", type=str, help="The content of the note.")
-    add_parser.add_argument("-c", "--category", type=str, default=None, help="Optional category for the note.")
+    add_parser.add_argument("-c", "--category", type=str, default=None, help="Optional category for the note. If none is provided, the last category will be used.")
     add_parser.add_argument("-i", "--importance", type=int, default=None, help="Optional importance level for the note (integer).")
 
+    sub_parser = subparsers.add_parser('sub', help='Add a sub-note to a note')
+    sub_parser.add_argument('parent_id', type=int, help='Parent note ID')
+    sub_parser.add_argument('note', type=str, help='Sub-note text')
+    sub_parser.add_argument("-i", "--importance", type=int, default=None, help="Optional importance level for the note (integer).")
+
     # Add subparser for 'list' command
     list_parser = subparsers.add_parser("list", help="List all notes.")
     list_parser.add_argument("-c", "--category", type=str, default=None, help="List notes from a specific category.")
     list_parser.add_argument("-i", "--importance", type=int, default=None, help="List notes with a specific importance level.")
     list_parser.add_argument("-v", "--verbose", action="store_true", help="Show importance and timestamp with each note.")
 
     mark_parser = subparsers.add_parser("mark", help="Mark a note as checked or unchecked.")
@@ -152,13 +218,15 @@
         list_notes(args.category, args.importance, args.verbose)
     elif args.subcommand == "mark":
         mark_note(args.id, not args.uncheck)
     elif args.subcommand == "delete":
         delete_note(args.id)
     elif args.subcommand == 'clear':
         clear_notes(args.category)
+    elif args.subcommand == 'sub':
+        create_sub_note(args.note, args.parent_id, args.importance)
     else:
         parser.print_help()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `tinote-0.3.2/tinote.egg-info/PKG-INFO` & `tinote-1.0.0/tinote.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 0.3.2
+Version: 1.0.0
 Summary: A command-line note-taking tool
 Home-page: https://github.com/yourusername/tinote
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 
 ```bash
 pip install tinote
 ```
 
 ## Usage
 
-Create a new note:
+Create a new note (if no category is provided, the last category will be used):
 
 ```bash
 ti add "a note to remember" -c <optional category> -i <optional importance>
 ```
 
 List all notes (verbose list will include importance and timestamp):
 
@@ -44,14 +44,20 @@
 
 List notes with filters (category or importance):
 
 ```bash
 ti list -c <category> -i <importance>
 ```
 
+Add a sub-note to a note (currently only supports one level)
+
+```bash
+ti sub <parent_id> "Text of your sub-note" -i <importance>
+```
+
 Mark a note as checked/unchecked:
 
 ```bash
 ti mark <note_id>
 ```
 
 Delete a note:
```

