# Comparing `tmp/lupin-danquin-1.0.2.dev2.tar.gz` & `tmp/lupin-danquin-1.0.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-danquin-1.0.2.dev2.tar", last modified: Mon Apr 17 13:46:48 2023, max compression
+gzip compressed data, was "lupin-danquin-1.0.2.dev4.tar", last modified: Mon Apr 17 15:44:42 2023, max compression
```

## Comparing `lupin-danquin-1.0.2.dev2.tar` & `lupin-danquin-1.0.2.dev4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 13:46:48.609414 lupin-danquin-1.0.2.dev2/
--rw-rw-rw-   0        0        0     1093 2023-04-11 13:56:08.000000 lupin-danquin-1.0.2.dev2/LICENCE
--rw-rw-rw-   0        0        0       67 2023-04-12 12:24:19.000000 lupin-danquin-1.0.2.dev2/MANIFEST.in
--rw-rw-rw-   0        0        0      573 2023-04-17 13:46:48.609414 lupin-danquin-1.0.2.dev2/PKG-INFO
--rw-rw-rw-   0        0        0     1809 2023-04-12 12:25:35.000000 lupin-danquin-1.0.2.dev2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 13:46:48.579342 lupin-danquin-1.0.2.dev2/lupin_danquin/
--rw-rw-rw-   0        0        0       28 2023-04-17 13:46:48.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/__init__.py
--rw-rw-rw-   0        0        0       78 2023-04-12 12:24:19.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:46:48.602901 lupin-danquin-1.0.2.dev2/lupin_danquin/core/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/core/__init__.py
--rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/core/application.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:46:48.603901 lupin-danquin-1.0.2.dev2/lupin_danquin/core/coding_rules_validator/
--rw-rw-rw-   0        0        0        0 2023-04-12 15:23:46.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/core/coding_rules_validator/__init__.py
--rw-rw-rw-   0        0        0     1390 2023-04-14 13:06:50.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/core/coding_rules_validator/coging_rules_validator.py
--rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/core/global_variable.py
--rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/core/line_ended.py
--rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/core/local_variable.py
--rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/core/parameter.py
--rw-rw-rw-   0        0        0     4619 2023-04-11 13:55:43.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/core/program.py
--rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/core/rules.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:46:48.606414 lupin-danquin-1.0.2.dev2/lupin_danquin/core/tools/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/core/tools/__init__.py
--rw-rw-rw-   0        0        0     2203 2023-04-17 13:46:10.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/core/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:46:48.607414 lupin-danquin-1.0.2.dev2/lupin_danquin/core/val3_doc_generator/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/core/val3_doc_generator/__init__.py
--rw-rw-rw-   0        0        0     2657 2023-04-12 15:23:46.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
--rw-rw-rw-   0        0        0     3117 2023-04-17 13:46:24.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/run.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:46:48.608414 lupin-danquin-1.0.2.dev2/lupin_danquin/templates/
--rw-rw-rw-   0        0        0     2801 2023-04-12 12:24:19.000000 lupin-danquin-1.0.2.dev2/lupin_danquin/templates/val3_documentation_md.j2
-drwxrwxrwx   0        0        0        0 2023-04-17 13:46:48.595420 lupin-danquin-1.0.2.dev2/lupin_danquin.egg-info/
--rw-rw-rw-   0        0        0      573 2023-04-17 13:46:48.000000 lupin-danquin-1.0.2.dev2/lupin_danquin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      996 2023-04-17 13:46:48.000000 lupin-danquin-1.0.2.dev2/lupin_danquin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 13:46:48.000000 lupin-danquin-1.0.2.dev2/lupin_danquin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-17 13:46:48.000000 lupin-danquin-1.0.2.dev2/lupin_danquin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 14:28:43.000000 lupin-danquin-1.0.2.dev2/lupin_danquin.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       90 2023-04-17 13:46:48.000000 lupin-danquin-1.0.2.dev2/lupin_danquin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-17 13:46:48.000000 lupin-danquin-1.0.2.dev2/lupin_danquin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      906 2023-04-17 13:46:48.614414 lupin-danquin-1.0.2.dev2/setup.cfg
--rw-rw-rw-   0        0        0      178 2023-04-11 14:20:31.000000 lupin-danquin-1.0.2.dev2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:44:42.126299 lupin-danquin-1.0.2.dev4/
+-rw-rw-rw-   0        0        0     1093 2023-04-11 13:56:08.000000 lupin-danquin-1.0.2.dev4/LICENCE
+-rw-rw-rw-   0        0        0       67 2023-04-12 12:24:19.000000 lupin-danquin-1.0.2.dev4/MANIFEST.in
+-rw-rw-rw-   0        0        0      573 2023-04-17 15:44:42.126299 lupin-danquin-1.0.2.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0     1809 2023-04-12 12:25:35.000000 lupin-danquin-1.0.2.dev4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 15:44:42.096258 lupin-danquin-1.0.2.dev4/lupin_danquin/
+-rw-rw-rw-   0        0        0       28 2023-04-17 15:44:42.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/__init__.py
+-rw-rw-rw-   0        0        0       78 2023-04-12 12:24:19.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:44:42.120790 lupin-danquin-1.0.2.dev4/lupin_danquin/core/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/core/__init__.py
+-rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/core/application.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:44:42.121791 lupin-danquin-1.0.2.dev4/lupin_danquin/core/coding_rules_validator/
+-rw-rw-rw-   0        0        0        0 2023-04-12 15:23:46.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/core/coding_rules_validator/__init__.py
+-rw-rw-rw-   0        0        0     1390 2023-04-14 13:06:50.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/core/coding_rules_validator/coging_rules_validator.py
+-rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/core/global_variable.py
+-rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/core/line_ended.py
+-rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/core/local_variable.py
+-rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/core/parameter.py
+-rw-rw-rw-   0        0        0     4619 2023-04-11 13:55:43.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/core/program.py
+-rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/core/rules.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:44:42.123790 lupin-danquin-1.0.2.dev4/lupin_danquin/core/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/core/tools/__init__.py
+-rw-rw-rw-   0        0        0     2008 2023-04-17 15:40:02.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/core/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:44:42.124791 lupin-danquin-1.0.2.dev4/lupin_danquin/core/val3_doc_generator/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/core/val3_doc_generator/__init__.py
+-rw-rw-rw-   0        0        0     2657 2023-04-12 15:23:46.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
+-rw-rw-rw-   0        0        0     3093 2023-04-17 15:41:36.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/run.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:44:42.124791 lupin-danquin-1.0.2.dev4/lupin_danquin/templates/
+-rw-rw-rw-   0        0        0     2801 2023-04-12 12:24:19.000000 lupin-danquin-1.0.2.dev4/lupin_danquin/templates/val3_documentation_md.j2
+drwxrwxrwx   0        0        0        0 2023-04-17 15:44:42.113275 lupin-danquin-1.0.2.dev4/lupin_danquin.egg-info/
+-rw-rw-rw-   0        0        0      573 2023-04-17 15:44:42.000000 lupin-danquin-1.0.2.dev4/lupin_danquin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      996 2023-04-17 15:44:42.000000 lupin-danquin-1.0.2.dev4/lupin_danquin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 15:44:42.000000 lupin-danquin-1.0.2.dev4/lupin_danquin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-17 15:44:42.000000 lupin-danquin-1.0.2.dev4/lupin_danquin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 14:28:43.000000 lupin-danquin-1.0.2.dev4/lupin_danquin.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       90 2023-04-17 15:44:42.000000 lupin-danquin-1.0.2.dev4/lupin_danquin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-17 15:44:42.000000 lupin-danquin-1.0.2.dev4/lupin_danquin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      906 2023-04-17 15:44:42.131306 lupin-danquin-1.0.2.dev4/setup.cfg
+-rw-rw-rw-   0        0        0      178 2023-04-17 15:42:06.000000 lupin-danquin-1.0.2.dev4/setup.py
```

### Comparing `lupin-danquin-1.0.2.dev2/LICENCE` & `lupin-danquin-1.0.2.dev4/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-danquin-1.0.2.dev2/PKG-INFO` & `lupin-danquin-1.0.2.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 1.0.2.dev2
+Version: 1.0.2.dev4
 Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
