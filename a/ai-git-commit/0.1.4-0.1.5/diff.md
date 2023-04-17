# Comparing `tmp/ai_git_commit-0.1.4.tar.gz` & `tmp/ai_git_commit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_git_commit-0.1.4.tar", max compression
+gzip compressed data, was "ai_git_commit-0.1.5.tar", max compression
```

## Comparing `ai_git_commit-0.1.4.tar` & `ai_git_commit-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1052 2023-03-15 18:58:44.790239 ai_git_commit-0.1.4/LICENSE.md
--rw-r--r--   0        0        0     2169 2023-03-20 06:52:08.237101 ai_git_commit-0.1.4/README.md
--rw-r--r--   0        0        0     1722 2023-03-30 12:37:31.809687 ai_git_commit-0.1.4/ai_git_commit/__init__.py
--rw-r--r--   0        0        0     2538 2023-03-30 12:36:39.371390 ai_git_commit-0.1.4/ai_git_commit/config.py
--rw-r--r--   0        0        0     5758 2023-03-30 13:04:03.265174 ai_git_commit-0.1.4/ai_git_commit/git.py
--rw-r--r--   0        0        0      783 2023-03-17 20:59:09.297438 ai_git_commit-0.1.4/ai_git_commit/openai.py
--rw-r--r--   0        0        0     8765 2023-03-20 05:41:38.617113 ai_git_commit-0.1.4/ai_git_commit/prompts.py
--rw-r--r--   0        0        0     1205 2023-03-30 13:10:02.855783 ai_git_commit-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3233 1970-01-01 00:00:00.000000 ai_git_commit-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-03-15 18:58:44.790239 ai_git_commit-0.1.5/LICENSE.md
+-rw-r--r--   0        0        0     2169 2023-03-20 06:52:08.237101 ai_git_commit-0.1.5/README.md
+-rw-r--r--   0        0        0     1722 2023-03-30 12:37:31.809687 ai_git_commit-0.1.5/ai_git_commit/__init__.py
+-rw-r--r--   0        0        0     4260 2023-04-17 06:58:51.213640 ai_git_commit-0.1.5/ai_git_commit/config.py
+-rw-r--r--   0        0        0    11770 2023-04-17 06:58:10.135492 ai_git_commit-0.1.5/ai_git_commit/git.py
+-rw-r--r--   0        0        0      783 2023-03-17 20:59:09.297438 ai_git_commit-0.1.5/ai_git_commit/openai.py
+-rw-r--r--   0        0        0     8765 2023-03-20 05:41:38.617113 ai_git_commit-0.1.5/ai_git_commit/prompts.py
+-rw-r--r--   0        0        0     1205 2023-04-17 07:00:29.483782 ai_git_commit-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3233 1970-01-01 00:00:00.000000 ai_git_commit-0.1.5/PKG-INFO
```

### Comparing `ai_git_commit-0.1.4/LICENSE.md` & `ai_git_commit-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ai_git_commit-0.1.4/README.md` & `ai_git_commit-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ai_git_commit-0.1.4/ai_git_commit/__init__.py` & `ai_git_commit-0.1.5/ai_git_commit/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_git_commit-0.1.4/ai_git_commit/config.py` & `ai_git_commit-0.1.5/ai_git_commit/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -50,39 +50,72 @@
 
 
 class ValidConfig(Dict[str, str]):
     pass
 
 
 def read_config_file() -> RawConfig:
+    """
+    The read_config_file function reads the configuration file and returns a RawConfig object.
+
+    The config_path is set to ~/.ai-git-commit if there is no .env file in the current directory, otherwise it's set to ./env. If there isn't a config_path, an empty RawConfig object is returned. Otherwise, we open the config_path for reading and parse it with ini (which returns a dictionary). We then return that dictionary as part of our RawConfig object.
+
+    :return: A rawconfig object.
+
+    :doc-author: coderj001
+    """
     config_path = (
         os.path.join(os.path.expanduser("~"), ".ai-git-commit")
         if not file_exists(".env")
         else os.path.join(os.getcwd(), ".env")
     )
     if not file_exists(config_path):
         return RawConfig()
     with open(config_path, "r") as f:
         raw_config = ini.parse(f.read())
         return RawConfig(raw_config)
 
 
 def set_configs(key_values: Tuple[Tuple[str, str], ...]):
+    """
+    The set_configs function takes a list of tuples, where each tuple is a key-value pair.
+    The keys are the names of config properties, and the values are strings that will be parsed
+    into whatever type is appropriate for that property. The function then writes these new values
+    to the user's config file.
+
+    :param key_values:Tuple[Tuple[str: Used to Specify the type of the key_values parameter.
+    :param str]: Used to Specify the type of the value.
+    :param ...]: Used to Indicate that the function can take any number of arguments.
+    :return: A string.
+
+    :doc-author: coderj001
+    """
     config = read_config_file()
     for key, value in key_values:
         if key not in config_parsers:
             raise KnownError(f"Invalid config property: {key}")
         parsed = config_parsers[key](value)
         config[key] = parsed
     config_path = os.path.join(os.path.expanduser("~"), ".ai-git-commit")
     with open(config_path, "w") as f:
         f.write(ini.stringify(config))
 
 
 def get_config(cli_config: Optional[RawConfig] = None) -> ValidConfig:
+    """
+    The get_config function is responsible for reading the configuration file and
+    parsing it into a dictionary of values. It also takes in an optional cli_config
+    parameter, which is used to override any config values that are passed in via the CLI.
+    The function returns a ValidConfig object, which is just a namedtuple containing all of the parsed config values.
+
+    :param cli_config:Optional[RawConfig]=None: Used to Pass in the config.
+    :return: A dictionary with the keys and values from the config file.
+
+    :doc-author: coderj001
+    """
     config = read_config_file()
     parsed_config = {}
     for key, parser in config_parsers.items():
         value = (
             cli_config.get(key) if cli_config and key in cli_config else config.get(key)
         )
         parsed_config[key] = parser(value)
```

### Comparing `ai_git_commit-0.1.4/ai_git_commit/openai.py` & `ai_git_commit-0.1.5/ai_git_commit/openai.py`

 * *Files identical despite different names*

### Comparing `ai_git_commit-0.1.4/ai_git_commit/prompts.py` & `ai_git_commit-0.1.5/ai_git_commit/prompts.py`

 * *Files identical despite different names*

### Comparing `ai_git_commit-0.1.4/pyproject.toml` & `ai_git_commit-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai-git-commit"
-version = "0.1.4"
+version = "0.1.5"
 description = " AI Git Commit is a Python-based tool that uses AI to generate Git commit messages automatically."
 authors = ["Raju Ghorai <rajughorai41410@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ai_git_commit"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ai_git_commit-0.1.4/PKG-INFO` & `ai_git_commit-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-git-commit
-Version: 0.1.4
+Version: 0.1.5
 Summary:  AI Git Commit is a Python-based tool that uses AI to generate Git commit messages automatically.
 License: MIT
 Author: Raju Ghorai
 Author-email: rajughorai41410@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ai-git-commit Version: 0.1.4 Summary: AI Git Commit
+Metadata-Version: 2.1 Name: ai-git-commit Version: 0.1.5 Summary: AI Git Commit
 is a Python-based tool that uses AI to generate Git commit messages
 automatically. License: MIT Author: Raju Ghorai Author-email:
 rajughorai41410@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.1.0,<24.0.0) Requires-Dist: click (>=8.1.3,<9.0.0)
```

