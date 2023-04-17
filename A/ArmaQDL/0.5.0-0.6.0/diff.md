# Comparing `tmp/armaqdl-0.5.0.tar.gz` & `tmp/armaqdl-0.6.0.tar.gz`

## Comparing `armaqdl-0.5.0.tar` & `armaqdl-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 armaqdl-0.5.0/.editorconfig
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 armaqdl-0.5.0/.flake8
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 armaqdl-0.5.0/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.5.0/armaqdl/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 armaqdl-0.5.0/armaqdl/__main__.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 armaqdl-0.5.0/armaqdl/_version.py
--rw-r--r--   0        0        0    14197 2020-02-02 00:00:00.000000 armaqdl-0.5.0/armaqdl/armaqdl.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 armaqdl-0.5.0/armaqdl/config.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 armaqdl-0.5.0/config/settings.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 armaqdl-0.5.0/tests/test_commands.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 armaqdl-0.5.0/tests/test_config.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 armaqdl-0.5.0/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 armaqdl-0.5.0/LICENSE
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 armaqdl-0.5.0/README.md
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 armaqdl-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 armaqdl-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 armaqdl-0.6.0/.editorconfig
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 armaqdl-0.6.0/.flake8
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 armaqdl-0.6.0/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.6.0/armaqdl/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 armaqdl-0.6.0/armaqdl/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 armaqdl-0.6.0/armaqdl/_version.py
+-rw-r--r--   0        0        0    14593 2020-02-02 00:00:00.000000 armaqdl-0.6.0/armaqdl/armaqdl.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 armaqdl-0.6.0/armaqdl/config.py
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 armaqdl-0.6.0/armaqdl/update.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 armaqdl-0.6.0/config/settings.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 armaqdl-0.6.0/tests/test_commands.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 armaqdl-0.6.0/tests/test_config.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 armaqdl-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 armaqdl-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 armaqdl-0.6.0/README.md
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 armaqdl-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5950 2020-02-02 00:00:00.000000 armaqdl-0.6.0/PKG-INFO
```

### Comparing `armaqdl-0.5.0/armaqdl/armaqdl.py` & `armaqdl-0.6.0/armaqdl/armaqdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import argparse
 import os
 import re
 import shutil
 import subprocess
-import sys
 import threading
 import time
 from pathlib import Path
 from urllib.parse import quote
 
 if os.name == "nt":
     import winreg
 
-from ._version import version as __version__
-from . import config
+from ._version import __version__
+from . import config, update
 
 
 VERBOSE = False
 DRY = False
 SETTINGS = None
 
 
@@ -56,15 +55,15 @@
 
         rpt_path = Path.home() / "AppData" / "Local" / "Arma 3"
         rpt_list = rpt_path.glob("*.rpt")
         last_rpt = max(rpt_list, key=os.path.getctime)
         if not DRY:
             os.startfile(last_rpt)
     else:
-        print("Warning: Opening last log only implemented for Windows.")
+        print("Warning! Opening last log only implemented for Windows.")
 
 
 def build_mod(path, tool):
     for build_tool in SETTINGS.get("build", {}):
         req_file = SETTINGS["build"][build_tool]["presence"]
         cmd = SETTINGS["build"][build_tool]["command"]
 
@@ -85,15 +84,15 @@
         print("=> Building failed! No build tool found.\n")
     else:
         print(f"=> Building failed! Specified build tool not found: {tool}\n")
     return False
 
 
 def process_mods(mods, build_dev_tool):
-    if not mods:
+    if not mods or "none" in mods:
         return ""
 
     if VERBOSE:
         print(f"Process mods: {mods}")
 
     paths, skips = [], []
     ignores = 0
@@ -343,21 +342,24 @@
         subprocess.Popen(process_cmd)
 
 
 def main():
     # Generate new config
     config.generate()
 
