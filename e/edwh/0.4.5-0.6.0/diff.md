# Comparing `tmp/edwh-0.4.5.tar.gz` & `tmp/edwh-0.6.0.tar.gz`

## Comparing `edwh-0.4.5.tar` & `edwh-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 edwh-0.4.5/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh-0.4.5/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.4.5/src/edwh/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.4.5/src/edwh/__init__.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 edwh-0.4.5/src/edwh/cli.py
--rw-r--r--   0        0        0    16612 2020-02-02 00:00:00.000000 edwh-0.4.5/src/edwh/tasks.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.4.5/tests/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 edwh-0.4.5/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.4.5/LICENSE.txt
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 edwh-0.4.5/README.md
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 edwh-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 edwh-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 edwh-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 edwh-0.6.0/config.toml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh-0.6.0/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.6.0/src/edwh/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.6.0/src/edwh/__init__.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 edwh-0.6.0/src/edwh/cli.py
+-rw-r--r--   0        0        0    21484 2020-02-02 00:00:00.000000 edwh-0.6.0/src/edwh/tasks.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 edwh-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 edwh-0.6.0/README.md
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 edwh-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 edwh-0.6.0/PKG-INFO
```

### Comparing `edwh-0.4.5/CHANGELOG.md` & `edwh-0.6.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.6.0 (2023-04-17)
+### Feature
+* **core:** Replaced invoke with fabric for possibly more plugin functionality ([`85838ea`](https://github.com/educationwarehouse/edwh/commit/85838ea3b4cd2a50dc6e8a90e3955d9d82778b0f))
+
+### Fix
+* **project:** Remove theoretical support for Python versions below 3.10 since that has never worked ([`2f567e2`](https://github.com/educationwarehouse/edwh/commit/2f567e2404a3c10019b9bc8efd39c2ed4248bca3))
+* **dependencies:** Importilb is only a package for python 2, not needed as dependency for py 3 ([`f5e0745`](https://github.com/educationwarehouse/edwh/commit/f5e0745f143d09cd6a9cfc4b5884d8f11faa2e35))
+
+## v0.5.0 (2023-04-17)
+
+
 ## v0.4.5 (2023-04-11)
 ### Documentation
 * **changelog:** Manual fix changelog for missing versions pt2 ([`488982d`](https://github.com/educationwarehouse/edwh/commit/488982d604266d1b54adfc02782fd876f8c9c6b5))
 * **changelog:** Manual fix changelog for missing versions ([`fba6cc2`](https://github.com/educationwarehouse/edwh/commit/fba6cc200576cf700faf867cb79efab6f3f13f71))
 
 ## v0.4.4 (2023-04-11)
 ### Feature
```

### Comparing `edwh-0.4.5/src/edwh/cli.py` & `edwh-0.6.0/src/edwh/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-import sys
 import pathlib
-from invoke import Program, Collection
-from .__about__ import __version__
+import sys
+
+from invoke import Collection
+from fabric.main import Fab  # instanceof invoke.Program
+from fabric import Config, Executor
+
 from . import tasks
-import importlib
+from .__about__ import __version__
 
 # https://docs.pyinvoke.org/en/stable/concepts/library.html
 
 collection = Collection.from_module(tasks)
 
 if sys.version_info < (3, 10):
     from importlib_metadata import entry_points
@@ -30,12 +33,18 @@
     try:
         import tasks as local_tasks
 
         local = Collection.from_module(local_tasks)
         collection.add_collection(local, 'local')
         break
     except ImportError as e:
-        if 'No module named \'tasks\'' not in str(e):
+        if "No module named 'tasks'" not in str(e):
             raise e
+
 sys.path = old_path
 
-program = Program(namespace=collection, version=__version__)
+program = Fab(
+    executor_class=Executor,
+    config_class=Config,
+    namespace=collection,
+    version=__version__,
+)
```

### Comparing `edwh-0.4.5/src/edwh/tasks.py` & `edwh-0.6.0/src/edwh/tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,89 @@
-import diceware
-
 try:
     import glob
     import csv
     import shlex
-    from statistics import median
-    from invoke import task, Result, Context
     import datetime
     import io
     import os
     import pathlib
     import random
     import re
     import sys
     import time
     import typing
     import json
-    import tabulate
-    import yaml
-    import tomlkit
+    import importlib.util
+    from collections import defaultdict, OrderedDict
     from dataclasses import dataclass, field
     from pathlib import Path
-    from collections import defaultdict, OrderedDict
+    from statistics import median
+
+    import tabulate
+    import yaml
+    from invoke import task, Result, Context
+
+    if sys.version_info > (3, 11):
+        import tomllib
+    else:
+        import tomlkit
 
 except ImportError as e:
     if sys.argv[0].split("/")[-1] in ("inv", "invoke"):
         print("WARNING: this tasks.py works best using the edwh command instead of using inv[oke] directly.\n")
     print("ImportError:", e)
     exit(1)
 
 
+def load_toml(file: Path) -> dict:
+    """
+    Depends on Python version
+    """
+    with file.open() as f:
+        contents = f.read()
+        if sys.version_info > (3, 11):
+            return tomllib.loads(contents)
+        else:
+            return tomlkit.parse(contents)
+
+
 def confirm(prompt: str, default=False) -> bool:
     allowed = {"y", "1"}
     if default:
-        allowed.add("")
+        allowed.add(" ")
 
-    return (input(prompt).lower().strip() + " ")[0] in allowed
+    answer = input(prompt).lower().strip()
+    answer += " "
+
+    return answer[0] in allowed
 
 
 @dataclass
 class TomlConfig:
     config: dict
     all_services: list[str]
     celeries: list[str]
     services_minimal: list[str]
     services_log: list[str]
     dotenv_path: Path
     __loaded: "TomlConfig" = field(init=False, default=None)  # cache using class instance singleton
 
     @classmethod
-    def load(cls):
+    def load(cls, fname="config.toml"):
         """
         Load config toml file, raising an error if it does not exist.
 
         Since this file should be in .git error suppression is not needed.
         Returns a dictionary with CONFIG, ALL_SERVICES, CELERIES and MINIMAL_SERVICES
         """
         if TomlConfig.__loaded:
             return TomlConfig.__loaded
 
-        with Path("config.toml").open() as config_file:
-            config = tomlkit.parse(config_file.read())
+        config_path = Path(fname)
+        config = load_toml(config_path)
 
         if config["services"]["services"] == "discover":
             with open("docker-compose.yml", "r") as compose:
                 compose = yaml.load(compose, yaml.SafeLoader)
                 all_services = compose["services"].keys()
         else:
             all_services = config["services"]["services"]
@@ -93,24 +112,24 @@
     :type service_arg: list of strings
     :return: list of unique services names that match the given list
     :rtype: list of string
     """
     import fnmatch
 
     config = TomlConfig.load()
-    selected = []
+    selected = set()
     for service in service_arg:
-        selected.extend(fnmatch.filter(config.all_services, service))
-    matched = list(set(selected))
-    if service_arg and not matched:
+        selected.update(fnmatch.filter(config.all_services, service))
+
+    if service_arg and not selected:
         # when no service matches the name, don't return an empty list, as that would `up` all services
         # instead of the wanted list. This includes typos, where a single typo could cause all services to be started.
         print(f"ERROR: No services found matching: {service_arg!r}")
         exit(1)
-    return matched
+    return list(selected)
 
 
 def executes_correctly(c: Context, argument: str) -> bool:
     """returns True if the execution was without error level"""
     return c.run(argument, warn=True, hide=True).ok
 
 
@@ -245,14 +264,143 @@
     hasher = hashlib.sha256(b"")
     for filename in filenames:
         hasher.update(filename.read_bytes())
     print("schema hash: ", hasher.hexdigest())
     return hasher.hexdigest()
 
 
+def exec_setup_in_other_task(run_setup):
+    # execute local_tasks setup
+    old_path = sys.path[:]
+
+    for path in ['.', '..', '../..']:
+        path = pathlib.Path(path)
+        sys.path = [str(path)] + old_path
+        try:
+            import tasks as local_tasks
+
+            try:
+                if run_setup:
+                    local_tasks.setup()
+            except:
+                print(
+                    "the setup in you're local tasks.py crashed, to not run the setup please give up the argument "
+                    "--no-run-setup"
+                )
+                raise
+            break
+        except ImportError:
+            continue
+
+    sys.path = old_path
+
+
+def print_services(services=None):
+    """
+    print all the services that are in the docker-compose.yml
+
+    :param services: docker services that are in the docker-compose.yml
+    :return: a list of all services in the docker-compose.yml
+    """
+
+    print("\n")
+    for index in range(len(services)):
+        if services[index] == "":
+            continue
+        print(f"{index + 1}: {services[index]}")
+    print("Press enter when you're done.\n")
+
+
+def get_services_from_user(services: list, input_string: str):
+    """
+    gets the input from the user and writes it to a string
+
+    :param services: docker services that are in the docker-compose.yml
+    :param input_string: string that the user will see when choosing dockers
+    :return: services that are chosen by the user
+    """
+    print_services(services)
+    chosen_services = ""
+
+    while (chosen_id := input(input_string)) != "":
+        chosen_services += '"' + services[int(chosen_id) - 1] + '",\n'
+
+    return chosen_services
+
+
+def write_user_input_to_config_toml(services: list):
+    """
+    write chosen user dockers to config.toml
+
+    :param services: list of all docker services that are in the docker-compose.yml
+    :return:
+    """
+    with open("config.toml", "w") as config_toml:
+        # let user choose services
+        chosen_services = get_services_from_user(services, "select a service by number(default is 'discover'): ")
+
+        # services you can choose from by minimal and logs
+        if len(chosen_services.replace(" ", "")) != 0:
+            services_to_choose_from = chosen_services.replace(",", "").replace('"', '').split("\n")
+        else:
+            services_to_choose_from = services
+
+        # get chosen services from user
+        chosen_minimal_services = get_services_from_user(services_to_choose_from, "select minimal services by number: ")
+
+        # check if user wants to include celeries
+        include_celeries = (
+            "true" if input("do you want to include celeries(Y/n): ").replace(" ", "") in ["", "y", "Y"] else "false"
+        )
+
+        chosen_log_services = get_services_from_user(
+            services_to_choose_from, "select services to be logged by number: "
+        )
+
+        config_toml.writelines(
+            [
+                "[services]\n",
+                f"services = [\n{chosen_services if len(chosen_services) != 0 else 'discover'}\n]\n",
+                f"minimal = [\n{chosen_minimal_services}\n]\n",
+                f"include_celeries_in_minimal = {include_celeries}\n",
+                f"logs = [\n{chosen_log_services}]\n",
+            ]
+        )
+
+        config_toml.close()
+
+
+@task(help={'run_setup': "executes local_tasks setup(default is True)"})
+def setup(c, run_setup=True):
+    """
+    sets up config.toml and tries to run setup in local tasks.py if it exists
+
+    while configuring the config.toml the program will ask you to select a service by id.
+    All service can be found by the print that is done above.
+    While giving up id's please only give 1 id at the time, this goes for the services and the minimal services
+
+    """
+
+    # create config file
+    if not os.path.exists(str(os.getcwd()) + "/config.toml"):
+        with open("config.toml", "x") as config_toml:
+            config_toml.close()
+    else:
+        continue_setup = input("are you sure you want to overwrite the config.toml file(Y/n): ").replace(" ", "")
+        if continue_setup not in ["", "y", "Y"]:
+            print()
+            sys.exit(255)
+
+    # get and print all found docker compose services
+    services = c.run("docker-compose config --services", hide=True).stdout.split("\n")
+
+    write_user_input_to_config_toml(services)
+    exec_setup_in_other_task(run_setup)
+
+
 @task()
 def search_adjacent_setting(c, key, silent=False):
     """
     Search for key in all ../*/.env files.
     """
     c: Context
     key = key.upper()
@@ -510,7 +658,12 @@
 
 # noinspection PyUnusedLocal
 @task()
 def zen(ctx):
     """Prints the Zen of Python"""
     # noinspection PyUnresolvedReferences
     import this
+
+
+@task
+def whoami(ctx):
+    print(ctx.run("whoami", hide=True).stdout, "@", ctx.run("hostname", hide=True).stdout)
```

### Comparing `edwh-0.4.5/LICENSE.txt` & `edwh-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh-0.4.5/README.md` & `edwh-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `edwh-0.4.5/pyproject.toml` & `edwh-0.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,43 +3,47 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "edwh"
 dynamic = ["version"]
 description = 'Education Warehouse maintenance tools'
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Remco Boerma", email = "remco.b@educationwarehouse.nl" },
   { name = "Robin van der Noord", email = "robin.vdn@educationwarehouse.nl" },
   { name = "Romy Schöller", email = "romy.s@educationwarehouse.nl" },
   { name = "Sven Keimpema", email = "sven.k@educationwarehouse.nl" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   'invoke',
+  'fabric >= 2.7, < 3',
   'importlib_metadata >=3.6 ; python_version < "3.10"',
   'tabulate',
   'pyyaml',
-  'tomlkit',
+  'tomlkit ; python_version < "3.11"',
   'diceware',
 ]
 [project.optional-dependencies]
+dev = [
+  "hatch",
+  "python-semantic-release",
+  "black",
+]
+
 omgeving = [
   'humanize',
   'tabulate',
   'pyyaml',
   'tomlkit'
 ]
 plugins = [
@@ -114,15 +118,15 @@
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+python = ["3.10", "3.11"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
```

### Comparing `edwh-0.4.5/PKG-INFO` & `edwh-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: edwh
-Version: 0.4.5
+Version: 0.6.0
 Summary: Education Warehouse maintenance tools
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Requires-Dist: diceware
+Requires-Dist: fabric<3,>=2.7
 Requires-Dist: importlib-metadata>=3.6; python_version < '3.10'
 Requires-Dist: invoke
 Requires-Dist: pyyaml
 Requires-Dist: tabulate
-Requires-Dist: tomlkit
+Requires-Dist: tomlkit; python_version < '3.11'
 Provides-Extra: bundle
 Requires-Dist: edwh-bundler-plugin; extra == 'bundle'
 Provides-Extra: bundler
 Requires-Dist: edwh-bundler-plugin; extra == 'bundler'
+Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: hatch; extra == 'dev'
+Requires-Dist: python-semantic-release; extra == 'dev'
 Provides-Extra: multipass
 Requires-Dist: edwh-multipass-plugin; extra == 'multipass'
 Provides-Extra: omgeving
 Requires-Dist: humanize; extra == 'omgeving'
 Requires-Dist: pyyaml; extra == 'omgeving'
 Requires-Dist: tabulate; extra == 'omgeving'
 Requires-Dist: tomlkit; extra == 'omgeving'
```

