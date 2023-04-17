# Comparing `tmp/update_pip_packages-0.1.0.tar.gz` & `tmp/update_pip_packages-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "update_pip_packages-0.1.0.tar", max compression
+gzip compressed data, was "update_pip_packages-0.1.1.tar", max compression
```

## Comparing `update_pip_packages-0.1.0.tar` & `update_pip_packages-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1668 2023-04-17 20:07:45.292878 update_pip_packages-0.1.0/README.md
--rw-r--r--   0        0        0      480 2023-04-17 20:09:35.352849 update_pip_packages-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-15 15:28:02.452473 update_pip_packages-0.1.0/update_project/__init__.py
--rw-r--r--   0        0        0     5154 2023-04-15 15:51:35.400818 update_pip_packages-0.1.0/update_project/update_packages.py
--rw-r--r--   0        0        0     2026 1970-01-01 00:00:00.000000 update_pip_packages-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2202 2023-04-17 21:03:45.931791 update_pip_packages-0.1.1/README.md
+-rw-r--r--   0        0        0      480 2023-04-17 21:02:27.951809 update_pip_packages-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-15 15:28:02.452473 update_pip_packages-0.1.1/update_project/__init__.py
+-rw-r--r--   0        0        0     5154 2023-04-15 15:51:35.400818 update_pip_packages-0.1.1/update_project/update_packages.py
+-rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 update_pip_packages-0.1.1/PKG-INFO
```

### Comparing `update_pip_packages-0.1.0/README.md` & `update_pip_packages-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # Update Pip and App Packages
-## v0.1.0
+## v0.1.1
 
 This Python script provides an efficient way to update Pip and app packages on various Linux distributions. The script supports Ubuntu, Debian, Fedora, CentOS, Red Hat, Arch, Manjaro, OpenSUSE, and SUSE distributions. It updates packages using the appropriate package manager for each distribution.
 
+**I know this script may seem useless. Moreover, updating all pip packages can lead to challenges in some projects.
+This script is only a part of my self-education journey.**
+
 ## Features
 
 - Update Pip and its packages to the latest versions.
 - Update app packages for supported Linux distributions using the corresponding package manager.
 - Command-line interface with options for updating Pip packages, app packages, or both.
 
 ## Usage
 
 To use the script, run the following command with the desired options:
 
-```
-python update_packages.py [--pip] [--app]
+```bash
+update-pip-packages [--pip] [--app]
 ```
 - -h, --help: Show this help message and exit
 - --pip: Update Pip packages.
 - --app: Update app packages.
 - If no options are provided, the script will display help information.
 
 ## Tests
@@ -35,16 +38,20 @@
 - [Python](https://www.python.org/) 3.6 or later
 - [Poetry](https://python-poetry.org/)
 - [pytest](https://pytest.org/)
 - [distro](https://pypi.org/project/distro/)
 
 ## Installation
 ```
-pip3 install update-pip-packages
+pip install update-pip-packages
 ```
 or
 ```
 python3 -m pip install update-pip-packages
 ```
 
 ## GitHub Repository
-For more information, source code, and installation instructions, please visit the GitHub repository: [GitHub: update_packages](https://github.com/OleksandrMakarov/Scripts/tree/main/update_project)
+For more information, source code, and installation instructions, please visit the GitHub repository: [GitHub: update_packages](https://github.com/OleksandrMakarov/Scripts/tree/main/update-pip-project)
+
+## Remarks
+There is also a [bash script](https://github.com/OleksandrMakarov/Scripts/tree/main/update-pip-project/update_packages.sh), I started with it and developed it into this Python project. 
+It does not support Linux distribution detection, but you can use it for the same purposes as the main(python) application in a Debian or Ubuntu environment.
```

### Comparing `update_pip_packages-0.1.0/update_project/update_packages.py` & `update_pip_packages-0.1.1/update_project/update_packages.py`

 * *Files identical despite different names*

### Comparing `update_pip_packages-0.1.0/PKG-INFO` & `update_pip_packages-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: update-pip-packages
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: OleksandrMakarov
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: distro (>=1.8.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Update Pip and App Packages
-## v0.1.0
+## v0.1.1
 
 This Python script provides an efficient way to update Pip and app packages on various Linux distributions. The script supports Ubuntu, Debian, Fedora, CentOS, Red Hat, Arch, Manjaro, OpenSUSE, and SUSE distributions. It updates packages using the appropriate package manager for each distribution.
 
+**I know this script may seem useless. Moreover, updating all pip packages can lead to challenges in some projects.
+This script is only a part of my self-education journey.**
+
 ## Features
 
 - Update Pip and its packages to the latest versions.
 - Update app packages for supported Linux distributions using the corresponding package manager.
 - Command-line interface with options for updating Pip packages, app packages, or both.
 
 ## Usage
 
 To use the script, run the following command with the desired options:
 
-```
-python update_packages.py [--pip] [--app]
+```bash
+update-pip-packages [--pip] [--app]
 ```
 - -h, --help: Show this help message and exit
 - --pip: Update Pip packages.
 - --app: Update app packages.
 - If no options are provided, the script will display help information.
 
 ## Tests
@@ -47,16 +50,21 @@
 - [Python](https://www.python.org/) 3.6 or later
 - [Poetry](https://python-poetry.org/)
 - [pytest](https://pytest.org/)
 - [distro](https://pypi.org/project/distro/)
 
 ## Installation
 ```
-pip3 install update-pip-packages
+pip install update-pip-packages
 ```
 or
 ```
 python3 -m pip install update-pip-packages
 ```
 
 ## GitHub Repository
-For more information, source code, and installation instructions, please visit the GitHub repository: [GitHub: update_packages](https://github.com/OleksandrMakarov/Scripts/tree/main/update_project)
+For more information, source code, and installation instructions, please visit the GitHub repository: [GitHub: update_packages](https://github.com/OleksandrMakarov/Scripts/tree/main/update-pip-project)
+
+## Remarks
+There is also a [bash script](https://github.com/OleksandrMakarov/Scripts/tree/main/update-pip-project/update_packages.sh), I started with it and developed it into this Python project. 
+It does not support Linux distribution detection, but you can use it for the same purposes as the main(python) application in a Debian or Ubuntu environment.
+
```

