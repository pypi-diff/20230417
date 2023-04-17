# Comparing `tmp/symeo-python-0.0.4.tar.gz` & `tmp/symeo-python-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symeo-python-0.0.4.tar", last modified: Mon Feb 27 13:16:03 2023, max compression
+gzip compressed data, was "symeo-python-0.0.5.tar", last modified: Mon Apr 17 08:35:34 2023, max compression
```

## Comparing `symeo-python-0.0.4.tar` & `symeo-python-0.0.5.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 ilysse     (501) staff       (20)        0 2023-02-27 13:16:03.842359 symeo-python-0.0.4/
--rw-r--r--   0 ilysse     (501) staff       (20)      245 2023-02-27 13:16:03.842081 symeo-python-0.0.4/PKG-INFO
--rw-r--r--   0 ilysse     (501) staff       (20)     4812 2023-02-17 08:58:44.000000 symeo-python-0.0.4/README.md
--rw-r--r--   0 ilysse     (501) staff       (20)      324 2023-02-13 12:53:47.000000 symeo-python-0.0.4/pyproject.toml
--rw-r--r--   0 ilysse     (501) staff       (20)       38 2023-02-27 13:16:03.842449 symeo-python-0.0.4/setup.cfg
--rw-r--r--   0 ilysse     (501) staff       (20)      601 2023-02-27 10:43:00.000000 symeo-python-0.0.4/setup.py
-drwxr-xr-x   0 ilysse     (501) staff       (20)        0 2023-02-27 13:16:03.829167 symeo-python-0.0.4/symeo_python/
--rw-r--r--   0 ilysse     (501) staff       (20)        0 2023-01-30 16:01:48.000000 symeo-python-0.0.4/symeo_python/__init__.py
-drwxr-xr-x   0 ilysse     (501) staff       (20)        0 2023-02-27 13:16:03.832263 symeo-python-0.0.4/symeo_python/api_client/
--rw-r--r--   0 ilysse     (501) staff       (20)        0 2023-02-13 13:08:27.000000 symeo-python-0.0.4/symeo_python/api_client/__init__.py
--rw-r--r--   0 ilysse     (501) staff       (20)      628 2023-02-27 13:15:38.000000 symeo-python-0.0.4/symeo_python/api_client/symeo_api_client.py
-drwxr-xr-x   0 ilysse     (501) staff       (20)        0 2023-02-27 13:16:03.834750 symeo-python-0.0.4/symeo_python/cli/
--rw-r--r--   0 ilysse     (501) staff       (20)        0 2023-02-04 15:04:29.000000 symeo-python-0.0.4/symeo_python/cli/__init__.py
--rw-r--r--   0 ilysse     (501) staff       (20)     1442 2023-02-13 13:40:56.000000 symeo-python-0.0.4/symeo_python/cli/cli.py
--rw-r--r--   0 ilysse     (501) staff       (20)      501 2023-02-13 13:17:40.000000 symeo-python-0.0.4/symeo_python/cli/main.py
--rw-r--r--   0 ilysse     (501) staff       (20)      273 2023-02-13 12:03:34.000000 symeo-python-0.0.4/symeo_python/cli/process_runner.py
--rw-r--r--   0 ilysse     (501) staff       (20)     2113 2023-02-27 10:42:44.000000 symeo-python-0.0.4/symeo_python/cli/symeo_python_cli.py
--rw-r--r--   0 ilysse     (501) staff       (20)      294 2023-02-13 13:17:14.000000 symeo-python-0.0.4/symeo_python/config.py
-drwxr-xr-x   0 ilysse     (501) staff       (20)        0 2023-02-27 13:16:03.837208 symeo-python-0.0.4/symeo_python/configuration/
--rw-r--r--   0 ilysse     (501) staff       (20)        0 2023-01-30 16:17:39.000000 symeo-python-0.0.4/symeo_python/configuration/__init__.py
--rw-r--r--   0 ilysse     (501) staff       (20)     1651 2023-02-17 10:32:51.000000 symeo-python-0.0.4/symeo_python/configuration/config_loader.py
--rw-r--r--   0 ilysse     (501) staff       (20)     1720 2023-02-13 13:07:35.000000 symeo-python-0.0.4/symeo_python/configuration/config_parser.py
--rw-r--r--   0 ilysse     (501) staff       (20)       62 2023-02-13 10:57:41.000000 symeo-python-0.0.4/symeo_python/configuration/configuration.py
-drwxr-xr-x   0 ilysse     (501) staff       (20)        0 2023-02-27 13:16:03.838173 symeo-python-0.0.4/symeo_python/yaml_converter/
--rw-r--r--   0 ilysse     (501) staff       (20)        0 2023-02-01 05:15:20.000000 symeo-python-0.0.4/symeo_python/yaml_converter/__init__.py
--rw-r--r--   0 ilysse     (501) staff       (20)     3492 2023-02-15 12:35:58.000000 symeo-python-0.0.4/symeo_python/yaml_converter/yaml_to_class_converter.py
-drwxr-xr-x   0 ilysse     (501) staff       (20)        0 2023-02-27 13:16:03.831700 symeo-python-0.0.4/symeo_python.egg-info/
--rw-r--r--   0 ilysse     (501) staff       (20)      245 2023-02-27 13:16:03.000000 symeo-python-0.0.4/symeo_python.egg-info/PKG-INFO
--rw-r--r--   0 ilysse     (501) staff       (20)     1020 2023-02-27 13:16:03.000000 symeo-python-0.0.4/symeo_python.egg-info/SOURCES.txt
--rw-r--r--   0 ilysse     (501) staff       (20)        1 2023-02-27 13:16:03.000000 symeo-python-0.0.4/symeo_python.egg-info/dependency_links.txt
--rw-r--r--   0 ilysse     (501) staff       (20)       59 2023-02-27 13:16:03.000000 symeo-python-0.0.4/symeo_python.egg-info/entry_points.txt
--rw-r--r--   0 ilysse     (501) staff       (20)       27 2023-02-27 13:16:03.000000 symeo-python-0.0.4/symeo_python.egg-info/requires.txt
--rw-r--r--   0 ilysse     (501) staff       (20)       18 2023-02-27 13:16:03.000000 symeo-python-0.0.4/symeo_python.egg-info/top_level.txt
-drwxr-xr-x   0 ilysse     (501) staff       (20)        0 2023-02-27 13:16:03.827111 symeo-python-0.0.4/test/
-drwxr-xr-x   0 ilysse     (501) staff       (20)        0 2023-02-27 13:16:03.839756 symeo-python-0.0.4/test/cli/
--rw-r--r--   0 ilysse     (501) staff       (20)        0 2023-02-04 15:51:09.000000 symeo-python-0.0.4/test/cli/__init__.py
--rw-r--r--   0 ilysse     (501) staff       (20)     3651 2023-02-13 13:41:59.000000 symeo-python-0.0.4/test/cli/cli_test.py
--rw-r--r--   0 ilysse     (501) staff       (20)     4296 2023-02-13 17:11:30.000000 symeo-python-0.0.4/test/cli/symeo_python_cli_test.py
-drwxr-xr-x   0 ilysse     (501) staff       (20)        0 2023-02-27 13:16:03.840648 symeo-python-0.0.4/test/config/
--rw-r--r--   0 ilysse     (501) staff       (20)        0 2023-01-30 16:15:33.000000 symeo-python-0.0.4/test/config/__init__.py
--rw-r--r--   0 ilysse     (501) staff       (20)     2213 2023-02-13 13:16:56.000000 symeo-python-0.0.4/test/config/configuration_parser_test.py
-drwxr-xr-x   0 ilysse     (501) staff       (20)        0 2023-02-27 13:16:03.841498 symeo-python-0.0.4/test/yaml_converter/
--rw-r--r--   0 ilysse     (501) staff       (20)        0 2023-02-01 05:21:32.000000 symeo-python-0.0.4/test/yaml_converter/__init__.py
--rw-r--r--   0 ilysse     (501) staff       (20)     3361 2023-02-13 13:16:48.000000 symeo-python-0.0.4/test/yaml_converter/yaml_to_class_converter_test.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:34.366193 symeo-python-0.0.5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      245 2023-04-17 08:35:34.366193 symeo-python-0.0.5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4789 2023-04-17 08:35:13.000000 symeo-python-0.0.5/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      324 2023-04-17 08:35:13.000000 symeo-python-0.0.5/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-17 08:35:34.366193 symeo-python-0.0.5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-04-17 08:35:13.000000 symeo-python-0.0.5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:34.362193 symeo-python-0.0.5/symeo_python/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:34.362193 symeo-python-0.0.5/symeo_python/api_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/api_client/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      628 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/api_client/symeo_api_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:34.362193 symeo-python-0.0.5/symeo_python/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2523 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/cli/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      704 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/cli/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      273 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/cli/process_runner.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3110 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/cli/symeo_python_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      294 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:34.366193 symeo-python-0.0.5/symeo_python/configuration/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/configuration/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1651 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/configuration/config_loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1720 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/configuration/config_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6872 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/configuration/config_validator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/configuration/configuration.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:34.366193 symeo-python-0.0.5/symeo_python/yaml_converter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/yaml_converter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4143 2023-04-17 08:35:13.000000 symeo-python-0.0.5/symeo_python/yaml_converter/yaml_to_class_converter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:34.362193 symeo-python-0.0.5/symeo_python.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      245 2023-04-17 08:35:34.000000 symeo-python-0.0.5/symeo_python.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1111 2023-04-17 08:35:34.000000 symeo-python-0.0.5/symeo_python.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-17 08:35:34.000000 symeo-python-0.0.5/symeo_python.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-04-17 08:35:34.000000 symeo-python-0.0.5/symeo_python.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2023-04-17 08:35:34.000000 symeo-python-0.0.5/symeo_python.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2023-04-17 08:35:34.000000 symeo-python-0.0.5/symeo_python.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:34.362193 symeo-python-0.0.5/test/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:34.366193 symeo-python-0.0.5/test/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:13.000000 symeo-python-0.0.5/test/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4133 2023-04-17 08:35:13.000000 symeo-python-0.0.5/test/cli/cli_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4296 2023-04-17 08:35:13.000000 symeo-python-0.0.5/test/cli/symeo_python_cli_test.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:34.366193 symeo-python-0.0.5/test/config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:13.000000 symeo-python-0.0.5/test/config/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2213 2023-04-17 08:35:13.000000 symeo-python-0.0.5/test/config/configuration_parser_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8799 2023-04-17 08:35:13.000000 symeo-python-0.0.5/test/config/configuration_validator_test.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:34.366193 symeo-python-0.0.5/test/yaml_converter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-17 08:35:13.000000 symeo-python-0.0.5/test/yaml_converter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4032 2023-04-17 08:35:13.000000 symeo-python-0.0.5/test/yaml_converter/yaml_to_class_converter_test.py
```

### Comparing `symeo-python-0.0.4/README.md` & `symeo-python-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
 ```shell
 $ symeo-python start -f symeo.local.yml -- $your_command_to_start_your_application
 ```
 
 ### Start application with configuration from Symeo platform
 
