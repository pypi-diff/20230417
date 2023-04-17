# Comparing `tmp/py-build-cmake-0.1.7.tar.gz` & `tmp/py-build-cmake-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-build-cmake-0.1.7.tar", last modified: Sun Apr 16 00:43:24 2023, max compression
+gzip compressed data, was "py-build-cmake-0.1.8.tar", last modified: Mon Apr 17 16:20:23 2023, max compression
```

## Comparing `py-build-cmake-0.1.7.tar` & `py-build-cmake-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1065 2023-04-16 00:43:05.473989 py-build-cmake-0.1.7/LICENSE
--rw-r--r--   0        0        0     5147 2023-04-16 00:43:05.474225 py-build-cmake-0.1.7/README.md
--rw-r--r--   0        0        0     1400 2023-04-16 00:43:05.527303 py-build-cmake-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      133 2023-04-16 00:43:05.528112 py-build-cmake-0.1.7/src/py_build_cmake/__init__.py
--rw-r--r--   0        0        0    30441 2023-04-16 00:43:05.528502 py-build-cmake-0.1.7/src/py_build_cmake/build.py
--rw-r--r--   0        0        0     9139 2023-04-16 00:43:05.528834 py-build-cmake-0.1.7/src/py_build_cmake/build_component.py
--rw-r--r--   0        0        0    10451 2023-04-16 00:43:05.529134 py-build-cmake-0.1.7/src/py_build_cmake/cli.py
--rw-r--r--   0        0        0     7896 2023-04-16 00:43:05.529402 py-build-cmake-0.1.7/src/py_build_cmake/cmake.py
--rw-r--r--   0        0        0     2393 2023-04-16 00:43:05.529648 py-build-cmake-0.1.7/src/py_build_cmake/cmd_runner.py
--rw-r--r--   0        0        0     9717 2023-04-16 00:43:05.529910 py-build-cmake-0.1.7/src/py_build_cmake/config.py
--rw-r--r--   0        0        0    28479 2023-04-16 00:43:05.530274 py-build-cmake-0.1.7/src/py_build_cmake/config_options.py
--rw-r--r--   0        0        0      289 2023-04-16 00:43:05.530549 py-build-cmake-0.1.7/src/py_build_cmake/datastructures.py
--rw-r--r--   0        0        0     4105 2023-04-16 00:43:05.530872 py-build-cmake-0.1.7/src/py_build_cmake/help/__init__.py
--rw-r--r--   0        0        0      173 2023-04-16 00:43:05.531112 py-build-cmake-0.1.7/src/py_build_cmake/help/__main__.py
--rw-r--r--   0        0        0        0 2023-04-16 00:43:05.531249 py-build-cmake-0.1.7/src/py_build_cmake/py.typed
--rw-r--r--   0        0        0    20011 2023-04-16 00:43:05.531551 py-build-cmake-0.1.7/src/py_build_cmake/pyproject_options.py
--rw-r--r--   0        0        0     2529 2023-04-16 00:43:05.531834 py-build-cmake-0.1.7/src/py_build_cmake/tags.py
--rw-r--r--   0        0        0     6305 1970-01-01 00:00:00.000000 py-build-cmake-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-04-17 16:18:08.007226 py-build-cmake-0.1.8/LICENSE
+-rw-r--r--   0        0        0     5271 2023-04-17 16:18:08.007226 py-build-cmake-0.1.8/README.md
+-rw-r--r--   0        0        0     1446 2023-04-17 16:18:08.054101 py-build-cmake-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      137 2023-04-17 16:18:08.054101 py-build-cmake-0.1.8/src/py_build_cmake/__init__.py
+-rw-r--r--   0        0        0    31176 2023-04-17 16:18:08.054101 py-build-cmake-0.1.8/src/py_build_cmake/build.py
+-rw-r--r--   0        0        0     9434 2023-04-17 16:18:08.054101 py-build-cmake-0.1.8/src/py_build_cmake/build_component.py
+-rw-r--r--   0        0        0    10712 2023-04-17 16:18:08.054101 py-build-cmake-0.1.8/src/py_build_cmake/cli.py
+-rw-r--r--   0        0        0     8112 2023-04-17 16:18:08.054101 py-build-cmake-0.1.8/src/py_build_cmake/cmake.py
+-rw-r--r--   0        0        0     2459 2023-04-17 16:18:08.054101 py-build-cmake-0.1.8/src/py_build_cmake/cmd_runner.py
+-rw-r--r--   0        0        0     9981 2023-04-17 16:18:08.054101 py-build-cmake-0.1.8/src/py_build_cmake/config.py
+-rw-r--r--   0        0        0    29249 2023-04-17 16:18:08.054101 py-build-cmake-0.1.8/src/py_build_cmake/config_options.py
+-rw-r--r--   0        0        0      306 2023-04-17 16:18:08.054101 py-build-cmake-0.1.8/src/py_build_cmake/datastructures.py
+-rw-r--r--   0        0        0     4217 2023-04-17 16:18:08.054101 py-build-cmake-0.1.8/src/py_build_cmake/help/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-17 16:18:08.054101 py-build-cmake-0.1.8/src/py_build_cmake/help/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-17 16:18:08.054101 py-build-cmake-0.1.8/src/py_build_cmake/py.typed
+-rw-r--r--   0        0        0    20405 2023-04-17 16:18:08.054101 py-build-cmake-0.1.8/src/py_build_cmake/pyproject_options.py
+-rw-r--r--   0        0        0     2612 2023-04-17 16:18:08.054101 py-build-cmake-0.1.8/src/py_build_cmake/tags.py
+-rw-r--r--   0        0        0     6305 1970-01-01 00:00:00.000000 py-build-cmake-0.1.8/PKG-INFO
```

### Comparing `py-build-cmake-0.1.7/README.md` & `py-build-cmake-0.1.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-[![Python Wheel](https://github.com/tttapa/py-build-cmake/actions/workflows/wheel.yml/badge.svg)](https://github.com/tttapa/py-build-cmake/actions/workflows/wheel.yml)
-[![Documentation](https://img.shields.io/badge/Documentation-main-blue)](https://tttapa.github.io/py-build-cmake)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/py-build-cmake?label=PyPI)](https://pypi.org/project/py-build-cmake)
-
-# py-build-cmake
-
-Modern, [PEP 517](https://www.python.org/dev/peps/pep-0517/) compliant build
-backend for creating Python packages with extensions built using CMake.
-
-## Features
-
- - Building and packaging C, C++ or Fortran extension modules for Python using CMake
- - Declarative configuration using `pyproject.toml` ([PEP 621](https://www.python.org/dev/peps/pep-0621/)), compatible with
-   [flit](https://github.com/pypa/flit)
- - Editable/development installations for Python modules ([PEP 660](https://www.python.org/dev/peps/pep-0660/))
- - Compatible with [pybind11](https://github.com/pybind/pybind11) and [nanobind](https://github.com/wjakob/nanobind)
- - Stub generation for type checking and autocompletion
- - Customizable CMake configuration, build and installation options
- - Support for multiple installation configurations and components
- - Cross-compilation support
- - No dependency on [setuptools](https://github.com/pypa/setuptools)
- - Compatible with [cibuildwheel](https://github.com/pypa/cibuildwheel) for building Wheels
-
-## Installation
-
-The py-build-cmake package is available on
-[PyPI](https://pypi.org/project/py-build-cmake/):
-
-```sh
-pip install py-build-cmake
-```
-
-## Documentation
-
-The documentation can be found on <https://tttapa.github.io/py-build-cmake>.
-
-The format of the configuration file is explained in 
-[Config.md](https://tttapa.github.io/py-build-cmake/Config.html).
-
-Alternatively, use the [command-line interface](https://tttapa.github.io/py-build-cmake/CLI.html)
-to get the documentation for all supported options:
-```sh
-py-build-cmake config format
-```
-
-## Usage
-
-If you don't have one already, add a `pyproject.toml` configuration file to your
-project's repository. Specify the metadata required by [PEP 621](https://www.python.org/dev/peps/pep-0621/),
-and tell py-build-cmake how to build your project. For example:
-
-```toml
-[project] # Project metadata
-name = "example-project"
-readme = "README.md"
-requires-python = ">=3.7"
-license = { "file" = "LICENSE" }
-authors = [{ "name" = "Pieter P", "email" = "pieter.p.dev@outlook.com" }]
-keywords = ["some", "keywords"]
-classifiers = ["Topic :: Scientific/Engineering"]
-urls = { "Documentation" = "https://tttapa.github.io/py-build-cmake" }
-dependencies = ["numpy"]
-dynamic = ["version", "description"]
-
-[build-system] # How pip and other frontends should build this project
-requires = ["py-build-cmake~=0.1.7"]
-build-backend = "py_build_cmake.build"
-
-[tool.py-build-cmake.module] # Where to find the Python module to package
-directory = "src-python"
-
-[tool.py-build-cmake.sdist] # What to include in source distributions
-include = ["CMakeLists.txt", "src/*"]
-
-[tool.py-build-cmake.cmake] # How to build the CMake project
-build_type = "RelWithDebInfo"
-source_path = "src"
-build_args = ["-j"]
-install_components = ["python_modules"]
-
-[tool.py-build-cmake.stubgen] # Whether and how to generate typed stub files
-```
-The README of [`examples/minimal`](https://github.com/tttapa/py-build-cmake/tree/main/examples/minimal)
-describes this configuration file in much more detail.
-
-Then use [`pip`](https://github.com/pypa/pip), [`build`](https://github.com/pypa/build)
-or another PEP 517 compatible frontend to build and/or install the package.
-
-Build sdist and wheel packages you can upload to PyPI:
-```sh
-python -m pip install -U build
-python -m build . # find the sdist and wheel file in the 'dist' folder
-```
-
-Install the package in the current environment:
-```sh
-pip install .    # normal installation
-pip install -e . # editable installation
-```
-
-## Examples
-
-As an introduction to py-build-cmake, see [`examples/minimal`](https://github.com/tttapa/py-build-cmake/tree/main/examples/minimal)
-for a detailed overview of the configuration files and the directory structure,
-using a very simple Python module as an example.  
-For a more advanced, real-world example, see [`examples/pybind11-project`](https://github.com/tttapa/py-build-cmake/tree/main/examples/pybind11-project)
-and [`examples/nanobind-project`](https://github.com/tttapa/py-build-cmake/tree/main/examples/nanobind-project).  
-If you are interested in packaging C/C++/Fortran programs using py-build-cmake,
-have a look at [`examples/minimal-program`](https://github.com/tttapa/py-build-cmake/tree/main/examples/minimal-program).
-
-## Projects using py-build-cmake
-
-If you need more examples, you can look at the following projects using
-py-build-cmake as their Python build backend:
-
-- [alpaqa](https://github.com/kul-optec/alpaqa/tree/develop)
-- [QPALM](https://github.com/kul-optec/QPALM)
-
-## Planned features
-
- - [x] ~~macOS support~~
- - [x] ~~Entry point support~~
- - [ ] Namespace package support ([PEP 420](https://www.python.org/dev/peps/pep-0420/))
- - [ ] Doxygen and Sphinx support
+[![Python Wheel](https://github.com/tttapa/py-build-cmake/actions/workflows/wheel.yml/badge.svg)](https://github.com/tttapa/py-build-cmake/actions/workflows/wheel.yml)
+[![Documentation](https://img.shields.io/badge/Documentation-main-blue)](https://tttapa.github.io/py-build-cmake)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/py-build-cmake?label=PyPI)](https://pypi.org/project/py-build-cmake)
+
+# py-build-cmake
+
+Modern, [PEP 517](https://www.python.org/dev/peps/pep-0517/) compliant build
+backend for creating Python packages with extensions built using CMake.
+
+## Features
+
+ - Building and packaging C, C++ or Fortran extension modules for Python using CMake
+ - Declarative configuration using `pyproject.toml` ([PEP 621](https://www.python.org/dev/peps/pep-0621/)), compatible with
+   [flit](https://github.com/pypa/flit)
+ - Editable/development installations for Python modules ([PEP 660](https://www.python.org/dev/peps/pep-0660/))
+ - Compatible with [pybind11](https://github.com/pybind/pybind11) and [nanobind](https://github.com/wjakob/nanobind)
+ - Stub generation for type checking and autocompletion
+ - Customizable CMake configuration, build and installation options
+ - Support for multiple installation configurations and components
+ - Cross-compilation support
+ - No dependency on [setuptools](https://github.com/pypa/setuptools)
+ - Compatible with [cibuildwheel](https://github.com/pypa/cibuildwheel) for building Wheels
+
+## Installation
+
+The py-build-cmake package is available on
+[PyPI](https://pypi.org/project/py-build-cmake/):
+
+```sh
+pip install py-build-cmake
+```
+
+## Documentation
+
+The documentation can be found on <https://tttapa.github.io/py-build-cmake>.
+
+The format of the configuration file is explained in 
+[Config.md](https://tttapa.github.io/py-build-cmake/Config.html).
+
+Alternatively, use the [command-line interface](https://tttapa.github.io/py-build-cmake/CLI.html)
+to get the documentation for all supported options:
+```sh
+py-build-cmake config format
+```
+
+## Usage
+
+If you don't have one already, add a `pyproject.toml` configuration file to your
+project's repository. Specify the metadata required by [PEP 621](https://www.python.org/dev/peps/pep-0621/),
+and tell py-build-cmake how to build your project. For example:
+
+```toml
+[project] # Project metadata
+name = "example-project"
+readme = "README.md"
+requires-python = ">=3.7"
+license = { "file" = "LICENSE" }
+authors = [{ "name" = "Pieter P", "email" = "pieter.p.dev@outlook.com" }]
+keywords = ["some", "keywords"]
+classifiers = ["Topic :: Scientific/Engineering"]
+urls = { "Documentation" = "https://tttapa.github.io/py-build-cmake" }
+dependencies = ["numpy"]
+dynamic = ["version", "description"]
+
+[build-system] # How pip and other frontends should build this project
+requires = ["py-build-cmake~=0.1.8"]
+build-backend = "py_build_cmake.build"
+
+[tool.py-build-cmake.module] # Where to find the Python module to package
+directory = "src-python"
+
+[tool.py-build-cmake.sdist] # What to include in source distributions
+include = ["CMakeLists.txt", "src/*"]
+
+[tool.py-build-cmake.cmake] # How to build the CMake project
+build_type = "RelWithDebInfo"
+source_path = "src"
+build_args = ["-j"]
+install_components = ["python_modules"]
+
+[tool.py-build-cmake.stubgen] # Whether and how to generate typed stub files
+```
+The README of [`examples/minimal`](https://github.com/tttapa/py-build-cmake/tree/main/examples/minimal)
+describes this configuration file in much more detail.
+
+Then use [`pip`](https://github.com/pypa/pip), [`build`](https://github.com/pypa/build)
+or another PEP 517 compatible frontend to build and/or install the package.
+
+Build sdist and wheel packages you can upload to PyPI:
+```sh
+python -m pip install -U build
+python -m build . # find the sdist and wheel file in the 'dist' folder
+```
+
+Install the package in the current environment:
+```sh
+pip install .    # normal installation
+pip install -e . # editable installation
+```
+
+## Examples
+
+As an introduction to py-build-cmake, see [`examples/minimal`](https://github.com/tttapa/py-build-cmake/tree/main/examples/minimal)
+for a detailed overview of the configuration files and the directory structure,
+using a very simple Python module as an example.  
+For a more advanced, real-world example, see [`examples/pybind11-project`](https://github.com/tttapa/py-build-cmake/tree/main/examples/pybind11-project)
+and [`examples/nanobind-project`](https://github.com/tttapa/py-build-cmake/tree/main/examples/nanobind-project).  
+If you are interested in packaging C/C++/Fortran programs using py-build-cmake,
+have a look at [`examples/minimal-program`](https://github.com/tttapa/py-build-cmake/tree/main/examples/minimal-program).
+
+## Projects using py-build-cmake
+
+If you need more examples, you can look at the following projects using
+py-build-cmake as their Python build backend:
+
+- [alpaqa](https://github.com/kul-optec/alpaqa/tree/develop)
+- [QPALM](https://github.com/kul-optec/QPALM)
+
+## Planned features
+
+ - [x] ~~macOS support~~
+ - [x] ~~Entry point support~~
+ - [ ] Namespace package support ([PEP 420](https://www.python.org/dev/peps/pep-0420/))
+ - [ ] Doxygen and Sphinx support
```

### Comparing `py-build-cmake-0.1.7/pyproject.toml` & `py-build-cmake-0.1.8/pyproject.toml`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-[build-system]
-requires = ["distlib", "flit_core>=3.7,<4", "tomli>=1.2.3,<3; python_version < '3.11'"]
-build-backend = "py_build_cmake.build"
-backend-path = ["src"]
-
-[project]
-name = "py-build-cmake"
-readme = "README.md"
-requires-python = ">=3.7"
-license = { "file" = "LICENSE" }
-authors = [{ "name" = "Pieter P", "email" = "pieter.p.dev@outlook.com" }]
-keywords = ["pep517", "cmake"]
-classifiers = [
-    "Development Status :: 4 - Beta",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Operating System :: POSIX :: Linux",
-    "Operating System :: Microsoft :: Windows",
-    "Operating System :: MacOS",
-]
-dependencies = [
-    "distlib~=0.3.5",
-    "flit_core>=3.7,<4",
-    "tomli>=1.2.3,<3; python_version < '3.11'",
-    "click~=8.1.3",
-]
-dynamic = ["version", "description"]
-
-[project.urls]
-Source = "https://github.com/tttapa/py-build-cmake"
-Documentation = "https://tttapa.github.io/py-build-cmake"
-Tracker = "https://github.com/tttapa/py-build-cmake/issues"
-
-[project.scripts]
-py-build-cmake = "py_build_cmake.cli:cli"
-
-[tool.py-build-cmake.module]
-name = "py_build_cmake"
-
-[tool.pytest.ini_options]
-testpaths = ["test"]
+[build-system]
+requires = ["distlib", "flit_core>=3.7,<4", "tomli>=1.2.3,<3; python_version < '3.11'"]
+build-backend = "py_build_cmake.build"
+backend-path = ["src"]
+
+[project]
+name = "py-build-cmake"
+readme = "README.md"
+requires-python = ">=3.7"
+license = { "file" = "LICENSE" }
+authors = [{ "name" = "Pieter P", "email" = "pieter.p.dev@outlook.com" }]
+keywords = ["pep517", "cmake"]
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: MacOS",
+]
+dependencies = [
+    "distlib~=0.3.5",
+    "flit_core>=3.7,<4",
+    "tomli>=1.2.3,<3; python_version < '3.11'",
+    "click~=8.1.3",
+]
+dynamic = ["version", "description"]
+
+[project.urls]
+Source = "https://github.com/tttapa/py-build-cmake"
+Documentation = "https://tttapa.github.io/py-build-cmake"
+Tracker = "https://github.com/tttapa/py-build-cmake/issues"
+
+[project.scripts]
+py-build-cmake = "py_build_cmake.cli:cli"
+
+[tool.py-build-cmake.module]
+name = "py_build_cmake"
+
+[tool.pytest.ini_options]
+testpaths = ["test"]
```

### Comparing `py-build-cmake-0.1.7/src/py_build_cmake/build.py` & `py-build-cmake-0.1.8/src/py_build_cmake/build.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,735 +1,735 @@
-import platform
-from pprint import pprint
-import os
-from pathlib import Path
-from copy import copy
-import shutil
-import textwrap
-from typing import Any, Dict, List, Optional
-import tempfile
-from glob import glob
-
-from . import config
-from . import cmake
-from .datastructures import BuildPaths, PackageInfo
-from .cmd_runner import CommandRunner
-
-import flit_core.common  # type: ignore
-import flit_core.config  # type: ignore
-from distlib.version import NormalizedVersion  # type: ignore
-
-_CMAKE_MINIMUM_REQUIRED = NormalizedVersion('3.15')
-
-
-class _BuildBackend(object):
-
-    # --- Constructor ---------------------------------------------------------
-
-    def __init__(self) -> None:
-        self.runner: CommandRunner = CommandRunner()
-
-    @property
-    def verbose(self):
-        return self.runner.verbose
-
-    # --- Methods required by PEP 517 -----------------------------------------
-
-    def get_requires_for_build_wheel(self, config_settings=None):
-        """https://www.python.org/dev/peps/pep-0517/#get-requires-for-build-wheel"""
-        self.parse_config_settings(config_settings)
-
-        pyproject = Path('pyproject.toml').resolve()
-        cfg = _BuildBackend.read_config(pyproject, config_settings,
-                                        self.verbose)
-        return self.get_requires_build_project(config_settings, cfg,
-                                               self.runner)
-
-    def get_requires_for_build_editable(self, config_settings=None):
-        """https://www.python.org/dev/peps/pep-0660/#get-requires-for-build-editable"""
-        return self.get_requires_for_build_wheel(config_settings)
-
-    def get_requires_for_build_sdist(self, config_settings=None):
-        """https://www.python.org/dev/peps/pep-0517/#get-requires-for-build-sdist"""
-        return []
-
-    def build_wheel(self,
-                    wheel_directory,
-                    config_settings=None,
-                    metadata_directory=None):
-        """https://www.python.org/dev/peps/pep-0517/#build-wheel"""
-        assert metadata_directory is None
-
-        # Parse options
-        self.parse_config_settings(config_settings)
-
-        # Build wheel
-        with tempfile.TemporaryDirectory() as tmp_build_dir:
-            whl_name = self.build_wheel_in_dir(wheel_directory, tmp_build_dir,
-                                               config_settings)
-        return whl_name
-
-    def build_editable(self,
-                       wheel_directory,
-                       config_settings=None,
-                       metadata_directory=None):
-        """https://www.python.org/dev/peps/pep-0660/#build-editable"""
-        assert metadata_directory is None
-
-        # Parse options
-        self.parse_config_settings(config_settings)
-
-        # Build wheel
-        with tempfile.TemporaryDirectory() as tmp_build_dir:
-            whl_name = self.build_wheel_in_dir(wheel_directory,
-                                               tmp_build_dir,
-                                               config_settings,
-                                               editable=True)
-        return whl_name
-
-    def build_sdist(self, sdist_directory, config_settings=None):
-        """https://www.python.org/dev/peps/pep-0517/#build-sdist"""
-        sdist_directory = Path(sdist_directory)
-        src_dir = Path().resolve()
-
-        # Parse options
-        self.parse_config_settings(config_settings)
-
-        # Load metadata
-        from flit_core.common import Module, make_metadata
-        pyproject = src_dir / 'pyproject.toml'
-        cfg = self.read_config(pyproject, config_settings, self.verbose)
-        import_name = cfg.module['name']
-        pkg = Module(import_name, src_dir / cfg.module['directory'])
-        metadata = make_metadata(pkg, cfg)
-        metadata.version = self.normalize_version(metadata.version)
-
-        # Export dist
-        from flit_core.sdist import SdistBuilder  # type: ignore
-        rel_pyproject = os.path.relpath(pyproject, src_dir)
-        extra_files = [str(rel_pyproject)] + cfg.referenced_files
-        sdist_cfg = cfg.sdist[self.get_os_name()]
-        sdist_builder = SdistBuilder(
-            pkg,
-            metadata=metadata,
-            cfgdir=src_dir,
-            reqs_by_extra=None,
-            entrypoints=cfg.entrypoints,
-            extra_files=extra_files,
-            data_directory=None,
-            include_patterns=sdist_cfg.get('include_patterns', []),
-            exclude_patterns=sdist_cfg.get('exclude_patterns', []),
-        )
-        sdist_tar = sdist_builder.build(Path(sdist_directory))
-        return os.path.relpath(sdist_tar, sdist_directory)
-
-    # --- Parsing config options and metadata ---------------------------------
-
-    @staticmethod
-    def is_verbose_enabled(config_settings: Optional[dict]):
-        if 'PY_BUILD_CMAKE_VERBOSE' in os.environ:
-            return True
-        if config_settings is None:
-            return False
-        if config_settings.keys() & {'verbose', '--verbose', 'V', '-V'}:
-            return True
-        return False
-
-    def parse_config_settings(self, config_settings: Optional[Dict]):
-        self.runner.verbose = self.is_verbose_enabled(config_settings)
-
-    @staticmethod
-    def read_config(pyproject_path: Path, config_settings: Optional[Dict],
-                    verbose: bool) -> config.Config:
-        config_settings = config_settings or {}
-        try:
-            if verbose:
-                print("Configuration settings:")
-                pprint(config_settings)
-            listify = lambda x: x if isinstance(x, list) else [x]
-            keys = ['--local', '--cross']
-            overrides = {
-                key: listify(config_settings.get(key) or [])
-                for key in keys
-            }
-            if verbose:
-                print("Configuration settings for local and "
-                      "cross-compilation overrides:")
-                pprint(overrides)
-            cfg = config.read_config(pyproject_path, overrides)
-        except flit_core.config.ConfigError as e:
-            e.args = ("\n"
-                      "\n"
-                      "\t❌ Error in user configuration:\n"
-                      "\n"
-                      f"\t\t{e}\n"
-                      "\n", )
-            raise
-        except AssertionError as e:
-            e.args = (
-                "\n"
-                "\n"
-                "\t❌ Internal error while processing the configuration\n"
-                "\t   Please notify the developers: https://github.com/tttapa/py-build-cmake/issues\n"
-                "\n"
-                f"\t\t{e}\n"
-                "\n", )
-            raise
-        if verbose:
-            _BuildBackend.print_config_verbose(cfg)
-        return cfg
-
-    @staticmethod
-    def get_requires_build_project(config_settings: Optional[dict],
-                                   cfg: config.Config, runner: CommandRunner):
-        deps: List[str] = []
-        # Check if we need CMake
-        if cfg.cmake:
-            _BuildBackend.check_cmake_program(cfg, deps, runner)
-        if cfg.stubgen:
-            _BuildBackend.check_stubgen_program(deps, runner)
-        if runner.verbose:
-            print('Dependencies for build:', deps)
-        return deps
-
-    # --- Building wheels -----------------------------------------------------
-
-    def build_wheel_in_dir(self,
-                           wheel_directory_,
-                           tmp_build_dir,
-                           config_settings,
-                           editable=False):
-        """This is the main function that contains all steps necessary to build
-        a complete wheel package, including the CMake builds etc."""
-        # Set up all paths
-        paths = BuildPaths(
-            source_dir=Path().resolve(),
-            wheel_dir=Path(wheel_directory_),
-            temp_dir=Path(tmp_build_dir),
-            staging_dir=Path(tmp_build_dir) / 'staging',
-            pkg_staging_dir=Path(tmp_build_dir) / 'staging',
-        )
-
-        # Load metadata from the pyproject.toml file
-        cfg, pkg, metadata = _BuildBackend.read_all_metadata(
-            paths.source_dir, config_settings, self.verbose)
-
-        pkg_info = PackageInfo(
-            version=metadata.version,
-            package_name=cfg.package_name,
-            module_name=cfg.module['name'],
-        )
-
-        # Copy the module's Python source files to the temporary folder
-        if not editable:
-            self.copy_pkg_source_to(paths.staging_dir, pkg)
-        else:
-            paths = self.do_editable_install(cfg, paths, pkg)
-
-        # Create dist-info folder
-        distinfo_dir = f'{pkg_info.package_name}-{pkg_info.version}.dist-info'
-        distinfo_dir = paths.pkg_staging_dir / distinfo_dir
-        os.makedirs(distinfo_dir, exist_ok=True)
-
-        # Write metadata
-        metadata_path = distinfo_dir / 'METADATA'
-        with open(metadata_path, 'w', encoding='utf-8') as f:
-            metadata.write_metadata_file(f)
-        # Write or copy license
-        self.write_license_files(cfg.license, paths.source_dir, distinfo_dir)
-        # Write entrypoints/scripts
-        self.write_entrypoints(distinfo_dir, cfg.entrypoints)
-
-        # Generate .pyi stubs (for the Python files only)
-        if cfg.stubgen is not None and not editable:
-            self.generate_stubs(paths, pkg, cfg.stubgen)
-
-        # Configure, build and install the CMake project
-        if cfg.cmake:
-            self.do_native_cross_cmake_build(paths, cfg, pkg_info)
-
-        # Create wheel
-        whl_name = self.create_wheel(paths, cfg, pkg_info)
-        return whl_name
-
-    @staticmethod
-    def read_all_metadata(src_dir, config_settings, verbose):
-        from flit_core.common import Module, make_metadata, ProblemInModule
-        cfg = _BuildBackend.read_config(src_dir / 'pyproject.toml',
-                                        config_settings, verbose)
-        pkg = Module(cfg.module['name'], src_dir / cfg.module['directory'])
-        try:
-            metadata = make_metadata(pkg, cfg)
-        except ImportError as e:
-            if hasattr(e, "msg"):
-                e.msg = (
-                    "\n"
-                    "\n"
-                    f"\t❌ Error importing {pkg.name} for reading metadata:\n"
-                    "\n"
-                    f"\t\t{e.msg}\n"
-                    "\n")
-            raise
-        except ProblemInModule as e:
-            e.args = ("\n"
-                      "\n"
-                      f"\t❌ Error reading metadata from {pkg.name}:"
-                      "\n"
-                      "\n"
-                      f"\t\t{e}\n"
-                      "\n", )
-            raise
-        metadata.version = _BuildBackend.normalize_version(metadata.version)
-        metadata.name = cfg.package_name
-        return cfg, pkg, metadata
-
-    @staticmethod
-    def create_wheel(paths, cfg, package_info):
-        """Create a wheel package from the build directory."""
-        from distlib.wheel import Wheel  # type: ignore
-        whl = Wheel()
-        whl.name = package_info.package_name
-        whl.version = package_info.version
-        pure = not cfg.cmake
-        libdir = 'purelib' if pure else 'platlib'
-        staging_dir = paths.pkg_staging_dir
-        whl_paths = {'prefix': str(staging_dir), libdir: str(staging_dir)}
-        whl.dirname = paths.wheel_dir
-        if pure:
-            tags = {'pyver': ['py3']}
-        elif cfg.cross:
-            tags = _BuildBackend.get_cross_tags(cfg.cross)
-        else:
-            tags = _BuildBackend.get_native_tags()
-        wheel_path = whl.build(whl_paths, tags=tags, wheel_version=(1, 0))
-        whl_name = os.path.relpath(wheel_path, paths.wheel_dir)
-        return whl_name
-
-    @staticmethod
-    def get_cmake_configs(cfg):
-        native_cmake_cfg = cfg.cmake[_BuildBackend.get_os_name()]
-        cmake_cfg = cfg.cmake['cross'] if cfg.cross else native_cmake_cfg
-        return cmake_cfg, native_cmake_cfg
-
-    def do_native_cross_cmake_build(self, paths: BuildPaths, cfg,
-                                    package_info):
-        """If not cross-compiling, just do a regular CMake build+install.
-        When cross-compiling, do a cross-build+install (using the provided 
-        CMake toolchain file).
-        If cfg.cross['copy_from_native_build'] is set, before cross-compiling, 
-        first a normal build+install is performed to a separate directory, then
-        the cross-build+install is performed, and finally the installed files
-        from the native build that match the patterns in
-        cfg.cross['copy_from_native_build'] are copied to the installation
-        directory of the cross-build for packaging."""
-        cmake_cfg, native_cmake_cfg = self.get_cmake_configs(cfg)
-        # When cross-compiling, optionally do a native build first
-        native_install_dir = None
-        if self.needs_cross_native_build(cfg):
-            native_install_dir = paths.temp_dir / 'native-install'
-            self.run_cmake(paths.source_dir, native_install_dir,
-                           native_cmake_cfg, None, package_info,
-                           native_install_dir)
-        # Then do the actual build
-        self.run_cmake(paths.source_dir, paths.staging_dir, cmake_cfg,
-                       cfg.cross, package_info, native_install_dir)
-        # Finally, move the files from the native build to the staging area
-        if native_install_dir:
-            self.copy_native_install(paths.staging_dir,
-                                     native_install_dir,
-                                     cfg.cross['copy_from_native_build'])
-
-    def copy_native_install(self, staging_dir, native_install_dir,
-                            native_install_patterns):
-        """Copy the files that match the patterns from the native installation
-        directory to the wheel staging directory."""
-        for pattern in native_install_patterns:
-            matches = sorted(glob(str(native_install_dir / pattern)))
-            for path in matches:
-                path = Path(path)
-                rel = path.relative_to(native_install_dir)
-                path.parent.mkdir(parents=True, exist_ok=True)
-                print('-- Moving:', path, '->', staging_dir / rel.parent)
-                shutil.move(path, staging_dir / rel.parent)
-                # TODO: what if the folder already exists?
-            if not matches:
-                raise RuntimeError(
-                    "Native build installed no files that matched the "
-                    "pattern '" + pattern + "'")
-        shutil.rmtree(native_install_dir)
-
-    # --- Files installation --------------------------------------------------
-
-    @staticmethod
-    def copy_pkg_source_to(staging_dir: Path, pkg: flit_core.common.Module,
-                           symlink: bool = False):
-        """Copy the files of a Python package to the build directory."""
-        for mod_file in pkg.iter_files():
-            rel_path = os.path.relpath(mod_file, pkg.path.parent)
-            dst = staging_dir / rel_path
-            os.makedirs(dst.parent, exist_ok=True)
-            if symlink:
-                dst.symlink_to(mod_file, target_is_directory=False)
-            else:
-                shutil.copy2(mod_file, dst, follow_symlinks=False)
-
-    @staticmethod
-    def write_license_files(license, srcdir: Path, distinfo_dir: Path):
-        """Write the LICENSE file from pyproject.toml to the distinfo
-        directory."""
-        if 'text' in license:
-            with (distinfo_dir / 'LICENSE').open('w', encoding='utf-8') as f:
-                f.write(license['text'])
-        elif 'file' in license:
-            assert not Path(license['file']).is_absolute()
-            shutil.copy2(srcdir / license['file'], distinfo_dir)
-
-    @staticmethod
-    def write_entrypoints(distinfo: Path, entrypoints: Dict[str, Dict[str,
-                                                                      str]]):
-        from flit_core.common import write_entry_points
-        with (distinfo / 'entry_points.txt').open('w', encoding='utf-8') as f:
-            write_entry_points(entrypoints, f)
-
-    # --- Editable installs ---------------------------------------------------
-
-    def do_editable_install(self, cfg, paths: BuildPaths,
-                            pkg: flit_core.common.Module):
-        mode = cfg.editable[self.get_os_name()]["mode"]
-        if mode == "wrapper":
-            self.write_editable_wrapper(paths.staging_dir, pkg)
-        elif mode == "hook":
-            self.write_editable_hook(paths.staging_dir, pkg),
-        elif mode == "symlink":
-            paths = self.write_editable_links(paths, pkg)
-        else:
-            assert False, "Invalid editable mode"
-        return paths
-
-    def write_editable_wrapper(self, staging_dir: Path,
-                               pkg: flit_core.common.Module):
-        """Write a fake __init__.py file that points to the development 
-        folder."""
-        tmp_pkg: Path = staging_dir / pkg.name
-        pkgpath = Path(pkg.path)
-        initpath = pkgpath / '__init__.py'
-        os.makedirs(tmp_pkg, exist_ok=True)
-        special_dunders = [
-            '__builtins__', '__cached__', '__file__', '__loader__', '__name__',
-            '__package__', '__path__', '__spec__'
-        ]
-        content = f"""\
-            # First extend the search path with the development folder
-            __spec__.submodule_search_locations.insert(0, {str(pkgpath)!a})
-            # Now manually import the development __init__.py
-            from importlib import util as _util
-            _spec = _util.spec_from_file_location("{pkg.name}",
-                                                  {str(initpath)!a})
-            _mod = _util.module_from_spec(_spec)
-            _spec.loader.exec_module(_mod)
-            # After importing, add its symbols to our global scope
-            _vars = _mod.__dict__.copy()
-            for _k in ['{"','".join(special_dunders)}']: _vars.pop(_k)
-            globals().update(_vars)
-            # Clean up
-            del _k, _spec, _mod, _vars, _util
-            """
-        (tmp_pkg / '__init__.py').write_text(textwrap.dedent(content),
-                                             encoding='utf-8')
-        # Add the py.typed file if it exists, so mypy picks up the stubs for
-        # the C++ extensions
-        py_typed: Path = pkg.path / 'py.typed'
-        if py_typed.exists():
-            shutil.copy2(py_typed, tmp_pkg)
-        # Write a path file so IDEs find the correct files as well
-        (staging_dir / f'{pkg.name}.pth').write_text(str(pkg.path.parent))
-
-    def write_editable_hook(self, staging_dir: Path,
-                            pkg: flit_core.common.Module):
-        # Write a hook that finds the installed compiled extension modules
-        pkg_hook: Path = staging_dir / (pkg.name + '_editable_hook')
-        os.makedirs(pkg_hook, exist_ok=True)
-        content = f"""\
-            import sys, inspect, os
-            from importlib.machinery import PathFinder
-
-            class EditablePathFinder(PathFinder):
-                def __init__(self, name, extra_path):
-                    self.name = name
-                    self.extra_path = extra_path
-                def find_spec(self, name, path=None, target=None):
-                    if name.split('.', 1)[0] != self.name:
-                        return None
-                    path = (path or []) + [self.extra_path]
-                    return super().find_spec(name, path, target)
-
-            def install(name: str):
-                source_path = os.path.abspath(inspect.getsourcefile(EditablePathFinder))
-                source_dir = os.path.dirname(source_path)
-                installed_path = os.path.join(source_dir, '..', name)
-                sys.meta_path.insert(0, EditablePathFinder(name, installed_path))
-
-            install('{pkg.name}')
-            """
-        (pkg_hook / '__init__.py').write_text(textwrap.dedent(content),
-                                              encoding='utf-8')
-        # Write a path file to find the development files
-        content = f"""\
-            {str(pkg.path.parent)}
-            import {pkg.name}_editable_hook"""
-        (staging_dir / f'{pkg.name}.pth').write_text(
-            textwrap.dedent(content))
-        
-    def write_editable_links(self, paths: BuildPaths,
-                             pkg: flit_core.common.Module):
-        paths = copy(paths)
-        cache_dir = paths.source_dir / '.py-build-cmake_cache'
-        cache_dir.mkdir(exist_ok=True)
-        paths.staging_dir = cache_dir / 'editable'
-        shutil.rmtree(paths.staging_dir, ignore_errors=True)
-        paths.staging_dir.mkdir()
-        self.copy_pkg_source_to(paths.staging_dir, pkg, symlink=True)
-        pth_file = paths.pkg_staging_dir / f'{pkg.name}.pth'
-        pth_file.parent.mkdir(exist_ok=True)
-        pth_file.write_text(str(paths.staging_dir))
-        return paths
-
-    # --- Invoking CMake builds -----------------------------------------------
-
-    def run_cmake(self, pkgdir, install_dir, cmake_cfg, cross_cfg,
-                  package_info, native_install_dir):
-        """Configure, build and install using CMake."""
-
-        cmaker = self.get_cmaker(pkgdir,
-                                 install_dir,
-                                 cmake_cfg,
-                                 cross_cfg,
-                                 native_install_dir,
-                                 package_info,
-                                 runner=self.runner)
-
-        cmaker.configure()
-        cmaker.build()
-        cmaker.install()
-
-    @staticmethod
-    def get_cmaker(pkg_dir: Path, install_dir: Optional[Path], cmake_cfg: dict,
-                   cross_cfg: Optional[dict],
-                   native_install_dir: Optional[Path],
-                   package_info: PackageInfo, **kwargs):
-        toolchain_file = None
-        if cross_cfg:
-            toolchain_file = cross_cfg['toolchain_file']
-
-        # Add some CMake configure options
-        options = cmake_cfg.get('options', {})
-        if native_install_dir:
-            options['PY_BUILD_CMAKE_NATIVE_INSTALL_DIR:PATH'] = \
-                str(native_install_dir)
-        btype = cmake_cfg.get('build_type')
-        if btype:  # -D CMAKE_BUILD_TYPE={type}
-            options['CMAKE_BUILD_TYPE:STRING'] = btype
-
-        # Build folder for each platform
-        build_cfg_name = _BuildBackend.get_build_config_name(cross_cfg)
-
-        # CMake options
-        return cmake.CMaker(
-            cmake_settings=cmake.CMakeSettings(
-                working_dir=Path(pkg_dir),
-                source_path=Path(cmake_cfg["source_path"]),
-                build_path=Path(cmake_cfg['build_path']) / build_cfg_name,
-                os=_BuildBackend.get_os_name(),
-                find_python=bool(cmake_cfg["find_python"]),
-                find_python3=bool(cmake_cfg["find_python3"]),
-                command=Path("cmake"),
-            ),
-            conf_settings=cmake.CMakeConfigureSettings(
-                environment=cmake_cfg.get("env", {}),
-                toolchain_file=toolchain_file,
-                build_type=cmake_cfg.get('build_type'),
-                options=options,
-                args=cmake_cfg.get('args', []),
-                preset=cmake_cfg.get('preset'),
-                generator=cmake_cfg.get('generator'),
-            ),
-            build_settings=cmake.CMakeBuildSettings(
-                args=cmake_cfg['build_args'],
-                tool_args=cmake_cfg['build_tool_args'],
-                presets=cmake_cfg.get('build_presets', []),
-                configs=cmake_cfg.get('config', []),
-            ),
-            install_settings=cmake.CMakeInstallSettings(
-                args=cmake_cfg['install_args'],
-                presets=cmake_cfg.get('install_presets', []),
-                configs=cmake_cfg.get('config', []),
-                components=cmake_cfg.get('install_components', []),
-                prefix=install_dir,
-            ),
-            package_info=package_info,
-            **kwargs,
-        )
-
-    # --- Generate stubs ------------------------------------------------------
-
-    def generate_stubs(self, paths: BuildPaths, pkg, cfg: Dict[str, Any]):
-        """Generate stubs (.pyi) using mypy stubgen."""
-        args = ['stubgen'] + cfg.get('args', [])
-        cfg.setdefault('packages', [pkg.name] if pkg.is_package else [])
-        for p in cfg['packages']:
-            args += ['-p', p]
-        cfg.setdefault('modules', [pkg.name] if not pkg.is_package else [])
-        for m in cfg['modules']:
-            args += ['-m', m]
-        args += cfg.get('files', [])
-        # Add output folder argument if not already specified in cfg['args']
-        if 'args' not in cfg or not ({'-o', '--output'} & set(cfg['args'])):
-            args += ['-o', str(paths.staging_dir)]
-        env = os.environ.copy()
-        env.setdefault('MYPY_CACHE_DIR', str(paths.temp_dir))
-        # Call mypy stubgen in a subprocess
-        self.runner.run(args, cwd=pkg.path.parent, check=True, env=env)
-
-    # --- Misc helper functions -----------------------------------------------
-
-    @staticmethod
-    def get_os_name():
-        return {
-            "Linux": "linux",
-            "Windows": "windows",
-            "Darwin": "mac",
-        }[platform.system()]
-
-    @staticmethod
-    def print_config_verbose(cfg):
-        from . import __version__
-        print("\npy-build-cmake (" + __version__ + ")")
-        print("options")
-        print("================================")
-        print("module:")
-        pprint(cfg.module)
-        print("editable:")
-        pprint(cfg.editable)
-        print("sdist:")
-        pprint(cfg.sdist)
-        print("cmake:")
-        pprint(cfg.cmake)
-        print("stubgen:")
-        pprint(cfg.stubgen)
-        print("cross:")
-        pprint(cfg.cross)
-        print("================================\n")
-
-    @staticmethod
-    def normalize_version(version):
-        from distlib.version import NormalizedVersion
-        norm_version = str(NormalizedVersion(version))
-        return norm_version
-
-    @staticmethod
-    def get_native_tags():
-        """Get the PEP 425 tags for the current platform."""
-        from .tags import get_python_tag, get_abi_tag, get_platform_tag
-        return {
-            'pyver': [get_python_tag()],
-            'abi': [get_abi_tag()],
-            'arch': [get_platform_tag()],
-        }
-
-    @staticmethod
-    def get_cross_tags(crosscfg):
-        """Get the PEP 425 tags to use when cross-compiling."""
-        tags = _BuildBackend.get_native_tags()
-        if 'implementation' in crosscfg and 'version' in crosscfg:
-            tags['pyver'] = [crosscfg['implementation'] + crosscfg['version']]
-        if 'abi' in crosscfg:
-            tags['abi'] = [crosscfg['abi']]
-        if 'arch' in crosscfg:
-            tags['arch'] = [crosscfg['arch']]
-        return tags
-
-    @staticmethod
-    def get_build_config_name(cross_cfg):
-        """Get a string representing the Python version, ABI and architecture,
-        used to name the build folder so builds for different versions don't
-        interfere."""
-        if cross_cfg:
-            tags = _BuildBackend.get_cross_tags(cross_cfg)
-        else:
-            tags = _BuildBackend.get_native_tags()
-        return '-'.join(map(lambda x: x[0], tags.values()))
-
-    @staticmethod
-    def needs_cross_native_build(cfg):
-        return cfg.cross and 'copy_from_native_build' in cfg.cross
-
-    @staticmethod
-    def iter_files(stagedir):
-        """Iterate over the files contained in the given folder.
-
-        Yields absolute paths - caller may want to make them relative.
-        Excludes any __pycache__ and *.pyc files."""
-
-        # https://github.com/pypa/flit/blob/a4524758604107bde8c77b5816612edb76a604aa/flit_core/flit_core/common.py#L73
-
-        def _include(path):
-            name = os.path.basename(path)
-            return name != '__pycache__' and not name.endswith('.pyc')
-
-        # Ensure we sort all files and directories so the order is stable
-        for dirpath, dirs, files in os.walk(str(stagedir)):
-            for file in sorted(files):
-                full_path = os.path.join(dirpath, file)
-                if _include(full_path):
-                    yield full_path
-
-            dirs[:] = [d for d in sorted(dirs) if _include(d)]
-
-    # --- Helper functions for finding programs like CMake --------------------
-
-    @staticmethod
-    def check_cmake_program(cfg: config.Config, deps: List[str],
-                            runner: CommandRunner):
-        assert cfg.cmake
-        # Do we need to perform a native build?
-        native = not cfg.cross or _BuildBackend.needs_cross_native_build(cfg)
-        native_cfg = cfg.cmake[_BuildBackend.get_os_name()] if native else {}
-        # Do we need to perform a cross build?
-        cross = cfg.cross
-        cross_cfg = cfg.cmake.get('cross', {})
-        # Find the strictest version requirement
-        min_cmake_ver = max(
-            _CMAKE_MINIMUM_REQUIRED,
-            NormalizedVersion(native_cfg.get('minimum_version', '0.0')),
-            NormalizedVersion(cross_cfg.get('minimum_version', '0.0')),
-        )
-        # If CMake in PATH doesn't work or is too old, add it as a build
-        # requirement
-        if not runner.check_program_version('cmake', min_cmake_ver, "CMake"):
-            deps.append("cmake>=" + str(min_cmake_ver))
-
-        # Check if we need Ninja
-        cfgs = []
-        if native: cfgs.append(native_cfg)
-        if cross: cfgs.append(cross_cfg)
-        # Do any of the configs require Ninja as a generator?
-        needs_ninja = lambda c: 'ninja' in c.get('generator', '').lower()
-        need_ninja = any(map(needs_ninja, cfgs))
-        if need_ninja:
-            # If so, check if a working version exists in the PATH, otherwise,
-            # add it as a build requirement
-            if not runner.check_program_version('ninja', None, "Ninja"):
-                deps.append("ninja")
-
-    @staticmethod
-    def check_stubgen_program(deps: List[str], runner: CommandRunner):
-        if not runner.check_program_version('stubgen', None, None, False):
-            deps.append("mypy")
-
-
-_BACKEND = _BuildBackend()
-get_requires_for_build_wheel = _BACKEND.get_requires_for_build_wheel
-get_requires_for_build_sdist = _BACKEND.get_requires_for_build_sdist
-get_requires_for_build_editable = _BACKEND.get_requires_for_build_editable
-build_wheel = _BACKEND.build_wheel
-build_sdist = _BACKEND.build_sdist
-build_editable = _BACKEND.build_editable
+import platform
+from pprint import pprint
+import os
+from pathlib import Path
+from copy import copy
+import shutil
+import textwrap
+from typing import Any, Dict, List, Optional
+import tempfile
+from glob import glob
+
+from . import config
+from . import cmake
+from .datastructures import BuildPaths, PackageInfo
+from .cmd_runner import CommandRunner
+
+import flit_core.common  # type: ignore
+import flit_core.config  # type: ignore
+from distlib.version import NormalizedVersion  # type: ignore
+
+_CMAKE_MINIMUM_REQUIRED = NormalizedVersion('3.15')
+
+
+class _BuildBackend(object):
+
+    # --- Constructor ---------------------------------------------------------
+
+    def __init__(self) -> None:
+        self.runner: CommandRunner = CommandRunner()
+
+    @property
+    def verbose(self):
+        return self.runner.verbose
+
+    # --- Methods required by PEP 517 -----------------------------------------
+
+    def get_requires_for_build_wheel(self, config_settings=None):
+        """https://www.python.org/dev/peps/pep-0517/#get-requires-for-build-wheel"""
+        self.parse_config_settings(config_settings)
+
+        pyproject = Path('pyproject.toml').resolve()
+        cfg = _BuildBackend.read_config(pyproject, config_settings,
+                                        self.verbose)
+        return self.get_requires_build_project(config_settings, cfg,
+                                               self.runner)
+
+    def get_requires_for_build_editable(self, config_settings=None):
+        """https://www.python.org/dev/peps/pep-0660/#get-requires-for-build-editable"""
+        return self.get_requires_for_build_wheel(config_settings)
+
+    def get_requires_for_build_sdist(self, config_settings=None):
+        """https://www.python.org/dev/peps/pep-0517/#get-requires-for-build-sdist"""
+        return []
+
+    def build_wheel(self,
+                    wheel_directory,
+                    config_settings=None,
+                    metadata_directory=None):
+        """https://www.python.org/dev/peps/pep-0517/#build-wheel"""
+        assert metadata_directory is None
+
+        # Parse options
+        self.parse_config_settings(config_settings)
+
+        # Build wheel
+        with tempfile.TemporaryDirectory() as tmp_build_dir:
+            whl_name = self.build_wheel_in_dir(wheel_directory, tmp_build_dir,
+                                               config_settings)
+        return whl_name
+
+    def build_editable(self,
+                       wheel_directory,
+                       config_settings=None,
+                       metadata_directory=None):
+        """https://www.python.org/dev/peps/pep-0660/#build-editable"""
+        assert metadata_directory is None
+
+        # Parse options
+        self.parse_config_settings(config_settings)
+
+        # Build wheel
+        with tempfile.TemporaryDirectory() as tmp_build_dir:
+            whl_name = self.build_wheel_in_dir(wheel_directory,
+                                               tmp_build_dir,
+                                               config_settings,
+                                               editable=True)
+        return whl_name
+
+    def build_sdist(self, sdist_directory, config_settings=None):
+        """https://www.python.org/dev/peps/pep-0517/#build-sdist"""
+        sdist_directory = Path(sdist_directory)
+        src_dir = Path().resolve()
+
+        # Parse options
+        self.parse_config_settings(config_settings)
+
+        # Load metadata
+        from flit_core.common import Module, make_metadata
+        pyproject = src_dir / 'pyproject.toml'
+        cfg = self.read_config(pyproject, config_settings, self.verbose)
+        import_name = cfg.module['name']
+        pkg = Module(import_name, src_dir / cfg.module['directory'])
+        metadata = make_metadata(pkg, cfg)
+        metadata.version = self.normalize_version(metadata.version)
+
+        # Export dist
+        from flit_core.sdist import SdistBuilder  # type: ignore
+        rel_pyproject = os.path.relpath(pyproject, src_dir)
+        extra_files = [str(rel_pyproject)] + cfg.referenced_files
+        sdist_cfg = cfg.sdist[self.get_os_name()]
+        sdist_builder = SdistBuilder(
+            pkg,
+            metadata=metadata,
+            cfgdir=src_dir,
+            reqs_by_extra=None,
+            entrypoints=cfg.entrypoints,
+            extra_files=extra_files,
+            data_directory=None,
+            include_patterns=sdist_cfg.get('include_patterns', []),
+            exclude_patterns=sdist_cfg.get('exclude_patterns', []),
+        )
+        sdist_tar = sdist_builder.build(Path(sdist_directory))
+        return os.path.relpath(sdist_tar, sdist_directory)
+
+    # --- Parsing config options and metadata ---------------------------------
+
+    @staticmethod
+    def is_verbose_enabled(config_settings: Optional[dict]):
+        if 'PY_BUILD_CMAKE_VERBOSE' in os.environ:
+            return True
+        if config_settings is None:
+            return False
+        if config_settings.keys() & {'verbose', '--verbose', 'V', '-V'}:
+            return True
+        return False
+
+    def parse_config_settings(self, config_settings: Optional[Dict]):
+        self.runner.verbose = self.is_verbose_enabled(config_settings)
+
+    @staticmethod
+    def read_config(pyproject_path: Path, config_settings: Optional[Dict],
+                    verbose: bool) -> config.Config:
+        config_settings = config_settings or {}
+        try:
+            if verbose:
+                print("Configuration settings:")
+                pprint(config_settings)
+            listify = lambda x: x if isinstance(x, list) else [x]
+            keys = ['--local', '--cross']
+            overrides = {
+                key: listify(config_settings.get(key) or [])
+                for key in keys
+            }
+            if verbose:
+                print("Configuration settings for local and "
+                      "cross-compilation overrides:")
+                pprint(overrides)
+            cfg = config.read_config(pyproject_path, overrides)
+        except flit_core.config.ConfigError as e:
+            e.args = ("\n"
+                      "\n"
+                      "\t❌ Error in user configuration:\n"
+                      "\n"
+                      f"\t\t{e}\n"
+                      "\n", )
+            raise
+        except AssertionError as e:
+            e.args = (
+                "\n"
+                "\n"
+                "\t❌ Internal error while processing the configuration\n"
+                "\t   Please notify the developers: https://github.com/tttapa/py-build-cmake/issues\n"
+                "\n"
+                f"\t\t{e}\n"
+                "\n", )
+            raise
+        if verbose:
+            _BuildBackend.print_config_verbose(cfg)
+        return cfg
+
+    @staticmethod
+    def get_requires_build_project(config_settings: Optional[dict],
+                                   cfg: config.Config, runner: CommandRunner):
+        deps: List[str] = []
+        # Check if we need CMake
+        if cfg.cmake:
+            _BuildBackend.check_cmake_program(cfg, deps, runner)
+        if cfg.stubgen:
+            _BuildBackend.check_stubgen_program(deps, runner)
+        if runner.verbose:
+            print('Dependencies for build:', deps)
+        return deps
+
+    # --- Building wheels -----------------------------------------------------
+
+    def build_wheel_in_dir(self,
+                           wheel_directory_,
+                           tmp_build_dir,
+                           config_settings,
+                           editable=False):
+        """This is the main function that contains all steps necessary to build
+        a complete wheel package, including the CMake builds etc."""
+        # Set up all paths
+        paths = BuildPaths(
+            source_dir=Path().resolve(),
+            wheel_dir=Path(wheel_directory_),
+            temp_dir=Path(tmp_build_dir),
+            staging_dir=Path(tmp_build_dir) / 'staging',
+            pkg_staging_dir=Path(tmp_build_dir) / 'staging',
+        )
+
+        # Load metadata from the pyproject.toml file
+        cfg, pkg, metadata = _BuildBackend.read_all_metadata(
+            paths.source_dir, config_settings, self.verbose)
+
+        pkg_info = PackageInfo(
+            version=metadata.version,
+            package_name=cfg.package_name,
+            module_name=cfg.module['name'],
+        )
+
+        # Copy the module's Python source files to the temporary folder
+        if not editable:
+            self.copy_pkg_source_to(paths.staging_dir, pkg)
+        else:
+            paths = self.do_editable_install(cfg, paths, pkg)
+
+        # Create dist-info folder
+        distinfo_dir = f'{pkg_info.package_name}-{pkg_info.version}.dist-info'
+        distinfo_dir = paths.pkg_staging_dir / distinfo_dir
+        os.makedirs(distinfo_dir, exist_ok=True)
+
+        # Write metadata
+        metadata_path = distinfo_dir / 'METADATA'
+        with open(metadata_path, 'w', encoding='utf-8') as f:
+            metadata.write_metadata_file(f)
+        # Write or copy license
+        self.write_license_files(cfg.license, paths.source_dir, distinfo_dir)
+        # Write entrypoints/scripts
+        self.write_entrypoints(distinfo_dir, cfg.entrypoints)
+
+        # Generate .pyi stubs (for the Python files only)
+        if cfg.stubgen is not None and not editable:
+            self.generate_stubs(paths, pkg, cfg.stubgen)
+
+        # Configure, build and install the CMake project
+        if cfg.cmake:
+            self.do_native_cross_cmake_build(paths, cfg, pkg_info)
+
+        # Create wheel
+        whl_name = self.create_wheel(paths, cfg, pkg_info)
+        return whl_name
+
+    @staticmethod
+    def read_all_metadata(src_dir, config_settings, verbose):
+        from flit_core.common import Module, make_metadata, ProblemInModule
+        cfg = _BuildBackend.read_config(src_dir / 'pyproject.toml',
+                                        config_settings, verbose)
+        pkg = Module(cfg.module['name'], src_dir / cfg.module['directory'])
+        try:
+            metadata = make_metadata(pkg, cfg)
+        except ImportError as e:
+            if hasattr(e, "msg"):
+                e.msg = (
+                    "\n"
+                    "\n"
+                    f"\t❌ Error importing {pkg.name} for reading metadata:\n"
+                    "\n"
+                    f"\t\t{e.msg}\n"
+                    "\n")
+            raise
+        except ProblemInModule as e:
+            e.args = ("\n"
+                      "\n"
+                      f"\t❌ Error reading metadata from {pkg.name}:"
+                      "\n"
+                      "\n"
+                      f"\t\t{e}\n"
+                      "\n", )
+            raise
+        metadata.version = _BuildBackend.normalize_version(metadata.version)
+        metadata.name = cfg.package_name
+        return cfg, pkg, metadata
+
+    @staticmethod
+    def create_wheel(paths, cfg, package_info):
+        """Create a wheel package from the build directory."""
+        from distlib.wheel import Wheel  # type: ignore
+        whl = Wheel()
+        whl.name = package_info.package_name
+        whl.version = package_info.version
+        pure = not cfg.cmake
+        libdir = 'purelib' if pure else 'platlib'
+        staging_dir = paths.pkg_staging_dir
+        whl_paths = {'prefix': str(staging_dir), libdir: str(staging_dir)}
+        whl.dirname = paths.wheel_dir
+        if pure:
+            tags = {'pyver': ['py3']}
+        elif cfg.cross:
+            tags = _BuildBackend.get_cross_tags(cfg.cross)
+        else:
+            tags = _BuildBackend.get_native_tags()
+        wheel_path = whl.build(whl_paths, tags=tags, wheel_version=(1, 0))
+        whl_name = os.path.relpath(wheel_path, paths.wheel_dir)
+        return whl_name
+
+    @staticmethod
+    def get_cmake_configs(cfg):
+        native_cmake_cfg = cfg.cmake[_BuildBackend.get_os_name()]
+        cmake_cfg = cfg.cmake['cross'] if cfg.cross else native_cmake_cfg
+        return cmake_cfg, native_cmake_cfg
+
+    def do_native_cross_cmake_build(self, paths: BuildPaths, cfg,
+                                    package_info):
+        """If not cross-compiling, just do a regular CMake build+install.
+        When cross-compiling, do a cross-build+install (using the provided 
+        CMake toolchain file).
+        If cfg.cross['copy_from_native_build'] is set, before cross-compiling, 
+        first a normal build+install is performed to a separate directory, then
+        the cross-build+install is performed, and finally the installed files
+        from the native build that match the patterns in
+        cfg.cross['copy_from_native_build'] are copied to the installation
+        directory of the cross-build for packaging."""
+        cmake_cfg, native_cmake_cfg = self.get_cmake_configs(cfg)
+        # When cross-compiling, optionally do a native build first
+        native_install_dir = None
+        if self.needs_cross_native_build(cfg):
+            native_install_dir = paths.temp_dir / 'native-install'
+            self.run_cmake(paths.source_dir, native_install_dir,
+                           native_cmake_cfg, None, package_info,
+                           native_install_dir)
+        # Then do the actual build
+        self.run_cmake(paths.source_dir, paths.staging_dir, cmake_cfg,
+                       cfg.cross, package_info, native_install_dir)
+        # Finally, move the files from the native build to the staging area
+        if native_install_dir:
+            self.copy_native_install(paths.staging_dir,
+                                     native_install_dir,
+                                     cfg.cross['copy_from_native_build'])
+
+    def copy_native_install(self, staging_dir, native_install_dir,
+                            native_install_patterns):
+        """Copy the files that match the patterns from the native installation
+        directory to the wheel staging directory."""
+        for pattern in native_install_patterns:
+            matches = sorted(glob(str(native_install_dir / pattern)))
+            for path in matches:
+                path = Path(path)
+                rel = path.relative_to(native_install_dir)
+                path.parent.mkdir(parents=True, exist_ok=True)
+                print('-- Moving:', path, '->', staging_dir / rel.parent)
+                shutil.move(path, staging_dir / rel.parent)
+                # TODO: what if the folder already exists?
+            if not matches:
+                raise RuntimeError(
+                    "Native build installed no files that matched the "
+                    "pattern '" + pattern + "'")
+        shutil.rmtree(native_install_dir)
+
+    # --- Files installation --------------------------------------------------
+
+    @staticmethod
+    def copy_pkg_source_to(staging_dir: Path, pkg: flit_core.common.Module,
+                           symlink: bool = False):
+        """Copy the files of a Python package to the build directory."""
+        for mod_file in pkg.iter_files():
+            rel_path = os.path.relpath(mod_file, pkg.path.parent)
+            dst = staging_dir / rel_path
+            os.makedirs(dst.parent, exist_ok=True)
+            if symlink:
+                dst.symlink_to(mod_file, target_is_directory=False)
+            else:
+                shutil.copy2(mod_file, dst, follow_symlinks=False)
+
+    @staticmethod
+    def write_license_files(license, srcdir: Path, distinfo_dir: Path):
+        """Write the LICENSE file from pyproject.toml to the distinfo
+        directory."""
+        if 'text' in license:
+            with (distinfo_dir / 'LICENSE').open('w', encoding='utf-8') as f:
+                f.write(license['text'])
+        elif 'file' in license:
+            assert not Path(license['file']).is_absolute()
+            shutil.copy2(srcdir / license['file'], distinfo_dir)
+
+    @staticmethod
+    def write_entrypoints(distinfo: Path, entrypoints: Dict[str, Dict[str,
+                                                                      str]]):
+        from flit_core.common import write_entry_points
+        with (distinfo / 'entry_points.txt').open('w', encoding='utf-8') as f:
+            write_entry_points(entrypoints, f)
+
+    # --- Editable installs ---------------------------------------------------
+
+    def do_editable_install(self, cfg, paths: BuildPaths,
+                            pkg: flit_core.common.Module):
+        mode = cfg.editable[self.get_os_name()]["mode"]
+        if mode == "wrapper":
+            self.write_editable_wrapper(paths.staging_dir, pkg)
+        elif mode == "hook":
+            self.write_editable_hook(paths.staging_dir, pkg),
+        elif mode == "symlink":
+            paths = self.write_editable_links(paths, pkg)
+        else:
+            assert False, "Invalid editable mode"
+        return paths
+
+    def write_editable_wrapper(self, staging_dir: Path,
+                               pkg: flit_core.common.Module):
+        """Write a fake __init__.py file that points to the development 
+        folder."""
+        tmp_pkg: Path = staging_dir / pkg.name
+        pkgpath = Path(pkg.path)
+        initpath = pkgpath / '__init__.py'
+        os.makedirs(tmp_pkg, exist_ok=True)
+        special_dunders = [
+            '__builtins__', '__cached__', '__file__', '__loader__', '__name__',
+            '__package__', '__path__', '__spec__'
+        ]
+        content = f"""\
+            # First extend the search path with the development folder
+            __spec__.submodule_search_locations.insert(0, {str(pkgpath)!a})
+            # Now manually import the development __init__.py
+            from importlib import util as _util
+            _spec = _util.spec_from_file_location("{pkg.name}",
+                                                  {str(initpath)!a})
+            _mod = _util.module_from_spec(_spec)
+            _spec.loader.exec_module(_mod)
+            # After importing, add its symbols to our global scope
+            _vars = _mod.__dict__.copy()
+            for _k in ['{"','".join(special_dunders)}']: _vars.pop(_k)
+            globals().update(_vars)
+            # Clean up
+            del _k, _spec, _mod, _vars, _util
+            """
+        (tmp_pkg / '__init__.py').write_text(textwrap.dedent(content),
+                                             encoding='utf-8')
+        # Add the py.typed file if it exists, so mypy picks up the stubs for
+        # the C++ extensions
+        py_typed: Path = pkg.path / 'py.typed'
+        if py_typed.exists():
+            shutil.copy2(py_typed, tmp_pkg)
+        # Write a path file so IDEs find the correct files as well
+        (staging_dir / f'{pkg.name}.pth').write_text(str(pkg.path.parent))
+
+    def write_editable_hook(self, staging_dir: Path,
+                            pkg: flit_core.common.Module):
+        # Write a hook that finds the installed compiled extension modules
+        pkg_hook: Path = staging_dir / (pkg.name + '_editable_hook')
+        os.makedirs(pkg_hook, exist_ok=True)
+        content = f"""\
+            import sys, inspect, os
+            from importlib.machinery import PathFinder
+
+            class EditablePathFinder(PathFinder):
+                def __init__(self, name, extra_path):
+                    self.name = name
+                    self.extra_path = extra_path
+                def find_spec(self, name, path=None, target=None):
+                    if name.split('.', 1)[0] != self.name:
+                        return None
+                    path = (path or []) + [self.extra_path]
+                    return super().find_spec(name, path, target)
+
+            def install(name: str):
+                source_path = os.path.abspath(inspect.getsourcefile(EditablePathFinder))
+                source_dir = os.path.dirname(source_path)
+                installed_path = os.path.join(source_dir, '..', name)
+                sys.meta_path.insert(0, EditablePathFinder(name, installed_path))
+
+            install('{pkg.name}')
+            """
+        (pkg_hook / '__init__.py').write_text(textwrap.dedent(content),
+                                              encoding='utf-8')
+        # Write a path file to find the development files
+        content = f"""\
+            {str(pkg.path.parent)}
+            import {pkg.name}_editable_hook"""
+        (staging_dir / f'{pkg.name}.pth').write_text(
+            textwrap.dedent(content))
+        
+    def write_editable_links(self, paths: BuildPaths,
+                             pkg: flit_core.common.Module):
+        paths = copy(paths)
+        cache_dir = paths.source_dir / '.py-build-cmake_cache'
+        cache_dir.mkdir(exist_ok=True)
+        paths.staging_dir = cache_dir / 'editable'
+        shutil.rmtree(paths.staging_dir, ignore_errors=True)
+        paths.staging_dir.mkdir()
+        self.copy_pkg_source_to(paths.staging_dir, pkg, symlink=True)
+        pth_file = paths.pkg_staging_dir / f'{pkg.name}.pth'
+        pth_file.parent.mkdir(exist_ok=True)
+        pth_file.write_text(str(paths.staging_dir))
+        return paths
+
+    # --- Invoking CMake builds -----------------------------------------------
+
+    def run_cmake(self, pkgdir, install_dir, cmake_cfg, cross_cfg,
+                  package_info, native_install_dir):
+        """Configure, build and install using CMake."""
+
+        cmaker = self.get_cmaker(pkgdir,
+                                 install_dir,
+                                 cmake_cfg,
+                                 cross_cfg,
+                                 native_install_dir,
+                                 package_info,
+                                 runner=self.runner)
+
+        cmaker.configure()
+        cmaker.build()
+        cmaker.install()
+
+    @staticmethod
+    def get_cmaker(pkg_dir: Path, install_dir: Optional[Path], cmake_cfg: dict,
+                   cross_cfg: Optional[dict],
+                   native_install_dir: Optional[Path],
+                   package_info: PackageInfo, **kwargs):
+        toolchain_file = None
+        if cross_cfg:
+            toolchain_file = cross_cfg['toolchain_file']
+
+        # Add some CMake configure options
+        options = cmake_cfg.get('options', {})
+        if native_install_dir:
+            options['PY_BUILD_CMAKE_NATIVE_INSTALL_DIR:PATH'] = \
+                str(native_install_dir)
+        btype = cmake_cfg.get('build_type')
+        if btype:  # -D CMAKE_BUILD_TYPE={type}
+            options['CMAKE_BUILD_TYPE:STRING'] = btype
+
+        # Build folder for each platform
+        build_cfg_name = _BuildBackend.get_build_config_name(cross_cfg)
+
+        # CMake options
+        return cmake.CMaker(
+            cmake_settings=cmake.CMakeSettings(
+                working_dir=Path(pkg_dir),
+                source_path=Path(cmake_cfg["source_path"]),
+                build_path=Path(cmake_cfg['build_path']) / build_cfg_name,
+                os=_BuildBackend.get_os_name(),
+                find_python=bool(cmake_cfg["find_python"]),
+                find_python3=bool(cmake_cfg["find_python3"]),
+                command=Path("cmake"),
+            ),
+            conf_settings=cmake.CMakeConfigureSettings(
+                environment=cmake_cfg.get("env", {}),
+                toolchain_file=toolchain_file,
+                build_type=cmake_cfg.get('build_type'),
+                options=options,
+                args=cmake_cfg.get('args', []),
+                preset=cmake_cfg.get('preset'),
+                generator=cmake_cfg.get('generator'),
+            ),
+            build_settings=cmake.CMakeBuildSettings(
+                args=cmake_cfg['build_args'],
+                tool_args=cmake_cfg['build_tool_args'],
+                presets=cmake_cfg.get('build_presets', []),
+                configs=cmake_cfg.get('config', []),
+            ),
+            install_settings=cmake.CMakeInstallSettings(
+                args=cmake_cfg['install_args'],
+                presets=cmake_cfg.get('install_presets', []),
+                configs=cmake_cfg.get('config', []),
+                components=cmake_cfg.get('install_components', []),
+                prefix=install_dir,
+            ),
+            package_info=package_info,
+            **kwargs,
+        )
+
+    # --- Generate stubs ------------------------------------------------------
+
+    def generate_stubs(self, paths: BuildPaths, pkg, cfg: Dict[str, Any]):
+        """Generate stubs (.pyi) using mypy stubgen."""
+        args = ['stubgen'] + cfg.get('args', [])
+        cfg.setdefault('packages', [pkg.name] if pkg.is_package else [])
+        for p in cfg['packages']:
+            args += ['-p', p]
+        cfg.setdefault('modules', [pkg.name] if not pkg.is_package else [])
+        for m in cfg['modules']:
+            args += ['-m', m]
+        args += cfg.get('files', [])
+        # Add output folder argument if not already specified in cfg['args']
+        if 'args' not in cfg or not ({'-o', '--output'} & set(cfg['args'])):
+            args += ['-o', str(paths.staging_dir)]
+        env = os.environ.copy()
+        env.setdefault('MYPY_CACHE_DIR', str(paths.temp_dir))
+        # Call mypy stubgen in a subprocess
+        self.runner.run(args, cwd=pkg.path.parent, check=True, env=env)
+
+    # --- Misc helper functions -----------------------------------------------
+
+    @staticmethod
+    def get_os_name():
+        return {
+            "Linux": "linux",
+            "Windows": "windows",
+            "Darwin": "mac",
+        }[platform.system()]
+
+    @staticmethod
+    def print_config_verbose(cfg):
+        from . import __version__
+        print("\npy-build-cmake (" + __version__ + ")")
+        print("options")
+        print("================================")
+        print("module:")
+        pprint(cfg.module)
+        print("editable:")
+        pprint(cfg.editable)
+        print("sdist:")
+        pprint(cfg.sdist)
+        print("cmake:")
+        pprint(cfg.cmake)
+        print("stubgen:")
+        pprint(cfg.stubgen)
+        print("cross:")
+        pprint(cfg.cross)
+        print("================================\n")
+
+    @staticmethod
+    def normalize_version(version):
+        from distlib.version import NormalizedVersion
+        norm_version = str(NormalizedVersion(version))
+        return norm_version
+
+    @staticmethod
+    def get_native_tags():
+        """Get the PEP 425 tags for the current platform."""
+        from .tags import get_python_tag, get_abi_tag, get_platform_tag
+        return {
+            'pyver': [get_python_tag()],
+            'abi': [get_abi_tag()],
+            'arch': [get_platform_tag()],
+        }
+
+    @staticmethod
+    def get_cross_tags(crosscfg):
+        """Get the PEP 425 tags to use when cross-compiling."""
+        tags = _BuildBackend.get_native_tags()
+        if 'implementation' in crosscfg and 'version' in crosscfg:
+            tags['pyver'] = [crosscfg['implementation'] + crosscfg['version']]
+        if 'abi' in crosscfg:
+            tags['abi'] = [crosscfg['abi']]
+        if 'arch' in crosscfg:
+            tags['arch'] = [crosscfg['arch']]
+        return tags
+
+    @staticmethod
+    def get_build_config_name(cross_cfg):
+        """Get a string representing the Python version, ABI and architecture,
+        used to name the build folder so builds for different versions don't
+        interfere."""
+        if cross_cfg:
+            tags = _BuildBackend.get_cross_tags(cross_cfg)
+        else:
+            tags = _BuildBackend.get_native_tags()
+        return '-'.join(map(lambda x: x[0], tags.values()))
+
+    @staticmethod
+    def needs_cross_native_build(cfg):
+        return cfg.cross and 'copy_from_native_build' in cfg.cross
+
+    @staticmethod
+    def iter_files(stagedir):
+        """Iterate over the files contained in the given folder.
+
+        Yields absolute paths - caller may want to make them relative.
+        Excludes any __pycache__ and *.pyc files."""
+
+        # https://github.com/pypa/flit/blob/a4524758604107bde8c77b5816612edb76a604aa/flit_core/flit_core/common.py#L73
+
+        def _include(path):
+            name = os.path.basename(path)
+            return name != '__pycache__' and not name.endswith('.pyc')
+
+        # Ensure we sort all files and directories so the order is stable
+        for dirpath, dirs, files in os.walk(str(stagedir)):
+            for file in sorted(files):
+                full_path = os.path.join(dirpath, file)
+                if _include(full_path):
+                    yield full_path
+
+            dirs[:] = [d for d in sorted(dirs) if _include(d)]
+
+    # --- Helper functions for finding programs like CMake --------------------
+
+    @staticmethod
+    def check_cmake_program(cfg: config.Config, deps: List[str],
+                            runner: CommandRunner):
+        assert cfg.cmake
+        # Do we need to perform a native build?
+        native = not cfg.cross or _BuildBackend.needs_cross_native_build(cfg)
+        native_cfg = cfg.cmake[_BuildBackend.get_os_name()] if native else {}
+        # Do we need to perform a cross build?
+        cross = cfg.cross
+        cross_cfg = cfg.cmake.get('cross', {})
+        # Find the strictest version requirement
+        min_cmake_ver = max(
+            _CMAKE_MINIMUM_REQUIRED,
+            NormalizedVersion(native_cfg.get('minimum_version', '0.0')),
+            NormalizedVersion(cross_cfg.get('minimum_version', '0.0')),
+        )
+        # If CMake in PATH doesn't work or is too old, add it as a build
+        # requirement
+        if not runner.check_program_version('cmake', min_cmake_ver, "CMake"):
+            deps.append("cmake>=" + str(min_cmake_ver))
+
+        # Check if we need Ninja
+        cfgs = []
+        if native: cfgs.append(native_cfg)
+        if cross: cfgs.append(cross_cfg)
+        # Do any of the configs require Ninja as a generator?
+        needs_ninja = lambda c: 'ninja' in c.get('generator', '').lower()
+        need_ninja = any(map(needs_ninja, cfgs))
+        if need_ninja:
+            # If so, check if a working version exists in the PATH, otherwise,
+            # add it as a build requirement
+            if not runner.check_program_version('ninja', None, "Ninja"):
+                deps.append("ninja")
+
+    @staticmethod
+    def check_stubgen_program(deps: List[str], runner: CommandRunner):
+        if not runner.check_program_version('stubgen', None, None, False):
+            deps.append("mypy")
+
+
+_BACKEND = _BuildBackend()
+get_requires_for_build_wheel = _BACKEND.get_requires_for_build_wheel
+get_requires_for_build_sdist = _BACKEND.get_requires_for_build_sdist
+get_requires_for_build_editable = _BACKEND.get_requires_for_build_editable
+build_wheel = _BACKEND.build_wheel
+build_sdist = _BACKEND.build_sdist
+build_editable = _BACKEND.build_editable
```

### Comparing `py-build-cmake-0.1.7/src/py_build_cmake/cli.py` & `py-build-cmake-0.1.8/src/py_build_cmake/cli.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,261 +1,261 @@
-from . import __version__
-from pathlib import Path
-import click
-
-
-def cmake_command(directory, build_path, verbose, dry, native, cross, local):
-
-    def get_cmaker():
-        from .build import _BuildBackend as backend
-        from .datastructures import PackageInfo
-        from .cmd_runner import CommandRunner
-        source_dir = Path(directory or '.').resolve()
-        config_settings = {
-            "--cross": list(cross),
-            "--local": list(local),
-        }
-        # Read configuration and package metadata
-        cfg, pkg, metadata = backend.read_all_metadata(source_dir,
-                                                       config_settings,
-                                                       verbose)
-
-        if not cfg.cmake:
-            print("Not a CMake package")
-            return None
-
-        pkg_info = PackageInfo(
-            version=metadata.version,
-            package_name=cfg.package_name,
-            module_name=cfg.module["name"],
-        )
-        # Select the right configuration (native build or cross build)
-        cmake_cfg, native_cmake_cfg = backend.get_cmake_configs(cfg)
-        cmake_cfg = native_cmake_cfg if native else cmake_cfg
-        cross_cfg = None if native else cfg.cross
-        # Override the build folder
-        if build_path is not None:
-            cmake_cfg['build_path'] = str(build_path)
-        # Configure all CMake options
-        return backend.get_cmaker(pkg_dir=source_dir,
-                                  install_dir=None,
-                                  cmake_cfg=cmake_cfg,
-                                  cross_cfg=cross_cfg,
-                                  native_install_dir=None,
-                                  package_info=pkg_info,
-                                  runner=CommandRunner(verbose=verbose,
-                                                       dry=dry))
-
-    return get_cmaker
-
-
-@click.group()
-@click.option("-C",
-              "--directory",
-              type=click.Path(exists=True, file_okay=False, dir_okay=True),
-              required=False,
-              help="The directory containing pyproject.toml.")
-@click.option("-B",
-              "--build-path",
-              type=click.Path(exists=False, file_okay=False, dir_okay=True),
-              required=False,
-              default=None,
-              help="Override py-build-cmake's default build folder.")
-@click.option("-V",
-              "--verbose",
-              is_flag=True,
-              help="Print verbose information about the commands being "
-              "executed.")
-@click.option("-n",
-              "--dry",
-              is_flag=True,
-              help="Print the commands without actually invoking CMake.")
-@click.option("--native",
-              is_flag=True,
-              help="When the configuration requests cross-compiling, "
-              "configure for a native build instead. Has no effect otherwise.")
-@click.option("--local",
-              type=click.Path(exists=False, file_okay=True, dir_okay=False),
-              required=False,
-              multiple=True,
-              help="Specifies a toml file that overrides the "
-              "tool.py-build-cmake section of pyproject.toml, "
-              "similar to py-build-cmake.local.toml.")
-@click.option("--cross",
-              type=click.Path(exists=False, file_okay=True, dir_okay=False),
-              required=False,
-              multiple=True,
-              help="Specifies a toml file that overrides the "
-              "tool.py-build-cmake.cross section of pyproject.toml, "
-              "similar to py-build-cmake.cross.toml.")
-@click.version_option(__version__, "-v", "--version")
-@click.pass_context
-def cli(ctx: click.Context, **kwargs):
-    ctx.obj = cmake_command(**kwargs)
-
-
-@cli.command(help="Configure the CMake project.")
-@click.pass_obj
-@click.option("--preset", nargs=1, type=str, required=False, metavar="PRESET")
-@click.argument("args", nargs=-1, required=False)
-def configure(obj, preset, args):
-    cmaker = obj()
-    if cmaker is None:
-        return
-    cmaker.conf_settings.args += args or []
-    if preset is not None:
-        cmaker.conf_settings.preset = preset
-    cmaker.configure()
-
-
-@cli.command(help="Build the CMake project.")
-@click.pass_obj
-@click.option("--preset",
-              nargs=1,
-              multiple=True,
-              type=str,
-              required=False,
-              metavar="PRESET")
-@click.option("--config",
-              nargs=1,
-              multiple=True,
-              type=str,
-              required=False,
-              metavar="CONFIG")
-@click.argument("args", nargs=-1, required=False)
-def build(obj, preset, config, args):
-    cmaker = obj()
-    if cmaker is None:
-        return
-    cmaker.build_settings.args += args or []
-    if preset or config:
-        cmaker.build_settings.presets = []
-        cmaker.build_settings.configs = []
-    if preset:
-        cmaker.build_settings.presets = preset
-    if config:
-        cmaker.build_settings.configs = config
-    cmaker.build()
-
-
-@cli.command(help="Install the CMake project.")
-@click.pass_obj
-@click.option("--preset",
-              nargs=1,
-              multiple=True,
-              type=str,
-              required=False,
-              metavar="PRESET")
-@click.option("--config",
-              nargs=1,
-              multiple=True,
-              type=str,
-              required=False,
-              metavar="CONFIG")
-@click.option("--component",
-              nargs=1,
-              multiple=True,
-              type=str,
-              required=False,
-              metavar="COMP")
-@click.argument("args", nargs=-1, required=False)
-def install(obj, preset, config, component, args):
-    cmaker = obj()
-    if cmaker is None:
-        return
-    cmaker.install_settings.args += args or []
-    if preset or config:
-        cmaker.install_settings.presets = []
-        cmaker.install_settings.configs = []
-    if preset:
-        cmaker.install_settings.presets = preset
-    if config:
-        cmaker.install_settings.configs = config
-    if component:
-        cmaker.install_settings.components = component
-    cmaker.install()
-
-
-@cli.group(help="Config file operations.")
-def config():
-    pass
-
-
-@config.command(help="Print documentation for the config file format.")
-@click.option("--md", is_flag=True, help="Use the MarkDown format.")
-@click.option("--component",
-              is_flag=True,
-              help="Documentation for the build_component backend.")
-def format(md, component):
-    from .pyproject_options import get_options, get_component_options
-    from .config_options import pth
-    if md:
-        from .help import help_print_md as help_print
-    else:
-        from .help import help_print as help_print
-    help_pth = pth('pyproject.toml/tool/py-build-cmake')
-    pr_md = print if md else lambda *args, **kwargs: None
-    pr_tx = lambda *args, **kwargs: None if md else print
-    if component:
-        pr_tx("List of py-build-cmake pyproject.toml options for the "
-              "build_component backend:")
-        pr_md("# py-build-cmake component build backend\n"
-              "The `py_build_cmake.build_component` build backend allows "
-              "building packages containing additional binaries that are not "
-              "included with the main distribution.\n")
-        pr_md("A possible use case is distributing debug symbols: these files "
-              "can be large, and most users don't need them, so distributing "
-              "them in a separate package makes sense.\n")
-        pr_md(
-            "You can find an example in the "
-            "[alpaqa](https://pypi.org/project/alpaqa) package: "
-            "<https://github.com/kul-optec/alpaqa/blob/main/python/alpaqa-debug/pyproject.toml>"
-        )
-        help_print(get_component_options(Path('/'))[help_pth])
-
-    else:
-        pr_tx("List of py-build-cmake pyproject.toml options:")
-        pr_md("# py-build-cmake configuration options\n")
-        pr_md("These options go in the `[tool.py-build-cmake]` section of "
-              "the `pyproject.toml` configuration file.\n")
-        help_print(get_options(Path('/'))[help_pth])
-        pr_md("# Local overrides\n")
-        pr_md("Additionally, two extra configuration files can be placed in "
-              "the same directory as `pyproject.toml` to override some "
-              "options for your specific use case:\n\n"
-              "- `py-build-cmake.local.toml`: the options in this file "
-              "override the values in the `tool.py-build-cmake` section of "
-              "`pyproject.toml`.<br/>This is useful if you need specific "
-              "arguments or CMake options to compile the package on your "
-              "system.\n"
-              "- `py-build-cmake.cross.toml`: the options in this file "
-              "override the values in the `tool.py-build-cmake.cross` section "
-              "of `pyproject.toml`.<br/>Useful for cross-compiling the "
-              "package without having to edit the main configuration file.\n")
-        pr_md("# Command line overrides\n")
-        pr_md("Instead of using the `py-build-cmake.local.toml` and "
-              "`py-build-cmake.cross.toml` files, you can also include "
-              "additional config files using command line options:\n\n"
-              "- `--local`: specifies a toml file that overrides the "
-              "`tool.py-build-cmake` section of `pyproject.toml`, "
-              "similar to `py-build-cmake.local.toml`\n"
-              "- `--cross`: specifies a toml file that overrides the "
-              "`tool.py-build-cmake.cross` section of `pyproject.toml`, "
-              "similar to `py-build-cmake.cross.toml`\n\n"
-              "These command line overrides are applied after the "
-              "`py-build-cmake.local.toml` and `py-build-cmake.cross.toml` "
-              "files in the project folder (if any).\n\n"
-              "When using PyPA build, these flags can be specified using "
-              "the `-C` or `--config-setting` flag: \n"
-              "```sh\n"
-              "python -m build . -C--cross=/path/to/my-cross-config.toml\n"
-              "```\n"
-              "The same flag may appear multiple times, for example: \n"
-              "```sh\n"
-              "python -m build . -C--local=conf-A.toml -C--local=conf-B.toml\n"
-              "```\n"
-              "For PyPA pip, you can use the `--config-settings` flag "
-              "instead.")
-
-
-if __name__ == '__main__':
-    cli()
+from . import __version__
+from pathlib import Path
+import click
+
+
+def cmake_command(directory, build_path, verbose, dry, native, cross, local):
+
+    def get_cmaker():
+        from .build import _BuildBackend as backend
+        from .datastructures import PackageInfo
+        from .cmd_runner import CommandRunner
+        source_dir = Path(directory or '.').resolve()
+        config_settings = {
+            "--cross": list(cross),
+            "--local": list(local),
+        }
+        # Read configuration and package metadata
+        cfg, pkg, metadata = backend.read_all_metadata(source_dir,
+                                                       config_settings,
+                                                       verbose)
+
+        if not cfg.cmake:
+            print("Not a CMake package")
+            return None
+
+        pkg_info = PackageInfo(
+            version=metadata.version,
+            package_name=cfg.package_name,
+            module_name=cfg.module["name"],
+        )
+        # Select the right configuration (native build or cross build)
+        cmake_cfg, native_cmake_cfg = backend.get_cmake_configs(cfg)
+        cmake_cfg = native_cmake_cfg if native else cmake_cfg
+        cross_cfg = None if native else cfg.cross
+        # Override the build folder
+        if build_path is not None:
+            cmake_cfg['build_path'] = str(build_path)
+        # Configure all CMake options
+        return backend.get_cmaker(pkg_dir=source_dir,
+                                  install_dir=None,
+                                  cmake_cfg=cmake_cfg,
+                                  cross_cfg=cross_cfg,
+                                  native_install_dir=None,
+                                  package_info=pkg_info,
+                                  runner=CommandRunner(verbose=verbose,
+                                                       dry=dry))
+
+    return get_cmaker
+
+
+@click.group()
+@click.option("-C",
+              "--directory",
+              type=click.Path(exists=True, file_okay=False, dir_okay=True),
+              required=False,
+              help="The directory containing pyproject.toml.")
+@click.option("-B",
+              "--build-path",
+              type=click.Path(exists=False, file_okay=False, dir_okay=True),
+              required=False,
+              default=None,
+              help="Override py-build-cmake's default build folder.")
+@click.option("-V",
+              "--verbose",
+              is_flag=True,
+              help="Print verbose information about the commands being "
+              "executed.")
+@click.option("-n",
+              "--dry",
+              is_flag=True,
+              help="Print the commands without actually invoking CMake.")
+@click.option("--native",
+              is_flag=True,
+              help="When the configuration requests cross-compiling, "
+              "configure for a native build instead. Has no effect otherwise.")
+@click.option("--local",
+              type=click.Path(exists=False, file_okay=True, dir_okay=False),
+              required=False,
+              multiple=True,
+              help="Specifies a toml file that overrides the "
+              "tool.py-build-cmake section of pyproject.toml, "
+              "similar to py-build-cmake.local.toml.")
+@click.option("--cross",
+              type=click.Path(exists=False, file_okay=True, dir_okay=False),
+              required=False,
+              multiple=True,
+              help="Specifies a toml file that overrides the "
+              "tool.py-build-cmake.cross section of pyproject.toml, "
+              "similar to py-build-cmake.cross.toml.")
+@click.version_option(__version__, "-v", "--version")
+@click.pass_context
+def cli(ctx: click.Context, **kwargs):
+    ctx.obj = cmake_command(**kwargs)
+
+
+@cli.command(help="Configure the CMake project.")
+@click.pass_obj
+@click.option("--preset", nargs=1, type=str, required=False, metavar="PRESET")
+@click.argument("args", nargs=-1, required=False)
+def configure(obj, preset, args):
+    cmaker = obj()
+    if cmaker is None:
+        return
+    cmaker.conf_settings.args += args or []
+    if preset is not None:
+        cmaker.conf_settings.preset = preset
+    cmaker.configure()
+
+
+@cli.command(help="Build the CMake project.")
+@click.pass_obj
+@click.option("--preset",
+              nargs=1,
+              multiple=True,
+              type=str,
+              required=False,
+              metavar="PRESET")
+@click.option("--config",
+              nargs=1,
+              multiple=True,
+              type=str,
+              required=False,
+              metavar="CONFIG")
+@click.argument("args", nargs=-1, required=False)
+def build(obj, preset, config, args):
+    cmaker = obj()
+    if cmaker is None:
+        return
+    cmaker.build_settings.args += args or []
+    if preset or config:
+        cmaker.build_settings.presets = []
+        cmaker.build_settings.configs = []
+    if preset:
+        cmaker.build_settings.presets = preset
+    if config:
+        cmaker.build_settings.configs = config
+    cmaker.build()
+
+
+@cli.command(help="Install the CMake project.")
+@click.pass_obj
+@click.option("--preset",
+              nargs=1,
+              multiple=True,
+              type=str,
+              required=False,
+              metavar="PRESET")
+@click.option("--config",
+              nargs=1,
+              multiple=True,
+              type=str,
+              required=False,
+              metavar="CONFIG")
+@click.option("--component",
+              nargs=1,
+              multiple=True,
+              type=str,
+              required=False,
+              metavar="COMP")
+@click.argument("args", nargs=-1, required=False)
+def install(obj, preset, config, component, args):
+    cmaker = obj()
+    if cmaker is None:
+        return
+    cmaker.install_settings.args += args or []
+    if preset or config:
+        cmaker.install_settings.presets = []
+        cmaker.install_settings.configs = []
+    if preset:
+        cmaker.install_settings.presets = preset
+    if config:
+        cmaker.install_settings.configs = config
+    if component:
+        cmaker.install_settings.components = component
+    cmaker.install()
+
+
+@cli.group(help="Config file operations.")
+def config():
+    pass
+
+
+@config.command(help="Print documentation for the config file format.")
+@click.option("--md", is_flag=True, help="Use the MarkDown format.")
+@click.option("--component",
+              is_flag=True,
+              help="Documentation for the build_component backend.")
+def format(md, component):
+    from .pyproject_options import get_options, get_component_options
+    from .config_options import pth
+    if md:
+        from .help import help_print_md as help_print
+    else:
+        from .help import help_print as help_print
+    help_pth = pth('pyproject.toml/tool/py-build-cmake')
+    pr_md = print if md else lambda *args, **kwargs: None
+    pr_tx = lambda *args, **kwargs: None if md else print
+    if component:
+        pr_tx("List of py-build-cmake pyproject.toml options for the "
+              "build_component backend:")
+        pr_md("# py-build-cmake component build backend\n"
+              "The `py_build_cmake.build_component` build backend allows "
+              "building packages containing additional binaries that are not "
+              "included with the main distribution.\n")
+        pr_md("A possible use case is distributing debug symbols: these files "
+              "can be large, and most users don't need them, so distributing "
+              "them in a separate package makes sense.\n")
+        pr_md(
+            "You can find an example in the "
+            "[alpaqa](https://pypi.org/project/alpaqa) package: "
+            "<https://github.com/kul-optec/alpaqa/blob/main/python/alpaqa-debug/pyproject.toml>"
+        )
+        help_print(get_component_options(Path('/'))[help_pth])
+
+    else:
+        pr_tx("List of py-build-cmake pyproject.toml options:")
+        pr_md("# py-build-cmake configuration options\n")
+        pr_md("These options go in the `[tool.py-build-cmake]` section of "
+              "the `pyproject.toml` configuration file.\n")
+        help_print(get_options(Path('/'))[help_pth])
+        pr_md("# Local overrides\n")
+        pr_md("Additionally, two extra configuration files can be placed in "
+              "the same directory as `pyproject.toml` to override some "
+              "options for your specific use case:\n\n"
+              "- `py-build-cmake.local.toml`: the options in this file "
+              "override the values in the `tool.py-build-cmake` section of "
+              "`pyproject.toml`.<br/>This is useful if you need specific "
+              "arguments or CMake options to compile the package on your "
+              "system.\n"
+              "- `py-build-cmake.cross.toml`: the options in this file "
+              "override the values in the `tool.py-build-cmake.cross` section "
+              "of `pyproject.toml`.<br/>Useful for cross-compiling the "
+              "package without having to edit the main configuration file.\n")
+        pr_md("# Command line overrides\n")
+        pr_md("Instead of using the `py-build-cmake.local.toml` and "
+              "`py-build-cmake.cross.toml` files, you can also include "
+              "additional config files using command line options:\n\n"
+              "- `--local`: specifies a toml file that overrides the "
+              "`tool.py-build-cmake` section of `pyproject.toml`, "
+              "similar to `py-build-cmake.local.toml`\n"
+              "- `--cross`: specifies a toml file that overrides the "
+              "`tool.py-build-cmake.cross` section of `pyproject.toml`, "
+              "similar to `py-build-cmake.cross.toml`\n\n"
+              "These command line overrides are applied after the "
+              "`py-build-cmake.local.toml` and `py-build-cmake.cross.toml` "
+              "files in the project folder (if any).\n\n"
+              "When using PyPA build, these flags can be specified using "
+              "the `-C` or `--config-setting` flag: \n"
+              "```sh\n"
+              "python -m build . -C--cross=/path/to/my-cross-config.toml\n"
+              "```\n"
+              "The same flag may appear multiple times, for example: \n"
+              "```sh\n"
+              "python -m build . -C--local=conf-A.toml -C--local=conf-B.toml\n"
+              "```\n"
+              "For PyPA pip, you can use the `--config-settings` flag "
+              "instead.")
+
+
+if __name__ == '__main__':
+    cli()
```

### Comparing `py-build-cmake-0.1.7/src/py_build_cmake/config.py` & `py-build-cmake-0.1.8/src/py_build_cmake/config.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,264 +1,264 @@
-from dataclasses import dataclass, field
-import re
-import os
-import warnings
-from typing import Any, Dict, List, Optional, Set, cast
-from pathlib import Path
-from flit_core.config import ConfigError, read_pep621_metadata  # type: ignore
-from flit_core.config import _check_glob_patterns  # type: ignore
-from distlib.util import normalize_name  # type: ignore
-
-from .config_options import ConfigNode, OverrideConfigOption
-from .pyproject_options import get_options, get_cross_path, get_tool_pbc_path, get_component_options
-
-try:
-    import tomllib as toml_  # type: ignore
-except ImportError:
-    import tomli as toml_  # type: ignore
-
-
-@dataclass
-class Config:
-    dynamic_metadata: Set[str] = field(default_factory=set)
-    entrypoints: Dict[str, Dict[str, str]] = field(default_factory=dict)
-    metadata: Dict[str, Any] = field(default_factory=dict)
-    referenced_files: List[str] = field(default_factory=list)
-    package_name: str = field(default='')
-    module: Dict[str, str] = field(default_factory=dict)
-    editable: Dict[str, Any] = field(default_factory=dict)
-    sdist: Dict[str, Dict[str, Any]] = field(default_factory=dict)
-    license: Dict[str, str] = field(default_factory=dict)
-    cmake: Optional[Dict[str, Any]] = field(default=None)
-    stubgen: Optional[Dict[str, Any]] = field(default=None)
-    cross: Optional[Dict[str, Any]] = field(default=None)
-
-
-def read_config(pyproject_path, flag_overrides: Dict[str,
-                                                     List[str]]) -> Config:
-    # Load the pyproject.toml file
-    pyproject_path = Path(pyproject_path)
-    pyproject_folder = pyproject_path.parent
-    pyproject = toml_.loads(pyproject_path.read_text('utf-8'))
-    if 'project' not in pyproject:
-        raise ConfigError('Missing [project] table')
-
-    # Load local override
-    localconfig_fname = 'py-build-cmake.local.toml'
-    localconfig_path = pyproject_folder / localconfig_fname
-    localconfig = None
-    if localconfig_path.exists():
-        localconfig = toml_.loads(localconfig_path.read_text('utf-8'))
-        # treat empty local override as no local override
-        localconfig = localconfig or None
-
-    # Load override for cross-compilation
-    crossconfig_fname = 'py-build-cmake.cross.toml'
-    crossconfig_path = pyproject_folder / crossconfig_fname
-    crossconfig = None
-    if crossconfig_path.exists():
-        crossconfig = toml_.loads(crossconfig_path.read_text('utf-8'))
-        crossconfig = crossconfig or None
-
-    # File names mapping to the actual dict with the config
-    config_files = {
-        "pyproject.toml": pyproject,
-        localconfig_fname: localconfig,
-        crossconfig_fname: crossconfig,
-    }
-    # Additional options for config_options
-    extra_options: List[OverrideConfigOption] = []
-
-    def try_load_local(path: Path):
-        if not path.exists():
-            raise FileNotFoundError(path.absolute())
-        return toml_.loads(path.read_text('utf-8'))
-
-    extra_flag_paths = {
-        '--local': get_tool_pbc_path(),
-        '--cross': get_cross_path(),
-    }
-
-    for flag, targetpath in extra_flag_paths.items():
-        for path in map(Path, flag_overrides[flag]):
-            if not path.is_absolute():
-                path = (Path(os.environ.get("PWD", ".")) / path).resolve()
-            extra_options.append(
-                OverrideConfigOption(
-                    str(path),
-                    "Command line override flag",
-                    targetpath=targetpath,
-                ))
-            config_files[str(path)] = try_load_local(path)
-
-    return check_config(pyproject_path, pyproject, config_files, extra_options)
-
-
-def check_config(pyproject_path, pyproject, config_files, extra_options):
-    # Check the package/module name and normalize it
-    f = 'name'
-    if f in pyproject['project']:
-        normname = normalize_name(pyproject['project'][f])
-        if pyproject['project'][f] != normname:
-            warnings.warn(
-                f"Name changed from {pyproject['project'][f]} to {normname}")
-        pyproject['project'][f] = normname
-
-    # Parse the [project] section for metadata (using flit's parser)
-    flit_cfg = read_pep621_metadata(pyproject['project'], pyproject_path)
-
-    # Create our own config data structure using flit's output
-    cfg = Config()
-    cfg.dynamic_metadata = set(flit_cfg.dynamic_metadata)
-    cfg.entrypoints = flit_cfg.entrypoints
-    cfg.metadata = flit_cfg.metadata
-    cfg.referenced_files = flit_cfg.referenced_files
-    cfg.license = pyproject['project'].setdefault('license', {})
-    cfg.package_name = normalize_name_wheel(cfg.metadata["name"])
-
-    if 'file' in cfg.license and Path(cfg.license['file']).is_absolute():
-        raise ConfigError("License path must be relative")
-
-    opts = get_options(pyproject_path.parent)
-    for o in extra_options:
-        opts.insert(o)
-
-    tree_config = ConfigNode.from_dict(config_files)
-    opts.verify_all(tree_config)
-    opts.override_all(tree_config)
-    opts.inherit_all(tree_config)
-    opts.update_default_all(tree_config)
-    dictcfg = cast(dict, tree_config.to_dict())
-    tool_cfg = dictcfg['pyproject.toml']['tool']['py-build-cmake']
-
-    # Store the module configuration
-    s = 'module'
-    if s in tool_cfg:
-        # Normalize the import and wheel name of the package
-        normname = normalize_name_wheel(tool_cfg[s]['name'])
-        if tool_cfg[s]['name'] != normname:
-            print(f"Name changed from {tool_cfg[s]['name']} to {normname}")
-            # TODO: use logging instead of print
-        tool_cfg[s]['name'] = normname
-        cfg.module = tool_cfg[s]
-    else:
-        assert False, "Missing [tools.py-build-cmake.module] section"
-
-    # Store the editable configuration
-    cfg.editable = {
-        os: tool_cfg[os]['editable']
-        for os in ("linux", "windows", "mac")
-        if os in tool_cfg and 'editable' in tool_cfg[os]
-    }
-
-    # Store the sdist folders (this is based on flit)
-    def get_sdist_cludes(cfg):
-        return {
-            cl + '_patterns': _check_glob_patterns(cfg['sdist'][cl], cl)
-            for cl in ('include', 'exclude')
-        }
-
-    cfg.sdist = {
-        os: get_sdist_cludes(tool_cfg[os])
-        for os in ("linux", "windows", "mac")
-    }
-    s = 'cross'
-    if s in tool_cfg:
-        cfg.sdist.update({
-            'cross': get_sdist_cludes(tool_cfg[s]),
-        })
-
-    # Store the CMake configuration
-    cfg.cmake = {
-        os: tool_cfg[os]['cmake']
-        for os in ("linux", "windows", "mac")
-        if os in tool_cfg and 'cmake' in tool_cfg[os]
-    }
-
-    # Store stubgen configuration
-    s = 'stubgen'
-    if s in tool_cfg:
-        cfg.stubgen = tool_cfg[s]
-
-    # Store the cross compilation configuration
-    s = 'cross'
-    if s in tool_cfg:
-        cfg.cross = tool_cfg[s]
-        f = 'copy_from_native_build'
-        if f in cfg.cross:
-            cfg.cross[f] = _check_glob_patterns(cfg.cross[f], f'cross.{f}')
-        cfg.cmake.update({
-            'cross': cfg.cross.pop('cmake', {}),
-        })
-
-    return cfg
-
-
-@dataclass
-class ComponentConfig:
-    dynamic_metadata: Set[str] = field(default_factory=set)
-    entrypoints: Dict[str, Dict[str, str]] = field(default_factory=dict)
-    metadata: Dict[str, Any] = field(default_factory=dict)
-    referenced_files: List[str] = field(default_factory=list)
-    package_name: str = field(default='')
-    component: Dict[str, Any] = field(default_factory=dict)
-    license: Dict[str, str] = field(default_factory=dict)
-
-
-def read_component_config(pyproject_path) -> ComponentConfig:
-    # Load the pyproject.toml file
-    pyproject_path = Path(pyproject_path)
-    pyproject = toml_.loads(pyproject_path.read_text('utf-8'))
-    if 'project' not in pyproject:
-        raise ConfigError('Missing [project] table')
-
-    # File names mapping to the actual dict with the config
-    config_files = {
-        "pyproject.toml": pyproject,
-    }
-    return check_component_config(pyproject_path, pyproject, config_files)
-
-
-def check_component_config(pyproject_path, pyproject, config_files):
-    # Check the package/module name and normalize it
-    f = 'name'
-    if f in pyproject['project']:
-        normname = normalize_name(pyproject['project'][f])
-        if pyproject['project'][f] != normname:
-            warnings.warn(
-                f"Name changed from {pyproject['project'][f]} to {normname}")
-        pyproject['project'][f] = normname
-
-    # Parse the [project] section for metadata (using flit's parser)
-    flit_cfg = read_pep621_metadata(pyproject['project'], pyproject_path)
-
-    # Create our own config data structure using flit's output
-    cfg = ComponentConfig()
-    cfg.dynamic_metadata = set(flit_cfg.dynamic_metadata)
-    cfg.entrypoints = flit_cfg.entrypoints
-    cfg.metadata = flit_cfg.metadata
-    cfg.referenced_files = flit_cfg.referenced_files
-    cfg.license = pyproject['project'].setdefault('license', {})
-    cfg.package_name = normalize_name_wheel(cfg.metadata["name"])
-
-    if 'file' in cfg.license and Path(cfg.license['file']).is_absolute():
-        raise ConfigError("License path must be relative")
-
-    opts = get_component_options(pyproject_path.parent)
-
-    tree_config = ConfigNode.from_dict(config_files)
-    opts.verify_all(tree_config)
-    opts.override_all(tree_config)
-    opts.inherit_all(tree_config)
-    opts.update_default_all(tree_config)
-    dictcfg = cast(dict, tree_config.to_dict())
-    tool_cfg = dictcfg['pyproject.toml']['tool']['py-build-cmake']
-
-    # Store the component configuration
-    cfg.component = tool_cfg['component']
-
-    return cfg
-
-
-def normalize_name_wheel(name):
-    """https://www.python.org/dev/peps/pep-0427/#escaping-and-unicode"""
-    return re.sub(r"[^\w\d.]+", "_", name, re.UNICODE)
+from dataclasses import dataclass, field
+import re
+import os
+import warnings
+from typing import Any, Dict, List, Optional, Set, cast
+from pathlib import Path
+from flit_core.config import ConfigError, read_pep621_metadata  # type: ignore
+from flit_core.config import _check_glob_patterns  # type: ignore
+from distlib.util import normalize_name  # type: ignore
+
+from .config_options import ConfigNode, OverrideConfigOption
+from .pyproject_options import get_options, get_cross_path, get_tool_pbc_path, get_component_options
+
+try:
+    import tomllib as toml_  # type: ignore
+except ImportError:
+    import tomli as toml_  # type: ignore
+
+
+@dataclass
+class Config:
+    dynamic_metadata: Set[str] = field(default_factory=set)
+    entrypoints: Dict[str, Dict[str, str]] = field(default_factory=dict)
+    metadata: Dict[str, Any] = field(default_factory=dict)
+    referenced_files: List[str] = field(default_factory=list)
+    package_name: str = field(default='')
+    module: Dict[str, str] = field(default_factory=dict)
+    editable: Dict[str, Any] = field(default_factory=dict)
+    sdist: Dict[str, Dict[str, Any]] = field(default_factory=dict)
+    license: Dict[str, str] = field(default_factory=dict)
+    cmake: Optional[Dict[str, Any]] = field(default=None)
+    stubgen: Optional[Dict[str, Any]] = field(default=None)
+    cross: Optional[Dict[str, Any]] = field(default=None)
+
+
+def read_config(pyproject_path, flag_overrides: Dict[str,
+                                                     List[str]]) -> Config:
+    # Load the pyproject.toml file
+    pyproject_path = Path(pyproject_path)
+    pyproject_folder = pyproject_path.parent
+    pyproject = toml_.loads(pyproject_path.read_text('utf-8'))
+    if 'project' not in pyproject:
+        raise ConfigError('Missing [project] table')
+
+    # Load local override
+    localconfig_fname = 'py-build-cmake.local.toml'
+    localconfig_path = pyproject_folder / localconfig_fname
+    localconfig = None
+    if localconfig_path.exists():
+        localconfig = toml_.loads(localconfig_path.read_text('utf-8'))
+        # treat empty local override as no local override
+        localconfig = localconfig or None
+
+    # Load override for cross-compilation
+    crossconfig_fname = 'py-build-cmake.cross.toml'
+    crossconfig_path = pyproject_folder / crossconfig_fname
+    crossconfig = None
+    if crossconfig_path.exists():
+        crossconfig = toml_.loads(crossconfig_path.read_text('utf-8'))
+        crossconfig = crossconfig or None
+
+    # File names mapping to the actual dict with the config
+    config_files = {
+        "pyproject.toml": pyproject,
+        localconfig_fname: localconfig,
+        crossconfig_fname: crossconfig,
+    }
+    # Additional options for config_options
+    extra_options: List[OverrideConfigOption] = []
+
+    def try_load_local(path: Path):
+        if not path.exists():
+            raise FileNotFoundError(path.absolute())
+        return toml_.loads(path.read_text('utf-8'))
+
+    extra_flag_paths = {
+        '--local': get_tool_pbc_path(),
+        '--cross': get_cross_path(),
+    }
+
+    for flag, targetpath in extra_flag_paths.items():
+        for path in map(Path, flag_overrides[flag]):
+            if not path.is_absolute():
+                path = (Path(os.environ.get("PWD", ".")) / path).resolve()
+            extra_options.append(
+                OverrideConfigOption(
+                    str(path),
+                    "Command line override flag",
+                    targetpath=targetpath,
+                ))
+            config_files[str(path)] = try_load_local(path)
+
+    return check_config(pyproject_path, pyproject, config_files, extra_options)
+
+
+def check_config(pyproject_path, pyproject, config_files, extra_options):
+    # Check the package/module name and normalize it
+    f = 'name'
+    if f in pyproject['project']:
+        normname = normalize_name(pyproject['project'][f])
+        if pyproject['project'][f] != normname:
+            warnings.warn(
+                f"Name changed from {pyproject['project'][f]} to {normname}")
+        pyproject['project'][f] = normname
+
+    # Parse the [project] section for metadata (using flit's parser)
+    flit_cfg = read_pep621_metadata(pyproject['project'], pyproject_path)
+
+    # Create our own config data structure using flit's output
+    cfg = Config()
+    cfg.dynamic_metadata = set(flit_cfg.dynamic_metadata)
+    cfg.entrypoints = flit_cfg.entrypoints
+    cfg.metadata = flit_cfg.metadata
+    cfg.referenced_files = flit_cfg.referenced_files
+    cfg.license = pyproject['project'].setdefault('license', {})
+    cfg.package_name = normalize_name_wheel(cfg.metadata["name"])
+
+    if 'file' in cfg.license and Path(cfg.license['file']).is_absolute():
+        raise ConfigError("License path must be relative")
+
+    opts = get_options(pyproject_path.parent)
+    for o in extra_options:
+        opts.insert(o)
+
+    tree_config = ConfigNode.from_dict(config_files)
+    opts.verify_all(tree_config)
+    opts.override_all(tree_config)
+    opts.inherit_all(tree_config)
+    opts.update_default_all(tree_config)
+    dictcfg = cast(dict, tree_config.to_dict())
+    tool_cfg = dictcfg['pyproject.toml']['tool']['py-build-cmake']
+
+    # Store the module configuration
+    s = 'module'
+    if s in tool_cfg:
+        # Normalize the import and wheel name of the package
+        normname = normalize_name_wheel(tool_cfg[s]['name'])
+        if tool_cfg[s]['name'] != normname:
+            print(f"Name changed from {tool_cfg[s]['name']} to {normname}")
+            # TODO: use logging instead of print
+        tool_cfg[s]['name'] = normname
+        cfg.module = tool_cfg[s]
+    else:
+        assert False, "Missing [tools.py-build-cmake.module] section"
+
+    # Store the editable configuration
+    cfg.editable = {
+        os: tool_cfg[os]['editable']
+        for os in ("linux", "windows", "mac")
+        if os in tool_cfg and 'editable' in tool_cfg[os]
+    }
+
+    # Store the sdist folders (this is based on flit)
+    def get_sdist_cludes(cfg):
+        return {
+            cl + '_patterns': _check_glob_patterns(cfg['sdist'][cl], cl)
+            for cl in ('include', 'exclude')
+        }
+
+    cfg.sdist = {
+        os: get_sdist_cludes(tool_cfg[os])
+        for os in ("linux", "windows", "mac")
+    }
+    s = 'cross'
+    if s in tool_cfg:
+        cfg.sdist.update({
+            'cross': get_sdist_cludes(tool_cfg[s]),
+        })
+
+    # Store the CMake configuration
+    cfg.cmake = {
+        os: tool_cfg[os]['cmake']
+        for os in ("linux", "windows", "mac")
+        if os in tool_cfg and 'cmake' in tool_cfg[os]
+    }
+
+    # Store stubgen configuration
+    s = 'stubgen'
+    if s in tool_cfg:
+        cfg.stubgen = tool_cfg[s]
+
+    # Store the cross compilation configuration
+    s = 'cross'
+    if s in tool_cfg:
+        cfg.cross = tool_cfg[s]
+        f = 'copy_from_native_build'
+        if f in cfg.cross:
+            cfg.cross[f] = _check_glob_patterns(cfg.cross[f], f'cross.{f}')
+        cfg.cmake.update({
+            'cross': cfg.cross.pop('cmake', {}),
+        })
+
+    return cfg
+
+
+@dataclass
+class ComponentConfig:
+    dynamic_metadata: Set[str] = field(default_factory=set)
+    entrypoints: Dict[str, Dict[str, str]] = field(default_factory=dict)
+    metadata: Dict[str, Any] = field(default_factory=dict)
+    referenced_files: List[str] = field(default_factory=list)
+    package_name: str = field(default='')
+    component: Dict[str, Any] = field(default_factory=dict)
+    license: Dict[str, str] = field(default_factory=dict)
+
+
+def read_component_config(pyproject_path) -> ComponentConfig:
+    # Load the pyproject.toml file
+    pyproject_path = Path(pyproject_path)
+    pyproject = toml_.loads(pyproject_path.read_text('utf-8'))
+    if 'project' not in pyproject:
+        raise ConfigError('Missing [project] table')
+
+    # File names mapping to the actual dict with the config
+    config_files = {
+        "pyproject.toml": pyproject,
+    }
+    return check_component_config(pyproject_path, pyproject, config_files)
+
+
+def check_component_config(pyproject_path, pyproject, config_files):
+    # Check the package/module name and normalize it
+    f = 'name'
+    if f in pyproject['project']:
+        normname = normalize_name(pyproject['project'][f])
+        if pyproject['project'][f] != normname:
+            warnings.warn(
+                f"Name changed from {pyproject['project'][f]} to {normname}")
+        pyproject['project'][f] = normname
+
+    # Parse the [project] section for metadata (using flit's parser)
+    flit_cfg = read_pep621_metadata(pyproject['project'], pyproject_path)
+
+    # Create our own config data structure using flit's output
+    cfg = ComponentConfig()
+    cfg.dynamic_metadata = set(flit_cfg.dynamic_metadata)
+    cfg.entrypoints = flit_cfg.entrypoints
+    cfg.metadata = flit_cfg.metadata
+    cfg.referenced_files = flit_cfg.referenced_files
+    cfg.license = pyproject['project'].setdefault('license', {})
+    cfg.package_name = normalize_name_wheel(cfg.metadata["name"])
+
+    if 'file' in cfg.license and Path(cfg.license['file']).is_absolute():
+        raise ConfigError("License path must be relative")
+
+    opts = get_component_options(pyproject_path.parent)
+
+    tree_config = ConfigNode.from_dict(config_files)
+    opts.verify_all(tree_config)
+    opts.override_all(tree_config)
+    opts.inherit_all(tree_config)
+    opts.update_default_all(tree_config)
+    dictcfg = cast(dict, tree_config.to_dict())
+    tool_cfg = dictcfg['pyproject.toml']['tool']['py-build-cmake']
+
+    # Store the component configuration
+    cfg.component = tool_cfg['component']
+
+    return cfg
+
+
+def normalize_name_wheel(name):
+    """https://www.python.org/dev/peps/pep-0427/#escaping-and-unicode"""
+    return re.sub(r"[^\w\d.]+", "_", name, re.UNICODE)
```

### Comparing `py-build-cmake-0.1.7/src/py_build_cmake/config_options.py` & `py-build-cmake-0.1.8/src/py_build_cmake/config_options.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,770 +1,770 @@
-"""
-Classes to define hierarchical configuration options which support inheriting
-from other options, default values, overriding options, etc.
-"""
-
-from abc import ABC, abstractmethod
-from copy import deepcopy
-from dataclasses import dataclass
-import os
-from pathlib import Path
-from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple, Union
-
-from flit_core.config import ConfigError  # type: ignore
-
-ConfPath = Tuple[str, ...]
-ConfValue = Optional[Union[bool, str, List[str], Dict[str, Any]]]
-Conf = Dict[str, Any]
-
-
-def pth(s: str) -> ConfPath:
-    if not s:
-        return ()
-    return tuple(s.split('/'))
-
-
-def pth2str(p: ConfPath) -> str:
-    return '/'.join(p)
-
-
-def joinpth(p1: ConfPath, p2: ConfPath) -> ConfPath:
-    while p1 and p2 and p2[0] == '^':
-        p1 = p1[:-1]
-        p2 = p2[1:]
-    return p1 + p2
-
-
-def hasparent(path: ConfPath) -> bool:
-    return len(path) >= 1
-
-
-def parent(path: ConfPath) -> ConfPath:
-    if not hasparent(path):
-        raise RuntimeError(f"Path {pth2str(path)} does not have a parent")
-    return path[:-1]
-
-
-def basename(path: ConfPath) -> str:
-    return path[-1]
-
-
-class ConfigNode:
-
-    def __init__(self,
-                 value: ConfValue = None,
-                 sub: Optional[Dict[str, 'ConfigNode']] = None) -> None:
-        self.value: ConfValue = value
-        self.sub: Optional[Dict[str, 'ConfigNode']] = sub
-
-    @classmethod
-    def from_dict(cls, d: dict):
-        node = cls()
-        node.sub = {}
-        for k, v in d.items():
-            if isinstance(v, dict):
-                node.sub[k] = cls.from_dict(v)
-            else:
-                node.sub[k] = cls(value=v)
-        return node
-
-    def to_dict(self):
-        if self.sub is None:
-            return self.value
-        return {k: v.to_dict() for k, v in self.sub.items()}
-
-    def iter_dfs(self, path: ConfPath = ()):
-        yield path, self.value
-        if self.sub is not None:
-            for name, sub in self.sub.items():
-                for y in sub.iter_dfs(path + (name, )):
-                    yield y
-
-    def __getitem__(self, key):
-        if isinstance(key, str):
-            if self.sub is None:
-                raise KeyError()
-            return self.sub[key]
-        elif isinstance(key, tuple):
-            if len(key) == 0:
-                return self
-            elif self.sub is None:
-                raise KeyError()
-            else:
-                return self.sub[key[0]][key[1:]]
-        else:
-            raise TypeError(key)
-
-    def get(self, key: ConfPath, default=None):
-        try:
-            return self[key]
-        except KeyError:
-            return default
-
-    def setdefault(self, path: ConfPath, default: Any):
-        tgt = self[parent(path)]
-        if tgt.sub is None:
-            tgt.sub = {}
-        return tgt.sub.setdefault(basename(path), default)
-
-    def contains(self, path: ConfPath):
-        try:
-            self[path]
-            return True
-        except KeyError:
-            return False
-
-
-@dataclass
-class DefaultValueWrapper:
-    value: ConfValue
-
-
-class DefaultValue(ABC):
-
-    @abstractmethod
-    def get_default(self, rootopts: 'ConfigOption', opt: 'ConfigOption',
-                    cfg: ConfigNode, cfgpath: ConfPath,
-                    optpath: ConfPath) -> Optional[DefaultValueWrapper]:
-        ...
-
-    @abstractmethod
-    def get_name(self) -> str:
-        ...
-
-
-class DefaultValueValue(DefaultValue):
-
-    def __init__(self, value: ConfValue) -> None:
-        self.value: ConfValue = value
-
-    def get_default(self, rootopts: 'ConfigOption', opt: 'ConfigOption',
-                    cfg: ConfigNode, cfgpath: ConfPath,
-                    optpath: ConfPath) -> Optional[DefaultValueWrapper]:
-        return DefaultValueWrapper(self.value)
-
-    def get_name(self):
-        if isinstance(self.value, bool):
-            return str(self.value).lower()
-        return repr(self.value)
-
-
-class NoDefaultValue(DefaultValue):
-
-    def __init__(self, name='none'):
-        self.name = name
-
-    def get_default(self, rootopts: 'ConfigOption', opt: 'ConfigOption',
-                    cfg: ConfigNode, cfgpath: ConfPath,
-                    optpath: ConfPath) -> Optional[DefaultValueWrapper]:
-        return None
-
-    def get_name(self):
-        return self.name
-
-
-class MissingDefaultError(ConfigError):
-    pass
-
-
-class RequiredValue(DefaultValue):
-
-    def get_default(self, rootopts: 'ConfigOption', opt: 'ConfigOption',
-                    cfg: ConfigNode, cfgpath: ConfPath,
-                    optpath: ConfPath) -> Optional[DefaultValueWrapper]:
-        raise MissingDefaultError(f'{pth2str(cfgpath)} requires a value')
-
-    def get_name(self):
-        return 'required'
-
-
-class RefDefaultValue(DefaultValue):
-
-    def __init__(self, path: ConfPath, relative: bool = False) -> None:
-        super().__init__()
-        self.path: ConfPath = path
-        self.relative = relative
-
-    def get_default(self, rootopts: 'ConfigOption', opt: 'ConfigOption',
-                    cfg: ConfigNode, cfgpath: ConfPath,
-                    optpath: ConfPath) -> Optional[DefaultValueWrapper]:
-        abscfgpath = absoptpath = self.path
-        if self.relative:
-            absoptpath = joinpth(optpath, ('^', ) + absoptpath)
-            abscfgpath = joinpth(cfgpath, ('^', ) + abscfgpath)
-        opt = rootopts.get(absoptpath)
-        if opt is None:
-            raise ValueError("DefaultValue: reference to nonexisting option "
-                             f"{pth2str(absoptpath)}")
-        return opt.update_default(rootopts, cfg, abscfgpath, absoptpath)
-
-    def get_name(self) -> str:
-        r = pth2str(self.path).replace('^', '..')
-        if not self.relative:
-            r = '/' + r
-        return r
-
-
-class ConfigOption:
-
-    allow_unknown_keys = False
-
-    def __init__(self,
-                 name: str,
-                 description: str = '',
-                 example: str = '',
-                 default: DefaultValue = NoDefaultValue(),
-                 inherit_from: Optional[ConfPath] = None,
-                 create_if_inheritance_target_exists: bool = False) -> None:
-        self.name = name
-        self.description = description
-        self.example = example
-        self.sub: Dict[str, 'ConfigOption'] = {}
-        self.default: DefaultValue = default
-        self.inherit_from: Optional[ConfPath] = inherit_from
-        self.create_if_inheritance_target_exists = create_if_inheritance_target_exists
-
-    def get_typename(self, md: bool = False):
-        return None
-
-    def insert(self, opt: 'ConfigOption'):
-        assert opt.name not in self.sub
-        self.sub[opt.name] = opt
-        return self.sub[opt.name]
-
-    def insert_multiple(self, opts: Iterable['ConfigOption']):
-        for opt in opts:
-            self.insert(opt)
-
-    def iter_opt_paths(self) -> Iterator[ConfPath]:
-        """DFS of the option tree."""
-        for name, subopt in self.sub.items():
-            yield (name, )
-            for p in subopt.iter_opt_paths():
-                yield (name, ) + p
-
-    def iter_leaf_opt_paths(self) -> Iterator[ConfPath]:
-        """DFS of the option tree."""
-        if not self.sub:
-            yield ()
-        else:
-            for name, subopt in self.sub.items():
-                for p in subopt.iter_leaf_opt_paths():
-                    yield (name, ) + p
-
-    def iter_dfs(self, path: ConfPath = ()):
-        yield path, self
-        for name, sub in self.sub.items():
-            for y in sub.iter_dfs(path + (name, )):
-                yield y
-
-    def __getitem__(self, key) -> 'ConfigOption':
-        if isinstance(key, str):
-            return self.sub[key]
-        elif isinstance(key, tuple):
-            if len(key) == 0:
-                return self
-            else:
-                return self.sub[key[0]][key[1:]]
-        else:
-            raise TypeError(key)
-
-    def get(self, key: ConfPath, default=None):
-        try:
-            return self[key]
-        except KeyError:
-            return default
-
-    def setdefault(self, path: ConfPath, default: Any):
-        tgt = self[parent(path)]
-        if tgt.sub is None:
-            tgt.sub = {}
-        return tgt.sub.setdefault(basename(path), default)
-
-    def contains(self, path: ConfPath):
-        try:
-            self[path]
-            return True
-        except KeyError:
-            return False
-
-    def inherit(self, rootopts: 'ConfigOption', cfg: ConfigNode,
-                selfpth: ConfPath):
-        superpth = self.inherit_from
-        if superpth is not None:
-            # If the super option is not set, there's nothing to inherit
-            supercfg = cfg.get(superpth)
-            if supercfg is None:
-                return
-
-            # If this option is not set, but the super option is,
-            # create our own config as well, including all of its parents,
-            # but only if create_if_inheritance_target_exists is set on those
-            # options
-            selfcfg = self.create_parent_config_for_inheritance(
-                rootopts, cfg, selfpth)
-            if selfcfg is None:
-                return
-
-            # Find the option we inherit from and make sure it exists
-            superopt = rootopts.get(superpth)
-            if superopt is None:
-                raise ValueError(f'{pth2str(superpth)} is not a valid option')
-
-            # Create a copy of the config of our super-option and override it
-            # with our own config
-            supercfg = deepcopy(supercfg)
-            superopt.explicit_override(self, supercfg, superpth, selfcfg,
-                                       selfpth)
-            selfcfg.sub = supercfg.sub
-        if self.sub:
-            for name, sub in self.sub.items():
-                sub.inherit(rootopts, cfg, selfpth + (name, ))
-
-    @staticmethod
-    def create_parent_config_for_inheritance(rootopts: 'ConfigOption',
-                                             cfg: ConfigNode,
-                                             selfpth: ConfPath):
-        """
-        Loop over all parent options of selfpth in rootopts and default-
-        initialize their configuration in cfg to empty ConfigNodes if the 
-        option's create_if_inheritance_target_exists is set to True.
-        Returns cfg[selfpth] or None if parents were not created because of
-        create_if_inheritance_target_exists.
-        """
-        selfcfg = None
-        p: ConfPath = ()
-        opt = rootopts
-        create_paths: List[ConfPath] = []
-        for s in selfpth:
-            p += s,
-            opt = opt[s]
-            selfcfg = cfg.get(p)
-            if selfcfg is None:
-                if not opt.create_if_inheritance_target_exists:
-                    return None
-                create_paths.append(p)
-        for p in create_paths:
-            selfcfg = cfg.setdefault(p, ConfigNode(sub={}))
-        return selfcfg
-
-    def explicit_override(self, rootopts: 'ConfigOption', selfcfg: ConfigNode,
-                          selfpth: ConfPath, overridecfg: ConfigNode,
-                          overridepath: ConfPath):
-        # The default ConfigOption simply overrides all of its sub-options, but
-        # this function is overridden by specific subclasses.
-        if overridecfg.sub is None:
-            return  # No sub-options, so nothing to override
-        for name, subopt in self.sub.items():
-            assert isinstance(selfcfg, ConfigNode)
-            assert isinstance(overridecfg, ConfigNode)
-            if name not in overridecfg.sub:
-                continue
-            subselfcfg = selfcfg.setdefault((name, ), ConfigNode())
-            subpath = selfpth + (name, )
-            suboverridepath = overridepath + (name, )
-            suboverridecfg = overridecfg.sub[name]
-            subopt.explicit_override(rootopts, subselfcfg, subpath,
-                                     suboverridecfg, suboverridepath)
-        if self.inherit_from is not None:
-            superopt = rootopts[self.inherit_from]
-            superopt.explicit_override(rootopts, selfcfg, selfpth, overridecfg,
-                                       overridepath)
-
-    def override(self, rootopts: 'ConfigOption', cfg: ConfigNode,
-                 selfpath: ConfPath):
-        """Override other options with this option if appropriate. This is a 
-        no-op in most cases and only does something in OverrideConfigOption."""
-        assert cfg.contains(selfpath)
-
-    def verify_impl(self, rootopts: 'ConfigOption', cfg: ConfigNode,
-                    cfgpath: ConfPath):
-        assert cfg.contains(cfgpath)
-        selfcfg = cfg[cfgpath]
-        # Check if there are any unknown options in the config
-        if not self.allow_unknown_keys:
-            unknwn = set(selfcfg.sub or ()) - set(self.sub or ())
-            if unknwn:
-                raise ConfigError(f'Unkown options in {pth2str(cfgpath)}: ' +
-                                  ', '.join(unknwn))
-        # Recursively verify the sub-options
-        if selfcfg.sub:
-            for name, sub in selfcfg.sub.items():
-                if name in self.sub:
-                    self.sub[name].verify(rootopts, cfg, cfgpath + (name, ))
-
-    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
-               cfgpath: ConfPath):
-        if self.inherit_from is None:
-            return self.verify_impl(rootopts, cfg, cfgpath)
-        else:
-            return rootopts[self.inherit_from].verify_impl(
-                rootopts, cfg, cfgpath)
-
-    def override_all(self, cfg: ConfigNode):
-        # This is just me being lazy, we probably don't need to iterate over
-        # all nodes ...
-        for p, opt in self.iter_dfs():
-            if cfg.contains(p):
-                opt.override(self, cfg, p)
-
-    def verify_all(self, cfg: ConfigNode):
-        self.verify(self, cfg, ())
-
-    def inherit_all(self, cfg: ConfigNode):
-        self.inherit(self, cfg, ())
-
-    def update_default(
-            self,
-            rootopts: 'ConfigOption',
-            cfg: ConfigNode,
-            cfgpath: ConfPath,
-            selfpath: Optional[ConfPath] = None
-    ) -> Optional[DefaultValueWrapper]:
-        if selfpath is None:
-            selfpath = cfgpath
-
-        result = None
-        # If the entire path exists in cfg, simply return that value
-        cfgval = cfg.get(cfgpath)
-        if cfgval is not None:
-            result = cfgval
-        # If the path is not yet in cfg
-        else:
-            assert self is rootopts[selfpath]
-            # Find the default value for this option
-            default = self.default.get_default(rootopts, self, cfg, cfgpath,
-                                               selfpath)
-            # If the parent is set in the config, set this value as well
-            if default is not None and cfg.contains(parent(cfgpath)):
-                cfgval = cfg.setdefault(cfgpath, ConfigNode())
-                cfgval.value = default.value
-                if cfgval.value is not None:
-                    self.verify(rootopts, cfg, cfgpath)
-            result = default
-
-        if self.inherit_from is not None:
-            targetopt = rootopts.get(self.inherit_from)
-            if targetopt is None:
-                raise ValueError(f"Inheritance {pth2str(selfpath)} targets "
-                                 f"nonexisting option "
-                                 f"{pth2str(self.inherit_from)}")
-            for p, opt in targetopt.iter_dfs():
-                if opt.inherit_from is not None:
-                    # TODO: this might be too restrictive, but we need to break
-                    # the recursion somehow ...
-                    continue
-                optpth = joinpth(self.inherit_from, p)
-                newcfgpth = joinpth(cfgpath, p)
-                opt.update_default(rootopts, cfg, newcfgpth, optpth)
-
-        return result
-
-    def update_default_all(self, cfg: ConfigNode):
-        for p, opt in self.iter_dfs():
-            if hasparent(p) and cfg.contains(parent(p)):
-                opt.update_default(self, cfg, p)
-
-
-class UncheckedConfigOption(ConfigOption):
-
-    allow_unknown_keys = True
-
-
-class StrConfigOption(ConfigOption):
-
-    def get_typename(self, md: bool = False):
-        return 'string'
-
-    def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
-                          selfpth: ConfPath, overridecfg: ConfigNode,
-                          overridepath: ConfPath):
-        assert not self.sub
-        assert not selfcfg.sub
-        assert not overridecfg.sub
-        selfcfg.value = deepcopy(overridecfg.value)
-
-    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
-               cfgpath: ConfPath):
-        if cfg[cfgpath].sub:
-            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
-                              f'{str}, not {dict}')
-        elif not isinstance(cfg[cfgpath].value, str):
-            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
-                              f'{str}, not {type(cfg[cfgpath].value)}')
-
-class EnumConfigOption(ConfigOption):
-
-    def __init__(self,
-                 name: str,
-                 description: str = '',
-                 example: str = '',
-                 default: DefaultValue = NoDefaultValue(),
-                 inherit_from: Optional[ConfPath] = None,
-                 create_if_inheritance_target_exists: bool = False,
-                 options: List[str] = []) -> None:
-        super().__init__(name, description, example, default, inherit_from, create_if_inheritance_target_exists)
-        self.options = options
-
-    def get_typename(self, md: bool = False):
-        if md:
-            return "`'" + "'` \| `'".join(self.options) + "'`"
-        else:
-            return "'" + "' | '".join(self.options) + "'"
-
-    def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
-                          selfpth: ConfPath, overridecfg: ConfigNode,
-                          overridepath: ConfPath):
-        assert not self.sub
-        assert not selfcfg.sub
-        assert not overridecfg.sub
-        selfcfg.value = deepcopy(overridecfg.value)
-
-    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
-               cfgpath: ConfPath):
-        if cfg[cfgpath].sub:
-            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
-                              f'{str}, not {dict}')
-        elif not isinstance(cfg[cfgpath].value, str):
-            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
-                              f'{str}, not {type(cfg[cfgpath].value)}')
-        if cfg[cfgpath].value not in self.options:
-            raise ConfigError(f'Value of {pth2str(cfgpath)} should be '
-                              'one of \'' + "', '".join(self.options) + '\'')
-
-class BoolConfigOption(ConfigOption):
-
-    def get_typename(self, md: bool = False):
-        return 'bool'
-
-    def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
-                          selfpth: ConfPath, overridecfg: ConfigNode,
-                          overridepath: ConfPath):
-        assert not self.sub
-        assert not selfcfg.sub
-        assert not overridecfg.sub
-        selfcfg.value = deepcopy(overridecfg.value)
-
-    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
-               cfgpath: ConfPath):
-        if cfg[cfgpath].sub:
-            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
-                              f'{bool}, not {dict}')
-        elif not isinstance(cfg[cfgpath].value, bool):
-            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
-                              f'{bool}, not {type(cfg[cfgpath].value)}')
-
-
-@dataclass
-class RelativeToCurrentConfig:
-    project_path: Path
-    description: str = 'current configuration file'
-
-
-@dataclass
-class RelativeToProject:
-    project_path: Path
-    description: str = 'project directory'
-
-
-class PathConfigOption(StrConfigOption):
-
-    def __init__(self,
-                 name: str,
-                 description: str = '',
-                 example: str = '',
-                 default: DefaultValue = NoDefaultValue(),
-                 must_exist: bool = True,
-                 expected_contents: List[str] = [],
-                 base_path: Optional[Union[RelativeToProject,
-                                           RelativeToCurrentConfig]] = None,
-                 allow_abs: bool = False,
-                 is_folder: bool = True):
-        super().__init__(name, description, example, default)
-        self.must_exist = must_exist or bool(expected_contents)
-        self.expected_contents = expected_contents
-        self.base_path = base_path
-        self.allow_abs = allow_abs
-        self.is_folder = is_folder
-        if self.base_path:
-            assert os.path.isabs(self.base_path.project_path)
-
-    def get_typename(self, md: bool = False):
-        return 'path' if self.is_folder else 'filepath'
-
-    def check_path(self, cfg: ConfigNode, cfgpath):
-        osp = os.path
-        path = osp.normpath(cfg[cfgpath].value)
-        # Absolute or relative path?
-        if osp.isabs(path):
-            # Absolute path
-            if not self.allow_abs:
-                raise ConfigError(f'{pth2str(cfgpath)}: "{str(path)}" '
-                                  f'must be a relative path')
-        else:
-            # Relative path
-            if isinstance(self.base_path, RelativeToCurrentConfig):
-                # cfgpath[0] is relative for files inside of the project,
-                # otherwise it is absolute
-                path = osp.join(osp.dirname(cfgpath[0]), path)
-                if not osp.isabs(path):
-                    path = osp.join(self.base_path.project_path, path)
-            elif isinstance(self.base_path, RelativeToProject):
-                path = osp.join(self.base_path.project_path, path)
-            else:
-                assert False, "Invalid relative path type"
-        assert osp.isabs(path), "Failed to make path absolute"
-        # Does the path exist?
-        if self.must_exist:
-            if not osp.exists(path):
-                raise ConfigError(f'{pth2str(cfgpath)}: "{str(path)}" '
-                                  f'does not exist')
-            if self.is_folder != osp.isdir(path):
-                type_ = 'directory' if self.is_folder else 'file'
-                raise ConfigError(f'{pth2str(cfgpath)}: "{str(path)}" '
-                                  f'should be a {type_}')
-            # Are any of the required contents missing?
-            missing = [
-                sub for sub in self.expected_contents
-                if not osp.exists(osp.join(path, sub))
-            ]
-            if missing:
-                missingstr = '", "'.join(missing)
-                raise ConfigError(f'{pth2str(cfgpath)}: "{str(path)}" '
-                                  f'does not contain the following '
-                                  f'required files or folders: "{missingstr}"')
-        cfg[cfgpath].value = osp.normpath(path)
-
-    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
-               cfgpath: ConfPath):
-        super().verify(rootopts, cfg, cfgpath)
-        self.check_path(cfg, cfgpath)
-
-
-class ListOfStrConfigOption(ConfigOption):
-
-    def __init__(self,
-                 name: str,
-                 description: str = '',
-                 example: str = '',
-                 default: DefaultValue = NoDefaultValue(),
-                 inherit_from: Optional[ConfPath] = None,
-                 create_if_inheritance_target_exists: bool = False,
-                 convert_str_to_singleton=False) -> None:
-        super().__init__(name, description, example, default, inherit_from,
-                         create_if_inheritance_target_exists)
-        self.convert_str_to_singleton = convert_str_to_singleton
-
-    def get_typename(self, md: bool = False):
-        return 'list'
-
-    def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
-                          selfpth: ConfPath, overridecfg: ConfigNode,
-                          overridepath: ConfPath):
-        assert not self.sub
-        assert not selfcfg.sub
-        assert not overridecfg.sub
-        if overridecfg.value is not None:
-            if selfcfg.value is None:
-                selfcfg.value = []
-            assert isinstance(selfcfg.value, list)
-            assert isinstance(overridecfg.value, list)
-            selfcfg.value += deepcopy(overridecfg.value)
-
-    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
-               cfgpath: ConfPath):
-        if cfg[cfgpath].sub:
-            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
-                              f'{list}, not {dict}')
-        elif not isinstance(cfg[cfgpath].value, list):
-            if self.convert_str_to_singleton and \
-                    isinstance(cfg[cfgpath].value, str):
-                cfg[cfgpath].value = [cfg[cfgpath].value]
-            else:
-                raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
-                                  f'{list}, not {type(cfg[cfgpath].value)}')
-        elif not all(isinstance(el, str) for el in cfg[cfgpath].value):
-            raise ConfigError(f'Type of elements in {pth2str(cfgpath)} should '
-                              f'be {str}')
-
-
-class DictOfStrConfigOption(ConfigOption):
-
-    def get_typename(self, md: bool = False):
-        return 'dict'
-
-    def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
-                          selfpth: ConfPath, overridecfg: ConfigNode,
-                          overridepath: ConfPath):
-        assert not self.sub
-        assert not selfcfg.value
-        assert not overridecfg.value
-        if overridecfg.sub is not None:
-            if selfcfg.sub is None:
-                selfcfg.sub = {}
-            assert isinstance(selfcfg.sub, dict)
-            assert isinstance(overridecfg.sub, dict)
-            selfcfg.sub.update(deepcopy(overridecfg.sub))
-
-    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
-               cfgpath: ConfPath):
-        if cfg[cfgpath].value is not None:
-            if isinstance(cfg[cfgpath].value, dict):
-                newcfg = ConfigNode.from_dict(cfg[cfgpath].value)
-                cfg[cfgpath].value = newcfg.value
-                cfg[cfgpath].sub = newcfg.sub
-            else:
-                raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
-                                  f'{dict}, not {type(cfg[cfgpath].value)}')
-        valdict = cfg[cfgpath].sub
-        if not isinstance(valdict, dict):
-            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
-                              f'{dict}, not {type(valdict)}')
-        elif not all(isinstance(el, str) for el in valdict.keys()):
-            raise ConfigError(f'Type of keys in {pth2str(cfgpath)} should '
-                              f'be {str}')
-        elif not all(isinstance(el.value, str) for el in valdict.values()):
-            raise ConfigError(f'Type of values in {pth2str(cfgpath)} should '
-                              f'be {str}')
-
-
-class OverrideConfigOption(ConfigOption):
-
-    def __init__(
-        self,
-        name: str,
-        description: str,
-        targetpath: ConfPath,
-        default: DefaultValue = NoDefaultValue()) -> None:
-        super().__init__(name, description, '', default)
-        self.targetpath = targetpath
-
-    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
-               cfgpath: ConfPath):
-        rootopts[self.targetpath].verify(rootopts, cfg, cfgpath)
-
-    def inherit(self, rootopts: 'ConfigOption', cfg: ConfigNode,
-                selfpth: ConfPath):
-        pass
-
-    def override(self, rootopts: ConfigOption, cfg: ConfigNode,
-                 cfgpath: ConfPath):
-        selfcfg = cfg.get(cfgpath, None)
-        if selfcfg is None:
-            return
-        elif selfcfg.value is None and selfcfg.sub is None:
-            return
-        super().override(rootopts, cfg, cfgpath)
-        curropt = rootopts[self.targetpath]
-        self.create_parent_config(cfg, self.targetpath)
-        currcfg = cfg[self.targetpath]
-        overridecfg = cfg[cfgpath]
-        # Override the config at those paths by our own config
-        curropt.explicit_override(rootopts, currcfg, self.targetpath,
-                                  overridecfg, cfgpath)
-
-    @staticmethod
-    def create_parent_config(cfg: ConfigNode, path: ConfPath):
-        parentcfg = cfg
-        for s in path:
-            assert parentcfg.sub is not None
-            parentcfg = parentcfg.sub.setdefault(s, ConfigNode(sub={}))
+"""
+Classes to define hierarchical configuration options which support inheriting
+from other options, default values, overriding options, etc.
+"""
+
+from abc import ABC, abstractmethod
+from copy import deepcopy
+from dataclasses import dataclass
+import os
+from pathlib import Path
+from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple, Union
+
+from flit_core.config import ConfigError  # type: ignore
+
+ConfPath = Tuple[str, ...]
+ConfValue = Optional[Union[bool, str, List[str], Dict[str, Any]]]
+Conf = Dict[str, Any]
+
+
+def pth(s: str) -> ConfPath:
+    if not s:
+        return ()
+    return tuple(s.split('/'))
+
+
+def pth2str(p: ConfPath) -> str:
+    return '/'.join(p)
+
+
+def joinpth(p1: ConfPath, p2: ConfPath) -> ConfPath:
+    while p1 and p2 and p2[0] == '^':
+        p1 = p1[:-1]
+        p2 = p2[1:]
+    return p1 + p2
+
+
+def hasparent(path: ConfPath) -> bool:
+    return len(path) >= 1
+
+
+def parent(path: ConfPath) -> ConfPath:
+    if not hasparent(path):
+        raise RuntimeError(f"Path {pth2str(path)} does not have a parent")
+    return path[:-1]
+
+
+def basename(path: ConfPath) -> str:
+    return path[-1]
+
+
+class ConfigNode:
+
+    def __init__(self,
+                 value: ConfValue = None,
+                 sub: Optional[Dict[str, 'ConfigNode']] = None) -> None:
+        self.value: ConfValue = value
+        self.sub: Optional[Dict[str, 'ConfigNode']] = sub
+
+    @classmethod
+    def from_dict(cls, d: dict):
+        node = cls()
+        node.sub = {}
+        for k, v in d.items():
+            if isinstance(v, dict):
+                node.sub[k] = cls.from_dict(v)
+            else:
+                node.sub[k] = cls(value=v)
+        return node
+
+    def to_dict(self):
+        if self.sub is None:
+            return self.value
+        return {k: v.to_dict() for k, v in self.sub.items()}
+
+    def iter_dfs(self, path: ConfPath = ()):
+        yield path, self.value
+        if self.sub is not None:
+            for name, sub in self.sub.items():
+                for y in sub.iter_dfs(path + (name, )):
+                    yield y
+
+    def __getitem__(self, key):
+        if isinstance(key, str):
+            if self.sub is None:
+                raise KeyError()
+            return self.sub[key]
+        elif isinstance(key, tuple):
+            if len(key) == 0:
+                return self
+            elif self.sub is None:
+                raise KeyError()
+            else:
+                return self.sub[key[0]][key[1:]]
+        else:
+            raise TypeError(key)
+
+    def get(self, key: ConfPath, default=None):
+        try:
+            return self[key]
+        except KeyError:
+            return default
+
+    def setdefault(self, path: ConfPath, default: Any):
+        tgt = self[parent(path)]
+        if tgt.sub is None:
+            tgt.sub = {}
+        return tgt.sub.setdefault(basename(path), default)
+
+    def contains(self, path: ConfPath):
+        try:
+            self[path]
+            return True
+        except KeyError:
+            return False
+
+
+@dataclass
+class DefaultValueWrapper:
+    value: ConfValue
+
+
+class DefaultValue(ABC):
+
+    @abstractmethod
+    def get_default(self, rootopts: 'ConfigOption', opt: 'ConfigOption',
+                    cfg: ConfigNode, cfgpath: ConfPath,
+                    optpath: ConfPath) -> Optional[DefaultValueWrapper]:
+        ...
+
+    @abstractmethod
+    def get_name(self) -> str:
+        ...
+
+
+class DefaultValueValue(DefaultValue):
+
+    def __init__(self, value: ConfValue) -> None:
+        self.value: ConfValue = value
+
+    def get_default(self, rootopts: 'ConfigOption', opt: 'ConfigOption',
+                    cfg: ConfigNode, cfgpath: ConfPath,
+                    optpath: ConfPath) -> Optional[DefaultValueWrapper]:
+        return DefaultValueWrapper(self.value)
+
+    def get_name(self):
+        if isinstance(self.value, bool):
+            return str(self.value).lower()
+        return repr(self.value)
+
+
+class NoDefaultValue(DefaultValue):
+
+    def __init__(self, name='none'):
+        self.name = name
+
+    def get_default(self, rootopts: 'ConfigOption', opt: 'ConfigOption',
+                    cfg: ConfigNode, cfgpath: ConfPath,
+                    optpath: ConfPath) -> Optional[DefaultValueWrapper]:
+        return None
+
+    def get_name(self):
+        return self.name
+
+
+class MissingDefaultError(ConfigError):
+    pass
+
+
+class RequiredValue(DefaultValue):
+
+    def get_default(self, rootopts: 'ConfigOption', opt: 'ConfigOption',
+                    cfg: ConfigNode, cfgpath: ConfPath,
+                    optpath: ConfPath) -> Optional[DefaultValueWrapper]:
+        raise MissingDefaultError(f'{pth2str(cfgpath)} requires a value')
+
+    def get_name(self):
+        return 'required'
+
+
+class RefDefaultValue(DefaultValue):
+
+    def __init__(self, path: ConfPath, relative: bool = False) -> None:
+        super().__init__()
+        self.path: ConfPath = path
+        self.relative = relative
+
+    def get_default(self, rootopts: 'ConfigOption', opt: 'ConfigOption',
+                    cfg: ConfigNode, cfgpath: ConfPath,
+                    optpath: ConfPath) -> Optional[DefaultValueWrapper]:
+        abscfgpath = absoptpath = self.path
+        if self.relative:
+            absoptpath = joinpth(optpath, ('^', ) + absoptpath)
+            abscfgpath = joinpth(cfgpath, ('^', ) + abscfgpath)
+        opt = rootopts.get(absoptpath)
+        if opt is None:
+            raise ValueError("DefaultValue: reference to nonexisting option "
+                             f"{pth2str(absoptpath)}")
+        return opt.update_default(rootopts, cfg, abscfgpath, absoptpath)
+
+    def get_name(self) -> str:
+        r = pth2str(self.path).replace('^', '..')
+        if not self.relative:
+            r = '/' + r
+        return r
+
+
+class ConfigOption:
+
+    allow_unknown_keys = False
+
+    def __init__(self,
+                 name: str,
+                 description: str = '',
+                 example: str = '',
+                 default: DefaultValue = NoDefaultValue(),
+                 inherit_from: Optional[ConfPath] = None,
+                 create_if_inheritance_target_exists: bool = False) -> None:
+        self.name = name
+        self.description = description
+        self.example = example
+        self.sub: Dict[str, 'ConfigOption'] = {}
+        self.default: DefaultValue = default
+        self.inherit_from: Optional[ConfPath] = inherit_from
+        self.create_if_inheritance_target_exists = create_if_inheritance_target_exists
+
+    def get_typename(self, md: bool = False):
+        return None
+
+    def insert(self, opt: 'ConfigOption'):
+        assert opt.name not in self.sub
+        self.sub[opt.name] = opt
+        return self.sub[opt.name]
+
+    def insert_multiple(self, opts: Iterable['ConfigOption']):
+        for opt in opts:
+            self.insert(opt)
+
+    def iter_opt_paths(self) -> Iterator[ConfPath]:
+        """DFS of the option tree."""
+        for name, subopt in self.sub.items():
+            yield (name, )
+            for p in subopt.iter_opt_paths():
+                yield (name, ) + p
+
+    def iter_leaf_opt_paths(self) -> Iterator[ConfPath]:
+        """DFS of the option tree."""
+        if not self.sub:
+            yield ()
+        else:
+            for name, subopt in self.sub.items():
+                for p in subopt.iter_leaf_opt_paths():
+                    yield (name, ) + p
+
+    def iter_dfs(self, path: ConfPath = ()):
+        yield path, self
+        for name, sub in self.sub.items():
+            for y in sub.iter_dfs(path + (name, )):
+                yield y
+
+    def __getitem__(self, key) -> 'ConfigOption':
+        if isinstance(key, str):
+            return self.sub[key]
+        elif isinstance(key, tuple):
+            if len(key) == 0:
+                return self
+            else:
+                return self.sub[key[0]][key[1:]]
+        else:
+            raise TypeError(key)
+
+    def get(self, key: ConfPath, default=None):
+        try:
+            return self[key]
+        except KeyError:
+            return default
+
+    def setdefault(self, path: ConfPath, default: Any):
+        tgt = self[parent(path)]
+        if tgt.sub is None:
+            tgt.sub = {}
+        return tgt.sub.setdefault(basename(path), default)
+
+    def contains(self, path: ConfPath):
+        try:
+            self[path]
+            return True
+        except KeyError:
+            return False
+
+    def inherit(self, rootopts: 'ConfigOption', cfg: ConfigNode,
+                selfpth: ConfPath):
+        superpth = self.inherit_from
+        if superpth is not None:
+            # If the super option is not set, there's nothing to inherit
+            supercfg = cfg.get(superpth)
+            if supercfg is None:
+                return
+
+            # If this option is not set, but the super option is,
+            # create our own config as well, including all of its parents,
+            # but only if create_if_inheritance_target_exists is set on those
+            # options
+            selfcfg = self.create_parent_config_for_inheritance(
+                rootopts, cfg, selfpth)
+            if selfcfg is None:
+                return
+
+            # Find the option we inherit from and make sure it exists
+            superopt = rootopts.get(superpth)
+            if superopt is None:
+                raise ValueError(f'{pth2str(superpth)} is not a valid option')
+
+            # Create a copy of the config of our super-option and override it
+            # with our own config
+            supercfg = deepcopy(supercfg)
+            superopt.explicit_override(self, supercfg, superpth, selfcfg,
+                                       selfpth)
+            selfcfg.sub = supercfg.sub
+        if self.sub:
+            for name, sub in self.sub.items():
+                sub.inherit(rootopts, cfg, selfpth + (name, ))
+
+    @staticmethod
+    def create_parent_config_for_inheritance(rootopts: 'ConfigOption',
+                                             cfg: ConfigNode,
+                                             selfpth: ConfPath):
+        """
+        Loop over all parent options of selfpth in rootopts and default-
+        initialize their configuration in cfg to empty ConfigNodes if the 
+        option's create_if_inheritance_target_exists is set to True.
+        Returns cfg[selfpth] or None if parents were not created because of
+        create_if_inheritance_target_exists.
+        """
+        selfcfg = None
+        p: ConfPath = ()
+        opt = rootopts
+        create_paths: List[ConfPath] = []
+        for s in selfpth:
+            p += s,
+            opt = opt[s]
+            selfcfg = cfg.get(p)
+            if selfcfg is None:
+                if not opt.create_if_inheritance_target_exists:
+                    return None
+                create_paths.append(p)
+        for p in create_paths:
+            selfcfg = cfg.setdefault(p, ConfigNode(sub={}))
+        return selfcfg
+
+    def explicit_override(self, rootopts: 'ConfigOption', selfcfg: ConfigNode,
+                          selfpth: ConfPath, overridecfg: ConfigNode,
+                          overridepath: ConfPath):
+        # The default ConfigOption simply overrides all of its sub-options, but
+        # this function is overridden by specific subclasses.
+        if overridecfg.sub is None:
+            return  # No sub-options, so nothing to override
+        for name, subopt in self.sub.items():
+            assert isinstance(selfcfg, ConfigNode)
+            assert isinstance(overridecfg, ConfigNode)
+            if name not in overridecfg.sub:
+                continue
+            subselfcfg = selfcfg.setdefault((name, ), ConfigNode())
+            subpath = selfpth + (name, )
+            suboverridepath = overridepath + (name, )
+            suboverridecfg = overridecfg.sub[name]
+            subopt.explicit_override(rootopts, subselfcfg, subpath,
+                                     suboverridecfg, suboverridepath)
+        if self.inherit_from is not None:
+            superopt = rootopts[self.inherit_from]
+            superopt.explicit_override(rootopts, selfcfg, selfpth, overridecfg,
+                                       overridepath)
+
+    def override(self, rootopts: 'ConfigOption', cfg: ConfigNode,
+                 selfpath: ConfPath):
+        """Override other options with this option if appropriate. This is a 
+        no-op in most cases and only does something in OverrideConfigOption."""
+        assert cfg.contains(selfpath)
+
+    def verify_impl(self, rootopts: 'ConfigOption', cfg: ConfigNode,
+                    cfgpath: ConfPath):
+        assert cfg.contains(cfgpath)
+        selfcfg = cfg[cfgpath]
+        # Check if there are any unknown options in the config
+        if not self.allow_unknown_keys:
+            unknwn = set(selfcfg.sub or ()) - set(self.sub or ())
+            if unknwn:
+                raise ConfigError(f'Unkown options in {pth2str(cfgpath)}: ' +
+                                  ', '.join(unknwn))
+        # Recursively verify the sub-options
+        if selfcfg.sub:
+            for name, sub in selfcfg.sub.items():
+                if name in self.sub:
+                    self.sub[name].verify(rootopts, cfg, cfgpath + (name, ))
+
+    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
+               cfgpath: ConfPath):
+        if self.inherit_from is None:
+            return self.verify_impl(rootopts, cfg, cfgpath)
+        else:
+            return rootopts[self.inherit_from].verify_impl(
+                rootopts, cfg, cfgpath)
+
+    def override_all(self, cfg: ConfigNode):
+        # This is just me being lazy, we probably don't need to iterate over
+        # all nodes ...
+        for p, opt in self.iter_dfs():
+            if cfg.contains(p):
+                opt.override(self, cfg, p)
+
+    def verify_all(self, cfg: ConfigNode):
+        self.verify(self, cfg, ())
+
+    def inherit_all(self, cfg: ConfigNode):
+        self.inherit(self, cfg, ())
+
+    def update_default(
+            self,
+            rootopts: 'ConfigOption',
+            cfg: ConfigNode,
+            cfgpath: ConfPath,
+            selfpath: Optional[ConfPath] = None
+    ) -> Optional[DefaultValueWrapper]:
+        if selfpath is None:
+            selfpath = cfgpath
+
+        result = None
+        # If the entire path exists in cfg, simply return that value
+        cfgval = cfg.get(cfgpath)
+        if cfgval is not None:
+            result = cfgval
+        # If the path is not yet in cfg
+        else:
+            assert self is rootopts[selfpath]
+            # Find the default value for this option
+            default = self.default.get_default(rootopts, self, cfg, cfgpath,
+                                               selfpath)
+            # If the parent is set in the config, set this value as well
+            if default is not None and cfg.contains(parent(cfgpath)):
+                cfgval = cfg.setdefault(cfgpath, ConfigNode())
+                cfgval.value = default.value
+                if cfgval.value is not None:
+                    self.verify(rootopts, cfg, cfgpath)
+            result = default
+
+        if self.inherit_from is not None:
+            targetopt = rootopts.get(self.inherit_from)
+            if targetopt is None:
+                raise ValueError(f"Inheritance {pth2str(selfpath)} targets "
+                                 f"nonexisting option "
+                                 f"{pth2str(self.inherit_from)}")
+            for p, opt in targetopt.iter_dfs():
+                if opt.inherit_from is not None:
+                    # TODO: this might be too restrictive, but we need to break
+                    # the recursion somehow ...
+                    continue
+                optpth = joinpth(self.inherit_from, p)
+                newcfgpth = joinpth(cfgpath, p)
+                opt.update_default(rootopts, cfg, newcfgpth, optpth)
+
+        return result
+
+    def update_default_all(self, cfg: ConfigNode):
+        for p, opt in self.iter_dfs():
+            if hasparent(p) and cfg.contains(parent(p)):
+                opt.update_default(self, cfg, p)
+
+
+class UncheckedConfigOption(ConfigOption):
+
+    allow_unknown_keys = True
+
+
+class StrConfigOption(ConfigOption):
+
+    def get_typename(self, md: bool = False):
+        return 'string'
+
+    def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
+                          selfpth: ConfPath, overridecfg: ConfigNode,
+                          overridepath: ConfPath):
+        assert not self.sub
+        assert not selfcfg.sub
+        assert not overridecfg.sub
+        selfcfg.value = deepcopy(overridecfg.value)
+
+    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
+               cfgpath: ConfPath):
+        if cfg[cfgpath].sub:
+            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
+                              f'{str}, not {dict}')
+        elif not isinstance(cfg[cfgpath].value, str):
+            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
+                              f'{str}, not {type(cfg[cfgpath].value)}')
+
+class EnumConfigOption(ConfigOption):
+
+    def __init__(self,
+                 name: str,
+                 description: str = '',
+                 example: str = '',
+                 default: DefaultValue = NoDefaultValue(),
+                 inherit_from: Optional[ConfPath] = None,
+                 create_if_inheritance_target_exists: bool = False,
+                 options: List[str] = []) -> None:
+        super().__init__(name, description, example, default, inherit_from, create_if_inheritance_target_exists)
+        self.options = options
+
+    def get_typename(self, md: bool = False):
+        if md:
+            return "`'" + "'` \| `'".join(self.options) + "'`"
+        else:
+            return "'" + "' | '".join(self.options) + "'"
+
+    def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
+                          selfpth: ConfPath, overridecfg: ConfigNode,
+                          overridepath: ConfPath):
+        assert not self.sub
+        assert not selfcfg.sub
+        assert not overridecfg.sub
+        selfcfg.value = deepcopy(overridecfg.value)
+
+    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
+               cfgpath: ConfPath):
+        if cfg[cfgpath].sub:
+            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
+                              f'{str}, not {dict}')
+        elif not isinstance(cfg[cfgpath].value, str):
+            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
+                              f'{str}, not {type(cfg[cfgpath].value)}')
+        if cfg[cfgpath].value not in self.options:
+            raise ConfigError(f'Value of {pth2str(cfgpath)} should be '
+                              'one of \'' + "', '".join(self.options) + '\'')
+
+class BoolConfigOption(ConfigOption):
+
+    def get_typename(self, md: bool = False):
+        return 'bool'
+
+    def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
+                          selfpth: ConfPath, overridecfg: ConfigNode,
+                          overridepath: ConfPath):
+        assert not self.sub
+        assert not selfcfg.sub
+        assert not overridecfg.sub
+        selfcfg.value = deepcopy(overridecfg.value)
+
+    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
+               cfgpath: ConfPath):
+        if cfg[cfgpath].sub:
+            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
+                              f'{bool}, not {dict}')
+        elif not isinstance(cfg[cfgpath].value, bool):
+            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
+                              f'{bool}, not {type(cfg[cfgpath].value)}')
+
+
+@dataclass
+class RelativeToCurrentConfig:
+    project_path: Path
+    description: str = 'current configuration file'
+
+
+@dataclass
+class RelativeToProject:
+    project_path: Path
+    description: str = 'project directory'
+
+
+class PathConfigOption(StrConfigOption):
+
+    def __init__(self,
+                 name: str,
+                 description: str = '',
+                 example: str = '',
+                 default: DefaultValue = NoDefaultValue(),
+                 must_exist: bool = True,
+                 expected_contents: List[str] = [],
+                 base_path: Optional[Union[RelativeToProject,
+                                           RelativeToCurrentConfig]] = None,
+                 allow_abs: bool = False,
+                 is_folder: bool = True):
+        super().__init__(name, description, example, default)
+        self.must_exist = must_exist or bool(expected_contents)
+        self.expected_contents = expected_contents
+        self.base_path = base_path
+        self.allow_abs = allow_abs
+        self.is_folder = is_folder
+        if self.base_path:
+            assert os.path.isabs(self.base_path.project_path)
+
+    def get_typename(self, md: bool = False):
+        return 'path' if self.is_folder else 'filepath'
+
+    def check_path(self, cfg: ConfigNode, cfgpath):
+        osp = os.path
+        path = osp.normpath(cfg[cfgpath].value)
+        # Absolute or relative path?
+        if osp.isabs(path):
+            # Absolute path
+            if not self.allow_abs:
+                raise ConfigError(f'{pth2str(cfgpath)}: "{str(path)}" '
+                                  f'must be a relative path')
+        else:
+            # Relative path
+            if isinstance(self.base_path, RelativeToCurrentConfig):
+                # cfgpath[0] is relative for files inside of the project,
+                # otherwise it is absolute
+                path = osp.join(osp.dirname(cfgpath[0]), path)
+                if not osp.isabs(path):
+                    path = osp.join(self.base_path.project_path, path)
+            elif isinstance(self.base_path, RelativeToProject):
+                path = osp.join(self.base_path.project_path, path)
+            else:
+                assert False, "Invalid relative path type"
+        assert osp.isabs(path), "Failed to make path absolute"
+        # Does the path exist?
+        if self.must_exist:
+            if not osp.exists(path):
+                raise ConfigError(f'{pth2str(cfgpath)}: "{str(path)}" '
+                                  f'does not exist')
+            if self.is_folder != osp.isdir(path):
+                type_ = 'directory' if self.is_folder else 'file'
+                raise ConfigError(f'{pth2str(cfgpath)}: "{str(path)}" '
+                                  f'should be a {type_}')
+            # Are any of the required contents missing?
+            missing = [
+                sub for sub in self.expected_contents
+                if not osp.exists(osp.join(path, sub))
+            ]
+            if missing:
+                missingstr = '", "'.join(missing)
+                raise ConfigError(f'{pth2str(cfgpath)}: "{str(path)}" '
+                                  f'does not contain the following '
+                                  f'required files or folders: "{missingstr}"')
+        cfg[cfgpath].value = osp.normpath(path)
+
+    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
+               cfgpath: ConfPath):
+        super().verify(rootopts, cfg, cfgpath)
+        self.check_path(cfg, cfgpath)
+
+
+class ListOfStrConfigOption(ConfigOption):
+
+    def __init__(self,
+                 name: str,
+                 description: str = '',
+                 example: str = '',
+                 default: DefaultValue = NoDefaultValue(),
+                 inherit_from: Optional[ConfPath] = None,
+                 create_if_inheritance_target_exists: bool = False,
+                 convert_str_to_singleton=False) -> None:
+        super().__init__(name, description, example, default, inherit_from,
+                         create_if_inheritance_target_exists)
+        self.convert_str_to_singleton = convert_str_to_singleton
+
+    def get_typename(self, md: bool = False):
+        return 'list'
+
+    def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
+                          selfpth: ConfPath, overridecfg: ConfigNode,
+                          overridepath: ConfPath):
+        assert not self.sub
+        assert not selfcfg.sub
+        assert not overridecfg.sub
+        if overridecfg.value is not None:
+            if selfcfg.value is None:
+                selfcfg.value = []
+            assert isinstance(selfcfg.value, list)
+            assert isinstance(overridecfg.value, list)
+            selfcfg.value += deepcopy(overridecfg.value)
+
+    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
+               cfgpath: ConfPath):
+        if cfg[cfgpath].sub:
+            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
+                              f'{list}, not {dict}')
+        elif not isinstance(cfg[cfgpath].value, list):
+            if self.convert_str_to_singleton and \
+                    isinstance(cfg[cfgpath].value, str):
+                cfg[cfgpath].value = [cfg[cfgpath].value]
+            else:
+                raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
+                                  f'{list}, not {type(cfg[cfgpath].value)}')
+        elif not all(isinstance(el, str) for el in cfg[cfgpath].value):
+            raise ConfigError(f'Type of elements in {pth2str(cfgpath)} should '
+                              f'be {str}')
+
+
+class DictOfStrConfigOption(ConfigOption):
+
+    def get_typename(self, md: bool = False):
+        return 'dict'
+
+    def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
+                          selfpth: ConfPath, overridecfg: ConfigNode,
+                          overridepath: ConfPath):
+        assert not self.sub
+        assert not selfcfg.value
+        assert not overridecfg.value
+        if overridecfg.sub is not None:
+            if selfcfg.sub is None:
+                selfcfg.sub = {}
+            assert isinstance(selfcfg.sub, dict)
+            assert isinstance(overridecfg.sub, dict)
+            selfcfg.sub.update(deepcopy(overridecfg.sub))
+
+    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
+               cfgpath: ConfPath):
+        if cfg[cfgpath].value is not None:
+            if isinstance(cfg[cfgpath].value, dict):
+                newcfg = ConfigNode.from_dict(cfg[cfgpath].value)
+                cfg[cfgpath].value = newcfg.value
+                cfg[cfgpath].sub = newcfg.sub
+            else:
+                raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
+                                  f'{dict}, not {type(cfg[cfgpath].value)}')
+        valdict = cfg[cfgpath].sub
+        if not isinstance(valdict, dict):
+            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
+                              f'{dict}, not {type(valdict)}')
+        elif not all(isinstance(el, str) for el in valdict.keys()):
+            raise ConfigError(f'Type of keys in {pth2str(cfgpath)} should '
+                              f'be {str}')
+        elif not all(isinstance(el.value, str) for el in valdict.values()):
+            raise ConfigError(f'Type of values in {pth2str(cfgpath)} should '
+                              f'be {str}')
+
+
+class OverrideConfigOption(ConfigOption):
+
+    def __init__(
+        self,
+        name: str,
+        description: str,
+        targetpath: ConfPath,
+        default: DefaultValue = NoDefaultValue()) -> None:
+        super().__init__(name, description, '', default)
+        self.targetpath = targetpath
+
+    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
+               cfgpath: ConfPath):
+        rootopts[self.targetpath].verify(rootopts, cfg, cfgpath)
+
+    def inherit(self, rootopts: 'ConfigOption', cfg: ConfigNode,
+                selfpth: ConfPath):
+        pass
+
+    def override(self, rootopts: ConfigOption, cfg: ConfigNode,
+                 cfgpath: ConfPath):
+        selfcfg = cfg.get(cfgpath, None)
+        if selfcfg is None:
+            return
+        elif selfcfg.value is None and selfcfg.sub is None:
+            return
+        super().override(rootopts, cfg, cfgpath)
+        curropt = rootopts[self.targetpath]
+        self.create_parent_config(cfg, self.targetpath)
+        currcfg = cfg[self.targetpath]
+        overridecfg = cfg[cfgpath]
+        # Override the config at those paths by our own config
+        curropt.explicit_override(rootopts, currcfg, self.targetpath,
+                                  overridecfg, cfgpath)
+
+    @staticmethod
+    def create_parent_config(cfg: ConfigNode, path: ConfPath):
+        parentcfg = cfg
+        for s in path:
+            assert parentcfg.sub is not None
+            parentcfg = parentcfg.sub.setdefault(s, ConfigNode(sub={}))
```

### Comparing `py-build-cmake-0.1.7/src/py_build_cmake/help/__init__.py` & `py-build-cmake-0.1.8/src/py_build_cmake/help/__init__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-import html
-import itertools
-import shutil
-import textwrap
-import re
-
-from ..config_options import ConfigOption, PathConfigOption, RequiredValue, pth2str
-
-
-def _print_wrapped(text, indent, width=None):
-    """Print the given string with the given indentation, wrapping it to the
-    desired width, preserving line endings. If `width` is None, use the width 
-    of the terminal, or 80 columns as a fallback."""
-    if width is None:
-        width = shutil.get_terminal_size((80, 24)).columns
-    wrapper = textwrap.TextWrapper(width=width,
-                                   initial_indent=indent,
-                                   subsequent_indent=indent)
-    wrapped = [wrapper.wrap(i) for i in text.split('\n')]
-    for line in itertools.chain.from_iterable(wrapped):
-        print(line)
-
-
-def get_default_str(opt: ConfigOption):
-    """Get a string representation of the default value for the given option."""
-    return opt.default.get_name()
-
-
-def help_print_md(pbc_opts: ConfigOption):
-    """
-    Prints the top-level options in `pbc_opts` as MarkDown tables.
-    """
-    for k, v in pbc_opts.sub.items():
-        print('##', k)
-        print(_get_full_description(v), '\n')
-        print('| Option | Description | Type | Default |')
-        print('|--------|-------------|------|---------|')
-        for kk, vv in v.sub.items() or {}:
-            typename = vv.get_typename(md=True) or ''
-            print('|', f'`{kk}`', '|', _get_full_description(vv), '|',
-                  typename, '|', f'`{get_default_str(vv)}`', '|')
-        print()
-
-def _get_full_description(vv: ConfigOption):
-    descr = _md_escape(vv.description)
-    if isinstance(vv, PathConfigOption):
-        descr += '<br/>' + _describe_path_option(vv).capitalize() + '.'
-    if vv.inherit_from:
-        descr += '<br/>Inherits from: `/' + pth2str(vv.inherit_from) + '`'
-    if vv.example:
-        descr += '<br/>For example: `' + vv.example + '`'
-    return descr
-
-
-def _md_escape(descr: str):
-    descr = html.escape(descr)
-    descr = descr.replace('*', '\\*')
-    descr = descr.replace('_', '\\_')
-    def unescape(m: re.Match):
-        m0 = m.group(0)
-        return html.unescape(m0.replace('\\_', '_').replace('\\*', '*'))
-    descr = re.sub(r'`.*`', unescape, descr)
-    descr = descr.replace('\n', '<br/>')
-    return descr
-
-
-def recursive_help_print(opt: ConfigOption, level=0):
-    """Recursively prints the help messages for the options in `opt`."""
-    for k, v in opt.sub.items():
-        if k == 'project':
-            continue
-        indent = 4 * level * ' '
-        header = '\n' + k
-        if v.sub:
-            header += ':'
-            print(textwrap.indent(header, indent))
-            if v.description:
-                _print_wrapped(v.description, indent + '  ')
-            recursive_help_print(v, level + 1)
-        else:
-            headerfields = []
-            typename = v.get_typename()
-            if typename is not None:
-                headerfields += [typename]
-            if isinstance(v, PathConfigOption):
-                headerfields += [_describe_path_option(v)]
-            is_required = isinstance(v.default, RequiredValue)
-            if is_required:
-                headerfields += ['required']
-            if v.inherit_from:
-                headerfields += ['inherits from /' + pth2str(v.inherit_from)]
-            if headerfields:
-                header += ' (' + ', '.join(headerfields) + ')'
-            print(textwrap.indent(header + ':', indent))
-            _print_wrapped(v.description, indent + '  ')
-            if v.example:
-                _print_wrapped('For example: ' + v.example, indent + '  ')
-            default = v.default.get_name()
-            if default is not None and not is_required:
-                print(textwrap.indent('Default: ' + default, indent + '  '))
-
-
-def _describe_path_option(v: PathConfigOption):
-    t = 'absolute or relative' if v.allow_abs else 'relative'
-    if v.base_path is not None:
-        t += ' to ' + v.base_path.description
-    return t
-
-
-def help_print(pbc_opts: ConfigOption):
-    recursive_help_print(pbc_opts)
-    print()
+import html
+import itertools
+import shutil
+import textwrap
+import re
+
+from ..config_options import ConfigOption, PathConfigOption, RequiredValue, pth2str
+
+
+def _print_wrapped(text, indent, width=None):
+    """Print the given string with the given indentation, wrapping it to the
+    desired width, preserving line endings. If `width` is None, use the width 
+    of the terminal, or 80 columns as a fallback."""
+    if width is None:
+        width = shutil.get_terminal_size((80, 24)).columns
+    wrapper = textwrap.TextWrapper(width=width,
+                                   initial_indent=indent,
+                                   subsequent_indent=indent)
+    wrapped = [wrapper.wrap(i) for i in text.split('\n')]
+    for line in itertools.chain.from_iterable(wrapped):
+        print(line)
+
+
+def get_default_str(opt: ConfigOption):
+    """Get a string representation of the default value for the given option."""
+    return opt.default.get_name()
+
+
+def help_print_md(pbc_opts: ConfigOption):
+    """
+    Prints the top-level options in `pbc_opts` as MarkDown tables.
+    """
+    for k, v in pbc_opts.sub.items():
+        print('##', k)
+        print(_get_full_description(v), '\n')
+        print('| Option | Description | Type | Default |')
+        print('|--------|-------------|------|---------|')
+        for kk, vv in v.sub.items() or {}:
+            typename = vv.get_typename(md=True) or ''
+            print('|', f'`{kk}`', '|', _get_full_description(vv), '|',
+                  typename, '|', f'`{get_default_str(vv)}`', '|')
+        print()
+
+def _get_full_description(vv: ConfigOption):
+    descr = _md_escape(vv.description)
+    if isinstance(vv, PathConfigOption):
+        descr += '<br/>' + _describe_path_option(vv).capitalize() + '.'
+    if vv.inherit_from:
+        descr += '<br/>Inherits from: `/' + pth2str(vv.inherit_from) + '`'
+    if vv.example:
+        descr += '<br/>For example: `' + vv.example + '`'
+    return descr
+
+
+def _md_escape(descr: str):
+    descr = html.escape(descr)
+    descr = descr.replace('*', '\\*')
+    descr = descr.replace('_', '\\_')
+    def unescape(m: re.Match):
+        m0 = m.group(0)
+        return html.unescape(m0.replace('\\_', '_').replace('\\*', '*'))
+    descr = re.sub(r'`.*`', unescape, descr)
+    descr = descr.replace('\n', '<br/>')
+    return descr
+
+
+def recursive_help_print(opt: ConfigOption, level=0):
+    """Recursively prints the help messages for the options in `opt`."""
+    for k, v in opt.sub.items():
+        if k == 'project':
+            continue
+        indent = 4 * level * ' '
+        header = '\n' + k
+        if v.sub:
+            header += ':'
+            print(textwrap.indent(header, indent))
+            if v.description:
+                _print_wrapped(v.description, indent + '  ')
+            recursive_help_print(v, level + 1)
+        else:
+            headerfields = []
+            typename = v.get_typename()
+            if typename is not None:
+                headerfields += [typename]
+            if isinstance(v, PathConfigOption):
+                headerfields += [_describe_path_option(v)]
+            is_required = isinstance(v.default, RequiredValue)
+            if is_required:
+                headerfields += ['required']
+            if v.inherit_from:
+                headerfields += ['inherits from /' + pth2str(v.inherit_from)]
+            if headerfields:
+                header += ' (' + ', '.join(headerfields) + ')'
+            print(textwrap.indent(header + ':', indent))
+            _print_wrapped(v.description, indent + '  ')
+            if v.example:
+                _print_wrapped('For example: ' + v.example, indent + '  ')
+            default = v.default.get_name()
+            if default is not None and not is_required:
+                print(textwrap.indent('Default: ' + default, indent + '  '))
+
+
+def _describe_path_option(v: PathConfigOption):
+    t = 'absolute or relative' if v.allow_abs else 'relative'
+    if v.base_path is not None:
+        t += ' to ' + v.base_path.description
+    return t
+
+
+def help_print(pbc_opts: ConfigOption):
+    recursive_help_print(pbc_opts)
+    print()
```

### Comparing `py-build-cmake-0.1.7/src/py_build_cmake/tags.py` & `py-build-cmake-0.1.8/src/py_build_cmake/tags.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-"""
-distlib.wheel doesn't always return the correct tags, and packaging.tags
-returns all tags supported by the interpreter, not the tags that should be used
-for the generated wheels. Therefore the only option here is to write our own
-(kind of hacky) functions based on packaging.tags.
-"""
-
-from typing import Dict
-import sys
-import sysconfig
-from importlib.machinery import EXTENSION_SUFFIXES
-from distlib.util import get_platform as get_platform_dashes  # type: ignore
-
-_INTERPRETER_SHORT_NAMES: Dict[str, str] = {
-    "python": "py",
-    "cpython": "cp",
-    "pypy": "pp",
-    "ironpython": "ip",
-    "jython": "jy",
-}
-
-
-def _normalize_string(s: str) -> str:
-    return s.replace(".", "_").replace("-", "_")
-
-
-def get_platform_tag() -> str:
-    return _normalize_string(get_platform_dashes())
-
-
-def get_interpreter_name() -> str:
-    name = sys.implementation.name
-    return _INTERPRETER_SHORT_NAMES.get(name) or name
-
-
-def get_interpreter_version() -> str:
-    return "".join(map(str, sys.version_info[:2]))
-
-
-def get_cpython_interpreter() -> str:
-    return f"cp{get_interpreter_version()}"
-
-
-def get_cpython_abi() -> str:
-    """
-    Get the ABI string for CPython, e.g. cp37m.
-
-    https://github.com/pypa/packaging/blob/917612f5774571a99902b5fe04d06099b9e8b667/packaging/tags.py#L135
-    """
-    py_version = sys.version_info[:2]
-    debug = pymalloc = ""
-    with_debug = sysconfig.get_config_var("Py_DEBUG")
-    has_refcount = hasattr(sys, "gettotalrefcount")
-    # Windows doesn't set Py_DEBUG, so checking for support of debug-compiled
-    # extension modules is the best option.
-    # https://github.com/pypa/pip/issues/3383#issuecomment-173267692
-    has_ext = "_d.pyd" in EXTENSION_SUFFIXES
-    if with_debug or (with_debug is None and (has_refcount or has_ext)):
-        debug = "d"
-    if py_version < (3, 8):
-        with_pymalloc = sysconfig.get_config_var("WITH_PYMALLOC")
-        if with_pymalloc or with_pymalloc is None:
-            pymalloc = "m"
-    return f"{get_cpython_interpreter()}{debug}{pymalloc}"
-
-
-def get_generic_interpreter() -> str:
-    return f"{get_interpreter_name()}{get_interpreter_version()}"
-
-
-def get_generic_abi() -> str:
-    abi = sysconfig.get_config_var("SOABI") or "none"
-    return _normalize_string(abi)
-
-
-def get_python_tag() -> str:
-    if get_interpreter_name() == "cp": return get_cpython_interpreter()
-    else: return get_generic_interpreter()
-
-
-def get_abi_tag() -> str:
-    if get_interpreter_name() == "cp": return get_cpython_abi()
-    else: return get_generic_abi()
+"""
+distlib.wheel doesn't always return the correct tags, and packaging.tags
+returns all tags supported by the interpreter, not the tags that should be used
+for the generated wheels. Therefore the only option here is to write our own
+(kind of hacky) functions based on packaging.tags.
+"""
+
+from typing import Dict
+import sys
+import sysconfig
+from importlib.machinery import EXTENSION_SUFFIXES
+from distlib.util import get_platform as get_platform_dashes  # type: ignore
+
+_INTERPRETER_SHORT_NAMES: Dict[str, str] = {
+    "python": "py",
+    "cpython": "cp",
+    "pypy": "pp",
+    "ironpython": "ip",
+    "jython": "jy",
+}
+
+
+def _normalize_string(s: str) -> str:
+    return s.replace(".", "_").replace("-", "_")
+
+
+def get_platform_tag() -> str:
+    return _normalize_string(get_platform_dashes())
+
+
+def get_interpreter_name() -> str:
+    name = sys.implementation.name
+    return _INTERPRETER_SHORT_NAMES.get(name) or name
+
+
+def get_interpreter_version() -> str:
+    return "".join(map(str, sys.version_info[:2]))
+
+
+def get_cpython_interpreter() -> str:
+    return f"cp{get_interpreter_version()}"
+
+
+def get_cpython_abi() -> str:
+    """
+    Get the ABI string for CPython, e.g. cp37m.
+
+    https://github.com/pypa/packaging/blob/917612f5774571a99902b5fe04d06099b9e8b667/packaging/tags.py#L135
+    """
+    py_version = sys.version_info[:2]
+    debug = pymalloc = ""
+    with_debug = sysconfig.get_config_var("Py_DEBUG")
+    has_refcount = hasattr(sys, "gettotalrefcount")
+    # Windows doesn't set Py_DEBUG, so checking for support of debug-compiled
+    # extension modules is the best option.
+    # https://github.com/pypa/pip/issues/3383#issuecomment-173267692
+    has_ext = "_d.pyd" in EXTENSION_SUFFIXES
+    if with_debug or (with_debug is None and (has_refcount or has_ext)):
+        debug = "d"
+    if py_version < (3, 8):
+        with_pymalloc = sysconfig.get_config_var("WITH_PYMALLOC")
+        if with_pymalloc or with_pymalloc is None:
+            pymalloc = "m"
+    return f"{get_cpython_interpreter()}{debug}{pymalloc}"
+
+
+def get_generic_interpreter() -> str:
+    return f"{get_interpreter_name()}{get_interpreter_version()}"
+
+
+def get_generic_abi() -> str:
+    abi = sysconfig.get_config_var("SOABI") or "none"
+    return _normalize_string(abi)
+
+
+def get_python_tag() -> str:
+    if get_interpreter_name() == "cp": return get_cpython_interpreter()
+    else: return get_generic_interpreter()
+
+
+def get_abi_tag() -> str:
+    if get_interpreter_name() == "cp": return get_cpython_abi()
+    else: return get_generic_abi()
```

### Comparing `py-build-cmake-0.1.7/PKG-INFO` & `py-build-cmake-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-build-cmake
-Version: 0.1.7
+Version: 0.1.8
 Summary: Modern, PEP 517 compliant build backend for creating Python packages with
 Keywords: pep517,cmake
 Author-email: Pieter P <pieter.p.dev@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -86,15 +86,15 @@
 keywords = ["some", "keywords"]
 classifiers = ["Topic :: Scientific/Engineering"]
 urls = { "Documentation" = "https://tttapa.github.io/py-build-cmake" }
 dependencies = ["numpy"]
 dynamic = ["version", "description"]
 
 [build-system] # How pip and other frontends should build this project
-requires = ["py-build-cmake~=0.1.7"]
+requires = ["py-build-cmake~=0.1.8"]
 build-backend = "py_build_cmake.build"
 
 [tool.py-build-cmake.module] # Where to find the Python module to package
 directory = "src-python"
 
 [tool.py-build-cmake.sdist] # What to include in source distributions
 include = ["CMakeLists.txt", "src/*"]
```

