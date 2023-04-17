# Comparing `tmp/pyriksprot_tagger-2023.4.1.tar.gz` & `tmp/pyriksprot_tagger-2023.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriksprot_tagger-2023.4.1.tar", max compression
+gzip compressed data, was "pyriksprot_tagger-2023.4.2.tar", max compression
```

## Comparing `pyriksprot_tagger-2023.4.1.tar` & `pyriksprot_tagger-2023.4.2.tar`

### file list

```diff
@@ -1,31 +1,35 @@
--rw-r--r--   0        0        0     1080 2022-03-14 19:05:45.701621 pyriksprot_tagger-2023.4.1/LICENSE
--rw-r--r--   0        0        0     3694 2023-03-27 14:40:27.622646 pyriksprot_tagger-2023.4.1/README.md
--rw-r--r--   0        0        0     4593 2023-04-13 13:21:06.650320 pyriksprot_tagger-2023.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.4.1/scripts/__init__.py
--rw-r--r--   0        0        0     7224 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.1/scripts/git-timesync
--rwxr-xr-x   0        0        0     1786 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.1/scripts/git_update_mtime.sh
--rw-r--r--   0        0        0      563 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.1/scripts/move_empty_files.sh
--rwxr-xr-x   0        0        0      251 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.1/scripts/setup-pipeline
--rwxr-xr-x   0        0        0      196 2023-04-13 12:39:25.781582 pyriksprot_tagger-2023.4.1/scripts/snake-it.sh
--rwxr-xr-x   0        0        0     1071 2023-04-13 12:39:25.781582 pyriksprot_tagger-2023.4.1/scripts/stanza-models.sh
--rwxr-xr-x   0        0        0     4244 2023-04-13 12:39:25.781582 pyriksprot_tagger-2023.4.1/scripts/tag-it.sh
--rw-r--r--   0        0        0      995 2023-03-28 10:59:30.619948 pyriksprot_tagger-2023.4.1/scripts/tag.py
--rw-r--r--   0        0        0      846 2023-04-13 12:39:25.781582 pyriksprot_tagger-2023.4.1/scripts/tag_info.py
--rw-r--r--   0        0        0     4328 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/Makefile
--rw-r--r--   0        0        0        0 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.4.1/workflow/README.md
--rw-r--r--   0        0        0     1714 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/Snakefile
--rw-r--r--   0        0        0        0 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.4.1/workflow/__init__.py
--rw-r--r--   0        0        0     5274 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/config.py
--rw-r--r--   0        0        0        0 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.4.1/workflow/rules/__init__.py
--rw-r--r--   0        0        0      188 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.4.1/workflow/rules/__paths__.py
--rw-r--r--   0        0        0      735 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/rules/compute_frequency.smk
--rw-r--r--   0        0        0      892 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/rules/extract_speeches.smk
--rw-r--r--   0        0        0      111 2022-03-14 19:05:45.729621 pyriksprot_tagger-2023.4.1/workflow/rules/help.smk
--rw-r--r--   0        0        0     1302 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/rules/tag_protocols.smk
--rw-r--r--   0        0        0     1758 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/rules/update_repository.smk
--rw-r--r--   0        0        0      121 2022-03-14 19:05:45.729621 pyriksprot_tagger-2023.4.1/workflow/taggers/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/taggers/registry.py
--rw-r--r--   0        0        0     1991 2022-03-14 19:05:45.729621 pyriksprot_tagger-2023.4.1/workflow/taggers/spacy2.py
--rw-r--r--   0        0        0     4235 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.4.1/workflow/taggers/stanza.py
--rw-r--r--   0        0        0     5575 2023-03-27 14:40:27.626646 pyriksprot_tagger-2023.4.1/workflow/utility.py
--rw-r--r--   0        0        0     4783 1970-01-01 00:00:00.000000 pyriksprot_tagger-2023.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-03-14 19:05:45.701621 pyriksprot_tagger-2023.4.2/LICENSE
+-rw-r--r--   0        0        0     3694 2023-03-27 14:40:27.622646 pyriksprot_tagger-2023.4.2/README.md
+-rw-r--r--   0        0        0     4674 2023-04-17 15:02:40.902581 pyriksprot_tagger-2023.4.2/pyproject.toml
+-rw-r--r--   0        0        0      259 2023-04-17 09:10:35.869007 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/__init__.py
+-rw-r--r--   0        0        0     5625 2023-04-17 13:47:26.532461 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/config.py
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/resources/__init__.py
+-rw-r--r--   0        0        0       68 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/resources/sparv/Makefile
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/resources/sparv/__init__.py
+-rw-r--r--   0        0        0     4963 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/resources/sparv/speech_xml_config.yaml
+-rw-r--r--   0        0        0        0 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/__init__.py
+-rw-r--r--   0        0        0     7224 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/git-timesync
+-rwxr-xr-x   0        0        0     1786 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/git_update_mtime.sh
+-rw-r--r--   0        0        0      563 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/move_empty_files.sh
+-rwxr-xr-x   0        0        0      251 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/setup-pipeline
+-rwxr-xr-x   0        0        0      196 2023-04-13 12:39:25.781582 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/snake-it.sh
+-rwxr-xr-x   0        0        0     1071 2023-04-13 12:39:25.781582 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/stanza-models.sh
+-rwxr-xr-x   0        0        0     4244 2023-04-13 12:39:25.781582 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/tag-it.sh
+-rw-r--r--   0        0        0     1038 2023-04-14 14:18:41.032914 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/tag.py
+-rw-r--r--   0        0        0      846 2023-04-14 09:19:33.724658 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/tag_info.py
+-rw-r--r--   0        0        0       70 2023-04-14 12:29:53.731729 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/taggers/__init__.py
+-rw-r--r--   0        0        0     1991 2022-03-14 19:05:45.729621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/taggers/spacy2.py
+-rw-r--r--   0        0        0     7179 2023-04-17 09:10:36.389014 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/taggers/stanza.py
+-rw-r--r--   0        0        0     5346 2023-04-17 09:10:49.005177 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/utility.py
+-rw-r--r--   0        0        0     4328 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/Makefile
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/README.md
+-rw-r--r--   0        0        0     1709 2023-04-14 14:21:13.246887 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/Snakefile
+-rw-r--r--   0        0        0       15 2023-04-14 14:12:34.288157 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/__init__.py
+-rw-r--r--   0        0        0      188 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/__paths__.py
+-rw-r--r--   0        0        0      735 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/compute_frequency.smk
+-rw-r--r--   0        0        0      892 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/extract_speeches.smk
+-rw-r--r--   0        0        0      111 2022-03-14 19:05:45.729621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/help.smk
+-rw-r--r--   0        0        0     1535 2023-04-17 13:47:47.336713 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/tag_protocols.smk
+-rw-r--r--   0        0        0     1758 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/update_repository.smk
+-rw-r--r--   0        0        0     4783 1970-01-01 00:00:00.000000 pyriksprot_tagger-2023.4.2/PKG-INFO
```

### Comparing `pyriksprot_tagger-2023.4.1/LICENSE` & `pyriksprot_tagger-2023.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.1/README.md` & `pyriksprot_tagger-2023.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.1/pyproject.toml` & `pyriksprot_tagger-2023.4.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [tool.poetry]
 name = "pyriksprot_tagger"
