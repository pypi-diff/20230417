# Comparing `tmp/rfdocsindexer-1.1.0.tar.gz` & `tmp/rfdocsindexer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfdocsindexer-1.1.0.tar", max compression
+gzip compressed data, was "rfdocsindexer-1.2.0.tar", max compression
```

## Comparing `rfdocsindexer-1.1.0.tar` & `rfdocsindexer-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    11357 2022-10-08 07:50:43.789633 rfdocsindexer-1.1.0/LICENSE
--rw-r--r--   0        0        0     2813 2022-10-08 07:50:43.789633 rfdocsindexer-1.1.0/README.md
--rw-r--r--   0        0        0     1637 2022-10-08 07:50:43.801633 rfdocsindexer-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-08 07:50:43.801633 rfdocsindexer-1.1.0/rfdocsindexer/__init__.py
--rw-r--r--   0        0        0     1609 2022-10-08 07:50:43.801633 rfdocsindexer-1.1.0/rfdocsindexer/cli.py
--rw-r--r--   0        0        0     2854 2022-10-08 07:50:43.801633 rfdocsindexer-1.1.0/rfdocsindexer/config.py
--rw-r--r--   0        0        0    10158 2022-10-08 07:50:43.801633 rfdocsindexer-1.1.0/rfdocsindexer/indexer.py
--rw-r--r--   0        0        0     3448 2022-10-08 07:50:43.801633 rfdocsindexer-1.1.0/rfdocsindexer/models.py
--rw-r--r--   0        0        0     3062 2022-10-08 07:50:43.801633 rfdocsindexer-1.1.0/rfdocsindexer/templates/index.html
--rw-r--r--   0        0        0     3834 1970-01-01 00:00:00.000000 rfdocsindexer-1.1.0/setup.py
--rw-r--r--   0        0        0     4335 1970-01-01 00:00:00.000000 rfdocsindexer-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-17 15:08:31.438335 rfdocsindexer-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2813 2023-04-17 15:08:31.438335 rfdocsindexer-1.2.0/README.md
+-rw-r--r--   0        0        0     1703 2023-04-17 15:08:31.450335 rfdocsindexer-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 15:08:31.450335 rfdocsindexer-1.2.0/rfdocsindexer/__init__.py
+-rw-r--r--   0        0        0     1609 2023-04-17 15:08:31.450335 rfdocsindexer-1.2.0/rfdocsindexer/cli.py
+-rw-r--r--   0        0        0     2854 2023-04-17 15:08:31.450335 rfdocsindexer-1.2.0/rfdocsindexer/config.py
+-rw-r--r--   0        0        0    10269 2023-04-17 15:08:31.450335 rfdocsindexer-1.2.0/rfdocsindexer/indexer.py
+-rw-r--r--   0        0        0     3448 2023-04-17 15:08:31.450335 rfdocsindexer-1.2.0/rfdocsindexer/models.py
+-rw-r--r--   0        0        0     3062 2023-04-17 15:08:31.450335 rfdocsindexer-1.2.0/rfdocsindexer/templates/index.html
+-rw-r--r--   0        0        0     4402 1970-01-01 00:00:00.000000 rfdocsindexer-1.2.0/PKG-INFO
```

### Comparing `rfdocsindexer-1.1.0/LICENSE` & `rfdocsindexer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rfdocsindexer-1.1.0/README.md` & `rfdocsindexer-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rfdocsindexer-1.1.0/pyproject.toml` & `rfdocsindexer-1.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 [tool.poetry]
 name = "rfdocsindexer"
-version = "1.1.0"
+version = "1.2.0"
 description = "A simple and configurable generator for RobotFramework documentation"
 license = "Apache-2.0"
 authors = ["Vincent Maire <maire.vincent31@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/Vincema/rfdocsindexer"
 repository = "https://github.com/Vincema/rfdocsindexer"
 keywords = ["RobotFramework", "Documentation", "Libdocs", "Testing"]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Framework :: Robot Framework",
     "Framework :: Robot Framework :: Tool",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Documentation",
     "Topic :: Software Development :: Testing",
     "Topic :: Software Development :: Quality Assurance",
     "Operating System :: iOS",
     "Operating System :: Unix",
     "Operating System :: Microsoft :: Windows",
 ]
 
 
 [tool.poetry.scripts]
 indexrfdocs = "rfdocsindexer.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-click = "^8.0.1"
