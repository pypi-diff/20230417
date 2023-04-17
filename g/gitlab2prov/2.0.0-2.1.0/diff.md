# Comparing `tmp/gitlab2prov-2.0.0.tar.gz` & `tmp/gitlab2prov-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab2prov-2.0.0.tar", last modified: Mon Oct 31 16:09:36 2022, max compression
+gzip compressed data, was "gitlab2prov-2.1.0.tar", last modified: Mon Apr 17 14:32:05 2023, max compression
```

## Comparing `gitlab2prov-2.0.0.tar` & `gitlab2prov-2.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:36.787057 gitlab2prov-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    11463 2022-10-31 16:09:36.787057 gitlab2prov-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9107 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:36.783057 gitlab2prov-2.0.0/gitlab2prov/
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:36.787057 gitlab2prov-2.0.0/gitlab2prov/adapters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:36.787057 gitlab2prov-2.0.0/gitlab2prov/adapters/fetch/
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/adapters/fetch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:36.787057 gitlab2prov-2.0.0/gitlab2prov/adapters/fetch/annotations/
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/adapters/fetch/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16016 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/adapters/fetch/annotations/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6050 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/adapters/fetch/annotations/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)     4677 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/adapters/fetch/git.py
--rw-r--r--   0 runner    (1001) docker     (121)     7222 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/adapters/fetch/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/adapters/fetch/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/adapters/repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:36.787057 gitlab2prov-2.0.0/gitlab2prov/config/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/config/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:36.787057 gitlab2prov-2.0.0/gitlab2prov/domain/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/domain/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/domain/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    11235 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/domain/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:36.787057 gitlab2prov-2.0.0/gitlab2prov/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9449 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/entrypoints/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:36.787057 gitlab2prov-2.0.0/gitlab2prov/prov/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/prov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11593 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/prov/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     8936 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/prov/operations.py
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/root.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:36.787057 gitlab2prov-2.0.0/gitlab2prov/service_layer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/service_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/service_layer/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/service_layer/messagebus.py
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/gitlab2prov/service_layer/unit_of_work.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:09:36.787057 gitlab2prov-2.0.0/gitlab2prov.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11463 2022-10-31 16:09:36.000000 gitlab2prov-2.0.0/gitlab2prov.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-10-31 16:09:36.000000 gitlab2prov-2.0.0/gitlab2prov.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 16:09:36.000000 gitlab2prov-2.0.0/gitlab2prov.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-10-31 16:09:36.000000 gitlab2prov-2.0.0/gitlab2prov.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-10-31 16:09:36.000000 gitlab2prov-2.0.0/gitlab2prov.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-31 16:09:36.000000 gitlab2prov-2.0.0/gitlab2prov.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-10-31 16:09:21.000000 gitlab2prov-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-31 16:09:36.787057 gitlab2prov-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:05.524767 gitlab2prov-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-04-17 14:32:05.524767 gitlab2prov-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:05.520767 gitlab2prov-2.1.0/gitlab2prov/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:05.524767 gitlab2prov-2.1.0/gitlab2prov/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:05.524767 gitlab2prov-2.1.0/gitlab2prov/adapters/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/adapters/fetch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:05.524767 gitlab2prov-2.1.0/gitlab2prov/adapters/fetch/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/adapters/fetch/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16016 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/adapters/fetch/annotations/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/adapters/fetch/annotations/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/adapters/fetch/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/adapters/fetch/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/adapters/fetch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/adapters/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:05.524767 gitlab2prov-2.1.0/gitlab2prov/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/config/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:05.524767 gitlab2prov-2.1.0/gitlab2prov/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/domain/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/domain/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/domain/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:05.524767 gitlab2prov-2.1.0/gitlab2prov/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/entrypoints/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:05.524767 gitlab2prov-2.1.0/gitlab2prov/prov/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/prov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/prov/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/prov/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/root.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:05.524767 gitlab2prov-2.1.0/gitlab2prov/service_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/service_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/service_layer/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/service_layer/messagebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/gitlab2prov/service_layer/unit_of_work.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:05.524767 gitlab2prov-2.1.0/gitlab2prov.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-04-17 14:32:05.000000 gitlab2prov-2.1.0/gitlab2prov.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-17 14:32:05.000000 gitlab2prov-2.1.0/gitlab2prov.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:32:05.000000 gitlab2prov-2.1.0/gitlab2prov.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-17 14:32:05.000000 gitlab2prov-2.1.0/gitlab2prov.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-17 14:32:05.000000 gitlab2prov-2.1.0/gitlab2prov.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 14:32:05.000000 gitlab2prov-2.1.0/gitlab2prov.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-17 14:31:46.000000 gitlab2prov-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:32:05.528767 gitlab2prov-2.1.0/setup.cfg
```

### Comparing `gitlab2prov-2.0.0/LICENSE` & `gitlab2prov-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/PKG-INFO` & `gitlab2prov-2.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab2prov
-Version: 2.0.0
+Version: 2.1.0
 Summary: Extract provenance information (W3C PROV) from GitLab projects.
 Author-email: Claas de Boer <claas.deboer@dlr.de>
 Maintainer-email: Andreas Schreiber <andreas.schreiber@dlr.de>
 License: MIT License
         
         Copyright (c) 2019 German Aerospace Center (DLR)
         
