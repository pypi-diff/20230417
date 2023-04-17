# Comparing `tmp/oai_tools-0.1.2.tar.gz` & `tmp/oai_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oai_tools-0.1.2.tar", last modified: Sun Apr 16 06:42:43 2023, max compression
+gzip compressed data, was "oai_tools-0.1.3.tar", last modified: Mon Apr 17 08:46:34 2023, max compression
```

## Comparing `oai_tools-0.1.2.tar` & `oai_tools-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:42:43.434271 oai_tools-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-16 06:42:29.000000 oai_tools-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-16 06:42:43.434271 oai_tools-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-16 06:42:29.000000 oai_tools-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:42:43.434271 oai_tools-0.1.2/oai_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-16 06:42:29.000000 oai_tools-0.1.2/oai_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-16 06:42:29.000000 oai_tools-0.1.2/oai_tools/cligpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:42:43.434271 oai_tools-0.1.2/oai_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-16 06:42:43.000000 oai_tools-0.1.2/oai_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-16 06:42:43.000000 oai_tools-0.1.2/oai_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 06:42:43.000000 oai_tools-0.1.2/oai_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-16 06:42:43.000000 oai_tools-0.1.2/oai_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-16 06:42:43.000000 oai_tools-0.1.2/oai_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-16 06:42:43.000000 oai_tools-0.1.2/oai_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-16 06:42:29.000000 oai_tools-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 06:42:43.434271 oai_tools-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-16 06:42:29.000000 oai_tools-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:46:34.284471 oai_tools-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-17 08:46:18.000000 oai_tools-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-17 08:46:34.284471 oai_tools-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-17 08:46:18.000000 oai_tools-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:46:34.280471 oai_tools-0.1.3/oai_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-17 08:46:18.000000 oai_tools-0.1.3/oai_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-17 08:46:18.000000 oai_tools-0.1.3/oai_tools/cligpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-17 08:46:18.000000 oai_tools-0.1.3/oai_tools/cligpt_completion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:46:34.284471 oai_tools-0.1.3/oai_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-17 08:46:34.000000 oai_tools-0.1.3/oai_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-17 08:46:34.000000 oai_tools-0.1.3/oai_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:46:34.000000 oai_tools-0.1.3/oai_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-17 08:46:34.000000 oai_tools-0.1.3/oai_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-17 08:46:34.000000 oai_tools-0.1.3/oai_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 08:46:34.000000 oai_tools-0.1.3/oai_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-17 08:46:18.000000 oai_tools-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 08:46:34.284471 oai_tools-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-17 08:46:18.000000 oai_tools-0.1.3/setup.py
```

### Comparing `oai_tools-0.1.2/LICENSE` & `oai_tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oai_tools-0.1.2/PKG-INFO` & `oai_tools-0.1.3/oai_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
-Name: oai_tools
-Version: 0.1.2
+Name: oai-tools
+Version: 0.1.3
 Summary: Collection of useful tools built on top of OpenAI's API
 Home-page: https://github.com/filipgrano/oai_tools/tree/main
 Author: Filip Granö
 Author-email: filip-accounts@grano.me
 License: UNKNOWN
 Description: # OAI Tools
         
         This repository contains a collection of useful tools built on top of OpenAI's API. These tools can help automate various tasks and provide assistance through natural language processing.
         
         ## Installation or Upgrade
         `pip install --upgrade oai-tools`
         
         ## Tools
         
-        1. **cligpt**: A command-line helper that takes a user prompt and returns shell commands, along with explanations of what they do. See [cligpt.md](doc/cligpt.md) for more details.
+        1. **cligpt**: A command-line helper that takes a user prompt and returns shell commands, along with explanations of what they do. It also supports command completions for various shells. See [cligpt.md](doc/cligpt.md) for more details.
         
         ## Configuration
         Configuration file is read from `~/.config/oai_tools/config.yaml` file. See the [config-example.yaml](doc/config-example.yaml) file for more details.
         
         ### API Key
         OpenAI's API key is required. 
         The key is read from the `OPENAI_API_KEY` environment variable. If this variable is not set, the API key is read from the `~/.config/oai_tools/api_key` file.
```

### Comparing `oai_tools-0.1.2/README.md` & `oai_tools-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This repository contains a collection of useful tools built on top of OpenAI's API. These tools can help automate various tasks and provide assistance through natural language processing.
 
 ## Installation or Upgrade
 `pip install --upgrade oai-tools`
 
 ## Tools
 
-1. **cligpt**: A command-line helper that takes a user prompt and returns shell commands, along with explanations of what they do. See [cligpt.md](doc/cligpt.md) for more details.
+1. **cligpt**: A command-line helper that takes a user prompt and returns shell commands, along with explanations of what they do. It also supports command completions for various shells. See [cligpt.md](doc/cligpt.md) for more details.
 
 ## Configuration
 Configuration file is read from `~/.config/oai_tools/config.yaml` file. See the [config-example.yaml](doc/config-example.yaml) file for more details.
 
 ### API Key
 OpenAI's API key is required. 
 The key is read from the `OPENAI_API_KEY` environment variable. If this variable is not set, the API key is read from the `~/.config/oai_tools/api_key` file.
