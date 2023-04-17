# Comparing `tmp/xh-dict-utils-0.0.4.tar.gz` & `tmp/xh-dict-utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xh-dict-utils-0.0.4.tar", last modified: Mon Apr 17 06:04:16 2023, max compression
+gzip compressed data, was "xh-dict-utils-0.0.5.tar", last modified: Mon Apr 17 08:17:38 2023, max compression
```

## Comparing `xh-dict-utils-0.0.4.tar` & `xh-dict-utils-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:04:16.943828 xh-dict-utils-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 06:04:16.943828 xh-dict-utils-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 06:04:16.943828 xh-dict-utils-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:04:16.939828 xh-dict-utils-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:04:16.939828 xh-dict-utils-0.0.4/src/xh_dict_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/src/xh_dict_utils/ExtractFromFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/src/xh_dict_utils/Layer1AppEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/src/xh_dict_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/src/xh_dict_utils/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/src/xh_dict_utils/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/src/xh_dict_utils/test_dict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:04:16.939828 xh-dict-utils-0.0.4/src/xh_dict_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 06:04:16.000000 xh-dict-utils-0.0.4/src/xh_dict_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 06:04:16.000000 xh-dict-utils-0.0.4/src/xh_dict_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 06:04:16.000000 xh-dict-utils-0.0.4/src/xh_dict_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 06:04:16.000000 xh-dict-utils-0.0.4/src/xh_dict_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:17:38.056219 xh-dict-utils-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 08:17:38.056219 xh-dict-utils-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 08:17:38.056219 xh-dict-utils-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:17:38.056219 xh-dict-utils-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:17:38.056219 xh-dict-utils-0.0.5/src/xh_dict_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/src/xh_dict_utils/ExtractFromFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/src/xh_dict_utils/Layer1AppEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/src/xh_dict_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/src/xh_dict_utils/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/src/xh_dict_utils/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/src/xh_dict_utils/test_dict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:17:38.056219 xh-dict-utils-0.0.5/src/xh_dict_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 08:17:38.000000 xh-dict-utils-0.0.5/src/xh_dict_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 08:17:38.000000 xh-dict-utils-0.0.5/src/xh_dict_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:17:38.000000 xh-dict-utils-0.0.5/src/xh_dict_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 08:17:38.000000 xh-dict-utils-0.0.5/src/xh_dict_utils.egg-info/top_level.txt
```

### Comparing `xh-dict-utils-0.0.4/LICENSE.txt` & `xh-dict-utils-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.4/PKG-INFO` & `xh-dict-utils-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-dict-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: A dictionary utility of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xh-dict-utils-0.0.4/pyproject.toml` & `xh-dict-utils-0.0.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-[build-system]
-requires = [
-    "setuptools>=61.0"
-]
-build-backend = "setuptools.build_meta"
-[project]
-name = "xh-dict-utils"
-version = "0.0.4"
-authors = [
-  { name="xethhung", email="pypi@xethh.dev" },
-]
-description = "A dictionary utility of self dev py library"
-readme = "README.md"
-requires-python = ">=3.6"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/xh-dev/xh-dict-utils"
-"Bug Tracker" = "https://github.com/xh-dev/xh-dict-utils/issues"
+[build-system]
+requires = [ "setuptools>=61.0",]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "xh-dict-utils"
+version = "0.0.5"
+description = "A dictionary utility of self dev py library"
+readme = "README.md"
+requires-python = ">=3.6"
+classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
+[[project.authors]]
+name = "xethhung"
+email = "pypi@xethh.dev"
+
+[project.urls]
+Homepage = "https://github.com/xh-dev/xh-dict-utils"
+"Bug Tracker" = "https://github.com/xh-dev/xh-dict-utils/issues"
```

### Comparing `xh-dict-utils-0.0.4/src/xh_dict_utils/ExtractFromFile.py` & `xh-dict-utils-0.0.5/src/xh_dict_utils/ExtractFromFile.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.4/src/xh_dict_utils/Layer1AppEngine.py` & `xh-dict-utils-0.0.5/src/xh_dict_utils/Layer1AppEngine.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         self.help = help
 
     @abstractmethod
     def parserOp(self, parser: argparse.ArgumentParser):
         pass
 
     @abstractmethod
-    def handleOp(self, argv: list[str]):
+    def handleOp(self, argv: [str]):
         pass
 
 
 class AppEngine:
     def __parser_setup(self) -> argparse.ArgumentParser:
         return argparse.ArgumentParser(
             prog=self.program_name,
@@ -37,29 +37,29 @@
         self.description = description
         self.root_parser = parser_setup(self)
         self.subparsers = sub_parser_setup(self)
         self.subCommands = dict()
         self.handlers = dict()
 
     def regSubCommand(self, key: str, help: str, parserOp: Callable[[argparse.ArgumentParser], None],
-                      handle: Callable[[list[str]], None]):
+                      handle: Callable[[[str]], None]):
         if key not in self.subCommands:
             parser = self.subparsers.add_parser(key, help=help)
             parserOp(parser)
             self.subCommands.update({key: parser})
 
             def handling(args):
                 # parsed_args = root_parser.parse_args(args)
                 parsed_args = parser.parse_args(args)
                 handle(parsed_args)
 
             self.handlers.update({key: handling})
         return
 
-    def process(self, allArgs: list[str]):
+    def process(self, allArgs: [str]):
         if len(allArgs) < 2:
             self.root_parser.print_help()
             exit(1)
 
         key = allArgs[1]
         if key not in self.subCommands:
             raise Exception(f"command[{key}] not valid")
