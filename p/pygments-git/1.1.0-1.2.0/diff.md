# Comparing `tmp/pygments_git-1.1.0.tar.gz` & `tmp/pygments_git-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygments_git-1.1.0.tar", last modified: Thu Apr  6 08:53:41 2023, max compression
+gzip compressed data, was "pygments_git-1.2.0.tar", last modified: Sun Apr 16 22:00:51 2023, max compression
```

## Comparing `pygments_git-1.1.0.tar` & `pygments_git-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-06 08:53:41.296082 pygments_git-1.1.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      293 2023-04-06 08:53:38.000000 pygments_git-1.1.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-04-01 11:07:54.000000 pygments_git-1.1.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-04-01 11:04:32.000000 pygments_git-1.1.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4324 2023-04-06 08:53:41.296136 pygments_git-1.1.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3174 2023-04-06 08:51:20.000000 pygments_git-1.1.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-04-01 13:54:14.000000 pygments_git-1.1.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1662 2023-04-06 08:53:41.296412 pygments_git-1.1.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-06 08:53:41.293787 pygments_git-1.1.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-06 08:53:41.295024 pygments_git-1.1.0/src/pygments_git/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     9522 2023-04-05 10:16:13.000000 pygments_git-1.1.0/src/pygments_git/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-01 11:04:33.000000 pygments_git-1.1.0/src/pygments_git/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-06 08:53:41.295847 pygments_git-1.1.0/src/pygments_git.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4324 2023-04-06 08:53:41.000000 pygments_git-1.1.0/src/pygments_git.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      432 2023-04-06 08:53:41.000000 pygments_git-1.1.0/src/pygments_git.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-04-06 08:53:41.000000 pygments_git-1.1.0/src/pygments_git.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)      172 2023-04-06 08:53:41.000000 pygments_git-1.1.0/src/pygments_git.egg-info/entry_points.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-04-06 08:53:41.000000 pygments_git-1.1.0/src/pygments_git.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)        9 2023-04-06 08:53:41.000000 pygments_git-1.1.0/src/pygments_git.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       13 2023-04-06 08:53:41.000000 pygments_git-1.1.0/src/pygments_git.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-06 08:53:41.295965 pygments_git-1.1.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7519 2023-04-05 10:19:23.000000 pygments_git-1.1.0/tests/test_pygments_git.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-16 22:00:51.967149 pygments_git-1.2.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      395 2023-04-16 22:00:48.000000 pygments_git-1.2.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-04-01 11:07:54.000000 pygments_git-1.2.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-04-01 11:04:32.000000 pygments_git-1.2.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4594 2023-04-16 22:00:51.967254 pygments_git-1.2.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3444 2023-04-10 17:30:19.000000 pygments_git-1.2.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-04-01 13:54:14.000000 pygments_git-1.2.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1769 2023-04-16 22:00:51.967645 pygments_git-1.2.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-16 22:00:51.965136 pygments_git-1.2.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-16 22:00:51.966086 pygments_git-1.2.0/src/pygments_git/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    12548 2023-04-12 10:52:33.000000 pygments_git-1.2.0/src/pygments_git/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-01 11:04:33.000000 pygments_git-1.2.0/src/pygments_git/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-16 22:00:51.966853 pygments_git-1.2.0/src/pygments_git.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4594 2023-04-16 22:00:51.000000 pygments_git-1.2.0/src/pygments_git.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      432 2023-04-16 22:00:51.000000 pygments_git-1.2.0/src/pygments_git.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-04-16 22:00:51.000000 pygments_git-1.2.0/src/pygments_git.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      281 2023-04-16 22:00:51.000000 pygments_git-1.2.0/src/pygments_git.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-04-16 22:00:51.000000 pygments_git-1.2.0/src/pygments_git.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        9 2023-04-16 22:00:51.000000 pygments_git-1.2.0/src/pygments_git.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       13 2023-04-16 22:00:51.000000 pygments_git-1.2.0/src/pygments_git.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-16 22:00:51.966964 pygments_git-1.2.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8663 2023-04-12 10:52:33.000000 pygments_git-1.2.0/tests/test_pygments_git.py
```

### Comparing `pygments_git-1.1.0/LICENSE` & `pygments_git-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygments_git-1.1.0/PKG-INFO` & `pygments_git-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygments_git
-Version: 1.1.0
+Version: 1.2.0
 Summary: Pygments lexers for Git output and files.
 Home-page: https://github.com/adamchainz/pygments-git
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pygments-git/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -80,26 +80,34 @@
     .. code-block:: git-console
 
         $ git log --oneline
         82fbbd3 D'oh! Fix math proof
         91e9879 Aye carumba! Grammar mistake
         61c4c08 Cowabunga! Update bibliography
 
