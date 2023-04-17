# Comparing `tmp/write_the-0.3.0.tar.gz` & `tmp/write_the-0.4.0.tar.gz`

## Comparing `write_the-0.3.0.tar` & `write_the-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,56 @@
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 write_the-0.3.0/mkdocs.yml
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 write_the-0.3.0/test.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 write_the-0.3.0/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 write_the-0.3.0/docs/reference/cli.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.3.0/docs/reference/cst.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 write_the-0.3.0/docs/reference/docs.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 write_the-0.3.0/docs/reference/mkdocs.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.3.0/docs/reference/utils.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 write_the-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/__main__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/utils.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cli/__init__.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cli/main.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cst/__init__.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cst/docstring_adder.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cst/docstring_remover.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cst/function_and_class_collector.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cst/node_extractor.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cst/node_remover.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cst/utils.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/docs/__init__.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/docs/chain.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/docs/write.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/mkdocs/__init__.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/mkdocs/write.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/tests/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 write_the-0.3.0/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 write_the-0.3.0/README.md
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 write_the-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 write_the-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 write_the-0.4.0/mkdocs.yml
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 write_the-0.4.0/test.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 write_the-0.4.0/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.4.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 write_the-0.4.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 write_the-0.4.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 write_the-0.4.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 write_the-0.4.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 write_the-0.4.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.4.0/docs/CNAME
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 write_the-0.4.0/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 write_the-0.4.0/docs/reference/cli.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.4.0/docs/reference/cst.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 write_the-0.4.0/docs/reference/docs.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 write_the-0.4.0/docs/reference/mkdocs.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 write_the-0.4.0/docs/reference/utils.md
+-rw-r--r--   0        0        0   161159 2020-02-02 00:00:00.000000 write_the-0.4.0/images/multiply.png
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 write_the-0.4.0/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.4.0/tests/cli/test_main.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 write_the-0.4.0/tests/cst/test_cst_utils.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 write_the-0.4.0/tests/cst/test_docstring_adder.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 write_the-0.4.0/tests/cst/test_docstring_remover.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 write_the-0.4.0/tests/cst/test_function_and_class_collector.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 write_the-0.4.0/tests/cst/test_node_extractor.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 write_the-0.4.0/tests/cst/test_node_remover.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 write_the-0.4.0/tests/docs/test_docs_chain.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 write_the-0.4.0/tests/docs/test_docs_write.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 write_the-0.4.0/tests/mkdocs/test_mkdocs_write.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.4.0/tests/tests/test_test_chain.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 write_the-0.4.0/tests/tests/test_tests_write.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/__about__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/__main__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/utils.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/cli/__init__.py
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/cli/main.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/cst/__init__.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/cst/docstring_adder.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/cst/docstring_remover.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/cst/function_and_class_collector.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/cst/node_extractor.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/cst/node_remover.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/cst/utils.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/docs/__init__.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/docs/chain.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/docs/write.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/mkdocs/__init__.py
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/mkdocs/write.py
+-rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/tests/__init__.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/tests/chain.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 write_the-0.4.0/write_the/tests/write.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 write_the-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 write_the-0.4.0/README.md
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 write_the-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 write_the-0.4.0/PKG-INFO
```

### Comparing `write_the-0.3.0/docs/index.md` & `write_the-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
----
-title: Home
----
 # Write-The: AI-powered Code Generation and Refactoring Tool
 
 [![PyPI - Version](https://img.shields.io/pypi/v/write-the.svg)](https://pypi.org/project/write-the)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/write-the.svg)](https://pypi.org/project/write-the)
 
 Write-The is an AI-powered code generation and refactoring tool that leverages GPT-4 to help developers automatically write tests, generate documentation, and refactor code. It is designed to streamline the development process, improve code quality, and increase productivity.
 
+![](images/multiply.png)
+
 -----
 
 **Table of Contents**
 
 - [Features](#Features)
 - [Requirements](#Requirements)
 - [Installation](#Installation)
```

### Comparing `write_the-0.3.0/write_the/utils.py` & `write_the-0.4.0/write_the/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.3.0/write_the/cli/main.py` & `write_the-0.4.0/write_the/cli/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import typer
+import os
 from write_the.__about__ import __version__
 from write_the.docs import write_the_docs
+from write_the.tests import write_the_tests
 from write_the.mkdocs import write_the_mkdocs
-from ..utils import list_python_files
+from write_the.utils import list_python_files
 from pathlib import Path
 from rich.console import Console
 from rich.syntax import Syntax
 from typing import List, Optional
+from black import InvalidInput
 
 app = typer.Typer()
 
 
 @app.callback()
 def callback():
     """
@@ -26,65 +29,126 @@
     ),
     force: bool = typer.Option(
         False, "--force", "-f", help="Generate docstings even if they already exist."
     ),
     context: bool = typer.Option(
         False, "--context", "-c", help="Send context with nodes."
     ),
+    pretty: bool = typer.Option(
+        False, "--pretty", "-p", help="Use Black to format the output."
+    ),
     nodes: List[str] = typer.Option(
         None,
         "--node",
         "-n",
         help="Generate docs for specific nodes (functions and classes).",
     ),
 ):
     """
-    Document and format your code!
+    Document your code!
     """
     if file.is_dir():
         files = list_python_files(file)
     else:
         assert file.suffix == ".py"
         files = [file]
     for file in files:
         if len(files) > 1:
             typer.secho(file, fg="green")
         result = write_the_docs(
-            file, nodes=nodes, force=force, inplace=inplace, context=context
+            file, nodes=nodes, force=force, inplace=inplace, context=context, pretty=pretty
         )
         if inplace:
             with open(file, "w") as f:
                 f.writelines(result)
-        else:
+        elif pretty:
             syntax = Syntax(result, "python")
             console = Console()
             console.print(syntax)
-
+        else:
+            typer.echo(result)
 
 @app.command()
 def mkdocs(
     code_dir: Path = typer.Argument(
         ...,
         help="Path to the projects code. Will use docstings for reference.",
         file_okay=False,
     ),
     readme: Optional[Path] = typer.Option(
         None, help="Path to projects README (used to create index.md).", dir_okay=False
     )
 ):
     """
-    Generates mkdocs for a project and populate the API reference
+    Generates mkdocs for a project and the API reference
     """
     write_the_mkdocs(code_dir=code_dir, readme=readme)
 
 
 @app.command()
-def tests():
-    raise NotImplementedError()
-
+def tests(
+    file: Path = typer.Argument(..., help="Path to the file to generate docs."),
+    save: bool = typer.Option(
+        False, "--save", "-s", help="Save the tests to the tests directory."
+    ),
+    force: bool = typer.Option(
+        False, "--force", "-f", help="Generate docstings even if they already exist."
+    ),
+    context: bool = typer.Option(
+        False, "--context", "-c", help="Send context with nodes."
+    ),
+    pretty: bool = typer.Option(
+        False, "--pretty", "-p", help="Syntax highlight the output."
+    ),
+    nodes: List[str] = typer.Option(
+        None,
+        "--node",
+        "-n",
+        help="Generate tests for specific nodes (functions and classes).",
+    ),
+):
+    """
+    Generate tests for your code. 
+    """
+    if file.is_dir():
+        files = list_python_files(file)
+    else:
+        assert file.suffix == ".py"
+        files = [file]
+    for file in files:
+        if file.stem.startswith('_'):
+            continue
+        parts = list(file.parts[1:-1])
+        parts.append(f"test_{file.stem}.py")
+        test_file = Path(os.path.join(*parts))
+        tests_dir = Path('tests')
+        test_file = tests_dir / test_file
+        if test_file.exists() and (not force and save):
+            continue
+        if len(files) > 1:
+            typer.secho(file, fg="green")
+        try:
+            result = write_the_tests(
+                file
+            )
+        except InvalidInput:
+            failed = True
+            result = ""
+        if save:
+            # create test file
+            tests_dir.mkdir(exist_ok=True)
+            test_file.parent.mkdir(exist_ok=True, parents=True)
+            with open(test_file, "w") as f:
+                f.writelines(result)
+        elif pretty:
+            syntax = Syntax(result, "python")
+            console = Console()
+            console.print(syntax)
+        else:
+            typer.echo(result)
 
 @app.command()
 def refactor():
     raise NotImplementedError()
 
 
 @app.command()
```

### Comparing `write_the-0.3.0/write_the/cst/docstring_adder.py` & `write_the-0.4.0/write_the/cst/docstring_adder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import libcst as cst
 from .utils import has_docstring
-
+import textwrap
 
 class DocstringAdder(cst.CSTTransformer):
     def __init__(self, docstrings, force):
         self.docstrings = docstrings
         self.current_class = None
         self.force = force
 
@@ -49,11 +49,13 @@
             f"{self.current_class}.{node.name.value}"
             if self.current_class
             else node.name.value
         )
         docstring = self.docstrings.get(key, None)
 
         if docstring and (not has_docstring(node) or self.force):
-            new_docstring = cst.parse_statement(f'"""{docstring}"""')
+            dedented_docstring = textwrap.dedent(docstring)
+            indented_docstring = textwrap.indent(dedented_docstring, '    ')
+            new_docstring = cst.parse_statement(f'"""{indented_docstring}    """')
             body = node.body.with_changes(body=[new_docstring] + list(node.body.body))
             return node.with_changes(body=body)
         return node
```

### Comparing `write_the-0.3.0/write_the/cst/docstring_remover.py` & `write_the-0.4.0/write_the/cst/docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.3.0/write_the/cst/function_and_class_collector.py` & `write_the-0.4.0/write_the/cst/function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.3.0/write_the/cst/node_extractor.py` & `write_the-0.4.0/write_the/cst/node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.3.0/write_the/cst/node_remover.py` & `write_the-0.4.0/write_the/cst/node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.3.0/write_the/cst/utils.py` & `write_the-0.4.0/write_the/cst/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.3.0/write_the/docs/chain.py` & `write_the-0.4.0/write_the/docs/chain.py`

 * *Files identical despite different names*

### Comparing `write_the-0.3.0/write_the/docs/write.py` & `write_the-0.4.0/write_the/docs/write.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from write_the.cst.function_and_class_collector import get_node_names
 from write_the.cst.node_extractor import extract_nodes_from_tree
 from write_the.cst.node_remover import remove_nodes_from_tree
 from .chain import run
 
 
 def write_the_docs(
-    filename: Path, nodes=[], force=False, inplace=False, context=True
+    filename: Path, nodes=[], force=False, inplace=False, context=True, pretty=False
 ) -> str:
     """
     Generates docstrings for a given file.
     Args:
       filename (Path): The path to the file to generate docstrings for.
       nodes (list): A list of nodes to generate docstrings for.
       force (bool): Whether to overwrite existing docstrings.
@@ -36,46 +36,47 @@
           Returns:
               int: The sum of `a` and `b`.
           \"\"\"
           return a + b"
     """
     with open(filename, "r") as file:
         source_code = file.read()
-
-    source_code = format_str(source_code, mode=FileMode())
+    if pretty:
+        source_code = format_str(source_code, mode=FileMode())
     tree = cst.parse_module(source_code)
     extract_specific_nodes = False
 
     if nodes:
         extract_specific_nodes = True
         force = True
     else:
         nodes = get_node_names(tree, force)
     if not nodes:
         return source_code
-    remove_docstrings_tree = remove_docstrings(tree, nodes)
+    tree_without_docstrings = remove_docstrings(tree, nodes)
     if not context:
         if extract_specific_nodes:
-            extracted_nodes = extract_nodes_from_tree(remove_docstrings_tree, nodes)
+            extracted_nodes = extract_nodes_from_tree(tree_without_docstrings, nodes)
             processed_tree = nodes_to_tree(extracted_nodes)
         else:
             all_nodes = get_node_names(tree, False)
             nodes_to_remove = [n for n in all_nodes if n not in nodes]
             processed_tree = remove_nodes_from_tree(
-                remove_docstrings_tree, nodes_to_remove
+                tree_without_docstrings, nodes_to_remove
             )
         code = processed_tree.code
     else:
-        code = remove_docstrings_tree.code
+        code = tree_without_docstrings.code
     result = run(code=code, nodes=nodes)
     docstring_dict = {}
     for line in result.split("\n\n"):
         (node_name, docsting) = line.split(":", 1)
-        docstring_dict[node_name] = docsting + "\n\n"
-    modified_tree = remove_docstrings_tree.visit(DocstringAdder(docstring_dict, force))
+        docstring_dict[node_name] = docsting + "\n"
+    modified_tree = tree_without_docstrings.visit(DocstringAdder(docstring_dict, force))
 
     if not inplace and extract_specific_nodes:
         extracted_nodes = extract_nodes_from_tree(tree, nodes)
         modified_tree = nodes_to_tree(extracted_nodes)
 
-    modified_code = modified_tree.code
-    return format_str(modified_code, mode=FileMode())
+    if pretty:
+        return format_str(modified_tree.code, mode=FileMode())
+    return modified_tree.code
```

### Comparing `write_the-0.3.0/write_the/mkdocs/write.py` & `write_the-0.4.0/write_the/mkdocs/write.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,29 +38,32 @@
 
     reference_path = Path("./docs/reference/")
     reference_path.mkdir(parents=True, exist_ok=True)
     for doc in references:
         with open(f"{reference_path}/{doc}.md", "w") as f:
             for ref in references[doc]:
                 f.write(ref + "\n\n")
-
     if readme:
         index_text = f"---\ntitle: Home\n---\n{readme.read_text()}"
         Path("./docs/index.md").write_text(index_text)
     if not Path("./mkdocs.yml").exists():
         Path("./mkdocs.yml").write_text(mkdocs)
+    action_path = Path(".github/workflows/mkdocs.yml")
+    if not action_path.exists():
+        action_path.parent.mkdir(parents=True, exist_ok=True)
+        action_path.write_text(action_template)
 
 
 mkdocs_template = """
 site_name: {project_name}
 # repo_url: https://github.com/wytamma/write-the
 
 theme:
   name: "material"
-  # homepage: https://github.com/wytamma/write-the
+  # homepage: https://write-the.wytamma.com
   # logo: assets/logo.png
   # favicon: images/favicon.png
   palette: 
     - scheme: default
       toggle:
         icon: material/brightness-7 
         name: Switch to dark mode
@@ -72,7 +75,32 @@
     - toc.follow
     - content.action.edit
 
 plugins:
 - search
 - mkdocstrings
 """
+
+action_template = """
+name: mkdocs 
+on:
+  push:
+    branches:
+      - master 
+      - main
+permissions:
+  contents: write
+jobs:
+  deploy:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        with:
+          python-version: 3.x
+      - uses: actions/cache@v2
+        with:
+          key: ${{ github.ref }}
+          path: .cache
+      - run: pip install "mkdocstrings[python]" "mkdocs-material"
+      - run: mkdocs gh-deploy --force
+"""
```

### Comparing `write_the-0.3.0/LICENSE.txt` & `write_the-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `write_the-0.3.0/README.md` & `write_the-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,42 @@
+Metadata-Version: 2.1
+Name: write-the
+Version: 0.4.0
+Summary: AI-powered Code Generation and Refactoring Tool
+Project-URL: Documentation, https://github.com/wytamma/write-the#readme
+Project-URL: Issues, https://github.com/wytamma/write-the/issues
+Project-URL: Source, https://github.com/wytamma/write-the
+Author-email: wytamma <wytamma.wirth@me.com>
+License-Expression: MIT
+License-File: LICENSE.txt
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.9
+Requires-Dist: black
+Requires-Dist: langchain
+Requires-Dist: libcst
+Requires-Dist: mkdocs-material
+Requires-Dist: mkdocstrings[python]
+Requires-Dist: typer[all]
+Description-Content-Type: text/markdown
+
 # Write-The: AI-powered Code Generation and Refactoring Tool
 
 [![PyPI - Version](https://img.shields.io/pypi/v/write-the.svg)](https://pypi.org/project/write-the)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/write-the.svg)](https://pypi.org/project/write-the)
 
 Write-The is an AI-powered code generation and refactoring tool that leverages GPT-4 to help developers automatically write tests, generate documentation, and refactor code. It is designed to streamline the development process, improve code quality, and increase productivity.
 
+![](images/multiply.png)
+
 -----
 
 **Table of Contents**
 
 - [Features](#Features)
 - [Requirements](#Requirements)
 - [Installation](#Installation)
```

### Comparing `write_the-0.3.0/pyproject.toml` & `write_the-0.4.0/pyproject.toml`

 * *Files identical despite different names*