```

### Comparing `lupin-danquin-1.0.2.dev2/README.md` & `lupin-danquin-1.0.2.dev4/README.md`

 * *Files identical despite different names*

### Comparing `lupin-danquin-1.0.2.dev2/lupin_danquin/core/application.py` & `lupin-danquin-1.0.2.dev4/lupin_danquin/core/application.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-1.0.2.dev2/lupin_danquin/core/coding_rules_validator/coging_rules_validator.py` & `lupin-danquin-1.0.2.dev4/lupin_danquin/core/coding_rules_validator/coging_rules_validator.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-1.0.2.dev2/lupin_danquin/core/global_variable.py` & `lupin-danquin-1.0.2.dev4/lupin_danquin/core/global_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-1.0.2.dev2/lupin_danquin/core/local_variable.py` & `lupin-danquin-1.0.2.dev4/lupin_danquin/core/local_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-1.0.2.dev2/lupin_danquin/core/parameter.py` & `lupin-danquin-1.0.2.dev4/lupin_danquin/core/parameter.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-1.0.2.dev2/lupin_danquin/core/program.py` & `lupin-danquin-1.0.2.dev4/lupin_danquin/core/program.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-1.0.2.dev2/lupin_danquin/core/tools/utils.py` & `lupin-danquin-1.0.2.dev4/lupin_danquin/core/tools/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -68,15 +68,7 @@
 
 def find_usrapp_dir() -> str:
     """Find the usrapp directory"""
     for dirpath, dirnames, filenames in os.walk(os.getcwd()):
         if "usrapp" in dirnames:
             return os.path.join(dirpath, "usrapp")
     die(msg="'usrapp' directory not found")