```

### Comparing `oai_tools-0.1.2/oai_tools/__init__.py` & `oai_tools-0.1.3/oai_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `oai_tools-0.1.2/oai_tools/cligpt.py` & `oai_tools-0.1.3/oai_tools/cligpt.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 LOG_LEVEL = cligpt_config.get("loglevel", "INFO")
 logging.basicConfig(level=logging.getLevelName(LOG_LEVEL))
 
 MODEL = cligpt_config.get("model", "gpt-3.5-turbo")
 AUTO_EXPLAIN = cligpt_config.get("auto_explain", False)
 MAX_TOKENS_COMMAND = cligpt_config.get("max_tokens", {}).get("command", 100)
 MAX_TOKENS_EXPLANATION = cligpt_config.get("max_tokens", {}).get("explanation", 100)
-TEMPERATURE_COMMAND = cligpt_config.get("temperature", {}).get("command", 0.9)
-TEMPERATURE_EXPLANATION = cligpt_config.get("temperature", {}).get("explanation", 0.9)
+TEMPERATURE_COMMAND = cligpt_config.get("temperature", {}).get("command", 0.1)
+TEMPERATURE_EXPLANATION = cligpt_config.get("temperature", {}).get("explanation", 0.1)
 
 
 def get_shell() -> str:
     """Get the default shell for the current platform."""
     system = platform.system()
     if system == "Windows":
         return os.environ.get("COMSPEC", "cmd.exe").strip()
@@ -32,15 +32,15 @@
         return os.environ.get("SHELL", "/bin/bash").strip()
 
     raise ValueError(f"Unsupported platform: {system}")
 
 
 def generate_command(prompt: str) -> openai.ChatCompletion:
     """Generate a shell command using GPT-3.5 based on the given prompt."""
-    query = f"""Write a shell command that works in the following shell: {get_shell()}
+    query = f"""Write a shell command that works on the {platform.system()} platform in the following shell: {os.path.basename(get_shell())}
 
         The command must accomplish this task:
 
         {prompt}
 
         Return ONLY the command, no other explanation, words, code highlighting, or text."""
 
@@ -54,15 +54,15 @@
         n=1,
     )
     return response
 
 
 def explain_command(suggestion: str, prompt: str) -> openai.ChatCompletion:
     """Generate an explanation of a suggested command using GPT-3.5."""
-    query = f"Explain in brief how the command '{suggestion}' works, what it does, and if it's safe to use (why not if not). Also state if it fulfills the requested task '{prompt}' or not. Return the explanation and task fulfillment status in a single line. No other words, code highlighting, or text. Don't repeat the command or the task."
+    query = f"Explain in brief how the command '{suggestion}' works on the {platform.system()} platform in the {os.path.basename(get_shell())} shell, what it does, and if it's safe to use (why not if not). Also state if it fulfills the requested task '{prompt}' or not. Return the explanation and task fulfillment status in a single line. No other words, code highlighting, or text. Don't repeat the command or the task."
 
     logging.debug("Explaining command: %s", suggestion)
 
     response = openai.ChatCompletion.create(
         model=MODEL,
         messages=[{"role": "user", "content": query}],
         max_tokens=MAX_TOKENS_EXPLANATION,
@@ -73,16 +73,23 @@
 
 
 def execute_command(command: str) -> None:
     """Execute a shell command and print its output and errors as they are produced."""
     shell = get_shell()
     logging.debug("Executing shell command in shell %s: %s", shell, command)
 
-    command = command.replace('"', r"\"")
-    command = f'{shell} -c "{command}" '
+    if platform.system() == "Windows":
+        if "powershell" in shell.lower():
+            command = f'powershell.exe -Command "& {{ {command} }}"'
+        else:
+            command = f'cmd.exe /C "{command}"'
+    else:
+        command = command.replace('"', r"\"")
+        command = f'{shell} -c "{command}"'
+
     return_code = os.system(command)
 
     logging.debug("Shell command results -- return code: %s", return_code)
 
 
 def main():
     try:
```

### Comparing `oai_tools-0.1.2/oai_tools.egg-info/PKG-INFO` & `oai_tools-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
-Name: oai-tools
-Version: 0.1.2
+Name: oai_tools
+Version: 0.1.3
 Summary: Collection of useful tools built on top of OpenAI's API
 Home-page: https://github.com/filipgrano/oai_tools/tree/main
 Author: Filip Granö
 Author-email: filip-accounts@grano.me
 License: UNKNOWN
 Description: # OAI Tools
         
         This repository contains a collection of useful tools built on top of OpenAI's API. These tools can help automate various tasks and provide assistance through natural language processing.
         
         ## Installation or Upgrade
         `pip install --upgrade oai-tools`
         
         ## Tools
         
-        1. **cligpt**: A command-line helper that takes a user prompt and returns shell commands, along with explanations of what they do. See [cligpt.md](doc/cligpt.md) for more details.
+        1. **cligpt**: A command-line helper that takes a user prompt and returns shell commands, along with explanations of what they do. It also supports command completions for various shells. See [cligpt.md](doc/cligpt.md) for more details.
         
         ## Configuration
         Configuration file is read from `~/.config/oai_tools/config.yaml` file. See the [config-example.yaml](doc/config-example.yaml) file for more details.
         
         ### API Key
         OpenAI's API key is required. 
         The key is read from the `OPENAI_API_KEY` environment variable. If this variable is not set, the API key is read from the `~/.config/oai_tools/api_key` file.
```

### Comparing `oai_tools-0.1.2/pyproject.toml` & `oai_tools-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oai_tools-0.1.2/setup.py` & `oai_tools-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="oai_tools",
-    version="0.1.2",
+    version="0.1.3",
     author="Filip Granö",
     author_email="filip-accounts@grano.me",
     description="Collection of useful tools built on top of OpenAI's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/filipgrano/oai_tools/tree/main",
     packages=find_packages(),
     install_requires=["openai>=0.27.0", "PyYAML", "types-PyYAML"],
     entry_points={
-        "console_scripts": [
-            "cligpt=oai_tools.cligpt:main",
-        ],
+        "console_scripts": ["cligpt=oai_tools.cligpt:main", "cligpt_completion=oai_tools.cligpt_completion:main"],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

