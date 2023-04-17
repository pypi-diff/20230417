# Comparing `tmp/toml_cli-0.4.0.tar.gz` & `tmp/toml_cli-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toml_cli-0.4.0.tar", max compression
+gzip compressed data, was "toml_cli-0.4.2.tar", max compression
```

## Comparing `toml_cli-0.4.0.tar` & `toml_cli-0.4.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-04-14 22:51:48.834797 toml_cli-0.4.0/LICENSE
--rw-r--r--   0        0        0      780 2023-04-14 22:51:48.834797 toml_cli-0.4.0/README.md
--rw-r--r--   0        0        0      646 2023-04-14 22:51:48.834797 toml_cli-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2612 2023-04-14 22:51:48.834797 toml_cli-0.4.0/toml_cli/__init__.py
--rw-r--r--   0        0        0     1569 1970-01-01 00:00:00.000000 toml_cli-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-17 18:46:19.815059 toml_cli-0.4.2/LICENSE
+-rw-r--r--   0        0        0      780 2023-04-17 18:46:19.815059 toml_cli-0.4.2/README.md
+-rw-r--r--   0        0        0      646 2023-04-17 18:46:19.815059 toml_cli-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2619 2023-04-17 18:46:19.815059 toml_cli-0.4.2/toml_cli/__init__.py
+-rw-r--r--   0        0        0     1569 1970-01-01 00:00:00.000000 toml_cli-0.4.2/PKG-INFO
```

### Comparing `toml_cli-0.4.0/LICENSE` & `toml_cli-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toml_cli-0.4.0/README.md` & `toml_cli-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `toml_cli-0.4.0/pyproject.toml` & `toml_cli-0.4.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "toml-cli"
-version = "0.4.0"
+version = "0.4.2"
 description = "Command line interface to read and write keys/values to/from toml files"
 authors = ["Marc Rijken"]
 license = "MIT"
 repository = "https://github.com/mrijken/toml-cli"
 readme = "README.md"
 packages = [{ include = "toml_cli" }]
```

### Comparing `toml_cli-0.4.0/toml_cli/__init__.py` & `toml_cli-0.4.2/toml_cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,26 +17,29 @@
     """Get a value from a toml file"""
     toml_part = tomlkit.parse(toml_path.read_text())
 
     if key is not None:
         for key_part in key.split("."):
             toml_part = toml_part[key_part]
 
-    typer.echo(json.dumps(toml_part))
+    typer.echo(toml_part)
 
 
 @app.command("set")
 def set_(
     key: str,
     value: str,
     toml_path: pathlib.Path = typer.Option(pathlib.Path("config.toml")),
     to_int: bool = typer.Option(False),
     to_float: bool = typer.Option(False),
     to_bool: bool = typer.Option(False),
-    to_array: bool = typer.Option(False, help="accepts a valid json array and covert it to toml, ie [\"Amsterdam\",\"Rotterdam\"]"),
+    to_array: bool = typer.Option(
+        False,
+        help='accepts a valid json array and covert it to toml, ie ["Amsterdam","Rotterdam"]',
+    ),
 ):
     """Set a value to a toml file"""
     toml_part = toml_file = tomlkit.parse(toml_path.read_text())
 
     for key_part in key.split(".")[:-1]:
         try:
             toml_part = toml_part[key_part]
```

### Comparing `toml_cli-0.4.0/PKG-INFO` & `toml_cli-0.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toml-cli
-Version: 0.4.0
+Version: 0.4.2
 Summary: Command line interface to read and write keys/values to/from toml files
 Home-page: https://github.com/mrijken/toml-cli
 License: MIT
 Author: Marc Rijken
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