-Jinja2 = "^3.0.1"
-pydantic = "^1.8.2"
-robotframework = ">=4,<6"
-toml = "^0.10.2"
+click = ">= 8"
+Jinja2 = ">= 3"
+pydantic = ">= 1"
+robotframework = ">= 4"
+toml = ">= 0"
 
 [tool.poetry.dev-dependencies]
 beautifulsoup4 = "^4.9.3"
-black = "^22.1"
-coverage = "^6.0"
+black = "^23.3"
+coverage = "^7.0"
 flake8 = "^5.0.4"
-invoke = "^1.6.0"
+invoke = "^2.0"
 isort = "^5.9.3"
-mypy = "^0.982"
+mypy = "^1.2"
 pytest = "^7.0.1"
-robotframework-tidy = "^3.2"
+robotframework-tidy = "^4.1"
 tox = "^3.24.0"
 tox-poetry-installer = {extras = ["poetry"], version = "^0.10.0"}
 types-toml = "^0.10.0"
-
+tox-gh-actions = "^2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rfdocsindexer-1.1.0/rfdocsindexer/cli.py` & `rfdocsindexer-1.2.0/rfdocsindexer/cli.py`

 * *Files identical despite different names*

### Comparing `rfdocsindexer-1.1.0/rfdocsindexer/config.py` & `rfdocsindexer-1.2.0/rfdocsindexer/config.py`

 * *Files identical despite different names*