+To preview the lexers, open the ``tests/index.html`` file within the repository.
+
 ``git-commit-edit-msg``
 -----------------------
 
 A lexer for the ``COMMIT_EDITMSG`` file that Git opens when you run ``git commit``.
 It calls out to |DiffLexer|__ for highlighting any diff, as added by |git commit --verbose|__.
 
 .. |DiffLexer| replace:: ``DiffLexer``
 __ https://pygments.org/docs/lexers/#pygments.lexers.diff.DiffLexer
 
 .. |git commit --verbose| replace:: ``git commit --verbose``
 __ https://git-scm.com/docs/git-commit#Documentation/git-commit.txt--v
 
+``git-conflict-markers``
+------------------------
+
+A lexer for the conflict markers that Git adds to indicate conflicts during a merge.
+All other text in the file is lexed as plain text.
+
 ``git-console``
 ---------------
 
 A lexer for interactive shell sessions with Git.
 It calls out to |BashLexer|__ for highlighting commands on lines starting with a ``$`` and |DiffLexer2|__ for highlighting inline diffs.
 
 .. |BashLexer| replace:: ``BashLexer``
```

### Comparing `pygments_git-1.1.0/README.rst` & `pygments_git-1.2.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -51,26 +51,34 @@
     .. code-block:: git-console
 
         $ git log --oneline
         82fbbd3 D'oh! Fix math proof
         91e9879 Aye carumba! Grammar mistake
         61c4c08 Cowabunga! Update bibliography
 
+To preview the lexers, open the ``tests/index.html`` file within the repository.
+
 ``git-commit-edit-msg``
 -----------------------
 
 A lexer for the ``COMMIT_EDITMSG`` file that Git opens when you run ``git commit``.
 It calls out to |DiffLexer|__ for highlighting any diff, as added by |git commit --verbose|__.
 
 .. |DiffLexer| replace:: ``DiffLexer``
 __ https://pygments.org/docs/lexers/#pygments.lexers.diff.DiffLexer
 
 .. |git commit --verbose| replace:: ``git commit --verbose``
 __ https://git-scm.com/docs/git-commit#Documentation/git-commit.txt--v
 
+``git-conflict-markers``
+------------------------
+
+A lexer for the conflict markers that Git adds to indicate conflicts during a merge.
+All other text in the file is lexed as plain text.
+
 ``git-console``
 ---------------
 
 A lexer for interactive shell sessions with Git.
 It calls out to |BashLexer|__ for highlighting commands on lines starting with a ``$`` and |DiffLexer2|__ for highlighting inline diffs.
 
 .. |BashLexer| replace:: ``BashLexer``
```

### Comparing `pygments_git-1.1.0/setup.cfg` & `pygments_git-1.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pygments_git
-version = 1.1.0
+version = 1.2.0
 description = Pygments lexers for Git output and files.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/pygments-git
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
@@ -40,15 +40,17 @@
 zip_safe = False
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 pygments.lexers = 
+	git-attributes=pygments_git:GitAttributesLexer
 	git-commit-edit-msg=pygments_git:GitCommitEditMsgLexer
+	git-conflict-markers=pygments_git:GitConflictMarkersLexer
 	git-console=pygments_git:GitBashSessionLexer
 	git-rebase-todo=pygments_git:GitRebaseTodoLexer
 
 [coverage:run]
 branch = True
 parallel = True
 source =
