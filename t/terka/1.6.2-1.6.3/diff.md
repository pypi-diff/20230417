# Comparing `tmp/terka-1.6.2.tar.gz` & `tmp/terka-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.6.2.tar", last modified: Mon Apr 17 15:24:27 2023, max compression
+gzip compressed data, was "terka-1.6.3.tar", last modified: Mon Apr 17 20:21:09 2023, max compression
```

## Comparing `terka-1.6.2.tar` & `terka-1.6.3.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:24:27.992607 terka-1.6.2/
--rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.6.2/LICENSE
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-17 15:24:27.992607 terka-1.6.2/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.6.2/README.md
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-17 15:24:27.992607 terka-1.6.2/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      872 2023-04-17 15:24:22.000000 terka-1.6.2/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:24:27.988608 terka-1.6.2/src/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.2/src/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:24:27.988608 terka-1.6.2/src/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.2/src/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    15295 2023-04-12 20:19:39.000000 terka-1.6.2/src/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.6.2/src/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:24:27.988608 terka-1.6.2/src/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.2/src/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.2/src/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    38030 2023-04-17 14:44:32.000000 terka-1.6.2/src/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.2/src/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.2/src/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.6.2/src/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.2/src/domain/event_history.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.2/src/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.2/src/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2177 2023-04-15 18:25:02.000000 terka-1.6.2/src/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.6.2/src/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.2/src/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.6.2/src/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.2/src/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.6.2/src/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:24:27.988608 terka-1.6.2/src/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.2/src/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     5069 2023-04-16 07:51:14.000000 terka-1.6.2/src/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:24:27.992607 terka-1.6.2/src/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.2/src/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    26258 2023-04-17 15:23:28.000000 terka-1.6.2/src/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.6.2/src/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.2/src/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.2/src/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     7617 2023-04-16 08:47:06.000000 terka-1.6.2/src/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:24:27.992607 terka-1.6.2/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-17 15:24:27.000000 terka-1.6.2/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      976 2023-04-17 15:24:27.000000 terka-1.6.2/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-17 15:24:27.000000 terka-1.6.2/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-17 15:24:27.000000 terka-1.6.2/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       37 2023-04-17 15:24:27.000000 terka-1.6.2/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-17 15:24:27.000000 terka-1.6.2/terka.egg-info/top_level.txt
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:24:27.992607 terka-1.6.2/tests/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.2/tests/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.6.2/tests/conftest.py
--rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.6.2/tests/test_commands.py
--rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.6.2/tests/test_orm.py
--rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.6.2/tests/test_task.py
--rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.6.2/tests/test_user.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.6.2/tests/test_utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.063365 terka-1.6.3/
+-rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.6.3/LICENSE
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-17 20:21:09.063365 terka-1.6.3/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.6.3/README.md
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-17 20:21:09.063365 terka-1.6.3/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      890 2023-04-17 20:21:02.000000 terka-1.6.3/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.055365 terka-1.6.3/src/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.3/src/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.055365 terka-1.6.3/src/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.3/src/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    15295 2023-04-12 20:19:39.000000 terka-1.6.3/src/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.6.3/src/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.059365 terka-1.6.3/src/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.3/src/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.3/src/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    38030 2023-04-17 14:44:32.000000 terka-1.6.3/src/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.3/src/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.3/src/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.6.3/src/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.3/src/domain/event_history.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.3/src/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.3/src/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2177 2023-04-15 18:25:02.000000 terka-1.6.3/src/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.6.3/src/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.3/src/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.6.3/src/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.3/src/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.6.3/src/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.059365 terka-1.6.3/src/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.3/src/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     5069 2023-04-17 20:19:14.000000 terka-1.6.3/src/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.059365 terka-1.6.3/src/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.3/src/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    26602 2023-04-17 20:07:43.000000 terka-1.6.3/src/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.6.3/src/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.3/src/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.3/src/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)      529 2023-04-17 20:19:26.000000 terka-1.6.3/src/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7617 2023-04-16 08:47:06.000000 terka-1.6.3/src/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.059365 terka-1.6.3/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-17 20:21:09.000000 terka-1.6.3/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)     1003 2023-04-17 20:21:09.000000 terka-1.6.3/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-17 20:21:09.000000 terka-1.6.3/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-17 20:21:09.000000 terka-1.6.3/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-17 20:21:09.000000 terka-1.6.3/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-17 20:21:09.000000 terka-1.6.3/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.063365 terka-1.6.3/tests/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.3/tests/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.6.3/tests/conftest.py
+-rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.6.3/tests/test_commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.6.3/tests/test_orm.py
+-rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.6.3/tests/test_task.py
+-rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.6.3/tests/test_user.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.6.3/tests/test_utils.py
```

### Comparing `terka-1.6.2/LICENSE` & `terka-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/PKG-INFO` & `terka-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.6.2
+Version: 1.6.3
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.6.2/README.md` & `terka-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/setup.py` & `terka-1.6.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.6.2",
+    version="1.6.3",
     description="CLI utility for creating and managing tasks in a terminal",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
     packages=find_packages(),
     include_package_data=True,
     package_data={"": ["service_layer/*.css"]},
     install_requires=[
-        "sqlalchemy", "pyaml", "rich", "textual==0.5.0"
+        "sqlalchemy", "pyaml", "rich", "textual==0.5.0", "plotext==5.2.8"
     ],
     setup_requires=["pytest-runner"],
     tests_requires=["pytest"],
     entry_points={
         "console_scripts": [
             "terka=src.entrypoints.cli:main"
         ]
```

### Comparing `terka-1.6.2/src/adapters/orm.py` & `terka-1.6.3/src/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/adapters/repository.py` & `terka-1.6.3/src/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/domain/collaborators.py` & `terka-1.6.3/src/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/domain/commands.py` & `terka-1.6.3/src/domain/commands.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/domain/commentary.py` & `terka-1.6.3/src/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/domain/epic.py` & `terka-1.6.3/src/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/domain/event_history.py` & `terka-1.6.3/src/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/domain/project.py` & `terka-1.6.3/src/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/domain/sprint.py` & `terka-1.6.3/src/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/domain/story.py` & `terka-1.6.3/src/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/domain/tag.py` & `terka-1.6.3/src/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/domain/task.py` & `terka-1.6.3/src/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/domain/time_tracker.py` & `terka-1.6.3/src/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/domain/user.py` & `terka-1.6.3/src/domain/user.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/entrypoints/cli.py` & `terka-1.6.3/src/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/service_layer/printer.py` & `terka-1.6.3/src/service_layer/printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from dataclasses import dataclass
 from operator import attrgetter
 import inspect
 from copy import deepcopy
 
 from collections import defaultdict
 from datetime import datetime, date, timedelta
+import plotext as plt
 import rich
 from rich.console import Console
 from rich.table import Table
 from statistics import mean, median
 
-from src.service_layer import services
+from src.service_layer import services, views
 from src.service_layer.ui import TerkaTask
 
 
 @dataclass
 class PrintOptions:
     show_tasks: bool = True
     show_history: bool = False
@@ -265,26 +266,36 @@
                           str(entity.end_date), entity.goal,
                           entity.status.name, str(len(open_tasks)),
                           str(len(tasks)), str(round(sum(story_points),
                                                      2)), collaborators_string,
                           str(time_spent))
         if table.row_count:
             self.console.print(table)