+    # Cleanup update files
+    update.clean()
+
     # Parse arguments
     parser = argparse.ArgumentParser(
-        prog="armaqdl",
+        prog=update.PACKAGE,
         description=f"Quick development Arma 3 launcher v{__version__}",
         formatter_class=argparse.RawTextHelpFormatter)
 
-    parser.add_argument("mods", metavar="loc:mod[:b[tool]][:s|:skip] ...", type=str, nargs="*", help="paths to mods")
+    parser.add_argument("mods", metavar="loc:mod[:b[tool]][:s|:skip] ...", type=str, nargs="*", help="paths to mods or 'none' for no mods")
     parser.add_argument("-m", "--mission", default="", type=str, help="mission to load")
 
     parser.add_argument("-s", "--server", action="store_true", help="start server")
     parser.add_argument("-j", "--join-server", nargs="?", const="", type=str, help="join server")
     parser.add_argument("-hc", "--headless", action="store_true", help="start headess client")
 
     parser.add_argument("-p", "--profile", default="", type=str, help="profile name")
@@ -373,50 +375,62 @@
                         help="build mods (auto-determine tool if unspecified)")
     parser.add_argument("-nl", "--no-log", action="store_true", help="don't open last log")
 
     parser.add_argument("--config", default=config.CONFIG_DIR, type=Path, help="load config from specified folder")
     parser.add_argument("--list", action="store_true", help="list active config locations and build tools")
     parser.add_argument("--dry", action="store_true", help="dry run without actually launching anything (simulate)")
     parser.add_argument("--verbose", action="store_true", help="verbose output")
+    parser.add_argument("--update", action="store_true", help="self-update")
     parser.add_argument("-v", "--version", action="store_true", help="show version")
 
     args = parser.parse_args()
 
     if args.version:
         print(f"ArmaQDL v{__version__}")
         return 0
 
+    if args.update:
+        update.update()
+        return 0
+    update.check()
+
     global VERBOSE
     VERBOSE = args.verbose
     global DRY
     DRY = args.dry
     if DRY:
         print("Dry run - simulating only!\n")
 
     # Config
     global SETTINGS
     SETTINGS = config.load(args.config)
     if not config.validate(SETTINGS):
         return 1
 
     if args.list:
-        epilog = f"ArmaQDL config location: {args.config}\n\n"
+        epilog = f"Config location: {args.config}\n\n"
         epilog += "Mod Locations:"
         for location in SETTINGS.get("locations", {}):
             epilog += f"\n  {location} => {SETTINGS['locations'][location]['path']}"
             if SETTINGS['locations'][location].get('build', False):
                 epilog += " (build)"
 
         epilog += "\n\nBuild Tools:"
         for tool in SETTINGS.get("build", {}):
             epilog += f"\n  {tool} ({SETTINGS['build'][tool]['presence']}) => {' '.join(SETTINGS['build'][tool]['command'])}"
 
         print(epilog)
         return 0
 
+    if "none" in args.mods:
+        print("Warning! Launching without any mods (vanilla!)")
+    elif not args.mods:
+        print("Empty mod paths - use 'none' to launch without any mods (vanilla).")
+        return 0
+
     # Arma path
     arma_path = find_arma(executable=True)
     if not arma_path:
         print("Error! Invalid Arma path.")
         return 2
 
     # Mods
@@ -451,14 +465,10 @@
         params.append(param_mission)
     if param_mods:
         params.append(param_mods)
 
     if os.name == "nt":
         run_arma(arma_path, params)
     else:
-        print("Warning: Launching Arma only implemented for Windows.")
+        print("Warning! Launching Arma only implemented for Windows.")
 
     return 0