```

### Comparing `pygments_git-1.1.0/src/pygments_git/__init__.py` & `pygments_git-1.2.0/src/pygments_git/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,20 +6,55 @@
 from pygments.lexer import RegexLexer
 from pygments.lexer import using
 from pygments.lexers.diff import DiffLexer
 from pygments.lexers.shell import BashLexer
 from pygments.token import Comment
 from pygments.token import Generic
 from pygments.token import Keyword
+from pygments.token import Literal
 from pygments.token import Name
 from pygments.token import Number
+from pygments.token import Operator
+from pygments.token import Punctuation
 from pygments.token import String
 from pygments.token import Text
 
 
+class GitAttributesLexer(RegexLexer):
+    name = "Git Attributes"
+    aliases = ("git-attributes",)
+    flags = re.MULTILINE
+
+    tokens = {
+        "root": [
+            (r"^#.*$", Comment),
+            (
+                r"^(\S+)(\s+)",
+                bygroups(Literal, Text),  # type: ignore[no-untyped-call]
+                "attributes",
+            ),
+            (r"^.*\n", Text),
+        ],
+        "attributes": [
+            (
+                r"(-)?(.+?)(=)([^ \t\n]+)",
+                bygroups(  # type: ignore[no-untyped-call]
+                    Operator, Name.Variable, Operator, String.Symbol
+                ),
+            ),
+            (
+                r"(-)?([^ \t\n]+)",
+                bygroups(Operator, Name.Variable),  # type: ignore[no-untyped-call]
+            ),
+            (r"[ \t]+", Text),
+            (r"$", Text, "#pop"),
+        ],
+    }
+
+
 class GitCommitEditMsgLexer(RegexLexer):
     name = "Git Commit Edit-Msg"
     aliases = ("git-commit-edit-msg",)
     flags = re.MULTILINE
 
     tokens = {
         "root": [
@@ -57,14 +92,85 @@
                 using(DiffLexer),  # type: ignore [no-untyped-call]
                 "#pop",
             ),
         ],
     }
 
 