+
         if print_options.show_tasks:
             task_print_options = deepcopy(print_options)
             task_print_options.show_commentaries = False
             self.print_task(entities=tasks,
                             repo=repo,
                             print_options=task_print_options,
                             story_points=story_points,
                             kwargs=kwargs,
                             show_window=False)
         if i == 0 and print_options.show_commentaries and (
                 commentaries := entities[0].commentaries):
             self.print_commentaries(commentaries)
+        time_entries = views.time_spent(repo.session, entity.start_date,
+                                        entity.end_date)
+        dates = [entry.get("date") for entry in time_entries]
+        times = [entry.get("time_spent_hours") for entry in time_entries]
+        plt.date_form('Y-m-d')
+        plt.plot_size(100, 15)
+        plt.title("Time tracker")
+        plt.bar(dates, times)
+        plt.show()
 
     def print_project(self, entities, print_options, kwargs=None):
         table = Table(box=rich.box.SQUARE_DOUBLE_HEAD, expand=True)
         non_active_projects = Table(box=rich.box.SQUARE_DOUBLE_HEAD)
         for column in ("id", "name", "description", "status", "open_tasks",
                        "overdue", "backlog", "todo", "in_progress", "review",
                        "done", "median_task_age"):
@@ -395,24 +406,24 @@
             repo=repo,
             story_points=story_points,
             show_window=show_window)
         if table.row_count:
             self.console.print(table)
         if print_options.show_completed and completed_tasks:
             table = Table(box=self.box)