-
-
-def load_env_file():
-    dotenv_path = os.path.join(os.getcwd(), ".env")
-    if os.path.exists(dotenv_path):
-        return dotenv_path
-    else:
-        die(msg=".env file not found")
```

### Comparing `lupin-danquin-1.0.2.dev2/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py` & `lupin-danquin-1.0.2.dev4/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-1.0.2.dev2/lupin_danquin/run.py` & `lupin-danquin-1.0.2.dev4/lupin_danquin/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from typing import Optional
+import os
 
-from dotenv import load_dotenv
+from dotenv import load_dotenv, find_dotenv
 import typer
 
 from lupin_danquin.core.tools.utils import (
     configure_logging,
     convert_application_name_to_list,
-    load_env_file,
     read_file,
 )
 
 from lupin_danquin.core.coding_rules_validator.coging_rules_validator import (
     CodingRulesValidator,
 )
 from lupin_danquin.core.val3_doc_generator.val3_doc_generator import Val3Documentation
 from lupin_danquin import __version__
 
 
-env_file = load_env_file()
-load_dotenv(dotenv_path=env_file)
-
 configure_logging()
+load_dotenv(find_dotenv(usecwd=True))
 
 cli = typer.Typer()
 
 
 @cli.command(help="Print version")
 def version():
     print(f"Version: {__version__}")
@@ -61,15 +59,14 @@
     :param beginning_file_path: Path to the file containing the beginning content of the documentation
     :type beginning_file_path: str
     :param end_file_path: Path to the file containing the end content of the documentation
     :type end_file_path: str
     :example: danq valdocs "App1,App2" --beginning-file-path "beginning.txt" --end-file-path "end.txt"
     or danq valdocs "App1,App2" -b "beginning.txt" -e "end.txt"
     """
-
     applications_list = convert_application_name_to_list(application_names)
 
     if not beginning_file_path:
         begining_of_file = ""
     else:
         begining_of_file = read_file(beginning_file_path)
     if not end_file_path:
```

### Comparing `lupin-danquin-1.0.2.dev2/lupin_danquin/templates/val3_documentation_md.j2` & `lupin-danquin-1.0.2.dev4/lupin_danquin/templates/val3_documentation_md.j2`

 * *Files identical despite different names*

### Comparing `lupin-danquin-1.0.2.dev2/lupin_danquin.egg-info/PKG-INFO` & `lupin-danquin-1.0.2.dev4/lupin_danquin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 1.0.2.dev2
+Version: 1.0.2.dev4
 Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
```

### Comparing `lupin-danquin-1.0.2.dev2/lupin_danquin.egg-info/SOURCES.txt` & `lupin-danquin-1.0.2.dev4/lupin_danquin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lupin-danquin-1.0.2.dev2/setup.cfg` & `lupin-danquin-1.0.2.dev4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7570 696e 2d64 616e 7175 696e   = lupin-danquin
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 302e  ..version = 1.0.
-00000030: 322e 6465 7632 0d0a 6465 7363 7269 7074  2.dev2..descript
+00000030: 322e 6465 7634 0d0a 6465 7363 7269 7074  2.dev4..descript
 00000040: 696f 6e20 3d20 5465 7374 696e 6720 2d20  ion = Testing - 
 00000050: 446f 6375 6d65 6e74 6174 696f 6e0d 0a6c  Documentation..l
 00000060: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000070: 3d20 5465 7374 2056 414c 3320 636f 6465  = Test VAL3 code
 00000080: 2061 6e64 2067 656e 6572 6174 6520 646f   and generate do
 00000090: 6375 6d65 6e74 6174 696f 6e20 6672 6f6d  cumentation from
 000000a0: 2069 740d 0a6b 6579 776f 7264 7320 3d20   it..keywords =
```