+class GitConflictMarkersLexer(RegexLexer):
+    name = "Git Conflict Markers"
+    aliases = ("git-conflict-markers",)
+    flags = re.MULTILINE
+
+    tokens = {
+        "root": [
+            (
+                r"^(<{7})( )?(.+)?$",
+                bygroups(  # type: ignore [no-untyped-call]
+                    Punctuation.Marker, Text, Name.Label
+                ),
+            ),
+            (
+                r"""(?x)
+                    ^
+                    (\|{7})
+                    (\ parent\ of\ )
+                    ([0-9a-f]{7})
+                    (\ \()
+                    (.*?)
+                    (\))
+                    $
+                """,
+                bygroups(  # type: ignore [no-untyped-call]
+                    Punctuation.Marker,
+                    Name.Label,
+                    Number.Hex,
+                    Text,
+                    Name.Label,
+                    Text,
+                ),
+            ),
+            (
+                r"^(\|{7})( )?(.*)$",
+                bygroups(  # type: ignore [no-untyped-call]
+                    Punctuation.Marker, Text, Name.Label
+                ),
+            ),
+            (
+                r"^(={7})( )?(.*)$",
+                bygroups(  # type: ignore [no-untyped-call]
+                    Punctuation.Marker, Text, Name.Label
+                ),
+            ),
+            (
+                r"""(?x)
+                    ^
+                    (>{7})
+                    (\ )
+                    ([0-9a-f]{7})
+                    (\ \()
+                    (.*?)
+                    (\))
+                    $
+                """,
+                bygroups(  # type: ignore [no-untyped-call]
+                    Punctuation.Marker, Text, Number.Hex, Text, Name.Label, Text
+                ),
+            ),
+            (
+                r"^(>{7})(\ )?(.*)?$",
+                bygroups(  # type: ignore [no-untyped-call]
+                    Punctuation.Marker, Text, Name.Label
+                ),
+            ),
+            (r".*\n", Text),
+        ]
+    }
+
+
 class GitBashSessionLexer(RegexLexer):
     name = "Git Bash Session"
     aliases = ("git-console",)
     flags = re.MULTILINE
 
     tokens = {
         "root": [
```

### Comparing `pygments_git-1.1.0/src/pygments_git.egg-info/PKG-INFO` & `pygments_git-1.2.0/src/pygments_git.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygments-git
-Version: 1.1.0
+Version: 1.2.0
 Summary: Pygments lexers for Git output and files.
 Home-page: https://github.com/adamchainz/pygments-git
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pygments-git/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -80,26 +80,34 @@
     .. code-block:: git-console
 
         $ git log --oneline
         82fbbd3 D'oh! Fix math proof
         91e9879 Aye carumba! Grammar mistake
         61c4c08 Cowabunga! Update bibliography
 
+To preview the lexers, open the ``tests/index.html`` file within the repository.
+
 ``git-commit-edit-msg``
 -----------------------
 
 A lexer for the ``COMMIT_EDITMSG`` file that Git opens when you run ``git commit``.
 It calls out to |DiffLexer|__ for highlighting any diff, as added by |git commit --verbose|__.
 
 .. |DiffLexer| replace:: ``DiffLexer``
 __ https://pygments.org/docs/lexers/#pygments.lexers.diff.DiffLexer
 
 .. |git commit --verbose| replace:: ``git commit --verbose``
 __ https://git-scm.com/docs/git-commit#Documentation/git-commit.txt--v
 
+``git-conflict-markers``
+------------------------
+
+A lexer for the conflict markers that Git adds to indicate conflicts during a merge.
+All other text in the file is lexed as plain text.
+
 ``git-console``
 ---------------
 
 A lexer for interactive shell sessions with Git.
 It calls out to |BashLexer|__ for highlighting commands on lines starting with a ``$`` and |DiffLexer2|__ for highlighting inline diffs.
 
 .. |BashLexer| replace:: ``BashLexer``
```

### Comparing `pygments_git-1.1.0/tests/test_pygments_git.py` & `pygments_git-1.2.0/tests/test_pygments_git.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,14 +74,22 @@
                 pre {
                   background: #eee;
                   padding: 0.5rem;
                 }
                 """
             ),
             formatter.get_style_defs(".highlight"),
+            dedent(
+                """\
+                .highlight .pm { /* Punctuation.Marker */
+                    color: #540099;
+                    font-weight: bold;
+                }
+                """
+            ),
             "</style>",
             "</head>",
             "<body>",
             "<h1>Tests</h1>",
         ]
         for testid, (lexer, given, result) in sorted(checker.cases.items()):
             lines.extend(
@@ -107,14 +115,29 @@
                 "</html>\n",
             ]
         )
 
         index.write_text("\n".join(lines))
 
 
+def test_git_attributes(golden_file):
+    golden_file.check(
+        "test_git_attributes",
+        "git-attributes",
+        """\
+        # Hello attributes
+        *.txt       text
+        *\ttext=auto
+        *.sh        text eol=lf
+        *.jpg -text
+        *.ps1 text working-tree-encoding=UTF-16LE eol=CRLF
+        """,
+    )
+
+
 def test_git_commit_edit_msg(golden_file):
     golden_file.check(
         "test_git_commit_edit_msg",
         "git-commit-edit-msg",
         """\
         Bop it
 
@@ -135,14 +158,46 @@
         @@ -1 +1 @@
         -twisted
         +bopped
         """,
     )
 
 
+def test_git_conflict_markers(golden_file):
+    golden_file.check(
+        "test_git_conflict_markers",
+        "git-conflict-markers",
+        """\
+        <<<<<<< HEAD
+        red
+        ||||||| parent of 09fb2fb (Make it blue)
+        yellow
+        =======
+        blue
+        >>>>>>> 09fb2fb (Make it blue)
+
+        <<<<<<< current
+        teal
+        ||||||| original
+        cerulean
+        ======= bla
+        cyan
+        >>>>>>> incoming
+
+        <<<<<<<
+        purple
+        |||||||
+        puce
+        =======
+        cerise
+        >>>>>>>
+        """,
+    )
+
+
 def test_git_console(golden_file):
     golden_file.check(
         "test_git_console",
         "git-console",
         """\
         $ git reflog
         0e87b4d (HEAD -> main, origin/main) HEAD@{0}: commit: Bop it
```

