# Comparing `tmp/theforensicator-0.1.5.tar.gz` & `tmp/theforensicator-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theforensicator-0.1.5.tar", max compression
+gzip compressed data, was "theforensicator-0.1.6.tar", max compression
```

## Comparing `theforensicator-0.1.5.tar` & `theforensicator-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2023-04-15 16:44:34.747566 theforensicator-0.1.5/LICENSE
--rw-r--r--   0        0        0     1091 2023-04-15 16:44:34.747566 theforensicator-0.1.5/README.md
--rw-r--r--   0        0        0     3100 2023-04-15 16:44:34.747566 theforensicator-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       45 2023-04-15 16:44:34.747566 theforensicator-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      586 2023-04-15 16:44:34.747566 theforensicator-0.1.5/tests/test_app.py
--rw-r--r--   0        0        0      145 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/__init__.py
--rw-r--r--   0        0        0     4939 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/app.py
--rw-r--r--   0        0        0      473 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/browser_chrome.yaml
--rw-r--r--   0        0        0      116 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/browser_edge.yaml
--rw-r--r--   0        0        0      668 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/browser_firefox.yaml
--rw-r--r--   0        0        0      467 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/browser_ie.yaml
--rw-r--r--   0        0        0      170 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/events_logs.yaml
--rw-r--r--   0        0        0       97 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/prefetch.yaml
--rw-r--r--   0        0        0      366 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/registry_system.yaml
--rw-r--r--   0        0        0      129 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/artefacts/registry_user.yaml
--rw-r--r--   0        0        0     2156 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/cli.py
--rw-r--r--   0        0        0       30 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/ewf/__init__.py
--rw-r--r--   0        0        0    19995 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/ewf/file_parsing.py
--rw-r--r--   0        0        0       65 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/fs/__init__.py
--rw-r--r--   0        0        0    12818 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/fs/defs.py
--rw-r--r--   0        0        0     4929 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/fs/gpt.py
--rw-r--r--   0        0        0     3421 2023-04-15 16:44:34.747566 theforensicator-0.1.5/theforensicator/fs/mbr.py
--rw-r--r--   0        0        0    35265 2023-04-15 16:44:34.751566 theforensicator-0.1.5/theforensicator/fs/ntfs.py
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 theforensicator-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-17 11:56:46.706176 theforensicator-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1091 2023-04-17 11:56:46.706176 theforensicator-0.1.6/README.md
+-rw-r--r--   0        0        0     3072 2023-04-17 11:56:46.706176 theforensicator-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-04-17 11:56:46.706176 theforensicator-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0      586 2023-04-17 11:56:46.706176 theforensicator-0.1.6/tests/test_app.py
+-rw-r--r--   0        0        0      145 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/__init__.py
+-rw-r--r--   0        0        0     4939 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/app.py
+-rw-r--r--   0        0        0      473 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/artefacts/browser_chrome.yaml
+-rw-r--r--   0        0        0      116 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/artefacts/browser_edge.yaml
+-rw-r--r--   0        0        0      668 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/artefacts/browser_firefox.yaml
+-rw-r--r--   0        0        0      467 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/artefacts/browser_ie.yaml
+-rw-r--r--   0        0        0      170 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/artefacts/events_logs.yaml
+-rw-r--r--   0        0        0       97 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/artefacts/prefetch.yaml
+-rw-r--r--   0        0        0      331 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/artefacts/registry_system.yaml
+-rw-r--r--   0        0        0      129 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/artefacts/registry_user.yaml
+-rw-r--r--   0        0        0     2158 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/cli.py
+-rw-r--r--   0        0        0       30 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/ewf/__init__.py
+-rw-r--r--   0        0        0    19995 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/ewf/file_parsing.py
+-rw-r--r--   0        0        0       65 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/fs/__init__.py
+-rw-r--r--   0        0        0    12818 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/fs/defs.py
+-rw-r--r--   0        0        0     4929 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/fs/gpt.py
+-rw-r--r--   0        0        0     3421 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/fs/mbr.py
+-rw-r--r--   0        0        0    35792 2023-04-17 11:56:46.706176 theforensicator-0.1.6/theforensicator/fs/ntfs.py
+-rw-r--r--   0        0        0     3485 1970-01-01 00:00:00.000000 theforensicator-0.1.6/PKG-INFO
```

### Comparing `theforensicator-0.1.5/LICENSE` & `theforensicator-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.5/README.md` & `theforensicator-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.5/pyproject.toml` & `theforensicator-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "theforensicator"
-version = "0.1.5"
+version = "0.1.6"
 homepage = "https://github.com/ValekoZ/theforensicator"
 description = "School project for forensic investigations."
 authors = [
     "Joël RABAH <joel.rabah@ecole2600.com>",
     "Edouard GOUT <edouard.gout@ecole2600.com>",
     "Yann MAJEROWICZ <yann.majerowicz@ecole2600.com>",
     "Bastien WINTER DURENNEL <bastien.winter-durennel@ecole2600.com>",
@@ -51,15 +51,14 @@
 twine  = { version = "^3.8.0", optional = true}
 mkdocs-autorefs = {version = "^0.3.1", optional = true}
 pre-commit = {version = "^2.17.0", optional = true}
 toml = {version = "^0.10.2", optional = true}
 livereload = {version = "^2.6.3", optional = true}
 pyreadline = {version = "^2.1", optional = true}
 mike = { version="^1.1.2", optional=true}
-pyreadpartitions = "^1.1.1"
 setuptools = {version = "^67.6.1", optional = true}
 pyyaml = "^6.0"
 
 [tool.poetry.extras]
 test = [
     "pytest",
     "black",
```

### Comparing `theforensicator-0.1.5/tests/test_app.py` & `theforensicator-0.1.6/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.5/theforensicator/app.py` & `theforensicator-0.1.6/theforensicator/app.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.5/theforensicator/artefacts/browser_firefox.yaml` & `theforensicator-0.1.6/theforensicator/artefacts/browser_firefox.yaml`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.5/theforensicator/cli.py` & `theforensicator-0.1.6/theforensicator/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from os.path import dirname, normpath, isfile, exists
 
 from pathlib import Path
 
 import yaml
 import glob
 
-def cmd(ewf_file: str, dump_dir: str = None, resolve_mft_file: str = None, dmp_file: str = None, clear_cache: str = None, extract_artefacts: str = None):
+def cmd(ewf_file: str, dump_dir: str = None, resolve_mft_file: str = None, dmp_file: str = None, clear_cache: str = None, extract_artefacts: bool = False):
     """Parses a EWF file and dump interesting files found in the windows file
     system
 
     Args:
         ewf_file: File that will be analysed (*.E01)
         dump_dir: Directory location to store dumped data (default location is current execution directory)
         resolve_mft_file: Output file where to store MFT files / directories in JSON format.
```

### Comparing `theforensicator-0.1.5/theforensicator/ewf/file_parsing.py` & `theforensicator-0.1.6/theforensicator/ewf/file_parsing.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.5/theforensicator/fs/defs.py` & `theforensicator-0.1.6/theforensicator/fs/defs.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.5/theforensicator/fs/gpt.py` & `theforensicator-0.1.6/theforensicator/fs/gpt.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.5/theforensicator/fs/mbr.py` & `theforensicator-0.1.6/theforensicator/fs/mbr.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.5/theforensicator/fs/ntfs.py` & `theforensicator-0.1.6/theforensicator/fs/ntfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,14 +257,15 @@
         """Analyze the NTFS header
 
         Args:
             out_file: Where to store the output
             dump_file: Where the output has been stored in a previous run
             resolve_mft_file: Where the resolved MFT in JSON format will be stored
         """
+        self.partition_idx = partition_idx
         mft_dump_filepath = f"MFT{partition_idx}.dump"
 
         if clear_cache:
             if isfile(mft_dump_filepath):
                 unlink(mft_dump_filepath)
                 print("[+] Cache cleared.")
 
@@ -287,19 +288,24 @@
 
     def _get_dump_mft_entry(self, idx: int):
         """Get a dump of the given mft entry
 
         Args:
             Index of the MFT entry to dump
         """
-        return (
-            self.dump_mft["mft"][str(idx)]
-            if self.is_mft_dump
-            else self.dump_mft["mft"][idx]
-        )
+        if self.is_mft_dump:
+            try:
+                return self.dump_mft["mft"][str(idx)]
+            except:
+                return None
+        
+        try:
+            return self.dump_mft["mft"][idx]
+        except:
+            return None
 
     def _resolve_path(self, mft_entry) -> list:
         """Resolve the path of the given mft entry
 
         Args:
             mft_entry: MFT entry to resolve
 
@@ -313,14 +319,17 @@
             path = ""
             parent_dir = mft_entry["parent_directory"]
             path += mft_entry["directory_name"]
 
             while parent_dir != FILE_root:
                 next_entry = self._get_dump_mft_entry(parent_dir)
 
+                if next_entry is None:
+                    break
+
                 if next_entry["is_directory"]:
                     parent_dir = next_entry["parent_directory"]
                     path = f'{next_entry["directory_name"]}\\{path}'
                 else:
                     return [{"type": "ORPHAN_DIRECTORY", "directory_name": path}]
 
             path = "C:\\" + path
@@ -328,23 +337,32 @@
             paths.append({"type": "DIRECTORY", "directory_name": path})
         else:
             for file in mft_entry["files"]:
                 path = ""
                 parent_dir = file["parent_directory"]
                 path += file["file_name"]
 
+                is_valid = True
+
                 while parent_dir != FILE_root:
                     next_entry = self._get_dump_mft_entry(parent_dir)
 
+                    if next_entry is None:
+                        is_valid = False
+                        break
+
                     if next_entry["is_directory"]:
                         parent_dir = next_entry["parent_directory"]
                         path = f'{next_entry["directory_name"]}\\{path}'
                     else:
                         return [{"type": "ORPHAN_FILE", "file_name": path}]
 
+                if not is_valid:
+                    continue
+
                 path = "C:\\" + path
 
                 paths.append({"type": "FILE", "file_name": path})
 
         return paths
 
     def resolve_mft(self, json_outfile: str):
@@ -386,15 +404,15 @@
                         "dates": entry["dates"],
                         "data": data,
                     }
 
         print("[+] MFT paths resolved ...")
 
         if json_outfile and type(json_outfile) is str:
-            with open(json_outfile, "w") as dmp:
+            with open(f"{json_outfile}.{self.partition_idx}", "w") as dmp:
                 dmp.write(json.dumps(self.resolved_mft))
                 dmp.close()
             print("[+] %s successfully written." % (json_outfile))
 
     def analyze_mft(self, out_file: str):
         """Analyze the MFT
 
@@ -835,20 +853,22 @@
             size_lcn_offset = run_header >> 4
 
             # print(current_datarun)
 
             lcn_length = unpack(
                 "<Q", current_datarun[1 : 1 + size_lcn_nb].ljust(8, b"\0")
             )[0]
-            lcn_offset = unpack(
-                "<Q",
-                current_datarun[
-                    1 + size_lcn_nb : 1 + size_lcn_nb + size_lcn_offset
-                ].ljust(8, b"\0"),
-            )[0]
+            
+            if lcn_length != 0x0:
+                lcn_offset = unpack(
+                    "<Q",
+                    current_datarun[
+                        1 + size_lcn_nb : 1 + size_lcn_nb + size_lcn_offset
+                    ].ljust(8, b"\0"),
+                )[0]
 
             # if it's a sparse file we continue to the next
             # run because we don't care of this data.
             if lcn_length == 0x0:
                 pass
                 # print("sparse file")
             else:
```

### Comparing `theforensicator-0.1.5/PKG-INFO` & `theforensicator-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theforensicator
-Version: 0.1.5
+Version: 0.1.6
 Summary: School project for forensic investigations.
 Home-page: https://github.com/ValekoZ/theforensicator
 License: MIT
 Author: Joël RABAH
 Author-email: joel.rabah@ecole2600.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -36,15 +36,14 @@
 Requires-Dist: mkdocs-include-markdown-plugin (>=3.2.3,<4.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material (>=8.1.11,<9.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0)
 Requires-Dist: mkdocstrings (>=0.18.0,<0.19.0) ; extra == "doc"
 Requires-Dist: pip (>=22.0.3,<23.0.0) ; extra == "dev"
 Requires-Dist: pre-commit (>=2.17.0,<3.0.0) ; extra == "dev"
 Requires-Dist: pyreadline (>=2.1,<3.0)
-Requires-Dist: pyreadpartitions (>=1.1.1,<2.0.0)
 Requires-Dist: pytest (>=7.0.1,<8.0.0) ; extra == "test"
 Requires-Dist: pytest-cov (>=3.0.0,<4.0.0) ; extra == "test"
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: setuptools (>=67.6.1,<68.0.0) ; extra == "doc"
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
 Requires-Dist: tox (>=3.24.5,<4.0.0) ; extra == "dev"
 Requires-Dist: twine (>=3.8.0,<4.0.0) ; extra == "dev"
```