```

### Comparing `xh-dict-utils-0.0.4/src/xh_dict_utils/app.py` & `xh-dict-utils-0.0.5/src/xh_dict_utils/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     class LoadPipe(CommandTemplate):
         def __init__(self):
             super().__init__("load-pipe", "load from pipe")
 
         def parserOp(self, parser: argparse.ArgumentParser):
             parser.add_argument("--format", choices=["json", "yaml"], default="yaml")
 
-        def handleOp(self, argv: list[str]):
+        def handleOp(self, argv: [str]):
             format_type = getattr(SupportedFormat, argv.format.upper())
             if format_type == SupportedFormat.YAML:
                 d = yaml.safe_load(sys.stdin.read())
             elif format_type == SupportedFormat.JSON:
                 d = json.loads(sys.stdin.read())
             else:
                 raise Exception("Not supported format")
@@ -41,15 +41,15 @@
         def __init__(self):
             super().__init__("load-file", "load file")
 
         def parserOp(self, parser: argparse.ArgumentParser):
             parser.add_argument("--format", choices=["json", "yaml"], default="yaml")
             parser.add_argument("--file")
 
-        def handleOp(self, argv: list[str]):
+        def handleOp(self, argv: [str]):
             format = getattr(SupportedFormat, argv.format.upper())
 
             def read_all_in_file(filePath) -> str:
                 if not os.path.exists(filePath):
                     raise Exception(f"Path[{filePath}] not exists")
 
                 if not os.path.isfile(filePath):
@@ -93,15 +93,15 @@
             parser.add_argument("--node-value-type-str", dest="node_value_type", action="store_const", const="str")
             parser.add_argument("--node-value-type-int", dest="node_value_type", action="store_const", const="int")
             parser.add_argument("--node-value-type-number", dest="node_value_type", action="store_const",
                                 const="number")
             parser.add_argument("--node-value-type-object", dest="node_value_type", action="store_const",
                                 const="object")
 
-        def handleOp(self, argv: list[str]):
+        def handleOp(self, argv: [str]):
             selector = argv.selector
 
             dict_from_pipe = argv.dict_from_pipe
             dict_from_file = argv.dict_from_file
             node_value_file = argv.node_value_file
             node_value = argv.node_value
             node_value_type = argv.node_value_type
@@ -180,15 +180,15 @@
     class RemoveNode(CommandTemplate):
         def __init__(self):
             super().__init__("remove-node", "remove a node")
 
         def parserOp(self, parser: argparse.ArgumentParser):
             parser.add_argument("--selector", type=str)
 
-        def handleOp(self, argv: list[str]):
+        def handleOp(self, argv: [str]):
             selector = argv.selector
             if Selector.from_notation(selector).is_array_group():
                 is_array_group = True
             else:
                 is_array_group = False
 
             d = yaml.safe_load(sys.stdin.read())
@@ -226,15 +226,15 @@
             parser.add_argument("--selector", type=str)
             parser.add_argument("--output", type=str, default="{selector} -> {value}")
             parser.add_argument("--exact", dest="notation_type", action="store_const", const="exact")
             parser.add_argument("--regex", dest="notation_type", action="store_const", const="regex")
             parser.set_defaults(notation_type="notation")
             parser.set_defaults(exact=False)
 
-        def handleOp(self, argv: list[str]):
+        def handleOp(self, argv: [str]):
             selector = argv.selector
             if argv.notation_type == "exact":
                 findings = Entries.from_dict(yaml.safe_load(sys.stdin)).match_exact(selector)
             elif argv.notation_type == "regex":
                 findings = Entries.from_dict(yaml.safe_load(sys.stdin)).match_regex(selector)
             if argv.notation_type == "notation":
                 findings = Entries.from_dict(yaml.safe_load(sys.stdin)).match_notation(selector)
@@ -252,15 +252,15 @@
             super().__init__("output", "output as json")
 
         def parserOp(self, parser: argparse.ArgumentParser):
             parser.add_argument("--store", type=str, default=None)
             parser.add_argument("--format", choices=["json", "yaml"])
             parser.add_argument("--pretty", action="store_true", default=False)
 
-        def handleOp(self, argv: list[str]):
+        def handleOp(self, argv: [str]):
             class Logger(object):
                 def __init__(self, channel: list):
                     self.channels = channel
 
                 def write(self, message):
                     for channel in self.channels:
                         channel.write(message)
```

### Comparing `xh-dict-utils-0.0.4/src/xh_dict_utils/dict_utils.py` & `xh-dict-utils-0.0.5/src/xh_dict_utils/dict_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,17 +160,17 @@
             return f"Entry({self.get_selector()}, {self.value})"
 
     def __repr__(self):
         return self.__str__()
 
 
 class Entries:
-    entries: list[Entry]
+    entries: [Entry]
 
-    def __init__(self, entries: list[Entry]):
+    def __init__(self, entries: [Entry]):
         self.entries = entries
 
     def match_exact(self, selector: str) -> "Entries":
         return Entries([t for t in self.entries if t.exact_selector(selector)])
 
     def match_regex(self, selector: str) -> "Entries":
         return Entries([t for t in self.entries if t.regex_selector(selector)])
```

### Comparing `xh-dict-utils-0.0.4/src/xh_dict_utils/test_dict_utils.py` & `xh-dict-utils-0.0.5/src/xh_dict_utils/test_dict_utils.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.4/src/xh_dict_utils.egg-info/PKG-INFO` & `xh-dict-utils-0.0.5/src/xh_dict_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-dict-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: A dictionary utility of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