@@ -81,14 +81,16 @@
 ---
 
 The `gitlab2prov` data model has been designed according to [W3C PROV](https://www.w3.org/TR/prov-overview/) specification.
 The model documentation can be found [here](https://github.com/DLR-SC/gitlab2prov/tree/master/docs).
 
 ## ️🏗️ ️Installation
 
+Please note that this tool requires Git to be installed on your machine.
+
 Clone the project and install using `pip`:
 ```bash
 pip install .
 ```
 
 Or install the latest release from [PyPi](https://pypi.org/project/gitlab2prov/):
 ```bash
@@ -97,14 +99,20 @@
 
 To install `gitlab2prov` with all extra dependencies require the `[dev]` extras:
 ```bash
 pip install .[dev]            # clone repo, install with extras
 pip install gitlab2prov[dev]  # PyPi, install with extras
 ```
 
+## ⚡ Getting started
+
+`gitlab2prov` needs a [personal access token](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html) to clone git repositories and to authenticate with the GitLab API.
+Follow [this guide](./docs/guides/tokens.md) to create an access token with the required [scopes](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html#personal-access-token-scopes).
+
+
 ## 🚀‍ Usage
 
 `gitlab2prov` can be configured using the command line interface or by providing a configuration file in `.yaml` format.
 
 ###  Command Line Usage
 The command line interface consists of commands that can be chained together like a unix pipeline.
 
@@ -231,10 +239,23 @@
 
 * Andreas Schreiber, Claas de Boer (2020). [Modelling Knowledge about Software Processes using Provenance Graphs and its Application to Git-based VersionControl Systems](https://dl.acm.org/doi/10.1145/3387940.3392220). In *ICSEW'20: Proceedings of the IEEE/ACM 42nd Conference on Software Engineering Workshops* (pp. 358–359).
 
 * Tim Sonnekalb, Thomas S. Heinze, Lynn von Kurnatowski, Andreas Schreiber, Jesus M. Gonzalez-Barahona, and Heather Packer (2020). [Towards automated, provenance-driven security audit for git-based repositories: applied to germany's corona-warn-app: vision paper](https://doi.org/10.1145/3416507.3423190). In *Proceedings of the 3rd ACM SIGSOFT International Workshop on Software Security from Design to Deployment* (pp. 15–18).
 
 * Andreas Schreiber (2020). [Visualization of contributions to open-source projects](https://doi.org/10.1145/3430036.3430057). In *Proceedings of the 13th International Symposium on Visual Information Communication and Interaction*. ACM, USA.
 
+## 📜 Dependencies 
+`gitlab2prov` depends on several open source packages that are made freely available under their respective licenses.
+
+| Package                                                         | License                                                                                                                   |
+| --------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
+| [GitPython](https://github.com/gitpython-developers/GitPython)  | [![License](https://img.shields.io/badge/License-BSD_3--Clause-orange.svg)](https://opensource.org/licenses/BSD-3-Clause) |
+| [click](https://github.com/pallets/click)                       | [![License](https://img.shields.io/badge/License-BSD_3--Clause-orange.svg)](https://opensource.org/licenses/BSD-3-Clause) |
+| [python-gitlab](https://github.com/python-gitlab/python-gitlab) | [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)       |
+| [prov](https://pypi.org/project/prov/)                          | [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)               |
+| [jsonschema](https://github.com/python-jsonschema/jsonschema)   | [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)               |
+| [ruamel.yaml](https://pypi.org/project/ruamel.yaml/)            | [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)               |
+| [pydot](https://github.com/pydot/pydot)                         | [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)               |
+
 ## 📝 License
 This project is [MIT](https://github.com/dlr-sc/gitlab2prov/blob/master/LICENSE) licensed.  
 Copyright © 2019 German Aerospace Center (DLR) and individual contributors.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gitlab2prov Version: 2.0.0 Summary: Extract
+Metadata-Version: 2.1 Name: gitlab2prov Version: 2.1.0 Summary: Extract
 provenance information (W3C PROV) from GitLab projects. Author-email: Claas de
 Boer
 deboer@dlr.de> Maintainer-email: Andreas Schreiber
 schreiber@dlr.de> License: MIT License Copyright (c) 2019 German Aerospace
 Center (DLR) Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
@@ -34,91 +34,118 @@
 Downloads_Monthly] [Twitter:_DLR_Software] [Badge:_Open_in_VSCode] [Badge:_DOI]
             [Badge:_W3C_PROV] [Badge:_Citation_File_Format_Inside]
 > `gitlab2prov` is a Python library and command line tool that extracts
 provenance information from GitLab projects. --- The `gitlab2prov` data model
 has been designed according to [W3C PROV](https://www.w3.org/TR/prov-overview/
 ) specification. The model documentation can be found [here](https://
 github.com/DLR-SC/gitlab2prov/tree/master/docs). ## ï¸ðï¸ ï¸Installation
-Clone the project and install using `pip`: ```bash pip install . ``` Or install
-the latest release from [PyPi](https://pypi.org/project/gitlab2prov/): ```bash
-pip install gitlab2prov ``` To install `gitlab2prov` with all extra
-dependencies require the `[dev]` extras: ```bash pip install .[dev] # clone
-repo, install with extras pip install gitlab2prov[dev] # PyPi, install with
-extras ``` ## ðâ Usage `gitlab2prov` can be configured using the command
-line interface or by providing a configuration file in `.yaml` format. ###
-Command Line Usage The command line interface consists of commands that can be
-chained together like a unix pipeline. ``` Usage: gitlab2prov [OPTIONS]
-COMMAND1 [ARGS]... [COMMAND2 [ARGS]...]... Extract provenance information from
-GitLab projects. Options: --version Show the version and exit. --verbose Enable
-logging to 'gitlab2prov.log'. --config FILE Read config from file. --validate
-FILE Validate config file and exit. --help Show this message and exit.
-Commands: combine Combine multiple graphs into one. extract Extract provenance
-information for one or more... load Load provenance files. merge-duplicated-
-agents Merge duplicated agents based on a name to... pseudonymize Pseudonymize
-a provenance graph. save Save provenance information to a file. stats Print
-statistics such as node counts and... ``` ### Configuration Files `gitlab2prov`
-supports configuration files in `.yaml` format that are functionally equivalent
-to command line invocations. To read configuration details from a file instead
-of specifying on the command line, use the `--config` option: ```ini # initiate
-a run using a config file gitlab2prov --config config/example.yaml ``` You can
-validate your config file using the provided JSON-Schema `gitlab2prov/config/
-schema.json` that comes packaged with every installation: ```ini # check config
-file for syntactical errors gitlab2prov --validate config/example.yaml ```
-Config file example: ```yaml - extract: url: ["https://gitlab.com/example/foo"]
-token: tokenA - extract: url: ["https://gitlab.com/example/bar"] token: tokenB
-- load: input: [example.rdf] - pseudonymize: - combine: - save: output:
-combined format: [json, rdf, xml, dot] - stats: fine: true explain: true
-formatter: table ``` The config file example is functionally equivalent to this
-command line invocation: ``` gitlab2prov extract -u https://gitlab.com/example/
-foo -t tokenFoo \ extract -u https://gitlab.com/example/bar -t tokenBar \ load
--i example.rdf \ pseudonymize \ combine \ save -o combined -f json -f rdf -
-f xml -f dot \ stats --fine --explain --formatter table ``` ### ð¨ Provenance
-Output Formats `gitlab2prov` supports output formats that the [`prov`](https://
-github.com/trungdong/prov) library provides: * [PROV-N](http://www.w3.org/TR/
-prov-n/) * [PROV-O](http://www.w3.org/TR/prov-o/) (RDF) * [PROV-XML](http://
-www.w3.org/TR/prov-xml/) * [PROV-JSON](http://www.w3.org/Submission/prov-json/
-) * [Graphviz](https://graphviz.org/) (DOT) ## ð¤ Contributing Contributions
-and pull requests are welcome! For major changes, please open an issue first to
-discuss what you would like to change. ## â¨ How to cite If you use
-GitLab2PROV in a scientific publication, we would appreciate citations to the
-following paper: * Schreiber, A., de Boer, C. and von Kurnatowski, L. (2021).
-[GitLab2PROVâProvenance of Software Projects hosted on GitLab](https://
-www.usenix.org/conference/tapp2021/presentation/schreiber). 13th International
-Workshop on Theory and Practice of Provenance (TaPP 2021), USENIX Association
-Bibtex entry: ```BibTeX @InProceedings{SchreiberBoerKurnatowski2021, author =
-{Andreas Schreiber and Claas de~Boer and Lynn von~Kurnatowski}, booktitle =
-{13th International Workshop on Theory and Practice of Provenance (TaPP 2021)},
-title = {{GitLab2PROV}{\textemdash}Provenance of Software Projects hosted on
-GitLab}, year = {2021}, month = jul, publisher = {{USENIX} Association}, url =
-{https://www.usenix.org/conference/tapp2021/presentation/schreiber}, } ``` You
-can also cite specific releases published on Zenodo: [![DOI](https://
-zenodo.org/badge/215042878.svg)](https://zenodo.org/badge/latestdoi/215042878)
-## âï¸ References **Influencial Software for `gitlab2prov`** * Martin
-Stoffers: "Gitlab2Graph", v1.0.0, October 13. 2019, [GitHub Link](https://
-github.com/DLR-SC/Gitlab2Graph), DOI 10.5281/zenodo.3469385 * Quentin Pradet:
-"How do you rate limit calls with aiohttp?", [GitHub Gist](https://
-gist.github.com/pquentin/5d8f5408cdad73e589d85ba509091741), MIT LICENSE
-**Influencial Papers for `gitlab2prov`**: * De Nies, T., Magliacane, S.,
-Verborgh, R., Coppens, S., Groth, P., Mannens, E., and Van de Walle, R. (2013).
-[Git2PROV: Exposing Version Control System Content as W3C PROV](https://
-dl.acm.org/doi/abs/10.5555/2874399.2874431). In *Poster and Demo Proceedings of
-the 12th International Semantic Web Conference* (Vol. 1035, pp. 125â128). *
-Packer, H. S., Chapman, A., and Carr, L. (2019). [GitHub2PROV: provenance for
-supporting software project management](https://dl.acm.org/doi/10.5555/
-3359032.3359039). In *11th International Workshop on Theory and Practice of
-Provenance (TaPP 2019)*. **Papers that refer to `gitlab2prov`**: * Andreas
-Schreiber, Claas de Boer (2020). [Modelling Knowledge about Software Processes
-using Provenance Graphs and its Application to Git-based VersionControl
-Systems](https://dl.acm.org/doi/10.1145/3387940.3392220). In *ICSEW'20:
-Proceedings of the IEEE/ACM 42nd Conference on Software Engineering Workshops*
-(pp. 358â359). * Tim Sonnekalb, Thomas S. Heinze, Lynn von Kurnatowski,
-Andreas Schreiber, Jesus M. Gonzalez-Barahona, and Heather Packer (2020).
-[Towards automated, provenance-driven security audit for git-based
-repositories: applied to germany's corona-warn-app: vision paper](https://
-doi.org/10.1145/3416507.3423190). In *Proceedings of the 3rd ACM SIGSOFT
-International Workshop on Software Security from Design to Deployment* (pp.
-15â18). * Andreas Schreiber (2020). [Visualization of contributions to open-
-source projects](https://doi.org/10.1145/3430036.3430057). In *Proceedings of
-the 13th International Symposium on Visual Information Communication and
-Interaction*. ACM, USA. ## ð License This project is [MIT](https://
-github.com/dlr-sc/gitlab2prov/blob/master/LICENSE) licensed. Copyright Â© 2019
-German Aerospace Center (DLR) and individual contributors.
+Please note that this tool requires Git to be installed on your machine. Clone
+the project and install using `pip`: ```bash pip install . ``` Or install the
+latest release from [PyPi](https://pypi.org/project/gitlab2prov/): ```bash pip
+install gitlab2prov ``` To install `gitlab2prov` with all extra dependencies
+require the `[dev]` extras: ```bash pip install .[dev] # clone repo, install
+with extras pip install gitlab2prov[dev] # PyPi, install with extras ``` ## â¡
+Getting started `gitlab2prov` needs a [personal access token](https://
+docs.gitlab.com/ee/user/profile/personal_access_tokens.html) to clone git
+repositories and to authenticate with the GitLab API. Follow [this guide](./
+docs/guides/tokens.md) to create an access token with the required [scopes]
+(https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html#personal-
+access-token-scopes). ## ðâ Usage `gitlab2prov` can be configured using
+the command line interface or by providing a configuration file in `.yaml`
+format. ### Command Line Usage The command line interface consists of commands
+that can be chained together like a unix pipeline. ``` Usage: gitlab2prov
+[OPTIONS] COMMAND1 [ARGS]... [COMMAND2 [ARGS]...]... Extract provenance
+information from GitLab projects. Options: --version Show the version and exit.
+--verbose Enable logging to 'gitlab2prov.log'. --config FILE Read config from
+file. --validate FILE Validate config file and exit. --help Show this message
+and exit. Commands: combine Combine multiple graphs into one. extract Extract
+provenance information for one or more... load Load provenance files. merge-
+duplicated-agents Merge duplicated agents based on a name to... pseudonymize
+Pseudonymize a provenance graph. save Save provenance information to a file.
+stats Print statistics such as node counts and... ``` ### Configuration Files
+`gitlab2prov` supports configuration files in `.yaml` format that are
+functionally equivalent to command line invocations. To read configuration
+details from a file instead of specifying on the command line, use the `--
+config` option: ```ini # initiate a run using a config file gitlab2prov --
+config config/example.yaml ``` You can validate your config file using the
+provided JSON-Schema `gitlab2prov/config/schema.json` that comes packaged with
+every installation: ```ini # check config file for syntactical errors
+gitlab2prov --validate config/example.yaml ``` Config file example: ```yaml -
+extract: url: ["https://gitlab.com/example/foo"] token: tokenA - extract: url:
+["https://gitlab.com/example/bar"] token: tokenB - load: input: [example.rdf] -
+pseudonymize: - combine: - save: output: combined format: [json, rdf, xml, dot]
+- stats: fine: true explain: true formatter: table ``` The config file example
+is functionally equivalent to this command line invocation: ``` gitlab2prov
+extract -u https://gitlab.com/example/foo -t tokenFoo \ extract -u https://
+gitlab.com/example/bar -t tokenBar \ load -i example.rdf \ pseudonymize \
+combine \ save -o combined -f json -f rdf -f xml -f dot \ stats --fine --
+explain --formatter table ``` ### ð¨ Provenance Output Formats `gitlab2prov`
+supports output formats that the [`prov`](https://github.com/trungdong/prov)
+library provides: * [PROV-N](http://www.w3.org/TR/prov-n/) * [PROV-O](http://
+www.w3.org/TR/prov-o/) (RDF) * [PROV-XML](http://www.w3.org/TR/prov-xml/) *
+[PROV-JSON](http://www.w3.org/Submission/prov-json/) * [Graphviz](https://
+graphviz.org/) (DOT) ## ð¤ Contributing Contributions and pull requests are
+welcome! For major changes, please open an issue first to discuss what you
+would like to change. ## â¨ How to cite If you use GitLab2PROV in a scientific
+publication, we would appreciate citations to the following paper: * Schreiber,
+A., de Boer, C. and von Kurnatowski, L. (2021). [GitLab2PROVâProvenance of
+Software Projects hosted on GitLab](https://www.usenix.org/conference/tapp2021/
+presentation/schreiber). 13th International Workshop on Theory and Practice of
+Provenance (TaPP 2021), USENIX Association Bibtex entry: ```BibTeX
+@InProceedings{SchreiberBoerKurnatowski2021, author = {Andreas Schreiber and
+Claas de~Boer and Lynn von~Kurnatowski}, booktitle = {13th International
+Workshop on Theory and Practice of Provenance (TaPP 2021)}, title = {
+{GitLab2PROV}{\textemdash}Provenance of Software Projects hosted on GitLab},
+year = {2021}, month = jul, publisher = {{USENIX} Association}, url = {https://
+www.usenix.org/conference/tapp2021/presentation/schreiber}, } ``` You can also
+cite specific releases published on Zenodo: [![DOI](https://zenodo.org/badge/
+215042878.svg)](https://zenodo.org/badge/latestdoi/215042878) ## âï¸
+References **Influencial Software for `gitlab2prov`** * Martin Stoffers:
+"Gitlab2Graph", v1.0.0, October 13. 2019, [GitHub Link](https://github.com/DLR-
+SC/Gitlab2Graph), DOI 10.5281/zenodo.3469385 * Quentin Pradet: "How do you rate
+limit calls with aiohttp?", [GitHub Gist](https://gist.github.com/pquentin/
+5d8f5408cdad73e589d85ba509091741), MIT LICENSE **Influencial Papers for
+`gitlab2prov`**: * De Nies, T., Magliacane, S., Verborgh, R., Coppens, S.,
+Groth, P., Mannens, E., and Van de Walle, R. (2013). [Git2PROV: Exposing
+Version Control System Content as W3C PROV](https://dl.acm.org/doi/abs/10.5555/
+2874399.2874431). In *Poster and Demo Proceedings of the 12th International
+Semantic Web Conference* (Vol. 1035, pp. 125â128). * Packer, H. S., Chapman,
+A., and Carr, L. (2019). [GitHub2PROV: provenance for supporting software
+project management](https://dl.acm.org/doi/10.5555/3359032.3359039). In *11th
+International Workshop on Theory and Practice of Provenance (TaPP 2019)*.
+**Papers that refer to `gitlab2prov`**: * Andreas Schreiber, Claas de Boer
+(2020). [Modelling Knowledge about Software Processes using Provenance Graphs
+and its Application to Git-based VersionControl Systems](https://dl.acm.org/
+doi/10.1145/3387940.3392220). In *ICSEW'20: Proceedings of the IEEE/ACM 42nd
+Conference on Software Engineering Workshops* (pp. 358â359). * Tim Sonnekalb,
+Thomas S. Heinze, Lynn von Kurnatowski, Andreas Schreiber, Jesus M. Gonzalez-
+Barahona, and Heather Packer (2020). [Towards automated, provenance-driven
+security audit for git-based repositories: applied to germany's corona-warn-
+app: vision paper](https://doi.org/10.1145/3416507.3423190). In *Proceedings of
+the 3rd ACM SIGSOFT International Workshop on Software Security from Design to
+Deployment* (pp. 15â18). * Andreas Schreiber (2020). [Visualization of
+contributions to open-source projects](https://doi.org/10.1145/
+3430036.3430057). In *Proceedings of the 13th International Symposium on Visual
+Information Communication and Interaction*. ACM, USA. ## ð Dependencies
+`gitlab2prov` depends on several open source packages that are made freely
+available under their respective licenses. | Package | License | | ------------
+--------------------------------------------------- | -------------------------
+-------------------------------------------------------------------------------
+----------------- | | [GitPython](https://github.com/gitpython-developers/
+GitPython) | [![License](https://img.shields.io/badge/License-BSD_3--Clause-
+orange.svg)](https://opensource.org/licenses/BSD-3-Clause) | | [click](https://
+github.com/pallets/click) | [![License](https://img.shields.io/badge/License-
+BSD_3--Clause-orange.svg)](https://opensource.org/licenses/BSD-3-Clause) | |
+[python-gitlab](https://github.com/python-gitlab/python-gitlab) | [![License:
+LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://
+www.gnu.org/licenses/lgpl-3.0) | | [prov](https://pypi.org/project/prov/) | [!
+[License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
+opensource.org/licenses/MIT) | | [jsonschema](https://github.com/python-
+jsonschema/jsonschema) | [![License: MIT](https://img.shields.io/badge/License-
+MIT-yellow.svg)](https://opensource.org/licenses/MIT) | | [ruamel.yaml](https:/
+/pypi.org/project/ruamel.yaml/) | [![License: MIT](https://img.shields.io/
+badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) | | [pydot]
+(https://github.com/pydot/pydot) | [![License: MIT](https://img.shields.io/
+badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) | ## ð
+License This project is [MIT](https://github.com/dlr-sc/gitlab2prov/blob/
+master/LICENSE) licensed. Copyright Â© 2019 German Aerospace Center (DLR) and
+individual contributors.
```

### Comparing `gitlab2prov-2.0.0/README.md` & `gitlab2prov-2.1.0/gitlab2prov.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,53 @@
+Metadata-Version: 2.1
+Name: gitlab2prov
+Version: 2.1.0
+Summary: Extract provenance information (W3C PROV) from GitLab projects.
+Author-email: Claas de Boer <claas.deboer@dlr.de>
+Maintainer-email: Andreas Schreiber <andreas.schreiber@dlr.de>
+License: MIT License
+        
+        Copyright (c) 2019 German Aerospace Center (DLR)
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Twitter, https://twitter.com/dlr_software
+Project-URL: Source Code, https://github.com/dlr-sc/gitlab2prov
+Project-URL: Issue Tracker, https://github.com/dlr-sc/gitlab2prov/issues
+Keywords: prov,gitlab,git,provenance,prov generation,software analytics,w3c prov
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development :: Version Control :: Git
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 <h1 align="center">Welcome to <code>gitlab2prov</code>! 👋</h1>
 <p align="center">
   <a href="https://github.com/dlr-sc/gitlab2prov/blob/master/LICENSE">
     <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-yellow.svg" target="_blank" />
   </a>
   <a href="https://img.shields.io/badge/Made%20with-Python-1f425f.svg">
     <img src="https://img.shields.io/badge/Made%20with-Python-1f425f.svg" alt="Badge: Made with Python"/>
@@ -35,14 +81,16 @@
 ---
 
 The `gitlab2prov` data model has been designed according to [W3C PROV](https://www.w3.org/TR/prov-overview/) specification.
 The model documentation can be found [here](https://github.com/DLR-SC/gitlab2prov/tree/master/docs).
 
 ## ️🏗️ ️Installation
 
+Please note that this tool requires Git to be installed on your machine.
+
 Clone the project and install using `pip`:
 ```bash
 pip install .
 ```
 
 Or install the latest release from [PyPi](https://pypi.org/project/gitlab2prov/):
 ```bash
@@ -51,14 +99,20 @@
 
 To install `gitlab2prov` with all extra dependencies require the `[dev]` extras:
 ```bash
 pip install .[dev]            # clone repo, install with extras
 pip install gitlab2prov[dev]  # PyPi, install with extras
 ```
 
+## ⚡ Getting started
+
+`gitlab2prov` needs a [personal access token](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html) to clone git repositories and to authenticate with the GitLab API.
+Follow [this guide](./docs/guides/tokens.md) to create an access token with the required [scopes](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html#personal-access-token-scopes).
+
+
 ## 🚀‍ Usage
 
 `gitlab2prov` can be configured using the command line interface or by providing a configuration file in `.yaml` format.
 
 ###  Command Line Usage
 The command line interface consists of commands that can be chained together like a unix pipeline.
 
@@ -185,10 +239,23 @@
 
 * Andreas Schreiber, Claas de Boer (2020). [Modelling Knowledge about Software Processes using Provenance Graphs and its Application to Git-based VersionControl Systems](https://dl.acm.org/doi/10.1145/3387940.3392220). In *ICSEW'20: Proceedings of the IEEE/ACM 42nd Conference on Software Engineering Workshops* (pp. 358–359).
 
 * Tim Sonnekalb, Thomas S. Heinze, Lynn von Kurnatowski, Andreas Schreiber, Jesus M. Gonzalez-Barahona, and Heather Packer (2020). [Towards automated, provenance-driven security audit for git-based repositories: applied to germany's corona-warn-app: vision paper](https://doi.org/10.1145/3416507.3423190). In *Proceedings of the 3rd ACM SIGSOFT International Workshop on Software Security from Design to Deployment* (pp. 15–18).
 
 * Andreas Schreiber (2020). [Visualization of contributions to open-source projects](https://doi.org/10.1145/3430036.3430057). In *Proceedings of the 13th International Symposium on Visual Information Communication and Interaction*. ACM, USA.
 
+## 📜 Dependencies 
+`gitlab2prov` depends on several open source packages that are made freely available under their respective licenses.
+
+| Package                                                         | License                                                                                                                   |
+| --------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
+| [GitPython](https://github.com/gitpython-developers/GitPython)  | [![License](https://img.shields.io/badge/License-BSD_3--Clause-orange.svg)](https://opensource.org/licenses/BSD-3-Clause) |
+| [click](https://github.com/pallets/click)                       | [![License](https://img.shields.io/badge/License-BSD_3--Clause-orange.svg)](https://opensource.org/licenses/BSD-3-Clause) |
+| [python-gitlab](https://github.com/python-gitlab/python-gitlab) | [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)       |
+| [prov](https://pypi.org/project/prov/)                          | [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)               |
+| [jsonschema](https://github.com/python-jsonschema/jsonschema)   | [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)               |
+| [ruamel.yaml](https://pypi.org/project/ruamel.yaml/)            | [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)               |
+| [pydot](https://github.com/pydot/pydot)                         | [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)               |
+
 ## 📝 License
 This project is [MIT](https://github.com/dlr-sc/gitlab2prov/blob/master/LICENSE) licensed.  
 Copyright © 2019 German Aerospace Center (DLR) and individual contributors.
```

#### html2text {}

```diff
@@ -1,93 +1,151 @@
+Metadata-Version: 2.1 Name: gitlab2prov Version: 2.1.0 Summary: Extract
+provenance information (W3C PROV) from GitLab projects. Author-email: Claas de
+Boer
+deboer@dlr.de> Maintainer-email: Andreas Schreiber
+schreiber@dlr.de> License: MIT License Copyright (c) 2019 German Aerospace
+Center (DLR) Permission is hereby granted, free of charge, to any person
+obtaining a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including without
+limitation the rights to use, copy, modify, merge, publish, distribute,
+sublicense, and/or sell copies of the Software, and to permit persons to whom
+the Software is furnished to do so, subject to the following conditions: The
+above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
+IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
+LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
+AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Twitter,
+https://twitter.com/dlr_software Project-URL: Source Code, https://github.com/
+dlr-sc/gitlab2prov Project-URL: Issue Tracker, https://github.com/dlr-sc/
+gitlab2prov/issues Keywords: prov,gitlab,git,provenance,prov
+generation,software analytics,w3c prov Classifier: Development Status :: 5 -
+Production/Stable Classifier: Environment :: Console Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 :: Only Classifier: Topic :: Scientific/Engineering Classifier:
+Topic :: Scientific/Engineering :: Information Analysis Classifier: Topic ::
+Software Development :: Version Control :: Git Requires-Python: >=3.10
+Description-Content-Type: text/markdown Provides-Extra: dev License-File:
+LICENSE
                   ****** Welcome to gitlab2prov! ð ******
   [License:_MIT] [Badge:_Made_with_Python] [Badge:_PyPi_Version] [Badge:_PyPi
 Downloads_Monthly] [Twitter:_DLR_Software] [Badge:_Open_in_VSCode] [Badge:_DOI]
             [Badge:_W3C_PROV] [Badge:_Citation_File_Format_Inside]
 > `gitlab2prov` is a Python library and command line tool that extracts
 provenance information from GitLab projects. --- The `gitlab2prov` data model
 has been designed according to [W3C PROV](https://www.w3.org/TR/prov-overview/
 ) specification. The model documentation can be found [here](https://
 github.com/DLR-SC/gitlab2prov/tree/master/docs). ## ï¸ðï¸ ï¸Installation
-Clone the project and install using `pip`: ```bash pip install . ``` Or install
-the latest release from [PyPi](https://pypi.org/project/gitlab2prov/): ```bash
-pip install gitlab2prov ``` To install `gitlab2prov` with all extra
-dependencies require the `[dev]` extras: ```bash pip install .[dev] # clone
-repo, install with extras pip install gitlab2prov[dev] # PyPi, install with
-extras ``` ## ðâ Usage `gitlab2prov` can be configured using the command
-line interface or by providing a configuration file in `.yaml` format. ###
-Command Line Usage The command line interface consists of commands that can be
-chained together like a unix pipeline. ``` Usage: gitlab2prov [OPTIONS]
-COMMAND1 [ARGS]... [COMMAND2 [ARGS]...]... Extract provenance information from
-GitLab projects. Options: --version Show the version and exit. --verbose Enable
-logging to 'gitlab2prov.log'. --config FILE Read config from file. --validate
-FILE Validate config file and exit. --help Show this message and exit.
-Commands: combine Combine multiple graphs into one. extract Extract provenance
-information for one or more... load Load provenance files. merge-duplicated-
-agents Merge duplicated agents based on a name to... pseudonymize Pseudonymize
-a provenance graph. save Save provenance information to a file. stats Print
-statistics such as node counts and... ``` ### Configuration Files `gitlab2prov`
-supports configuration files in `.yaml` format that are functionally equivalent
-to command line invocations. To read configuration details from a file instead
-of specifying on the command line, use the `--config` option: ```ini # initiate
-a run using a config file gitlab2prov --config config/example.yaml ``` You can
-validate your config file using the provided JSON-Schema `gitlab2prov/config/
-schema.json` that comes packaged with every installation: ```ini # check config
-file for syntactical errors gitlab2prov --validate config/example.yaml ```
-Config file example: ```yaml - extract: url: ["https://gitlab.com/example/foo"]
-token: tokenA - extract: url: ["https://gitlab.com/example/bar"] token: tokenB
-- load: input: [example.rdf] - pseudonymize: - combine: - save: output:
-combined format: [json, rdf, xml, dot] - stats: fine: true explain: true
-formatter: table ``` The config file example is functionally equivalent to this
-command line invocation: ``` gitlab2prov extract -u https://gitlab.com/example/
-foo -t tokenFoo \ extract -u https://gitlab.com/example/bar -t tokenBar \ load
--i example.rdf \ pseudonymize \ combine \ save -o combined -f json -f rdf -
-f xml -f dot \ stats --fine --explain --formatter table ``` ### ð¨ Provenance
-Output Formats `gitlab2prov` supports output formats that the [`prov`](https://
-github.com/trungdong/prov) library provides: * [PROV-N](http://www.w3.org/TR/
-prov-n/) * [PROV-O](http://www.w3.org/TR/prov-o/) (RDF) * [PROV-XML](http://
-www.w3.org/TR/prov-xml/) * [PROV-JSON](http://www.w3.org/Submission/prov-json/
-) * [Graphviz](https://graphviz.org/) (DOT) ## ð¤ Contributing Contributions
-and pull requests are welcome! For major changes, please open an issue first to
-discuss what you would like to change. ## â¨ How to cite If you use
-GitLab2PROV in a scientific publication, we would appreciate citations to the
-following paper: * Schreiber, A., de Boer, C. and von Kurnatowski, L. (2021).
-[GitLab2PROVâProvenance of Software Projects hosted on GitLab](https://
-www.usenix.org/conference/tapp2021/presentation/schreiber). 13th International
-Workshop on Theory and Practice of Provenance (TaPP 2021), USENIX Association
-Bibtex entry: ```BibTeX @InProceedings{SchreiberBoerKurnatowski2021, author =
-{Andreas Schreiber and Claas de~Boer and Lynn von~Kurnatowski}, booktitle =
-{13th International Workshop on Theory and Practice of Provenance (TaPP 2021)},
-title = {{GitLab2PROV}{\textemdash}Provenance of Software Projects hosted on
-GitLab}, year = {2021}, month = jul, publisher = {{USENIX} Association}, url =
-{https://www.usenix.org/conference/tapp2021/presentation/schreiber}, } ``` You
-can also cite specific releases published on Zenodo: [![DOI](https://
-zenodo.org/badge/215042878.svg)](https://zenodo.org/badge/latestdoi/215042878)
-## âï¸ References **Influencial Software for `gitlab2prov`** * Martin
-Stoffers: "Gitlab2Graph", v1.0.0, October 13. 2019, [GitHub Link](https://
-github.com/DLR-SC/Gitlab2Graph), DOI 10.5281/zenodo.3469385 * Quentin Pradet:
-"How do you rate limit calls with aiohttp?", [GitHub Gist](https://
-gist.github.com/pquentin/5d8f5408cdad73e589d85ba509091741), MIT LICENSE
-**Influencial Papers for `gitlab2prov`**: * De Nies, T., Magliacane, S.,
-Verborgh, R., Coppens, S., Groth, P., Mannens, E., and Van de Walle, R. (2013).
-[Git2PROV: Exposing Version Control System Content as W3C PROV](https://
-dl.acm.org/doi/abs/10.5555/2874399.2874431). In *Poster and Demo Proceedings of
-the 12th International Semantic Web Conference* (Vol. 1035, pp. 125â128). *
-Packer, H. S., Chapman, A., and Carr, L. (2019). [GitHub2PROV: provenance for
-supporting software project management](https://dl.acm.org/doi/10.5555/
-3359032.3359039). In *11th International Workshop on Theory and Practice of
-Provenance (TaPP 2019)*. **Papers that refer to `gitlab2prov`**: * Andreas
-Schreiber, Claas de Boer (2020). [Modelling Knowledge about Software Processes
-using Provenance Graphs and its Application to Git-based VersionControl
-Systems](https://dl.acm.org/doi/10.1145/3387940.3392220). In *ICSEW'20:
-Proceedings of the IEEE/ACM 42nd Conference on Software Engineering Workshops*
-(pp. 358â359). * Tim Sonnekalb, Thomas S. Heinze, Lynn von Kurnatowski,
-Andreas Schreiber, Jesus M. Gonzalez-Barahona, and Heather Packer (2020).
-[Towards automated, provenance-driven security audit for git-based
-repositories: applied to germany's corona-warn-app: vision paper](https://
-doi.org/10.1145/3416507.3423190). In *Proceedings of the 3rd ACM SIGSOFT
-International Workshop on Software Security from Design to Deployment* (pp.
-15â18). * Andreas Schreiber (2020). [Visualization of contributions to open-
-source projects](https://doi.org/10.1145/3430036.3430057). In *Proceedings of
-the 13th International Symposium on Visual Information Communication and
-Interaction*. ACM, USA. ## ð License This project is [MIT](https://
-github.com/dlr-sc/gitlab2prov/blob/master/LICENSE) licensed. Copyright Â© 2019
-German Aerospace Center (DLR) and individual contributors.
+Please note that this tool requires Git to be installed on your machine. Clone
+the project and install using `pip`: ```bash pip install . ``` Or install the
+latest release from [PyPi](https://pypi.org/project/gitlab2prov/): ```bash pip
+install gitlab2prov ``` To install `gitlab2prov` with all extra dependencies
+require the `[dev]` extras: ```bash pip install .[dev] # clone repo, install
+with extras pip install gitlab2prov[dev] # PyPi, install with extras ``` ## â¡
+Getting started `gitlab2prov` needs a [personal access token](https://
+docs.gitlab.com/ee/user/profile/personal_access_tokens.html) to clone git
+repositories and to authenticate with the GitLab API. Follow [this guide](./
+docs/guides/tokens.md) to create an access token with the required [scopes]
+(https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html#personal-
+access-token-scopes). ## ðâ Usage `gitlab2prov` can be configured using
+the command line interface or by providing a configuration file in `.yaml`
+format. ### Command Line Usage The command line interface consists of commands
+that can be chained together like a unix pipeline. ``` Usage: gitlab2prov
+[OPTIONS] COMMAND1 [ARGS]... [COMMAND2 [ARGS]...]... Extract provenance
+information from GitLab projects. Options: --version Show the version and exit.
+--verbose Enable logging to 'gitlab2prov.log'. --config FILE Read config from
+file. --validate FILE Validate config file and exit. --help Show this message
+and exit. Commands: combine Combine multiple graphs into one. extract Extract
+provenance information for one or more... load Load provenance files. merge-
+duplicated-agents Merge duplicated agents based on a name to... pseudonymize
+Pseudonymize a provenance graph. save Save provenance information to a file.
+stats Print statistics such as node counts and... ``` ### Configuration Files
+`gitlab2prov` supports configuration files in `.yaml` format that are
+functionally equivalent to command line invocations. To read configuration
+details from a file instead of specifying on the command line, use the `--
+config` option: ```ini # initiate a run using a config file gitlab2prov --
+config config/example.yaml ``` You can validate your config file using the
+provided JSON-Schema `gitlab2prov/config/schema.json` that comes packaged with
+every installation: ```ini # check config file for syntactical errors
+gitlab2prov --validate config/example.yaml ``` Config file example: ```yaml -
+extract: url: ["https://gitlab.com/example/foo"] token: tokenA - extract: url:
+["https://gitlab.com/example/bar"] token: tokenB - load: input: [example.rdf] -
+pseudonymize: - combine: - save: output: combined format: [json, rdf, xml, dot]
+- stats: fine: true explain: true formatter: table ``` The config file example
+is functionally equivalent to this command line invocation: ``` gitlab2prov
+extract -u https://gitlab.com/example/foo -t tokenFoo \ extract -u https://
+gitlab.com/example/bar -t tokenBar \ load -i example.rdf \ pseudonymize \
+combine \ save -o combined -f json -f rdf -f xml -f dot \ stats --fine --
+explain --formatter table ``` ### ð¨ Provenance Output Formats `gitlab2prov`
+supports output formats that the [`prov`](https://github.com/trungdong/prov)
+library provides: * [PROV-N](http://www.w3.org/TR/prov-n/) * [PROV-O](http://
+www.w3.org/TR/prov-o/) (RDF) * [PROV-XML](http://www.w3.org/TR/prov-xml/) *
+[PROV-JSON](http://www.w3.org/Submission/prov-json/) * [Graphviz](https://
+graphviz.org/) (DOT) ## ð¤ Contributing Contributions and pull requests are
+welcome! For major changes, please open an issue first to discuss what you
+would like to change. ## â¨ How to cite If you use GitLab2PROV in a scientific
+publication, we would appreciate citations to the following paper: * Schreiber,
+A., de Boer, C. and von Kurnatowski, L. (2021). [GitLab2PROVâProvenance of
+Software Projects hosted on GitLab](https://www.usenix.org/conference/tapp2021/
+presentation/schreiber). 13th International Workshop on Theory and Practice of
+Provenance (TaPP 2021), USENIX Association Bibtex entry: ```BibTeX
+@InProceedings{SchreiberBoerKurnatowski2021, author = {Andreas Schreiber and
+Claas de~Boer and Lynn von~Kurnatowski}, booktitle = {13th International
+Workshop on Theory and Practice of Provenance (TaPP 2021)}, title = {
+{GitLab2PROV}{\textemdash}Provenance of Software Projects hosted on GitLab},
+year = {2021}, month = jul, publisher = {{USENIX} Association}, url = {https://
+www.usenix.org/conference/tapp2021/presentation/schreiber}, } ``` You can also
+cite specific releases published on Zenodo: [![DOI](https://zenodo.org/badge/
+215042878.svg)](https://zenodo.org/badge/latestdoi/215042878) ## âï¸
+References **Influencial Software for `gitlab2prov`** * Martin Stoffers:
+"Gitlab2Graph", v1.0.0, October 13. 2019, [GitHub Link](https://github.com/DLR-
+SC/Gitlab2Graph), DOI 10.5281/zenodo.3469385 * Quentin Pradet: "How do you rate
+limit calls with aiohttp?", [GitHub Gist](https://gist.github.com/pquentin/
+5d8f5408cdad73e589d85ba509091741), MIT LICENSE **Influencial Papers for
+`gitlab2prov`**: * De Nies, T., Magliacane, S., Verborgh, R., Coppens, S.,
+Groth, P., Mannens, E., and Van de Walle, R. (2013). [Git2PROV: Exposing
+Version Control System Content as W3C PROV](https://dl.acm.org/doi/abs/10.5555/
+2874399.2874431). In *Poster and Demo Proceedings of the 12th International
+Semantic Web Conference* (Vol. 1035, pp. 125â128). * Packer, H. S., Chapman,
+A., and Carr, L. (2019). [GitHub2PROV: provenance for supporting software
+project management](https://dl.acm.org/doi/10.5555/3359032.3359039). In *11th
+International Workshop on Theory and Practice of Provenance (TaPP 2019)*.
+**Papers that refer to `gitlab2prov`**: * Andreas Schreiber, Claas de Boer
+(2020). [Modelling Knowledge about Software Processes using Provenance Graphs
+and its Application to Git-based VersionControl Systems](https://dl.acm.org/
+doi/10.1145/3387940.3392220). In *ICSEW'20: Proceedings of the IEEE/ACM 42nd
+Conference on Software Engineering Workshops* (pp. 358â359). * Tim Sonnekalb,
+Thomas S. Heinze, Lynn von Kurnatowski, Andreas Schreiber, Jesus M. Gonzalez-
+Barahona, and Heather Packer (2020). [Towards automated, provenance-driven
+security audit for git-based repositories: applied to germany's corona-warn-
+app: vision paper](https://doi.org/10.1145/3416507.3423190). In *Proceedings of
+the 3rd ACM SIGSOFT International Workshop on Software Security from Design to
+Deployment* (pp. 15â18). * Andreas Schreiber (2020). [Visualization of
+contributions to open-source projects](https://doi.org/10.1145/
+3430036.3430057). In *Proceedings of the 13th International Symposium on Visual
+Information Communication and Interaction*. ACM, USA. ## ð Dependencies
+`gitlab2prov` depends on several open source packages that are made freely
+available under their respective licenses. | Package | License | | ------------
+--------------------------------------------------- | -------------------------
+-------------------------------------------------------------------------------
+----------------- | | [GitPython](https://github.com/gitpython-developers/
+GitPython) | [![License](https://img.shields.io/badge/License-BSD_3--Clause-
+orange.svg)](https://opensource.org/licenses/BSD-3-Clause) | | [click](https://
+github.com/pallets/click) | [![License](https://img.shields.io/badge/License-
+BSD_3--Clause-orange.svg)](https://opensource.org/licenses/BSD-3-Clause) | |
+[python-gitlab](https://github.com/python-gitlab/python-gitlab) | [![License:
+LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://
+www.gnu.org/licenses/lgpl-3.0) | | [prov](https://pypi.org/project/prov/) | [!
+[License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
+opensource.org/licenses/MIT) | | [jsonschema](https://github.com/python-
+jsonschema/jsonschema) | [![License: MIT](https://img.shields.io/badge/License-
+MIT-yellow.svg)](https://opensource.org/licenses/MIT) | | [ruamel.yaml](https:/
+/pypi.org/project/ruamel.yaml/) | [![License: MIT](https://img.shields.io/
+badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) | | [pydot]
+(https://github.com/pydot/pydot) | [![License: MIT](https://img.shields.io/
+badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) | ## ð
+License This project is [MIT](https://github.com/dlr-sc/gitlab2prov/blob/
+master/LICENSE) licensed. Copyright Â© 2019 German Aerospace Center (DLR) and
+individual contributors.
```

### Comparing `gitlab2prov-2.0.0/gitlab2prov/adapters/fetch/annotations/classifiers.py` & `gitlab2prov-2.1.0/gitlab2prov/adapters/fetch/annotations/classifiers.py`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/gitlab2prov/adapters/fetch/annotations/parse.py` & `gitlab2prov-2.1.0/gitlab2prov/adapters/fetch/annotations/parse.py`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/gitlab2prov/adapters/fetch/git.py` & `gitlab2prov-2.1.0/gitlab2prov/adapters/fetch/git.py`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/gitlab2prov/adapters/fetch/gitlab.py` & `gitlab2prov-2.1.0/gitlab2prov/adapters/fetch/gitlab.py`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/gitlab2prov/adapters/repository.py` & `gitlab2prov-2.1.0/gitlab2prov/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/gitlab2prov/bootstrap.py` & `gitlab2prov-2.1.0/gitlab2prov/bootstrap.py`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/gitlab2prov/config/parser.py` & `gitlab2prov-2.1.0/gitlab2prov/config/parser.py`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/gitlab2prov/domain/constants.py` & `gitlab2prov-2.1.0/gitlab2prov/domain/constants.py`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/gitlab2prov/domain/objects.py` & `gitlab2prov-2.1.0/gitlab2prov/domain/objects.py`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/gitlab2prov/entrypoints/cli.py` & `gitlab2prov-2.1.0/gitlab2prov/entrypoints/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 from functools import partial
 from functools import update_wrapper
 from functools import wraps
 
 import click
+import git
 
 from gitlab2prov import __version__
 from gitlab2prov import bootstrap
 from gitlab2prov.config import ConfigParser
 from gitlab2prov.domain import commands
 from gitlab2prov.log import create_logger
 from gitlab2prov.prov import operations
 
 
+def is_git_available():
+    """Check whether git is installed using the GitPython package."""
+    try:
+        git.Git().execute(["git", "--version"])
+        return True
+    except git.exc.GitCommandNotFound:
+        return False
+
+
 def enable_logging(ctx: click.Context, _, enable: bool):
     """Callback that optionally enables logging."""
     if enable:
         create_logger()
 
 
 def invoke_from_config(ctx: click.Context, _, filepath: str):
@@ -93,14 +103,16 @@
     help="Validate config file and exit.",
 )
 @click.pass_context
 def cli(ctx):
     """
     Extract provenance information from GitLab projects.
     """
+    if not is_git_available():
+        ctx.fail("Could not find git. Please install git.")
     ctx.obj = bootstrap.bootstrap()
 
 
 @cli.result_callback()
 def process_commands(processors, **kwargs):
     """This result callback is invoked with an iterable of all the chained
     subcommands.  As each subcommand returns a function
@@ -116,21 +128,23 @@
 
     # Evaluate the stream and throw away the items.
     for _ in stream:
         pass
 
 
 @cli.command("extract")
-@click.option("-u", "--url", "urls", multiple=True, type=str, required=True, help="Project url[s].")
+@click.option(
+    "-u", "--url", "urls", multiple=True, type=str, required=True, help="Project url[s]."
+)
 @click.option("-t", "--token", required=True, type=str, help="Gitlab API token.")
 @click.pass_obj
 @generator
 def do_extract(bus, urls: list[str], token: str):
     """Extract provenance information for one or more gitlab projects.
-    
+
     This command extracts provenance information from one or multiple gitlab projects.
     The extracted provenance is returned as a combined provenance graph.
     """
     for url in urls:
         bus.handle(commands.Fetch(url, token))
 
     graph = bus.handle(commands.Serialize())
@@ -147,15 +161,15 @@
     multiple=True,
     type=click.Path(exists=True, dir_okay=False),
     help="Provenance file path (specify '-' to read from <stdin>).",
 )
 @generator
 def load(input):
     """Load provenance information from a file.
-    
+
     This command reads one provenance graph from a file or multiple graphs from multiple files.
     """
     for filepath in input:
         try:
             if filepath == "-":
                 graph = operations.deserialize_graph()
                 graph.description = f"'<stdin>'"
@@ -182,15 +196,15 @@
     "--output",
     default="gitlab2prov-graph-{:04}",
     help="Output file path.",
 )
 @processor
 def save(graphs, format, output):
     """Save provenance information to a file.
-    
+
     This command writes each provenance graph that is piped to it to a file.
     """
     for idx, graph in enumerate(graphs, start=1):
         for fmt in format:
             try:
                 serialized = operations.serialize_graph(graph, fmt)
                 if output == "-":
@@ -203,15 +217,15 @@
         yield graph
 
 
 @cli.command("pseudonymize")
 @processor
 def pseudonymize(graphs):
     """Pseudonymize a provenance graph.
-    
+
     This command pseudonymizes each provenance graph that is piped to it.
     """
     for graph in graphs:
         try:
             pseud = operations.pseudonymize(graph)
             pseud.description = f"pseudonymized {graph.description}"
             yield pseud
@@ -219,37 +233,53 @@
             click.echo(f"Could not pseudonymize {graph.description}: {e}", err=True)
 
 
 @cli.command("combine")
 @processor
 def combine(graphs):
     """Combine multiple graphs into one.
-    
+
     This command combines all graphs that are piped to it into one.
     """
     graphs = list(graphs)
     try:
         combined = operations.combine(iter(graphs))
         descriptions = ", ".join(graph.description for graph in graphs)
         combined.description = f"combination of {descriptions}"
         yield combined
     except Exception as e:
         descriptions = "with ".join(graph.description for graph in graphs)
         click.echo(f"Could not combine {descriptions}: {e}", err=True)
 
 
 @cli.command("stats")
-@click.option("--coarse", "resolution", flag_value="coarse", default=True, help="Print the number of PROV elements aswell as the overall number of relations.")
-@click.option("--fine", "resolution", flag_value="fine", help="Print the number of PROV elements aswell as the number of PROV relations for each relation type.")
-@click.option("--explain", "show_description", is_flag=True, help="Print a textual summary of all operations applied to the graphs.")
+@click.option(
+    "--coarse",
+    "resolution",
+    flag_value="coarse",
+    default=True,
+    help="Print the number of PROV elements aswell as the overall number of relations.",
+)
+@click.option(
+    "--fine",
+    "resolution",
+    flag_value="fine",
+    help="Print the number of PROV elements aswell as the number of PROV relations for each relation type.",
+)
+@click.option(
+    "--explain",
+    "show_description",
+    is_flag=True,
+    help="Print a textual summary of all operations applied to the graphs.",
+)
 @click.option("--formatter", type=click.Choice(["csv", "table"]), default="table")
 @processor
 def stats(graphs, resolution, show_description, formatter):
     """Print statistics such as node counts and relation counts.
-    
+
     This command prints statistics for each processed provenance graph.
     Statistics include the number of elements for each element type aswell as the number of relations for each relation type.
     Optionally, a short textual summary of all operations applied to the processed graphs can be printed to stdout.
     """
     for graph in graphs:
         try:
             if show_description:
@@ -273,15 +303,15 @@
     "--mapping",
     type=click.Path(exists=True, dir_okay=False),
     help="File path to duplicate agent mapping.",
 )
 @processor
 def merge_duplicated_agents(graphs, mapping):
     """Merge duplicated agents based on a name to aliases mapping.
-    
+
     This command solves the problem of duplicated agents that can occur when the same physical user
     uses different user names and emails for his git and gitlab account.
     Based on a mapping of names to aliases the duplicated agents can be merged.
     """
     for graph in graphs:
         graph = operations.merge_duplicated_agents(graph, mapping)
         graph.description += f"merged double agents {graph.description}"
```

### Comparing `gitlab2prov-2.0.0/gitlab2prov/prov/model.py` & `gitlab2prov-2.1.0/gitlab2prov/prov/model.py`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/gitlab2prov/prov/operations.py` & `gitlab2prov-2.1.0/gitlab2prov/prov/operations.py`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/gitlab2prov/service_layer/handlers.py` & `gitlab2prov-2.1.0/gitlab2prov/service_layer/handlers.py`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/gitlab2prov/service_layer/messagebus.py` & `gitlab2prov-2.1.0/gitlab2prov/service_layer/messagebus.py`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/gitlab2prov/service_layer/unit_of_work.py` & `gitlab2prov-2.1.0/gitlab2prov/service_layer/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/gitlab2prov.egg-info/SOURCES.txt` & `gitlab2prov-2.1.0/gitlab2prov.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab2prov-2.0.0/pyproject.toml` & `gitlab2prov-2.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 [build-system]
-requires = ["setuptools>=65.0", "wheel"]
+requires = [
+    "setuptools>=65.0", # MIT License
+    "wheel",            # MIT License
+]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gitlab2prov"
 description = "Extract provenance information (W3C PROV) from GitLab projects."
 requires-python = ">=3.10"
 readme = { file = "README.md", content-type = "text/markdown" }
 license = { file = "LICENSE" }
 authors = [{ name = "Claas de Boer", email = "claas.deboer@dlr.de" }]
 maintainers = [
     { name = "Andreas Schreiber", email = "andreas.schreiber@dlr.de" },
 ]
-dependencies = ["prov>=2.0.0", "git-python", "python-gitlab", "jsonschema", "ruamel.yaml", "pydot>=1.2.0"]
+dependencies = [
+    "prov>=2.0.0",   # MIT License
+    "git-python",    # BSD 3-Clause License
+    "python-gitlab", # LGPL-3.0 License
+    "jsonschema",    # MIT License
+    "ruamel.yaml",   # MIt License
+    "pydot>=1.2.0",  # MIT License
+    "click",         # BSD 3-Clause License
+]
 keywords = [
     "prov",
     "gitlab",
     "git",
     "provenance",
     "prov generation",
     "software analytics",
@@ -32,15 +43,21 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Software Development :: Version Control :: Git",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-dev = ["pytest", "pytest-mock", "black", "isort", "bump2version"]
+dev = [
+    "pytest",       # MIT License
+    "pytest-mock",  # MIT License
+    "black",        # MIT License
+    "isort",        # MIT License
+    "bump2version", # MIT License
+]
 
 [project.scripts]
 gitlab2prov = "gitlab2prov.entrypoints.cli:cli"
 
 [project.urls]
 Twitter = "https://twitter.com/dlr_software"
 "Source Code" = "https://github.com/dlr-sc/gitlab2prov"
```