-            table, *rest = self._print_task(table=table,
-                                            entities=completed_tasks,
-                                            default_columns=default_columns,
-                                            repo=repo,
-                                            story_points=completed_story_points,
-                                            show_window=show_window,
-                                            all_tasks=False)
+            table, *rest = self._print_task(
+                table=table,
+                entities=completed_tasks,
+                default_columns=default_columns,
+                repo=repo,
+                story_points=completed_story_points,
+                show_window=show_window,
+                all_tasks=False)
             if table.row_count:
-                self.console.print(
-                    f"[green]****COMPLETED TASKS*****[/green]")
+                self.console.print(f"[green]****COMPLETED TASKS*****[/green]")
                 self.console.print(table)
         # TODO: not working
         if print_options.show_commentaries and (commentaries :=
                                                 entity.commentaries):
             self.print_commentaries(commentaries)
         if print_options.show_history and (history := entity.history):
             self.print_history(history)
@@ -561,15 +572,17 @@
             time_spent = self._calculate_time_spent(entity)
             if entity.status.name in ("DELETED", "DONE") and all_tasks:
                 completed_tasks.append(entity)
                 if story_points:
                     completed_story_points.append(story_point)
                 continue
             entity_name = f"{entity.name}" if not comments else f"{entity.name} [blue][{len(comments)}][/blue]"
-            if entity.due_date and entity.due_date <= date.today():
+            if not all_tasks:
+                entity_id = str(entity.id)
+            elif entity.due_date and entity.due_date <= date.today():
                 entity_id = f"[red]{entity.id}[/red]"
             elif (event_history := entity.history) and entity.status.name in (
                     "TODO", "IN_PROGRESS", "REVIEW"):
                 if max([event.date for event in event_history
                         ]) < (datetime.today() - timedelta(days=5)):
                     entity_id = f"[yellow]{entity.id}[/yellow]"
                 else:
```

### Comparing `terka-1.6.2/src/service_layer/services.py` & `terka-1.6.3/src/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/service_layer/ui.py` & `terka-1.6.3/src/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/service_layer/vertical_layout.css` & `terka-1.6.3/src/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/src/utils.py` & `terka-1.6.3/src/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/terka.egg-info/PKG-INFO` & `terka-1.6.3/terka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.6.2
+Version: 1.6.3
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.6.2/terka.egg-info/SOURCES.txt` & `terka-1.6.3/terka.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 src/entrypoints/__init__.py
 src/entrypoints/cli.py
 src/service_layer/__init__.py
 src/service_layer/printer.py
 src/service_layer/services.py
 src/service_layer/ui.py
 src/service_layer/vertical_layout.css
+src/service_layer/views.py
 terka.egg-info/PKG-INFO
 terka.egg-info/SOURCES.txt
 terka.egg-info/dependency_links.txt
 terka.egg-info/entry_points.txt
 terka.egg-info/requires.txt
 terka.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `terka-1.6.2/tests/test_orm.py` & `terka-1.6.3/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/tests/test_task.py` & `terka-1.6.3/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.2/tests/test_user.py` & `terka-1.6.3/tests/test_user.py`

 * *Files identical despite different names*