-version = "2023.4.1"
+version = "2023.4.2"
 description = "Pipeline that tags pyriksprot Parla-Clarin XML files"
 authors = ["Roger Mähler <roger.mahler@hotmail.com>"]
 packages = [
-    { include = "workflow" },
-    { include = "scripts" },
+    { include = "pyriksprot_tagger" },
 ]
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
     'Operating System :: OS Independent',
     'Topic :: Software Development',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
@@ -33,15 +32,15 @@
 loguru = "*"
 stanza = "*"
 # torch = "==1.11.0+cu113"
 
 # pip install torch==1.7.0 torchvision==0.8.1 -f https://download.pytorch.org/whl/cu101/torch_stable.html
 # beräkningsserver: pip install torch==1.11.0+cu113 torchvision==0.12.0+cu113 torchaudio==0.11.0+cu113 -f https://download.pytorch.org/whl/cu113/torch_stable.html
 poetry = "^1.4.2"
-pyriksprot = "^2023.4.1"
+pyriksprot = "^2023.4.2"
 
 [tool.poetry.dev-dependencies]
 black = "==20.*,>=20.8.0.b1"
 coverage = "==5.*,>=5.4.0"
 flake8 = "==3.*,>=3.8.4"
 flake8-black = "==0.*,>=0.2.1"
 isort = "==5.*,>=5.7.0"