-
-
-if __name__ == "__main__":
-    sys.exit(main())
```

### Comparing `armaqdl-0.5.0/armaqdl/config.py` & `armaqdl-0.6.0/armaqdl/config.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.5.0/config/settings.toml` & `armaqdl-0.6.0/config/settings.toml`

 * *Files identical despite different names*

### Comparing `armaqdl-0.5.0/tests/test_config.py` & `armaqdl-0.6.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.5.0/.gitignore` & `armaqdl-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `armaqdl-0.5.0/LICENSE` & `armaqdl-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `armaqdl-0.5.0/README.md` & `armaqdl-0.6.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -21,80 +21,116 @@
 - Easy **dedicated server and headless client launching**
 - Load mission on dedicated server (by manipulating `server.cfg`)
 - Join server
 
 
 ## Installation
 
-ArmaQDL is distributed on [PyPI](https://pypi.org/). Installation as a user is recommended to avoid permission issues with CLI script installation.
+ArmaQDL is distributed on [PyPI](https://pypi.org/) as well as a Standalone executable (Windows only).
+- Use Standalone if you are on Windows and don't have Python installed.
+- Use PyPI if you have Python installed or are not using Windows.
+
+PyPI provides easier updating of ArmaQDL, while Standalone requires manual updates.
+
+#### Standalone
+
+Download `armaqdl.exe` from [latest release](https://github.com/jonpas/ArmaQDL/releases/latest) and place it in a convenient location.
+
+Open Command Prompt, PowerShell or any other terminal application, navigate to the location of `armaqdl.exe` and run it once to generate configuration files without launching Arma.
+
+```sh
+# Command Prompt
+$ armaqdl
+# PowerShell
+$ .\armaqdl
+```
+_Note: Add `.exe` if `armaqdl` is not enough to find the executable._
+
+
+#### PyPI
+
+Installation as a user is recommended to avoid permission issues with CLI script installation.
 
 ```
 $ pip install --user ArmaQDL
 ```
 _Note: Add pip installation directory to `PATH` environmental variable to use it directly._
 
-Run it once to generate configuration files.
+Run it once to generate configuration files without launching Arma.
 
+```sh
+# Directly (only works if in PATH)
+$ armaqdl
+# As a Python module
+$ python -m armaqdl
 ```
-$ armaqdl -h
-$ python -m armaqdl -h
-```
 
-Modify settings to your needs. Settings file can be found in your operating system's standard configuration directory, usually:
+## Setup
+
+You should modify the [default settings](https://github.com/jonpas/ArmaQDL/blob/master/config/settings.toml) to your needs. Launching without setup may create a new profile and result in failed launches.
+
+Settings file can be found in your operating system's standard configuration directory, usually:
 - Windows: `%AppData%\ArmaQDL\settings.toml`
 - Linux: `~/.config/ArmaQDL/settings.toml`
 
 Settings are in [TOML](https://toml.io/en/) format and can be edited with any text editor.
 
 
 ## Usage
 
-ArmaQDL will install a CLI script _(requires it to be in `PATH`)_, but it can also be used as a Python module.
+ArmaQDL is a CLI script, view all the options with the `--help` flag.
 
-```
+```sh
 $ armaqdl -h
-$ python -m armaqdl -h
 ```
+_Note: All examples use `armaqdl` to launch ArmaQDL, replace it appropriately depending on your install._
 
 **Example 1:**
 
 Launches Arma with CBA from P-drive, ACE3 from Workshop install and ACRE2 from local development folder. Additionally builds ACRE2 mod and opens the latest log file. Loads Arma directly into the editor using the specified mission from the "Soldier" profile.
 
-```
+```sh
 $ armaqdl p:x\cba workshop:@ace dev:acre2:b -m Soldier:test.vr
 ```
 
 Specific build tool can also be specified, such as HEMTT:
-```
+```sh
 $ armaqdl p:x\cba workshop:@ace dev:acre2:bhemtt -m Soldier:test.vr
 ```
 
 **Example 2:**
 
 Launches Arma Server with CBA from P-drive and loads specified mission from default profile's missions folder, copying it to the server in the process.
 
-```
+```sh
 $ armaqdl p:x\cba -m test.vr -s
 ```
 
 Launches Arma with CBA from P-drive and connects to the given server with the given password (`-j` defaults to the settings file).
 
-```
+```sh
 $ armaqdl p:x\cba -j 192.168.1.1:2302:test
 ```
 
 
 ## Development
 
 ArmaQDL uses [Hatchling](https://hatch.pypa.io/latest/) as a build backend and [flake8](https://flake8.pycqa.org/en/latest/) as a style guide.
 
-```
+```sh
 $ pip install --user -e .
 ```
 
-[Hatch](https://hatch.pypa.io/latest/) is the primary project manager of choice, but any project adhering to PEP 621 (`pyproject.toml` specification)  can be used.
+[Hatch](https://hatch.pypa.io/latest/) is the primary project manager of choice, but any project adhering to PEP 621 (`pyproject.toml` specification) can be used.
 
-```
-$ hatch shell
+```sh
+# Run development build
+$ hatch run armaqdl
+# Lint with flake8
+$ hatch run lint
+# Test with pytest
+$ hatch run test
+# Bundle with PyInstaller
+$ hatch run static:bundle
 ```
 
 Limited Linux support exists for testing purposes, but launching Arma or opening the last log file is not supported. Contributions are welcome!
```

### Comparing `armaqdl-0.5.0/pyproject.toml` & `armaqdl-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -54,33 +54,35 @@
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "armaqdl/_version.py"
 
+
 ## Hatch environments
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
+  "flake8",
 ]
 
 [tool.hatch.envs.default.scripts]
-full = "pytest {args:tests}"
+test = "pytest {args:tests}"
+lint = "flake8 {args:.}"
 
-[[tool.hatch.envs.test.matrix]]
-python = ["37", "38", "39", "310", "311"]
 
-[tool.hatch.envs.lint]
-detached = true
+[tool.hatch.envs.static]
+template = "static"
 dependencies = [
-  "flake8",
+  "pyinstaller",
 ]
+dev-mode = false
 
-[tool.hatch.envs.lint.scripts]
-style = [
-  "flake8 {args:.}",
-]
-all = [
-  "style",
+[tool.hatch.envs.static.scripts]
+bundle = "pyinstaller armaqdl/__main__.py --add-data armaqdl;armaqdl --add-data config;config -n armaqdl --onefile"
+
+[tool.hatch.envs.static.overrides]
+platform.linux.scripts = [
+  "bundle=pyinstaller armaqdl/__main__.py --add-data armaqdl:armaqdl --add-data config:config -n armaqdl --onefile",
 ]
```

### Comparing `armaqdl-0.5.0/PKG-INFO` & `armaqdl-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: ArmaQDL
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python program for quick launching various mod development configurations for Arma through a simple CLI.
 Project-URL: Homepage, https://github.com/jonpas/Arma-QDL
 Project-URL: Bug Tracker, https://github.com/jonpas/Arma-QDL/issues
 Author-email: Jonpas <jonpas33@gmail.com>
+License-Expression: MIT
 License-File: LICENSE
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -44,80 +45,116 @@
 - Easy **dedicated server and headless client launching**
 - Load mission on dedicated server (by manipulating `server.cfg`)
 - Join server
 
 
 ## Installation
 
-ArmaQDL is distributed on [PyPI](https://pypi.org/). Installation as a user is recommended to avoid permission issues with CLI script installation.
+ArmaQDL is distributed on [PyPI](https://pypi.org/) as well as a Standalone executable (Windows only).
+- Use Standalone if you are on Windows and don't have Python installed.
+- Use PyPI if you have Python installed or are not using Windows.
+
+PyPI provides easier updating of ArmaQDL, while Standalone requires manual updates.
+
+#### Standalone
+
+Download `armaqdl.exe` from [latest release](https://github.com/jonpas/ArmaQDL/releases/latest) and place it in a convenient location.
+
+Open Command Prompt, PowerShell or any other terminal application, navigate to the location of `armaqdl.exe` and run it once to generate configuration files without launching Arma.
+
+```sh
+# Command Prompt
+$ armaqdl
+# PowerShell
+$ .\armaqdl
+```
+_Note: Add `.exe` if `armaqdl` is not enough to find the executable._
+
+
+#### PyPI
+
+Installation as a user is recommended to avoid permission issues with CLI script installation.
 
 ```
 $ pip install --user ArmaQDL
 ```
 _Note: Add pip installation directory to `PATH` environmental variable to use it directly._
 
-Run it once to generate configuration files.
+Run it once to generate configuration files without launching Arma.
 
+```sh
+# Directly (only works if in PATH)
+$ armaqdl
+# As a Python module
+$ python -m armaqdl
 ```
-$ armaqdl -h
-$ python -m armaqdl -h
-```
 
-Modify settings to your needs. Settings file can be found in your operating system's standard configuration directory, usually:
+## Setup
+
+You should modify the [default settings](https://github.com/jonpas/ArmaQDL/blob/master/config/settings.toml) to your needs. Launching without setup may create a new profile and result in failed launches.
+
+Settings file can be found in your operating system's standard configuration directory, usually:
 - Windows: `%AppData%\ArmaQDL\settings.toml`
 - Linux: `~/.config/ArmaQDL/settings.toml`
 
 Settings are in [TOML](https://toml.io/en/) format and can be edited with any text editor.
 
 
 ## Usage
 
-ArmaQDL will install a CLI script _(requires it to be in `PATH`)_, but it can also be used as a Python module.
+ArmaQDL is a CLI script, view all the options with the `--help` flag.
 
-```
+```sh
 $ armaqdl -h
-$ python -m armaqdl -h
 ```
+_Note: All examples use `armaqdl` to launch ArmaQDL, replace it appropriately depending on your install._
 
 **Example 1:**
 
 Launches Arma with CBA from P-drive, ACE3 from Workshop install and ACRE2 from local development folder. Additionally builds ACRE2 mod and opens the latest log file. Loads Arma directly into the editor using the specified mission from the "Soldier" profile.
 
-```
+```sh
 $ armaqdl p:x\cba workshop:@ace dev:acre2:b -m Soldier:test.vr
 ```
 
 Specific build tool can also be specified, such as HEMTT:
-```
+```sh
 $ armaqdl p:x\cba workshop:@ace dev:acre2:bhemtt -m Soldier:test.vr
 ```
 
 **Example 2:**
 
 Launches Arma Server with CBA from P-drive and loads specified mission from default profile's missions folder, copying it to the server in the process.
 
-```
+```sh
 $ armaqdl p:x\cba -m test.vr -s
 ```
 
 Launches Arma with CBA from P-drive and connects to the given server with the given password (`-j` defaults to the settings file).
 
-```
+```sh
 $ armaqdl p:x\cba -j 192.168.1.1:2302:test
 ```
 
 
 ## Development
 
 ArmaQDL uses [Hatchling](https://hatch.pypa.io/latest/) as a build backend and [flake8](https://flake8.pycqa.org/en/latest/) as a style guide.
 
-```
+```sh
 $ pip install --user -e .
 ```
 
-[Hatch](https://hatch.pypa.io/latest/) is the primary project manager of choice, but any project adhering to PEP 621 (`pyproject.toml` specification)  can be used.
+[Hatch](https://hatch.pypa.io/latest/) is the primary project manager of choice, but any project adhering to PEP 621 (`pyproject.toml` specification) can be used.
 
-```
-$ hatch shell
+```sh
+# Run development build
+$ hatch run armaqdl
+# Lint with flake8
+$ hatch run lint
+# Test with pytest
+$ hatch run test
+# Bundle with PyInstaller
+$ hatch run static:bundle
 ```
 
 Limited Linux support exists for testing purposes, but launching Arma or opening the last log file is not supported. Contributions are welcome!
```

