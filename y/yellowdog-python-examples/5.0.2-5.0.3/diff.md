# Comparing `tmp/yellowdog-python-examples-5.0.2.tar.gz` & `tmp/yellowdog-python-examples-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowdog-python-examples-5.0.2.tar", last modified: Fri Apr 14 14:21:00 2023, max compression
+gzip compressed data, was "yellowdog-python-examples-5.0.3.tar", last modified: Mon Apr 17 15:01:32 2023, max compression
```

## Comparing `yellowdog-python-examples-5.0.2.tar` & `yellowdog-python-examples-5.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-14 14:21:00.040494 yellowdog-python-examples-5.0.2/
--rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-5.0.2/LICENSE
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-04-14 14:21:00.040572 yellowdog-python-examples-5.0.2/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-5.0.2/PYPI_README.md
--rw-r--r--   0 pwt        (501) staff       (20)   109044 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.2/README.md
--rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.2/pyproject.toml
--rw-r--r--   0 pwt        (501) staff       (20)       46 2023-03-31 14:34:07.000000 yellowdog-python-examples-5.0.2/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-04-14 14:21:00.040868 yellowdog-python-examples-5.0.2/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.2/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-14 14:21:00.033852 yellowdog-python-examples-5.0.2/yd_commands/
--rw-r--r--   0 pwt        (501) staff       (20)       22 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.2/yd_commands/__init__.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3378 2023-03-28 12:34:54.000000 yellowdog-python-examples-5.0.2/yd_commands/abort.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-5.0.2/yd_commands/admin.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    17864 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.2/yd_commands/args.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     5077 2023-02-22 19:37:56.000000 yellowdog-python-examples-5.0.2/yd_commands/cancel.py
--rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-5.0.2/yd_commands/check_imports.py
--rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-5.0.2/yd_commands/compact_json.py
--rw-r--r--   0 pwt        (501) staff       (20)    18238 2023-03-31 13:51:41.000000 yellowdog-python-examples-5.0.2/yd_commands/config.py
--rw-r--r--   0 pwt        (501) staff       (20)     5474 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.2/yd_commands/config_keys.py
--rw-r--r--   0 pwt        (501) staff       (20)    12183 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.2/yd_commands/csv_data.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1647 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.2/yd_commands/delete.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3616 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.2/yd_commands/download.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     9203 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.2/yd_commands/instantiate.py
--rw-r--r--   0 pwt        (501) staff       (20)     3749 2022-12-01 11:00:21.000000 yellowdog-python-examples-5.0.2/yd_commands/interactive.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.2/yd_commands/jsonnet2json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     7539 2023-03-02 09:05:10.000000 yellowdog-python-examples-5.0.2/yd_commands/list.py
--rw-r--r--   0 pwt        (501) staff       (20)     3012 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.2/yd_commands/object_utilities.py
--rw-r--r--   0 pwt        (501) staff       (20)     9590 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.2/yd_commands/printing.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    16885 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.2/yd_commands/provision.py
--rw-r--r--   0 pwt        (501) staff       (20)      789 2023-03-13 13:46:12.000000 yellowdog-python-examples-5.0.2/yd_commands/provision_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.2/yd_commands/reformat_json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3231 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.2/yd_commands/shutdown.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    39150 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.2/yd_commands/submit.py
--rw-r--r--   0 pwt        (501) staff       (20)     6051 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.2/yd_commands/submit_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2756 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.2/yd_commands/terminate.py
--rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-5.0.2/yd_commands/type_check.py
--rw-r--r--   0 pwt        (501) staff       (20)     2252 2023-03-15 09:01:37.000000 yellowdog-python-examples-5.0.2/yd_commands/upload.py
--rw-r--r--   0 pwt        (501) staff       (20)     3389 2023-03-14 20:22:33.000000 yellowdog-python-examples-5.0.2/yd_commands/upload_utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     1630 2023-03-02 09:05:10.000000 yellowdog-python-examples-5.0.2/yd_commands/validate_properties.py
--rw-r--r--   0 pwt        (501) staff       (20)    10735 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.2/yd_commands/variables.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-5.0.2/yd_commands/version.py
--rw-r--r--   0 pwt        (501) staff       (20)     2200 2023-02-04 22:01:25.000000 yellowdog-python-examples-5.0.2/yd_commands/wrapper.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-14 14:21:00.040384 yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-04-14 14:21:00.000000 yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-04-14 14:21:00.000000 yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2023-04-14 14:21:00.000000 yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      574 2023-04-14 14:21:00.000000 yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)       61 2023-04-14 14:21:00.000000 yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)       12 2023-04-14 14:21:00.000000 yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-17 15:01:32.908262 yellowdog-python-examples-5.0.3/
+-rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-5.0.3/LICENSE
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-04-17 15:01:32.908331 yellowdog-python-examples-5.0.3/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-5.0.3/PYPI_README.md
+-rw-r--r--   0 pwt        (501) staff       (20)   109332 2023-04-17 15:00:55.000000 yellowdog-python-examples-5.0.3/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.3/pyproject.toml
+-rw-r--r--   0 pwt        (501) staff       (20)       46 2023-03-31 14:34:07.000000 yellowdog-python-examples-5.0.3/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-04-17 15:01:32.908630 yellowdog-python-examples-5.0.3/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.3/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-17 15:01:32.907327 yellowdog-python-examples-5.0.3/yd_commands/
+-rw-r--r--   0 pwt        (501) staff       (20)       22 2023-04-17 15:00:55.000000 yellowdog-python-examples-5.0.3/yd_commands/__init__.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3378 2023-03-28 12:34:54.000000 yellowdog-python-examples-5.0.3/yd_commands/abort.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-5.0.3/yd_commands/admin.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    17864 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.3/yd_commands/args.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     5077 2023-02-22 19:37:56.000000 yellowdog-python-examples-5.0.3/yd_commands/cancel.py
+-rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-5.0.3/yd_commands/check_imports.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-5.0.3/yd_commands/compact_json.py
+-rw-r--r--   0 pwt        (501) staff       (20)    18238 2023-03-31 13:51:41.000000 yellowdog-python-examples-5.0.3/yd_commands/config.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5474 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.3/yd_commands/config_keys.py
+-rw-r--r--   0 pwt        (501) staff       (20)    12183 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.3/yd_commands/csv_data.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1647 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.3/yd_commands/delete.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3616 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.3/yd_commands/download.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     9203 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.3/yd_commands/instantiate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3749 2022-12-01 11:00:21.000000 yellowdog-python-examples-5.0.3/yd_commands/interactive.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.3/yd_commands/jsonnet2json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     7539 2023-03-02 09:05:10.000000 yellowdog-python-examples-5.0.3/yd_commands/list.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3012 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.3/yd_commands/object_utilities.py
+-rw-r--r--   0 pwt        (501) staff       (20)     9590 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.3/yd_commands/printing.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    16885 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.3/yd_commands/provision.py
+-rw-r--r--   0 pwt        (501) staff       (20)      789 2023-03-13 13:46:12.000000 yellowdog-python-examples-5.0.3/yd_commands/provision_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.3/yd_commands/reformat_json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3231 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.3/yd_commands/shutdown.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    39847 2023-04-17 15:00:55.000000 yellowdog-python-examples-5.0.3/yd_commands/submit.py
+-rw-r--r--   0 pwt        (501) staff       (20)     6051 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.3/yd_commands/submit_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2756 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.3/yd_commands/terminate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-5.0.3/yd_commands/type_check.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2252 2023-03-15 09:01:37.000000 yellowdog-python-examples-5.0.3/yd_commands/upload.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3389 2023-03-14 20:22:33.000000 yellowdog-python-examples-5.0.3/yd_commands/upload_utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1630 2023-03-02 09:05:10.000000 yellowdog-python-examples-5.0.3/yd_commands/validate_properties.py
+-rw-r--r--   0 pwt        (501) staff       (20)    11055 2023-04-17 15:00:55.000000 yellowdog-python-examples-5.0.3/yd_commands/variables.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-5.0.3/yd_commands/version.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2200 2023-02-04 22:01:25.000000 yellowdog-python-examples-5.0.3/yd_commands/wrapper.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-17 15:01:32.908155 yellowdog-python-examples-5.0.3/yellowdog_python_examples.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-04-17 15:01:32.000000 yellowdog-python-examples-5.0.3/yellowdog_python_examples.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-04-17 15:01:32.000000 yellowdog-python-examples-5.0.3/yellowdog_python_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2023-04-17 15:01:32.000000 yellowdog-python-examples-5.0.3/yellowdog_python_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      574 2023-04-17 15:01:32.000000 yellowdog-python-examples-5.0.3/yellowdog_python_examples.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       61 2023-04-17 15:01:32.000000 yellowdog-python-examples-5.0.3/yellowdog_python_examples.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       12 2023-04-17 15:01:32.000000 yellowdog-python-examples-5.0.3/yellowdog_python_examples.egg-info/top_level.txt
```

### Comparing `yellowdog-python-examples-5.0.2/LICENSE` & `yellowdog-python-examples-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/PKG-INFO` & `yellowdog-python-examples-5.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 5.0.2
+Version: 5.0.3
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-5.0.2/PYPI_README.md` & `yellowdog-python-examples-5.0.3/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/README.md` & `yellowdog-python-examples-5.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -744,22 +744,26 @@
 
 ## Variable Substitutions in Work Requirement Properties
 
 Variable substitutions can be used within any property value in TOML configuration files or Work Requirement JSON files. See the description [above](#variable-substitutions) for more details on variable substitutions. This is a powerful feature that allows Work Requirements to be parameterised by supplying values on the command line, via environment variables or via the TOML file.
 
 ### Task and Task Group Name Substitution
 
-The following numbering substitutions are available for use in Task and Task Group naming, i.e., they can be used in the `name` properties for Tasks and Task Groups respectively in JSON Work Requirements. Note that Task Group names cannot use the `{{task_number}}` directive.
+The following numbering and naming substitutions are available for use in Task and Task Group naming, i.e., they can be used in the `name` properties for Tasks and Task Groups respectively in JSON Work Requirements. Note that Task Group names cannot use the `{{task_number}}` directive.
 
-| Directive               | Description                                       | Task Group | Task |
-|:------------------------|:--------------------------------------------------|:-----------|:-----|
-| `{{task_group_count}}`  | The number of Task Groups in the Work Requirement | Yes        | Yes  |
-| `{{task_group_number}}` | The current Task Group number                     | Yes        | Yes  |
-| `{{task_count}}`        | The number of Tasks in the current Task Group     | Yes        | Yes  |
-| `{{task_number}}`       | The current Task number                           |            | Yes  |
+**Tasks** can also use any of the substitutions in any of their properties.
+
+| Directive               | Description                                       | Task | Task Group |
+|:------------------------|:--------------------------------------------------|:-----|:-----------|
+| `{{task_number}}`       | The current Task number                           | Yes  |            |
+| `{{task_name}}`         | The current Task name                             | Yes  |            |
+| `{{task_group_name}}`   | The current Task Group name                       | Yes  |            |
+| `{{task_count}}`        | The number of Tasks in the current Task Group     | Yes  | Yes        |
+| `{{task_group_number}}` | The current Task Group number                     | Yes  | Yes        |
+| `{{task_group_count}}`  | The number of Task Groups in the Work Requirement | Yes  | Yes        |
 
 Numbers are zero-padded for neat formatting and sorting, e.g., Task number 37 of 1000 Tasks would be substituted as `0037`.
 
 As an example, the following JSON Work Requirement:
 
 ```json
 {
```

### Comparing `yellowdog-python-examples-5.0.2/pyproject.toml` & `yellowdog-python-examples-5.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/setup.cfg` & `yellowdog-python-examples-5.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/abort.py` & `yellowdog-python-examples-5.0.3/yd_commands/abort.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/admin.py` & `yellowdog-python-examples-5.0.3/yd_commands/admin.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/args.py` & `yellowdog-python-examples-5.0.3/yd_commands/args.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/cancel.py` & `yellowdog-python-examples-5.0.3/yd_commands/cancel.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/check_imports.py` & `yellowdog-python-examples-5.0.3/yd_commands/check_imports.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/compact_json.py` & `yellowdog-python-examples-5.0.3/yd_commands/compact_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/config.py` & `yellowdog-python-examples-5.0.3/yd_commands/config.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/config_keys.py` & `yellowdog-python-examples-5.0.3/yd_commands/config_keys.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/csv_data.py` & `yellowdog-python-examples-5.0.3/yd_commands/csv_data.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/delete.py` & `yellowdog-python-examples-5.0.3/yd_commands/delete.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/download.py` & `yellowdog-python-examples-5.0.3/yd_commands/download.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/instantiate.py` & `yellowdog-python-examples-5.0.3/yd_commands/instantiate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/interactive.py` & `yellowdog-python-examples-5.0.3/yd_commands/interactive.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/jsonnet2json.py` & `yellowdog-python-examples-5.0.3/yd_commands/jsonnet2json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/list.py` & `yellowdog-python-examples-5.0.3/yd_commands/list.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/object_utilities.py` & `yellowdog-python-examples-5.0.3/yd_commands/object_utilities.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/printing.py` & `yellowdog-python-examples-5.0.3/yd_commands/printing.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/provision.py` & `yellowdog-python-examples-5.0.3/yd_commands/provision.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/provision_utils.py` & `yellowdog-python-examples-5.0.3/yd_commands/provision_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/reformat_json.py` & `yellowdog-python-examples-5.0.3/yd_commands/reformat_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/shutdown.py` & `yellowdog-python-examples-5.0.3/yd_commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/submit.py` & `yellowdog-python-examples-5.0.3/yd_commands/submit.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,17 +68,20 @@
     check_str,
 )
 from yd_commands.upload_utils import unique_upload_pathname
 from yd_commands.validate_properties import validate_properties
 from yd_commands.variables import (
     L_TASK_COUNT,
     L_TASK_GROUP_COUNT,
+    L_TASK_GROUP_NAME,
     L_TASK_GROUP_NUMBER,
+    L_TASK_NAME,
     L_TASK_NUMBER,
     L_WR_NAME,
+    add_substitution_overwrite,
     add_substitutions,
     load_json_file_with_variable_substitutions,
     load_jsonnet_file_with_variable_substitutions,
     load_toml_file_with_variable_substitutions,
     process_variable_substitutions,
 )
 from yd_commands.wrapper import CLIENT, CONFIG_COMMON, main_wrapper