@@ -58,15 +57,16 @@
 
 [tool.poe.tasks]
 portal1_torch = """
     pip install torch==1.11.0+cu113 torchvision==0.12.0+cu113 torchaudio==0.11.0+cu113 -f https://download.pytorch.org/whl/cu113/torch_stable.html
 """
 
 [tool.poetry.scripts]
-tag_info = "scripts.tag_info:main"
+tag_info = "pyriksprot_tagger.scripts.tag_info:main"
+pos_tag = "pyriksprot_tagger.scripts.tag:main"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = ["-rfE", "-q"]
 log_cli = "False"
 testpaths = ["tests"]
 python_files = "*_test.py"
@@ -117,16 +117,16 @@
     [tool.coverage.run]
         source = ["workflow"]
         branch = true
         data_file = "tests/coverage/data.bin"
         omit = [
             "**/__init__.py",
             "tests/*",
-            "workflow/Snakefile",
-            "workflow/rules/*.smk",
+            "pyriksprot_tagger/workflow/Snakefile",
+            "pyriksprot_tagger/workflow/rules/*.smk",
         ]
 
     [tool.coverage.report]
         exclude_lines = [
             "pragma: no cover",
             "def __repr__",
             "if TYPE_CHECKING:",
```

### Comparing `pyriksprot_tagger-2023.4.1/scripts/git-timesync` & `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/git-timesync`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.1/scripts/git_update_mtime.sh` & `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/git_update_mtime.sh`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.1/scripts/move_empty_files.sh` & `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/move_empty_files.sh`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.1/scripts/stanza-models.sh` & `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/stanza-models.sh`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.1/scripts/tag-it.sh` & `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/tag-it.sh`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.1/scripts/tag_info.py` & `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/tag_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Prints tag & commit info (SHA & tag) for a Git repository.
 
 """
 import click
-
 from pyriksprot.gitchen import GitInfo
 from pyriksprot.utility import write_yaml
 
 # pylint: disable=too-many-arguments, unused-argument
 
 
 @click.command()
@@ -20,12 +19,12 @@
     default=None,
 )
 def main(folder: str = None, tag: str = None, key: str = None):
     data: dict = GitInfo(folder).tag_info(source='workdir', tag=tag)
     if key:
         print(data.get(key, ""))
     else:
-        write_yaml(data=data,file="-")
+        write_yaml(data=data, file="-")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyriksprot_tagger-2023.4.1/workflow/Makefile` & `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/Makefile`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.1/workflow/Snakefile` & `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/Snakefile`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 
 
 PACKAGE_PATH = abspath(jj(dirname(realpath(workflow.snakefile)), ".."))
 
 if PACKAGE_PATH not in sys.path:
     sys.path.insert(0, PACKAGE_PATH)
 
-
-from workflow.config import Config
-from workflow.utility import sync_delta_names, expand_target_files, setup_logging
+from pyriksprot import sync_delta_names
+from pyriksprot_tagger import Config, expand_target_files, setup_logging
 
 
 setup_logging()
 
 if sys.platform not in ["win32"]:
     shell.prefix("set -o pipefail; ")
```

### Comparing `pyriksprot_tagger-2023.4.1/workflow/config.py` & `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,33 @@
+from __future__ import annotations
+
+import importlib
 import io
 import os
 import time
-from os.path import join as jj
+from dataclasses import dataclass, field
+from functools import cached_property
+from os.path import abspath, join, normpath
 from pathlib import Path
 
 import yaml
 from dotenv import load_dotenv
-from pyriksprot import norm_join as nj
+from pyriksprot import ITaggerFactory, dget
 
-from .utility import dget, sparv_datadir, stanza_dir
+from .utility import sparv_datadir, stanza_dir
 
 load_dotenv()
 
 # pylint: disable=too-many-arguments
 
 
+def nj(*paths) -> str | None:
+    return normpath(join(*paths)) if not None in paths else None
+
+
 class SafeLoaderIgnoreUnknown(yaml.SafeLoader):  # pylint: disable=too-many-ancestors
     def let_unknown_through(self, node):  # pylint: disable=unused-argument
         return None
 
 
 SafeLoaderIgnoreUnknown.add_constructor(None, SafeLoaderIgnoreUnknown.let_unknown_through)
 
@@ -33,66 +42,60 @@
             raise ValueError("Corpus tag cannot be empty")
 
         self.repository_folder: str = nj(repository_folder)
         self.repository_tag: str = repository_tag
         self.repository_url: str = self.REPOSITORY_URL
         self.extension: str = extension
 
-    def __repr__(self):
-        return f"{self.__class__.__name__}(repository_folder={self.repository_folder},repository_url={self.repository_url},repository_tag={self.repository_tag},folder={self.folder},extension={self.extension})"
-
     @property
     def folder(self) -> str:
-        return jj(self.repository_folder, "corpus/protocols")
+        return nj(self.repository_folder, "corpus/protocols")
 
     @property
     def parent_folder(self) -> str:
-        return os.path.abspath(nj(self.repository_folder, '..'))
+        return abspath(nj(self.repository_folder, '..'))
 
 
+@dataclass
 class TargetConfig:
-    def __init__(self, folder: str, extension: str = "xml"):
-        self.folder: str = nj(folder) if folder else None
-        self.extension: str = extension
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}(folder={self.folder},extension={self.extension})"
+    folder: str
+    extension: str = field(default="xml")
 
 
+@dataclass
 class DehyphenConfig:
