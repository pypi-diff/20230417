# Comparing `tmp/openai_shell_craft-0.4.0.tar.gz` & `tmp/openai_shell_craft-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_shell_craft-0.4.0.tar", last modified: Fri Mar 31 20:47:27 2023, max compression
+gzip compressed data, was "openai_shell_craft-0.5.4.tar", last modified: Mon Apr 17 16:24:56 2023, max compression
```

## Comparing `openai_shell_craft-0.4.0.tar` & `openai_shell_craft-0.5.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:47:27.073289 openai_shell_craft-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-03-31 20:47:27.073289 openai_shell_craft-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:47:27.065288 openai_shell_craft-0.4.0/openai_shell_craft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-03-31 20:47:27.000000 openai_shell_craft-0.4.0/openai_shell_craft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-31 20:47:27.000000 openai_shell_craft-0.4.0/openai_shell_craft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 20:47:27.000000 openai_shell_craft-0.4.0/openai_shell_craft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-31 20:47:27.000000 openai_shell_craft-0.4.0/openai_shell_craft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-31 20:47:27.000000 openai_shell_craft-0.4.0/openai_shell_craft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-31 20:47:27.000000 openai_shell_craft-0.4.0/openai_shell_craft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 20:47:27.073289 openai_shell_craft-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:47:27.069289 openai_shell_craft-0.4.0/shell_craft/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:47:27.069289 openai_shell_craft-0.4.0/shell_craft/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/cli/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/cli/key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/cli/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/cli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/cli/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/cli/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:47:27.069289 openai_shell_craft-0.4.0/shell_craft/factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/factories/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:47:27.073289 openai_shell_craft-0.4.0/shell_craft/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/prompts/feature_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/prompts/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/prompts/prompt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/shell_craft/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:47:27.073289 openai_shell_craft-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-03-31 20:47:10.000000 openai_shell_craft-0.4.0/tests/test_factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:24:56.962135 openai_shell_craft-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-04-17 16:24:56.962135 openai_shell_craft-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:24:56.958135 openai_shell_craft-0.5.4/openai_shell_craft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-04-17 16:24:56.000000 openai_shell_craft-0.5.4/openai_shell_craft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-17 16:24:56.000000 openai_shell_craft-0.5.4/openai_shell_craft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:24:56.000000 openai_shell_craft-0.5.4/openai_shell_craft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-17 16:24:56.000000 openai_shell_craft-0.5.4/openai_shell_craft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 16:24:56.000000 openai_shell_craft-0.5.4/openai_shell_craft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 16:24:56.000000 openai_shell_craft-0.5.4/openai_shell_craft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:24:56.962135 openai_shell_craft-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:24:56.958135 openai_shell_craft-0.5.4/shell_craft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:24:56.958135 openai_shell_craft-0.5.4/shell_craft/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/cli/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:24:56.958135 openai_shell_craft-0.5.4/shell_craft/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/factories/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:24:56.962135 openai_shell_craft-0.5.4/shell_craft/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/prompts/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/prompts/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/prompts/templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/shell_craft/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:24:56.962135 openai_shell_craft-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-17 16:24:48.000000 openai_shell_craft-0.5.4/tests/test_factories.py
```

### Comparing `openai_shell_craft-0.4.0/LICENSE` & `openai_shell_craft-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/PKG-INFO` & `openai_shell_craft-0.5.4/openai_shell_craft.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openai_shell_craft
-Version: 0.4.0
+Name: openai-shell-craft
+Version: 0.5.4
 Summary: Generating shell commands and code using natural language models (OpenAI ChatGPT).
 Author-email: Johnathan Irvin <irvinjohnathan@gmail.com>
 Project-URL: Homepage, https://github.com/JohnnyIrvin/shell-craft
 Project-URL: Bug Tracker, https://github.com/JohnnyIrvin/shell-craft/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,21 @@
 
 ## Install using Pip
 
 ```sh
 pip install openai-shell-craft
 ```
 
+## Build from Docker and Run
+
+```sh
+docker build . --tag shell_craft --target shell_craft
+docker run shell_craft --help
+```
+
 ## Command Line Interface
 
 All command line usage follows the following format:
 
 ```bash
 shell-craft <request>
 ```