@@ -473,14 +476,22 @@
     tasks_list: List[Task] = []
     if num_task_batches > 1 and not ARGS_PARSER.dry_run:
         print_log(
             f"Adding Tasks to Task Group '{task_group.name}' in "
             f"{num_task_batches} batches"
         )
 
+    # Add lazy substitutions for use in any Task property
+    add_substitution_overwrite(L_TASK_COUNT, str(num_tasks))
+    add_substitution_overwrite(L_TASK_GROUP_NAME, task_group.name)
+    add_substitution_overwrite(
+        L_TASK_GROUP_NUMBER, formatted_number_str(tg_number, num_task_groups)
+    )
+    add_substitution_overwrite(L_TASK_GROUP_COUNT, str(num_task_groups))
+
     # Iterate through batches
     for batch_number in range(num_task_batches):
         # Iterate through tasks in the batch
         for task_number in range(
             (TASK_BATCH_SIZE * batch_number),
             min(TASK_BATCH_SIZE * (batch_number + 1), num_tasks),
         ):
@@ -491,14 +502,21 @@
                     task.get(NAME, task.get(TASK_NAME, CONFIG_WR.task_name)),
                     task_number,
                     num_tasks,
                     tg_number,
                     num_task_groups,
                 )
             )
+
+            add_substitution_overwrite(L_TASK_NAME, str(task_name))
+            add_substitution_overwrite(
+                L_TASK_NUMBER, formatted_number_str(task_number, num_tasks)
+            )
+            process_variable_substitutions(task)
+
             executable = check_str(
                 task.get(
                     EXECUTABLE,
                     task_group_data.get(
                         EXECUTABLE, wr_data.get(EXECUTABLE, CONFIG_WR.executable)
                     ),
                 )
```

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/submit_utils.py` & `yellowdog-python-examples-5.0.3/yd_commands/submit_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/terminate.py` & `yellowdog-python-examples-5.0.3/yd_commands/terminate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/type_check.py` & `yellowdog-python-examples-5.0.3/yd_commands/type_check.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/upload.py` & `yellowdog-python-examples-5.0.3/yd_commands/upload.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/upload_utils.py` & `yellowdog-python-examples-5.0.3/yd_commands/upload_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/validate_properties.py` & `yellowdog-python-examples-5.0.3/yd_commands/validate_properties.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/variables.py` & `yellowdog-python-examples-5.0.3/yd_commands/variables.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,17 @@
     "datetime": UTCNOW.strftime("%y%m%d-%H%M%S"),
     "random": hex(randint(0, RAND_SIZE + 1))[2:].lower().zfill(len(hex(RAND_SIZE)) - 2),
 }
 
 # Lazy substitutions: 'submit' only
 if "submit" in sys.argv[0]:
     L_WR_NAME = "wr_name"
+    L_TASK_NAME = "task_name"
     L_TASK_NUMBER = "task_number"
+    L_TASK_GROUP_NAME = "task_group_name"
     L_TASK_GROUP_NUMBER = "task_group_number"
     L_TASK_COUNT = "task_count"
     L_TASK_GROUP_COUNT = "task_group_count"
 
 # Type annotations for variable type substitutions
 NUMBER_SUB = "num:"
 BOOL_SUB = "bool:"
@@ -81,27 +83,35 @@
     resolve remaining variables if possible.
     """
     global VARIABLE_SUBSTITUTIONS
     subs.update(VARIABLE_SUBSTITUTIONS)
     VARIABLE_SUBSTITUTIONS = subs
 
     # Populate variables that can now be substituted
+    # Ensure that the value is stored as a string
     for key, value in VARIABLE_SUBSTITUTIONS.items():
-        VARIABLE_SUBSTITUTIONS[key] = substitute_variable_str(value)
+        VARIABLE_SUBSTITUTIONS[key] = substitute_variable_str(str(value))
+
+
+def add_substitution_overwrite(key: str, value: str):
+    """
+    Add a substitution to the dictionary, overwriting existing values.
+    """
+    VARIABLE_SUBSTITUTIONS[key] = str(value)
 
 
 def simple_variable_substitution(input_string: Optional[str]) -> Optional[str]:
     """
     Apply basic variable substitutions.
     """
     if input_string is None:
         return None
 
     for sub, value in VARIABLE_SUBSTITUTIONS.items():
-        input_string = input_string.replace(f"{{{{{sub}}}}}", value)
+        input_string = input_string.replace(f"{{{{{sub}}}}}", str(value))
 
     return input_string
 
 
 def process_variable_substitutions(
     dict_data: Dict,
     prefix: str = "",
```

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/version.py` & `yellowdog-python-examples-5.0.3/yd_commands/version.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yd_commands/wrapper.py` & `yellowdog-python-examples-5.0.3/yd_commands/wrapper.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/PKG-INFO` & `yellowdog-python-examples-5.0.3/yellowdog_python_examples.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 5.0.2
+Version: 5.0.3
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/SOURCES.txt` & `yellowdog-python-examples-5.0.3/yellowdog_python_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.2/yellowdog_python_examples.egg-info/entry_points.txt` & `yellowdog-python-examples-5.0.3/yellowdog_python_examples.egg-info/entry_points.txt`

 * *Files identical despite different names*