-    def __init__(self, folder: str, tf_filename: str = None):
-        self.folder: str = folder
-        self.tf_filename: str = tf_filename or jj(folder, "riksdagen-corpus-term-frequencies.pkl")
+    folder: str
+    tf_filename: str
 
 
+@dataclass
 class ExtractConfig:
-    def __init__(self, folder: str, template: str = "", extension: str = "xml"):
-        self.folder: str = nj(folder) if folder else None
-        self.template: str = template
-        self.extension: str = extension
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}(folder={self.folder},template={self.template},extension={self.extension})"
+    folder: str
+    template: str = field(default="")
+    extension: str = field(default="xml")
 
 
 class Config:
     def __init__(
         self,
         data_folder: str,
         source_opts: SourceConfig = None,
         target_opts: TargetConfig = None,
         extract_opts: ExtractConfig = None,
         dehyphen_opts: DehyphenConfig = None,
+        tagger_module: str = None,
+        tagger_opts: dict = field(default_factory=dict),
     ):
         self.data_folder: str = nj(data_folder)
         self.source: SourceConfig = source_opts
         self.target: TargetConfig = target_opts
         self.extract: ExtractConfig = extract_opts
         self.dehyphen: DehyphenConfig = dehyphen_opts
-        self.log_basename: str = f'parla_clarin_{time.strftime("%Y%m%d%H%M")}.log'
+        self.tagger_module: str | None = tagger_module
+        self.tagger_opts: dict = tagger_opts or {}
 
     @staticmethod
     def load(source: str) -> "Config":
         """Load YAML configuration named `config_name` in resources folder. Return typed config."""
 
         if source is None:
             raise ValueError("Config source cannot be None")
@@ -107,44 +110,60 @@
         )
 
         data_folder: str = dget(data, "data_folder", "root_folder")
 
         return Config(
             data_folder=data_folder,
             target_opts=TargetConfig(
-                folder=dget(data, "target_folder", "target.folder"),
+                folder=nj(dget(data, "target_folder", "target.folder")),
                 extension=dget(data, "target_extension", "target.extension", default="zip"),
             ),
             source_opts=SourceConfig(
                 repository_folder=dget(
-                    data, "repository.folder", "repository_folder", default=jj(data_folder, "riksdagen-corpus")
+                    data, "repository.folder", "repository_folder", default=nj(data_folder, "riksdagen-corpus")
                 ),
                 repository_tag=dget(
                     data, "tag", "repository.tag", "repository_tag", default=os.environ.get("RIKSPROT_REPOSITORY_TAG")
                 ),
             ),
             extract_opts=ExtractConfig(
-                folder=dget(data, "export.folder", "export_folder"),
+                folder=nj(dget(data, "export.folder", "export_folder")),
                 template=dget(data, "export.template", "export_template"),
                 extension=dget(data, "export.extension", "export_extension"),
             ),
             dehyphen_opts=DehyphenConfig(
-                folder=dget(data, "dehyphen_folder", "dehypen.folder", default=data_folder),
-                tf_filename=dget(data, "tf_filename", "dehyphen.tf_filename", default=None),
+                folder=dget(data, "dehyphen_folder", "dehyphen.folder", default=data_folder),
+                tf_filename=dget(
+                    data, "tf_filename", "dehyphen.tf_filename", default=nj(data_folder, "word-frequencies.pkl")
+                ),
             ),
+            tagger_module=dget(data, "tagger_module"),
+            tagger_opts=dget(data, "tagger_opts")
+            if "tagger_opts" in data
+            else {k.lstrip("tagger_"): v for k, v in data.items() if k.startswith("tagger_") and k != "tegger_module"},
         )
 