@@ -53,14 +60,15 @@
 | Language      | [PowerShell](https://learn.microsoft.com/en-us/powershell/)           | `powershell`      |
 | Language      | [Python](https://www.python.org/)                                     | `python`          |
 | Language      | [C](https://en.wikipedia.org/wiki/C_(programming_language))           | `c`               |
 | Language      | [C#](https://learn.microsoft.com/en-us/dotnet/csharp/)                | `c_sharp`         |
 | Language      | [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) | `javascript`      |
 | Language      | [Java](https://dev.java/)                                             | `java`            |
 | Language      | [Go](https://go.dev/)                                                 | `go`              |
+| Template      | Bug Report                                                            | `bug_report`      |
 | Template      | Feature Request                                                       | `feature_request` |
 
 When `--prompt` is not specified, Shell Craft will use `bash` unless PowerShell is used to call Shell Craft, then it uses `powershell`.
 
 ### Help Prompt
 
 For additional help you can run:
@@ -181,15 +189,21 @@
 3. Click the "Create new secret key" button.
 4. Copy the key that is generated for you.
 
 Once you have your API key, you **must** pass it to Shell Craft via **one** of the following methods.
 
 ### Option 1 (Recommended) - Configuration file:
 
-Create a file named `config.json`:
+shell-craft looks for a configuration file in the following places, in order:
+  - the current directory, named config.json
+  - the file named by $SHELLCRAFT_CONFIG
+  - $XDG_CONFIG_HOME/shell-craft/config.json
+  - $HOME/.config/shell-craft/config.json
+
+The contents are simple json:
 ```
 {
     "openai_api_key": "<your secret key>"
 }
 ```
 
 Now, Shell Craft will know your API key in order to run future prompts without having to specify it or ensure it exists in the environmental variables.
```

### Comparing `openai_shell_craft-0.4.0/README.md` & `openai_shell_craft-0.5.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 
 ## Install using Pip
 
 ```sh
 pip install openai-shell-craft
 ```
 
+## Build from Docker and Run
+
+```sh
+docker build . --tag shell_craft --target shell_craft
+docker run shell_craft --help
+```
+
 ## Command Line Interface
 
 All command line usage follows the following format:
 
 ```bash
 shell-craft <request>
 ```
@@ -39,14 +46,15 @@
 | Language      | [PowerShell](https://learn.microsoft.com/en-us/powershell/)           | `powershell`      |
 | Language      | [Python](https://www.python.org/)                                     | `python`          |
 | Language      | [C](https://en.wikipedia.org/wiki/C_(programming_language))           | `c`               |
 | Language      | [C#](https://learn.microsoft.com/en-us/dotnet/csharp/)                | `c_sharp`         |
 | Language      | [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) | `javascript`      |
 | Language      | [Java](https://dev.java/)                                             | `java`            |
 | Language      | [Go](https://go.dev/)                                                 | `go`              |
+| Template      | Bug Report                                                            | `bug_report`      |
 | Template      | Feature Request                                                       | `feature_request` |
 
 When `--prompt` is not specified, Shell Craft will use `bash` unless PowerShell is used to call Shell Craft, then it uses `powershell`.
 
 ### Help Prompt
 
 For additional help you can run:
@@ -167,15 +175,21 @@
 3. Click the "Create new secret key" button.
 4. Copy the key that is generated for you.
 
 Once you have your API key, you **must** pass it to Shell Craft via **one** of the following methods.
 
 ### Option 1 (Recommended) - Configuration file:
 
-Create a file named `config.json`:
+shell-craft looks for a configuration file in the following places, in order:
+  - the current directory, named config.json
+  - the file named by $SHELLCRAFT_CONFIG
+  - $XDG_CONFIG_HOME/shell-craft/config.json
+  - $HOME/.config/shell-craft/config.json
+
+The contents are simple json:
 ```
 {
     "openai_api_key": "<your secret key>"
 }
 ```
 
 Now, Shell Craft will know your API key in order to run future prompts without having to specify it or ensure it exists in the environmental variables.
```

### Comparing `openai_shell_craft-0.4.0/openai_shell_craft.egg-info/PKG-INFO` & `openai_shell_craft-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openai-shell-craft
-Version: 0.4.0
+Name: openai_shell_craft
+Version: 0.5.4
 Summary: Generating shell commands and code using natural language models (OpenAI ChatGPT).
 Author-email: Johnathan Irvin <irvinjohnathan@gmail.com>
 Project-URL: Homepage, https://github.com/JohnnyIrvin/shell-craft
 Project-URL: Bug Tracker, https://github.com/JohnnyIrvin/shell-craft/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,21 @@
 
 ## Install using Pip
 
 ```sh
 pip install openai-shell-craft
 ```
 
+## Build from Docker and Run
+
+```sh
+docker build . --tag shell_craft --target shell_craft
+docker run shell_craft --help
+```
+
 ## Command Line Interface
 
 All command line usage follows the following format:
 
 ```bash
 shell-craft <request>
 ```
@@ -53,14 +60,15 @@
 | Language      | [PowerShell](https://learn.microsoft.com/en-us/powershell/)           | `powershell`      |
 | Language      | [Python](https://www.python.org/)                                     | `python`          |
 | Language      | [C](https://en.wikipedia.org/wiki/C_(programming_language))           | `c`               |
 | Language      | [C#](https://learn.microsoft.com/en-us/dotnet/csharp/)                | `c_sharp`         |
 | Language      | [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) | `javascript`      |
 | Language      | [Java](https://dev.java/)                                             | `java`            |
 | Language      | [Go](https://go.dev/)                                                 | `go`              |
+| Template      | Bug Report                                                            | `bug_report`      |
 | Template      | Feature Request                                                       | `feature_request` |
 
 When `--prompt` is not specified, Shell Craft will use `bash` unless PowerShell is used to call Shell Craft, then it uses `powershell`.
 
 ### Help Prompt
 
 For additional help you can run:
@@ -181,15 +189,21 @@
 3. Click the "Create new secret key" button.
 4. Copy the key that is generated for you.
 
 Once you have your API key, you **must** pass it to Shell Craft via **one** of the following methods.
 
 ### Option 1 (Recommended) - Configuration file:
 
-Create a file named `config.json`:
+shell-craft looks for a configuration file in the following places, in order:
+  - the current directory, named config.json
+  - the file named by $SHELLCRAFT_CONFIG
+  - $XDG_CONFIG_HOME/shell-craft/config.json
+  - $HOME/.config/shell-craft/config.json
+
+The contents are simple json:
 ```
 {
     "openai_api_key": "<your secret key>"
 }
 ```
 
 Now, Shell Craft will know your API key in order to run future prompts without having to specify it or ensure it exists in the environmental variables.
```

### Comparing `openai_shell_craft-0.4.0/openai_shell_craft.egg-info/SOURCES.txt` & `openai_shell_craft-0.5.4/openai_shell_craft.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 shell_craft/cli/models.py
 shell_craft/cli/parser.py
 shell_craft/cli/prompt.py
 shell_craft/cli/request.py
 shell_craft/factories/__init__.py
 shell_craft/factories/prompt.py
 shell_craft/prompts/__init__.py
-shell_craft/prompts/feature_request.py
 shell_craft/prompts/languages.py
 shell_craft/prompts/prompt.py
+shell_craft/prompts/templates.py
 tests/test_factories.py
```

### Comparing `openai_shell_craft-0.4.0/pyproject.toml` & `openai_shell_craft-0.5.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openai_shell_craft"
-version = "0.4.0"
+version = "0.5.4"
 authors = [
   { name="Johnathan Irvin", email="irvinjohnathan@gmail.com" },
 ]
 description = "Generating shell commands and code using natural language models (OpenAI ChatGPT)."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `openai_shell_craft-0.4.0/shell_craft/__init__.py` & `openai_shell_craft-0.5.4/shell_craft/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/shell_craft/__main__.py` & `openai_shell_craft-0.5.4/shell_craft/__main__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/shell_craft/cli/__init__.py` & `openai_shell_craft-0.5.4/shell_craft/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/shell_craft/cli/help.py` & `openai_shell_craft-0.5.4/shell_craft/cli/help.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/shell_craft/cli/key.py` & `openai_shell_craft-0.5.4/shell_craft/cli/key.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,24 +39,43 @@
     Returns:
         str: The API key.
     """
     api_key = os.environ.get("OPENAI_API_KEY")
     if api_key:
         return api_key
 
-    if not os.path.exists("config.json"):
+    candidates = ["config.json"]
+
+    if 'SHELLCRAFT_CONFIG' in os.environ:
+        candidates.append(os.environ['SHELLCRAFT_CONFIG'])
+
+    config_dir = None
+    if 'XDG_CONFIG_HOME' in os.environ:
+        config_dir = os.path.join(os.environ['XDG_CONFIG_HOME'])
+    elif 'HOME' in os.environ:
+        config_dir = os.path.join(os.environ['HOME'], '.config')
+
+    if config_dir:
+        candidates.append(os.path.join(config_dir, 'shell-craft', 'config.json'))
+
+    filename = None
+    for candidate in candidates:
+        if os.path.exists(candidate):
+            filename = candidate
+            break
+    else:
         raise ValueError("No API key found")
-    
-    with open("config.json") as f:
+
+    with open(filename) as f:
         config = json.load(f)
 
     api_key = config.get("openai_api_key")
     if api_key:
         return api_key
-    
+
     raise ValueError("No API key found")
 
 def add_arguments(parser: ArgumentParser):
     """
     Adds '--api-key' to the parser as an argument. If the argument is not
     provided, the API key is retrieved from the environment variable OPENAI_API_KEY,
     or from the config.json file. If neither are found, a ValueError is raised. The
@@ -68,9 +87,14 @@
     """
     parser.add_argument(
         "--api-key",
         type=str,
         help="The OpenAI API key to use.",
     )
 
-    if not parser.parse_known_args()[0].api_key:
-        parser.set_defaults(api_key=get_api_key())
+    try:
+        if not parser.parse_known_args()[0].api_key:
+            parser.set_defaults(api_key=get_api_key())
+    except ValueError:
+        print("No API key found. Please provide one with the --api-key argument.")
+        parser.print_help()
+        exit(1)
```

### Comparing `openai_shell_craft-0.4.0/shell_craft/cli/language.py` & `openai_shell_craft-0.5.4/shell_craft/cli/language.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/shell_craft/cli/main.py` & `openai_shell_craft-0.5.4/shell_craft/cli/main.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/shell_craft/cli/models.py` & `openai_shell_craft-0.5.4/shell_craft/cli/models.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/shell_craft/cli/parser.py` & `openai_shell_craft-0.5.4/shell_craft/cli/parser.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/shell_craft/cli/prompt.py` & `openai_shell_craft-0.5.4/shell_craft/cli/prompt.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/shell_craft/cli/request.py` & `openai_shell_craft-0.5.4/shell_craft/cli/request.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/shell_craft/factories/__init__.py` & `openai_shell_craft-0.5.4/shell_craft/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/shell_craft/factories/prompt.py` & `openai_shell_craft-0.5.4/shell_craft/factories/prompt.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/shell_craft/prompts/__init__.py` & `openai_shell_craft-0.5.4/shell_craft/prompts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 # LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 # WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-from .feature_request import FEATURE_REQUEST_PROMPT
 from .languages import (BASH_PROMPT, C_PROMPT, C_SHARP_PROMPT, GO_PROMPT,
                         JAVA_PROMPT, JAVASCRIPT_PROMPT, POWERSHELL_PROMPT,
                         PYTHON_PROMPT)
 from .prompt import Prompt
+from .templates import BUG_REPORT_PROMPT, FEATURE_REQUEST_PROMPT
 
 __all__ = [
     "BASH_PROMPT",
+    "BUG_REPORT_PROMPT",
     "C_PROMPT",
     "C_SHARP_PROMPT",
     "GO_PROMPT",
     "JAVA_PROMPT",
     "JAVASCRIPT_PROMPT",
     "FEATURE_REQUEST_PROMPT",
     "POWERSHELL_PROMPT",
```

### Comparing `openai_shell_craft-0.4.0/shell_craft/prompts/feature_request.py` & `openai_shell_craft-0.5.4/shell_craft/prompts/templates.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,21 +25,43 @@
 Fill out this form:
 
 ```
 ---
 name: <Name Of Feature>
 about: <Short Description>
 labels: < Documentation, Enhancement, Question, Bug, etc. >
-
 ---
 
 **Is your feature request related to a problem? Please describe.**
 A clear and concise description of what the problem is. Ex. I'm always frustrated when [...]
 
 **Describe the solution you'd like**
 A clear and concise description of what you want to happen.
 
 **Describe alternatives you've considered**
 A clear and concise description of any alternative solutions or features you've considered.
 ```
-"""
-)
+""")
+
+BUG_REPORT_PROMPT = Prompt(
+    content="""
+Fill out this form with as much detail as possible with the provided information:
+```
+---
+name: <Name Of Bug>
+about: <Short Description>
+labels: < Documentation, Enhancement, Question, Bug, etc. >
+---
+
+**Describe the bug**
+A clear and concise description of what the bug is.
+
+**To Reproduce**
+Steps to reproduce the behavior:
+1. Go to '...'
+2. Click on '....'
+3. Scroll down to '....'
+4. See error
+
+**Expected behavior**
+A clear and concise description of what you expected to happen.
+""")
```

### Comparing `openai_shell_craft-0.4.0/shell_craft/prompts/languages.py` & `openai_shell_craft-0.5.4/shell_craft/prompts/languages.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/shell_craft/prompts/prompt.py` & `openai_shell_craft-0.5.4/shell_craft/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/shell_craft/service.py` & `openai_shell_craft-0.5.4/shell_craft/service.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.4.0/tests/test_factories.py` & `openai_shell_craft-0.5.4/tests/test_factories.py`

 * *Files identical despite different names*