-After creating an environment and its api key in the [Symeo platform](https://app-config-staging.symeo.io/), run
+After creating an environment and its api key in the [Symeo platform](https://app.symeo.io/), run
 
 ```shell
 $ symeo-python start -k $YOUR_ENVIRONMENT_API_KEY -- uvicorn main:app
 ```
 
 So the sdk fetch the values for the given environment and starts your application with those values.
 
@@ -187,15 +187,15 @@
 
 `-k, --api-key`
 
 The environment api key to use to fetch values from Symeo platform. If empty, values will be fetched from local value file (`symeo.local.yml` by default). If specified, parameter `-f, --values-file` is ignored.
 
 `-a, --api-url`
 
-The api endpoint used to fetch your configuration with the api key. Default is `https://api-staging.symeo.io/api/v1/values`.
+The api endpoint used to fetch your configuration with the api key. Default is `https://api.symeo.io/api/v1/values`.
 
 
 # Help
 
 To get some help with the CLI, please use the following commands :
 
 `symeo-python build --help`
```

### Comparing `symeo-python-0.0.4/setup.py` & `symeo-python-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # type: ignore
 
 setup(
     name="symeo-python",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(exclude=["test"]),
     install_requires=["pyyaml", "typer[all]", "requests"],
     license="Apache-2.0 license",
     extra_require={},
     url="https://github.com/symeo-io/symeo-python",
     author="Symeo.io",
     author_email="support@symeo.io",
```

### Comparing `symeo-python-0.0.4/symeo_python/api_client/symeo_api_client.py` & `symeo-python-0.0.5/symeo_python/api_client/symeo_api_client.py`

 * *Files identical despite different names*

### Comparing `symeo-python-0.0.4/symeo_python/cli/cli.py` & `symeo-python-0.0.5/symeo_python/cli/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,65 @@
 import os
+from typing import List
+
+import typer
+from rich.console import Console
+from rich.table import Table
 
 from symeo_python.cli.process_runner import ProcessRunnerPort
 from symeo_python.configuration.config_loader import (
     SYMEO_API_KEY,
     SYMEO_LOCAL_FILE,
     SYMEO_API_URL,
 )
 from symeo_python.configuration.config_parser import ConfigParserPort
+from symeo_python.configuration.config_validator import ConfigValidatorPort
 
 
 class CliPort:
     def generate_configuration_from_contract_file(self, config_contract: str):
         pass
 
+    def prepare_env_and_start_validation(self, config_contract: str, cli_input_data: dict):
+        pass
+
     def prepare_env_and_start_sub_process(self, cli_input_data: dict):
         pass
 
 
 class DefaultCliAdapter(CliPort):
     def __init__(
-        self, conf_parser_port: ConfigParserPort, process_runner_port: ProcessRunnerPort
+            self, conf_parser_port: ConfigParserPort, config_validator_port: ConfigValidatorPort,
+            process_runner_port: ProcessRunnerPort
     ):
         self.__conf_parser_port = conf_parser_port
+        self.__config_validator_port = config_validator_port
         self.__process_runner_port = process_runner_port
 
     def generate_configuration_from_contract_file(self, config_contract: str):
         self.__conf_parser_port.generate_configuration(config_contract)
 
+    def prepare_env_and_start_validation(self, config_contract: str, cli_input_data: dict):
+        self.__prepare_env(cli_input_data)
+        errors: List[str] = self.__config_validator_port.validate_config_from_env(config_contract)
+        if len(errors) > 0:
+            console = Console()
+            table = Table("N°", "Error", show_lines=True)
+            for error in errors:
+                table.add_row(str(errors.index(error) + 1), error)
+            console.print(table)
+            exit(1)
+        print("Configuration values matching contract")
+
     def prepare_env_and_start_sub_process(self, cli_input_data: dict):
+        self.__prepare_env(cli_input_data)
+        self.__process_runner_port.run_process(cli_input_data["sub_process"])
+
+    @staticmethod
+    def __prepare_env(cli_input_data: dict) -> None:
         if "api_key" in cli_input_data and "api_url" in cli_input_data:
             os.environ[SYMEO_API_KEY] = cli_input_data["api_key"]
             os.environ[SYMEO_API_URL] = cli_input_data["api_url"]
         elif "config_values_path" in cli_input_data:
             os.environ[SYMEO_LOCAL_FILE] = cli_input_data["config_values_path"]
         else:
             raise Exception("Missing api_key/api_url or config_values_path")
-        self.__process_runner_port.run_process(cli_input_data["sub_process"])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `symeo-python-0.0.4/symeo_python/cli/symeo_python_cli.py` & `symeo-python-0.0.5/symeo_python/cli/symeo_python_cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from pathlib import Path
 from typing import List
 
+import typer
 from typer import Option, Typer  # type: ignore
 
 from symeo_python.cli.cli import CliPort
 
 DEFAULT_CONFIG_CONTRACT_PATH = "./symeo.config.yml"
 DEFAULT_CONFIG_VALUES_PATH = "./symeo.local.yml"
 DEFAULT_SYMEO_API_URL = "https://api.symeo.io/api/v1/values"
@@ -14,46 +15,67 @@
 class SymeoPythonCli:
     __cli_port: CliPort
 
     def __init__(self, cli_port: CliPort):
         self.__cli_port = cli_port
 
     def load_commands(
-        self,
+            self,
     ) -> Typer:
         cli = Typer()
 
         def generate_config(config_contract):
             config_contract_path: Path = Path(os.getcwd()) / config_contract
             print(
                 f"Starting to generate Config class from configuration contract {config_contract_path}"
             )
             self.__cli_port.generate_configuration_from_contract_file(
                 str(config_contract_path)
             )
 
         @cli.command()
         def build(
-            config_contract: str = Option(
-                DEFAULT_CONFIG_CONTRACT_PATH, "--config-contract", "-c"
-            )
+                config_contract: str = Option(
+                    DEFAULT_CONFIG_CONTRACT_PATH, "--config-contract", "-c"
+                )
+        ):
+            generate_config(config_contract)
+
+        @cli.command()
+        def validate(
+                api_key: str = Option("", "--api-key", "-k"),
+                api_url: str = Option(DEFAULT_SYMEO_API_URL, "--api-url", "-a"),
+                config_values: str = Option(
+                    DEFAULT_CONFIG_VALUES_PATH, "--config-values", "-f"
+                ),
+                config_contract: str = Option(
+                    DEFAULT_CONFIG_CONTRACT_PATH, "--config-contract", "-c"
+                ),
         ):
             generate_config(config_contract)
+            config_values_path: Path = Path(os.getcwd()) / config_values
+            cli_input_data = {
+                "config_values_path": str(config_values_path),
+            }
+            if api_key != "":
+                cli_input_data["api_key"] = api_key
+                cli_input_data["api_url"] = api_url
+            self.__cli_port.prepare_env_and_start_validation(config_contract, cli_input_data)
 
         @cli.command()
         def start(
-            sub_process: List[str],
-            api_key: str = Option("", "--api-key", "-k"),
-            api_url: str = Option(DEFAULT_SYMEO_API_URL, "--api-url", "-a"),
-            config_values: str = Option(
-                DEFAULT_CONFIG_VALUES_PATH, "--config-values", "-f"
-            ),
-            config_contract: str = Option(
-                DEFAULT_CONFIG_CONTRACT_PATH, "--config-contract", "-c"
-            ),
+                sub_process: List[str],
+                api_key: str = Option("", "--api-key", "-k"),
+                api_url: str = Option(DEFAULT_SYMEO_API_URL, "--api-url", "-a"),
+                config_values: str = Option(
+                    DEFAULT_CONFIG_VALUES_PATH, "--config-values", "-f"
+                ),
+                config_contract: str = Option(
+                    DEFAULT_CONFIG_CONTRACT_PATH, "--config-contract", "-c"
+                ),
         ):
             generate_config(config_contract)
             config_values_path: Path = Path(os.getcwd()) / config_values
             cli_input_data = {
                 "config_values_path": str(config_values_path),
                 "sub_process": sub_process,
             }
```

### Comparing `symeo-python-0.0.4/symeo_python/configuration/config_loader.py` & `symeo-python-0.0.5/symeo_python/configuration/config_loader.py`

 * *Files identical despite different names*

### Comparing `symeo-python-0.0.4/symeo_python/configuration/config_parser.py` & `symeo-python-0.0.5/symeo_python/configuration/config_parser.py`

 * *Files identical despite different names*

### Comparing `symeo-python-0.0.4/symeo_python/yaml_converter/yaml_to_class_converter.py` & `symeo-python-0.0.5/symeo_python/yaml_converter/yaml_to_class_converter.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,64 +6,68 @@
 
 class YamlToClassPort:
     def parse_configuration_from_path(self, configuration_path):
         pass
 
 
 class YamlToClassAdapter(YamlToClassPort):
-
     __target_file_path: str
     __ROOT_CONFIG_CLASS_NAME = "Config"
     __TAB = "    "
 
     def __init__(
-        self,
-        target_file_path: str = f"{os.path.dirname(os.path.abspath(__file__))}/../configuration/configuration.py",
+            self,
+            target_file_path: str = f"{os.path.dirname(os.path.abspath(__file__))}/../configuration/configuration.py",
     ):
         self.__target_file_path = target_file_path
 
     def parse_configuration_from_path(self, configuration_path):
         with open(configuration_path, "r") as yaml_file:
             yaml_data = yaml.load(yaml_file, Loader=yaml.FullLoader)
             class_definition = self.__yaml_data_to_class_with_mapping_methods(
                 yaml_data, self.__ROOT_CONFIG_CLASS_NAME, []
             )
             with open(self.__target_file_path, "w") as file:
                 print(f"Writing conf from contract to {configuration_path}")
                 file.write(class_definition)
 
     def __yaml_data_to_class_with_mapping_methods(
-        self, yaml_data: dict, class_name: str, nested_classes: List[str]
+            self, yaml_data: dict, class_name: str, nested_classes: List[str]
     ) -> str:
         attribute = ""
         constructor = f"{self.__TAB}def __init__(self, yaml_data):\n"
         (
             attribute,
             constructor,
         ) = self.__yaml_data_to_attribute_constructor_and_nested_classes(
             attribute, constructor, nested_classes, yaml_data
         )
         conf_class = ""
         if class_name == self.__ROOT_CONFIG_CLASS_NAME:
-            python_conf_file_content = ""
+            python_conf_file_content = "from typing import Optional\n\n\n"
             for nested_classe in nested_classes:
                 python_conf_file_content += f"{nested_classe}\n\n"
             conf_class = python_conf_file_content
         conf_class += f"class {class_name}:\n{attribute}\n{constructor}"
         return conf_class
 
     def __yaml_data_to_attribute_constructor_and_nested_classes(
-        self, attribute, constructor, nested_classes, yaml_data
+            self, attribute, constructor, nested_classes, yaml_data
     ):
         for key in yaml_data:
             attribute_name = str(key).replace("-", "_")
             if "type" in yaml_data[key]:
-                constructor += f'{self.__TAB}{self.__TAB}self.{attribute_name} = yaml_data["{key}"]\n'
                 type = self.__get_type(yaml_data[key]["type"])
-                attribute += f"{self.__TAB}{attribute_name}: {type}\n"
+                optional = self.__get_optional(yaml_data[key])
+                if optional:
+                    constructor += f'{self.__TAB}{self.__TAB}self.{attribute_name} = yaml_data.get("{key}")\n'
+                    attribute += f"{self.__TAB}{attribute_name}: Optional[{type}]\n"
+                else:
+                    constructor += f'{self.__TAB}{self.__TAB}self.{attribute_name} = yaml_data["{key}"]\n'
+                    attribute += f"{self.__TAB}{attribute_name}: {type}\n"
             else:
                 nested_class_name = self.__get_camel_cased_class_name(key)
                 constructor += f'{self.__TAB}{self.__TAB}self.{attribute_name} = {nested_class_name}(yaml_data["{key}"])\n'
                 nested_classes.append(
                     self.__yaml_data_to_class_with_mapping_methods(
                         yaml_data[key], nested_class_name, nested_classes
                     )
@@ -83,8 +87,17 @@
 
     @staticmethod
     def __get_type(type: str) -> str:
         if type == "string":
             return "str"
         elif type == "integer":
             return "int"
+        elif type == "float":
+            return "float"
+        elif type == "boolean":
+            return "bool"
         raise Exception(f"Wrong type {type}")
+
+    @staticmethod
+    def __get_optional(key_attribute: dict) -> bool:
+        optional: bool = key_attribute.get("optional")
+        return True if optional else False
```

### Comparing `symeo-python-0.0.4/symeo_python.egg-info/SOURCES.txt` & `symeo-python-0.0.5/symeo_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 symeo_python/cli/cli.py
 symeo_python/cli/main.py
 symeo_python/cli/process_runner.py
 symeo_python/cli/symeo_python_cli.py
 symeo_python/configuration/__init__.py
 symeo_python/configuration/config_loader.py
 symeo_python/configuration/config_parser.py
+symeo_python/configuration/config_validator.py
 symeo_python/configuration/configuration.py
 symeo_python/yaml_converter/__init__.py
 symeo_python/yaml_converter/yaml_to_class_converter.py
 test/cli/__init__.py
 test/cli/cli_test.py
 test/cli/symeo_python_cli_test.py
 test/config/__init__.py
 test/config/configuration_parser_test.py
+test/config/configuration_validator_test.py
 test/yaml_converter/__init__.py
 test/yaml_converter/yaml_to_class_converter_test.py
```

### Comparing `symeo-python-0.0.4/test/cli/cli_test.py` & `symeo-python-0.0.5/test/cli/cli_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,36 +2,39 @@
 import unittest
 from typing import List
 
 from symeo_python.cli.cli import DefaultCliAdapter
 from symeo_python.cli.process_runner import ProcessRunnerPort
 from symeo_python.configuration.config_loader import SYMEO_LOCAL_FILE, SYMEO_API_KEY
 from symeo_python.configuration.config_parser import ConfigParserPort
+from symeo_python.configuration.config_validator import ConfigValidatorPort
 
 
 class CliTest(unittest.TestCase):
     def test_should_parse_conf_from_yaml(self):
         # Given
         conf_parser_mock = ConfigParserAdapterMock()
+        conf_validate_mock = ConfigValidatorAdapterMock()
         process_runner_adapter_mock = ProcessRunnerAdapterMock()
-        cli_adapter = DefaultCliAdapter(conf_parser_mock, process_runner_adapter_mock)
+        cli_adapter = DefaultCliAdapter(conf_parser_mock, conf_validate_mock, process_runner_adapter_mock)
         contract_path = "fake/config/contract/path"
 
         # When
         cli_adapter.generate_configuration_from_contract_file(contract_path)
 
         # Then
         self.assertEqual(contract_path, conf_parser_mock.configuration_path)
         self.assertIsNone(process_runner_adapter_mock.process)
 
     def test_should_prepare_env_with_api_key_and_run_sub_process(self):
         # Given
-        conf_parser_mock = ConfigParserAdapterMock()
+        config_parser_mock = ConfigParserAdapterMock()
+        config_validator_mock = ConfigValidatorAdapterMock()
         process_runner_adapter_mock = ProcessRunnerAdapterMock()
-        cli_adapter = DefaultCliAdapter(conf_parser_mock, process_runner_adapter_mock)
+        cli_adapter = DefaultCliAdapter(config_parser_mock, config_validator_mock, process_runner_adapter_mock)
         api_key = "FAKE_API_KEY_111"
         api_url = "http://fake.111"
         sub_process = ["echo", "'Test1'"]
         cli_input_data = {
             "api_key": api_key,
             "api_url": api_url,
             "sub_process": sub_process,
@@ -42,17 +45,18 @@
 
         # Then
         self.assertEqual(sub_process, process_runner_adapter_mock.process)
         self.assertEqual(api_key, os.getenv(SYMEO_API_KEY))
 
     def test_should_prepare_env_with_local_file_and_run_sub_process(self):
         # Given
-        conf_parser_mock = ConfigParserAdapterMock()
+        config_parser_mock = ConfigParserAdapterMock()
+        config_validate_mock = ConfigValidatorAdapterMock()
         process_runner_adapter_mock = ProcessRunnerAdapterMock()
-        cli_adapter = DefaultCliAdapter(conf_parser_mock, process_runner_adapter_mock)
+        cli_adapter = DefaultCliAdapter(config_parser_mock, config_validate_mock, process_runner_adapter_mock)
         config_values_path = "./fake_local_file_111.yml"
         api_url = "http://fake.111"
         sub_process = ["echo", "'Test2'"]
         cli_input_data = {
             "config_values_path": config_values_path,
             "api_url": api_url,
             "sub_process": sub_process,
@@ -63,17 +67,18 @@
 
         # Then
         self.assertEqual(sub_process, process_runner_adapter_mock.process)
         self.assertEqual(config_values_path, os.getenv(SYMEO_LOCAL_FILE))
 
     def test_should_raise_exception_for_missing_cli_input_data(self):
         # Given
-        conf_parser_mock = ConfigParserAdapterMock()
+        config_parser_mock = ConfigParserAdapterMock()
+        config_validator_mock = ConfigValidatorAdapterMock()
         process_runner_adapter_mock = ProcessRunnerAdapterMock()
-        cli_adapter = DefaultCliAdapter(conf_parser_mock, process_runner_adapter_mock)
+        cli_adapter = DefaultCliAdapter(config_parser_mock, config_validator_mock, process_runner_adapter_mock)
         sub_process = ["echo", "'Test2'"]
         cli_input_data = {
             "sub_process": sub_process,
         }
 
         # When
         exception = None
@@ -92,12 +97,16 @@
 
     process: str = None
 
     def run_process(self, process: List[str]) -> None:
         self.process = process
 
 
+class ConfigValidatorAdapterMock(ConfigValidatorPort):
+    pass
+
+
 class ConfigParserAdapterMock(ConfigParserPort):
     configuration_path: str
 
     def generate_configuration(self, configuration_path: str) -> None:
         self.configuration_path = configuration_path
```

### Comparing `symeo-python-0.0.4/test/cli/symeo_python_cli_test.py` & `symeo-python-0.0.5/test/cli/symeo_python_cli_test.py`

 * *Files identical despite different names*

### Comparing `symeo-python-0.0.4/test/config/configuration_parser_test.py` & `symeo-python-0.0.5/test/config/configuration_parser_test.py`

 * *Files identical despite different names*

### Comparing `symeo-python-0.0.4/test/yaml_converter/yaml_to_class_converter_test.py` & `symeo-python-0.0.5/test/yaml_converter/yaml_to_class_converter_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # import yaml  # type: ignore
 
 from symeo_python.configuration.config_parser import ConfigParserAdapter
 from symeo_python.yaml_converter.yaml_to_class_converter import YamlToClassAdapter
 
 
 class YamlToClassConverterTest(unittest.TestCase):
-
     __temp_dir: str
     __current_absolute_path = os.path.dirname(os.path.abspath(__file__))
 
     def setUp(self) -> None:
         self.__temp_dir = tempfile.mkdtemp()
 
     def tearDown(self) -> None:
@@ -32,19 +31,31 @@
         )
         self.__assert_generated_python_file_equals_expected_python_file(
             "simple_yaml_2.yml", "simple_yaml_2.py"
         )
         self.__assert_generated_python_file_equals_expected_python_file(
             "simple_yaml_with_two_attributes.yml", "simple_yaml_with_two_attributes.py"
         )
+        self.__assert_generated_python_file_equals_expected_python_file(
+            "simple_yaml_with_every_conf_type.yml", "simple_yaml_with_every_conf_type.py"
+        )
+        self.__assert_generated_python_file_equals_expected_python_file(
+            "simple_yaml_with_optional.yml", "simple_yaml_with_optional.py"
+        )
 
     def test_should_convert_complex_yaml_files(self):
         self.__assert_generated_python_file_equals_expected_python_file(
             "yaml_with_nested_conf.yml", "yaml_with_nested_conf.py"
         )
+        self.__assert_generated_python_file_equals_expected_python_file(
+            "complex_yaml_with_every_conf_type.yml", "complex_yaml_with_every_conf_type.py"
+        )
+        self.__assert_generated_python_file_equals_expected_python_file(
+            "complex_yaml_with_optional.yml", "complex_yaml_with_optional.py"
+        )
 
     def test_should_convert_complex_name(self):
         self.__assert_generated_python_file_equals_expected_python_file(
             "yaml_with_complex_name.yml", "yaml_with_complex_name.py"
         )
         self.__assert_generated_python_file_equals_expected_python_file(
             "complex_yaml_with_complex_class_name.yml",
@@ -64,15 +75,15 @@
                 config.infrastructure.database.mongo_db.url, "http://localhost"
             )
             self.assertEqual(config.infrastructure.database.mongo_db.port, 5132)
             self.assertEqual(config.infrastructure.name, "fake")
             self.assertEqual(config.infrastructure.github.api, "http://github.api.com")
 
     def __assert_generated_python_file_equals_expected_python_file(
-        self, yaml_file_name, python_file_name
+            self, yaml_file_name, python_file_name
     ):
         given_yaml_file = f"{self.__current_absolute_path}/resources/given_contract_yaml_files/{yaml_file_name}"
         target_path = f"{self.__temp_dir}/%s" % python_file_name
         yaml_to_class_converter = YamlToClassAdapter(target_path)
         expected_python_file = f"{self.__current_absolute_path}/resources/expected_python_files/{python_file_name}"
         # When
         yaml_to_class_converter.parse_configuration_from_path(given_yaml_file)
```