-    @property
+    @cached_property
     def stanza_dir(self):
         return stanza_dir(self.data_folder)
 
-    @property
+    @cached_property
     def sparv_datadir(self):
         return sparv_datadir(self.data_folder)
 
-    @property
+    @cached_property
     def log_folder(self):
-        return jj(self.data_folder, "logs")
+        return nj(self.data_folder, "logs")
 
-    @property
+    @cached_property
     def log_filename(self):
-        return jj(self.log_folder, self.log_basename)
+        return nj(self.log_folder, f'parla_clarin_{time.strftime("%Y%m%d%H%M")}.log')
+
+    @cached_property
+    def tagger_factory(self) -> ITaggerFactory:
+        if self.tagger_module is None:
+            return None
+        tagger_module = importlib.import_module(self.tagger_module)
+        abstract_factory = getattr(tagger_module, "tagger_factory")
+        if abstract_factory is None:
+            raise ValueError(f"Module {self.tagger_module} does not implement `tagger_factory`.")
+        return abstract_factory(self)
```

### Comparing `pyriksprot_tagger-2023.4.1/workflow/rules/compute_frequency.smk` & `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/compute_frequency.smk`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.1/workflow/rules/extract_speeches.smk` & `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/extract_speeches.smk`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.1/workflow/rules/tag_protocols.smk` & `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/tag_protocols.smk`

 * *Files 11% similar despite different names*

```diff
@@ -5,27 +5,32 @@
 PoS tags Parla-CLARIN XML files using Stanza.
 """
 from os import makedirs
 from os.path import join as jj
 
 from pyriksprot import tag_protocol_xml
 
-from workflow.config import Config
-from workflow.taggers import TaggerRegistry
-from workflow.utility import check_cuda
+from pyriksprot import TaggerRegistry
+from pyriksprot_tagger import StanzaTaggerFactory, check_cuda, Config
 
 typed_config: Config = typed_config
 disable_gpu: bool = config.get("disable_gpu", 0) == 1
 
 check_cuda()
 
 makedirs(typed_config.target.folder, exist_ok=True)
 
+def create_factory():
+    typed_config.tagger_opts['use_gpu'] = not disable_gpu
+    return typed_config.tagger_factory.create()
+
 def tagger():
-    return TaggerRegistry.stanza(typed_config, disable_gpu=disable_gpu)
+    if StanzaTaggerFactory.identifier in TaggerRegistry.instances:
+        return TaggerRegistry.instances[StanzaTaggerFactory.identifier]
+    return TaggerRegistry.get(create_factory())
 
 rule tag_protocols:
     message:
         "step: tag_protocols"
     params:
         template=typed_config.extract.template,
     # threads: workflow.cores * 0.75
```

### Comparing `pyriksprot_tagger-2023.4.1/workflow/rules/update_repository.smk` & `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/update_repository.smk`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.1/workflow/taggers/spacy2.py` & `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/taggers/spacy2.py`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.1/PKG-INFO` & `pyriksprot_tagger-2023.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriksprot-tagger
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: Pipeline that tags pyriksprot Parla-Clarin XML files
 Home-page: https://westac.se
 License: Apache-2.0
 Author: Roger Mähler
 Author-email: roger.mahler@hotmail.com
 Requires-Python: >=3.11.0,<3.12.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,15 +18,15 @@
 Requires-Dist: click
 Requires-Dist: cookiecutter
 Requires-Dist: dehyphen
 Requires-Dist: loguru
 Requires-Dist: pandas
 Requires-Dist: poetry (>=1.4.2,<2.0.0)
 Requires-Dist: pygit2
-Requires-Dist: pyriksprot (>=2023.4.1,<2024.0.0)
+Requires-Dist: pyriksprot (>=2023.4.2,<2024.0.0)
 Requires-Dist: snakefmt
 Requires-Dist: snakemake
 Requires-Dist: stanza
 Project-URL: Repository, https://github.com/welfare-state-analytics/pyriksprot_tagger
 Description-Content-Type: text/markdown
 
 # Riksdagens Protokoll Part-Of-Speech Tagging
```