### Comparing `rfdocsindexer-1.1.0/rfdocsindexer/indexer.py` & `rfdocsindexer-1.2.0/rfdocsindexer/indexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,14 @@
     """
     ext_resources: List[ExternalResource] = []
 
     if len(urls) == 0:
         return []
 
     for raw_url in urls:
-
         # Extract url components (can be "name | http://example")
         name_delimiter = " | "
         name: str = raw_url
         url: str = raw_url
 
         try:
             if raw_url.count(name_delimiter) > 1:
@@ -183,15 +182,15 @@
             parsed_url = urlparse(url)
             if not parsed_url.netloc or not parsed_url.scheme:
                 raise ValueError
 
         except ValueError:
             raise RuntimeError(f'Url format is invalid for url "{url}"')
 
-        ext_resources += [ExternalResource(url=url, name=name)]
+        ext_resources += [ExternalResource(url=url, name=name)]  # type: ignore
 
     print("Indexed external resources")
 
     return ext_resources
 
 
 def _gen_index_file(
@@ -277,31 +276,33 @@
         libdoc_html.convert_docs_to_html()
 
         html_filepath = output_dir / HTML_LIBDOC_DIR / (lib.name + ".html")
         libdoc_html.save(html_filepath, "HTML")
 
         xml_filepath: Optional[Path] = None
         json_filepath: Optional[Path] = None
+        libspec_filepath: Optional[Path] = None
         if gen_machine_readable_libdocs:
             libdoc_robot = copy.deepcopy(lib.libdoc)
 
             xml_filepath = output_dir / XML_LIBDOC_DIR / (lib.name + ".xml")
             libdoc_robot.save(xml_filepath, "XML")
 
             json_filepath = output_dir / JSON_LIBDOC_DIR / (lib.name + ".json")
             libdoc_robot.save(json_filepath, "JSON")
 
             libspec_filepath = output_dir / LIBSPEC_DIR / (lib.name + ".spec")
-            libdoc_html.save(libspec_filepath, "LIBSPEC")
+            libdoc_robot.save(libspec_filepath, "LIBSPEC")
 
         indexed_libraries += [
             IndexedRFLibrary(
                 html_libdoc_path=html_filepath,
                 xml_libdoc_path=xml_filepath,
                 json_libdoc_path=json_filepath,
+                libspec_path=libspec_filepath,
                 libdata=lib.copy(deep=True),
             )
         ]
 
         print(f'Generated doc for "{lib.name}"')
 
     return indexed_libraries
```

### Comparing `rfdocsindexer-1.1.0/rfdocsindexer/models.py` & `rfdocsindexer-1.2.0/rfdocsindexer/models.py`

 * *Files identical despite different names*

### Comparing `rfdocsindexer-1.1.0/rfdocsindexer/templates/index.html` & `rfdocsindexer-1.2.0/rfdocsindexer/templates/index.html`

 * *Files identical despite different names*

### Comparing `rfdocsindexer-1.1.0/setup.py` & `rfdocsindexer-1.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,102 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: rfdocsindexer
+Version: 1.2.0
+Summary: A simple and configurable generator for RobotFramework documentation
+Home-page: https://github.com/Vincema/rfdocsindexer
+License: Apache-2.0
+Keywords: RobotFramework,Documentation,Libdocs,Testing
+Author: Vincent Maire
+Author-email: maire.vincent31@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Robot Framework
+Classifier: Framework :: Robot Framework :: Tool
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+Classifier: Operating System :: iOS
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Documentation
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Requires-Dist: Jinja2 (>=3)
+Requires-Dist: click (>=8)
+Requires-Dist: pydantic (>=1)
+Requires-Dist: robotframework (>=4)
+Requires-Dist: toml (>=0)
+Project-URL: Repository, https://github.com/Vincema/rfdocsindexer
+Description-Content-Type: text/markdown
+
+# RF Documentations Indexer
+
+Rfdocsindexer is a simple Python3 module to generate [RobotFramework](https://robotframework.org/) 4+ libraries documentation.
+
+One can configure the tool from a simple [TOML](https://github.com/toml-lang/toml) configuration file and run it from a console.
+
+The tool then uses the RobotFramework [Libdoc](https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#libdoc) module to generate an HTML, XML, JSON or Libspec documentation for any RobotFramework keyword library.
+
+An HTML index is also generated to centralize the generated documentations.
+
+![RFDocsIndexer Diagram](https://github.com/Vincema/rfdocsindexer/raw/main/docs/diagrams/rfdocsindexer_diagram.svg)
+
+Below is an overview of the HTML index generated. It makes it easy to navigate among external resources and keywords documentation.
+
+![Index File Overview](https://github.com/Vincema/rfdocsindexer/raw/main/docs/rfdocsindexer-overview.gif)
+
+## Installing the tool
+
+Install from Pypi:
+```bash
+pip install rfdocsindexer
+```
+
+## Configuring the tool
+
+The tool can be configured with a config file in [TOML](https://github.com/toml-lang/toml) format.
+
+Example configuration file:
+
+```toml
+[rfdocsindexer]
+library_paths = ["**/libraries/*.robot", "my_library.resource"]
+library_names = ["MyLibrary", "MyOtherLibary.MyOtherLibrary"]
+extra_modules_searchpaths = ["./library_dir"]
+external_resources = ["RF homepage | https://robotframework.org/", "http://example.org"]
+build_machine_readable_libdoc = true
+include_robotframework_resources = true
+```
+
+The configuration file must contain the section `[rfdocindexer]` and any or none of the following options:
+
+* `library_paths`: a list of paths (glob format accepted) to RF resource files (can be `*.resource`, `*.robot`, `*.spec`...)
+* `library_names`: a list of RF library modules
+* `extra_modules_searchpaths`: a list of paths to append to `PYTHONPATH`
+* `external_resources`: a list of URLs which will be added to the HTML index file, or `<name> | <URL>`. Useful to include frequently used external resources when developing tests.
+* `build_machine_readable_libdoc`: whether to generate documentation in XML, JSON and Libspec format. If set to `False`, only the HTML documenation will be generated. Default is `False`.
+* `include_robotframework_resources`: whether to generate documentation for default RobotFramework libraries (`BuiltIn`, `Collection`, ...). Default is `True`.
+
+
+## Running the tool
+
+In a standard shell, run the following:
+
+```bash
+# To generate documentation for default RobotFramework libraries
+indexrfdocs
+
+# To specify the configuration file to use
+indexrfdocs -c path/to/configfile.toml
+
+# To specify the output directory (content will not be erased if already existing), default is "rfdocs"
+indexrfdocs -o path/to/outdir
+```
 
-packages = \
-['rfdocsindexer']
-
-package_data = \
-{'': ['*'], 'rfdocsindexer': ['templates/*']}
-
-install_requires = \
-['Jinja2>=3.0.1,<4.0.0',
- 'click>=8.0.1,<9.0.0',
- 'pydantic>=1.8.2,<2.0.0',
- 'robotframework>=4,<6',
- 'toml>=0.10.2,<0.11.0']
-
-entry_points = \
-{'console_scripts': ['indexrfdocs = rfdocsindexer.cli:cli']}
-
-setup_kwargs = {
-    'name': 'rfdocsindexer',
-    'version': '1.1.0',
-    'description': 'A simple and configurable generator for RobotFramework documentation',
-    'long_description': '# RF Documentations Indexer\n\nRfdocsindexer is a simple Python3 module to generate [RobotFramework](https://robotframework.org/) 4+ libraries documentation.\n\nOne can configure the tool from a simple [TOML](https://github.com/toml-lang/toml) configuration file and run it from a console.\n\nThe tool then uses the RobotFramework [Libdoc](https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#libdoc) module to generate an HTML, XML, JSON or Libspec documentation for any RobotFramework keyword library.\n\nAn HTML index is also generated to centralize the generated documentations.\n\n![RFDocsIndexer Diagram](https://github.com/Vincema/rfdocsindexer/raw/main/docs/diagrams/rfdocsindexer_diagram.svg)\n\nBelow is an overview of the HTML index generated. It makes it easy to navigate among external resources and keywords documentation.\n\n![Index File Overview](https://github.com/Vincema/rfdocsindexer/raw/main/docs/rfdocsindexer-overview.gif)\n\n## Installing the tool\n\nInstall from Pypi:\n```bash\npip install rfdocsindexer\n```\n\n## Configuring the tool\n\nThe tool can be configured with a config file in [TOML](https://github.com/toml-lang/toml) format.\n\nExample configuration file:\n\n```toml\n[rfdocsindexer]\nlibrary_paths = ["**/libraries/*.robot", "my_library.resource"]\nlibrary_names = ["MyLibrary", "MyOtherLibary.MyOtherLibrary"]\nextra_modules_searchpaths = ["./library_dir"]\nexternal_resources = ["RF homepage | https://robotframework.org/", "http://example.org"]\nbuild_machine_readable_libdoc = true\ninclude_robotframework_resources = true\n```\n\nThe configuration file must contain the section `[rfdocindexer]` and any or none of the following options:\n\n* `library_paths`: a list of paths (glob format accepted) to RF resource files (can be `*.resource`, `*.robot`, `*.spec`...)\n* `library_names`: a list of RF library modules\n* `extra_modules_searchpaths`: a list of paths to append to `PYTHONPATH`\n* `external_resources`: a list of URLs which will be added to the HTML index file, or `<name> | <URL>`. Useful to include frequently used external resources when developing tests.\n* `build_machine_readable_libdoc`: whether to generate documentation in XML, JSON and Libspec format. If set to `False`, only the HTML documenation will be generated. Default is `False`.\n* `include_robotframework_resources`: whether to generate documentation for default RobotFramework libraries (`BuiltIn`, `Collection`, ...). Default is `True`.\n\n\n## Running the tool\n\nIn a standard shell, run the following:\n\n```bash\n# To generate documentation for default RobotFramework libraries\nindexrfdocs\n\n# To specify the configuration file to use\nindexrfdocs -c path/to/configfile.toml\n\n# To specify the output directory (content will not be erased if already existing), default is "rfdocs"\nindexrfdocs -o path/to/outdir\n```\n',
-    'author': 'Vincent Maire',
-    'author_email': 'maire.vincent31@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Vincema/rfdocsindexer',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

