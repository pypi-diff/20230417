# Comparing `tmp/terka-1.6.0.tar.gz` & `tmp/terka-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.6.0.tar", last modified: Sun Apr 16 18:40:18 2023, max compression
+gzip compressed data, was "terka-1.6.1.tar", last modified: Mon Apr 17 15:18:27 2023, max compression
```

## Comparing `terka-1.6.0.tar` & `terka-1.6.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.721919 terka-1.6.0/
--rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.6.0/LICENSE
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-16 18:40:18.721919 terka-1.6.0/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.6.0/README.md
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-16 18:40:18.721919 terka-1.6.0/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      872 2023-04-16 18:39:09.000000 terka-1.6.0/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.717919 terka-1.6.0/src/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.0/src/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.717919 terka-1.6.0/src/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.0/src/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    15295 2023-04-12 20:19:39.000000 terka-1.6.0/src/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.6.0/src/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.721919 terka-1.6.0/src/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.0/src/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.0/src/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    37918 2023-04-16 18:32:21.000000 terka-1.6.0/src/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.0/src/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.0/src/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.6.0/src/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.0/src/domain/event_history.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.0/src/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.0/src/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2177 2023-04-15 18:25:02.000000 terka-1.6.0/src/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.6.0/src/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.0/src/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.6.0/src/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.0/src/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.6.0/src/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.721919 terka-1.6.0/src/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.0/src/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     5069 2023-04-16 07:51:14.000000 terka-1.6.0/src/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.721919 terka-1.6.0/src/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.0/src/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    30299 2023-04-16 18:29:06.000000 terka-1.6.0/src/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.6.0/src/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.0/src/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.0/src/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     7617 2023-04-16 08:47:06.000000 terka-1.6.0/src/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.721919 terka-1.6.0/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-16 18:40:18.000000 terka-1.6.0/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      976 2023-04-16 18:40:18.000000 terka-1.6.0/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-16 18:40:18.000000 terka-1.6.0/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-16 18:40:18.000000 terka-1.6.0/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       37 2023-04-16 18:40:18.000000 terka-1.6.0/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-16 18:40:18.000000 terka-1.6.0/terka.egg-info/top_level.txt
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.721919 terka-1.6.0/tests/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.0/tests/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.6.0/tests/conftest.py
--rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.6.0/tests/test_commands.py
--rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.6.0/tests/test_orm.py
--rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.6.0/tests/test_task.py
--rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.6.0/tests/test_user.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.6.0/tests/test_utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:18:27.298875 terka-1.6.1/
+-rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.6.1/LICENSE
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-17 15:18:27.298875 terka-1.6.1/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.6.1/README.md
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-17 15:18:27.298875 terka-1.6.1/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      872 2023-04-17 15:18:18.000000 terka-1.6.1/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:18:27.294875 terka-1.6.1/src/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.1/src/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:18:27.294875 terka-1.6.1/src/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.1/src/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    15295 2023-04-12 20:19:39.000000 terka-1.6.1/src/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.6.1/src/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:18:27.294875 terka-1.6.1/src/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.1/src/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.1/src/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    38030 2023-04-17 14:44:32.000000 terka-1.6.1/src/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.1/src/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.1/src/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.6.1/src/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.1/src/domain/event_history.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.1/src/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.1/src/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2177 2023-04-15 18:25:02.000000 terka-1.6.1/src/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.6.1/src/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.1/src/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.6.1/src/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.1/src/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.6.1/src/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:18:27.294875 terka-1.6.1/src/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.1/src/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     5069 2023-04-16 07:51:14.000000 terka-1.6.1/src/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:18:27.298875 terka-1.6.1/src/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.1/src/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    26216 2023-04-17 15:12:24.000000 terka-1.6.1/src/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.6.1/src/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.1/src/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.1/src/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     7617 2023-04-16 08:47:06.000000 terka-1.6.1/src/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:18:27.298875 terka-1.6.1/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-17 15:18:27.000000 terka-1.6.1/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      976 2023-04-17 15:18:27.000000 terka-1.6.1/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-17 15:18:27.000000 terka-1.6.1/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-17 15:18:27.000000 terka-1.6.1/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       37 2023-04-17 15:18:27.000000 terka-1.6.1/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-17 15:18:27.000000 terka-1.6.1/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 15:18:27.298875 terka-1.6.1/tests/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.1/tests/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.6.1/tests/conftest.py
+-rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.6.1/tests/test_commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.6.1/tests/test_orm.py
+-rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.6.1/tests/test_task.py
+-rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.6.1/tests/test_user.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.6.1/tests/test_utils.py
```

### Comparing `terka-1.6.0/LICENSE` & `terka-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/PKG-INFO` & `terka-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.6.0
+Version: 1.6.1
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.6.0/README.md` & `terka-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/setup.py` & `terka-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.6.0",
+    version="1.6.1",
     description="CLI utility for creating and managing tasks in a terminal",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.6.0/src/adapters/orm.py` & `terka-1.6.1/src/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/adapters/repository.py` & `terka-1.6.1/src/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/domain/collaborators.py` & `terka-1.6.1/src/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/domain/commands.py` & `terka-1.6.1/src/domain/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -793,21 +793,23 @@
                     task_params.update({"due_date": sprint.end_date})
                 self.execute("update", "tasks", task_params)
         elif command == "show":
             if len(kwargs) == 1 and "project" in kwargs:
                 kwargs["id"] = kwargs["project"]
                 del kwargs["project"]
             print_options = printer.PrintOptions(
-                show_history=bool(kwargs.get("show_history")),
-                show_commentaries=bool(kwargs.get("show_commentaries")),
-                show_completed=bool(kwargs.get("show_completed")))
+                show_history=bool(kwargs.pop("show_history", False)),
+                show_commentaries=bool(kwargs.pop("show_commentaries", False)),
+                show_completed=bool(kwargs.pop("show_completed", False)))
             if kwargs.pop("partial_project_view", False):
                 print_options.show_epics = bool(kwargs.pop("epics", False))
                 print_options.show_tasks = bool(kwargs.pop("tasks", False))
                 print_options.show_stories = bool(kwargs.pop("stories", False))
+            if entity_type == "tasks":
+                print_options.show_completed = True
             if not (task_id := kwargs.get("id")):
                 if entity_type == "sprints":
                     active_sprint = self.repo.list(Sprint,
                                                    {"status": "ACTIVE"})
                     if len(active_sprint) == 1:
                         task_id = active_sprint[0].id
                     else:
```

### Comparing `terka-1.6.0/src/domain/commentary.py` & `terka-1.6.1/src/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/domain/epic.py` & `terka-1.6.1/src/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/domain/event_history.py` & `terka-1.6.1/src/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/domain/project.py` & `terka-1.6.1/src/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/domain/sprint.py` & `terka-1.6.1/src/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/domain/story.py` & `terka-1.6.1/src/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/domain/tag.py` & `terka-1.6.1/src/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/domain/task.py` & `terka-1.6.1/src/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/domain/time_tracker.py` & `terka-1.6.1/src/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/domain/user.py` & `terka-1.6.1/src/domain/user.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/entrypoints/cli.py` & `terka-1.6.1/src/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/service_layer/printer.py` & `terka-1.6.1/src/service_layer/printer.py`

 * *Files 16% similar despite different names*

```diff
@@ -266,21 +266,23 @@
                           entity.status.name, str(len(open_tasks)),
                           str(len(tasks)), str(round(sum(story_points),
                                                      2)), collaborators_string,
                           str(time_spent))
         if table.row_count:
             self.console.print(table)
         if print_options.show_tasks:
-            self.print_sprint_task(entities=tasks,
-                                   repo=repo,
-                                   show_completed=print_options.show_completed,
-                                   story_points=story_points,
-                                   kwargs=kwargs)
+            task_print_options = deepcopy(print_options)
+            task_print_options.show_commentaries = False
+            self.print_task(entities=tasks,
+                            repo=repo,
+                            print_options=task_print_options,
+                            story_points=story_points,
+                            kwargs=kwargs)
         if i == 0 and print_options.show_commentaries and (
-                commentaries := entity.commentaries):
+                commentaries := entities[0].commentaries):
             self.print_commentaries(commentaries)
 
     def print_project(self, entities, print_options, kwargs=None):
         table = Table(box=rich.box.SQUARE_DOUBLE_HEAD, expand=True)
         non_active_projects = Table(box=rich.box.SQUARE_DOUBLE_HEAD)
         for column in ("id", "name", "description", "status", "open_tasks",
                        "overdue", "backlog", "todo", "in_progress", "review",
@@ -334,254 +336,84 @@
         if print_options.show_epics and (epics := entity.epics):
             self.console.print("")
             self.print_epic(epics, self.repo, non_task_view_options)
         if print_options.show_stories and (stories := entity.stories):
             self.console.print("")
             self.print_story(stories, self.repo, non_task_view_options)
         if print_options.show_tasks and (tasks := entity.tasks):
+            task_print_options = deepcopy(print_options)
+            task_print_options.show_commentaries = False
             self.console.print("")
             self.print_task(entities=tasks,
                             repo=self.repo,
-                            print_options=print_options,
+                            print_options=task_print_options,
                             show_window=False,
                             kwargs=kwargs)
         if print_options.show_commentaries and (commentaries :=
                                                 entity.commentaries):
             self.print_commentaries(commentaries)
         if print_options.show_history and (history := entity.history):
             self.print_history(history)
 
-    def print_sprint_task(self,
-                          entities,
-                          repo,
-                          show_completed=False,
-                          history=None,
-                          comments=None,
-                          story_points=None,
-                          kwargs=None):
-        table = Table(box=self.box)
-        default_columns = ("id", "name", "description", "story points",
-                           "status", "priority", "project", "due_date", "tags",
-                           "collaborators", "time_spent")
-        for column in default_columns:
-            table.add_column(column)
-        entities = list(entities)
-        if kwargs:
-            entities = self._get_filtered_entities(entities, kwargs)
-        completed_tasks = []
-        completed_tasks_story_points = []
-        printable_entities = 0
-        for entity, story_point in sorted(zip(entities, story_points),
-                                          key=lambda x: x[0].status.value,
-                                          reverse=True):
-            if tags := entity.tags:
-                tag_texts = sorted([tag.base_tag.text for tag in list(tags)])
-                tag_string = ",".join(tag_texts)
-            else:
-                tag_string = ""
-            if collaborators := entity.collaborators:
-                collaborators_texts = sorted([
-                    collaborator.users.name
-                    for collaborator in list(collaborators)
-                ])
-                collaborator_string = ",".join(collaborators_texts)
-            else:
-                collaborator_string = ""
-            if comments := entity.commentaries:
-                comments.sort(key=lambda c: c.date, reverse=False)
-            if history := entity.history:
-                history.sort(key=lambda c: c.date, reverse=False)
-            try:
-                project_obj = services.lookup_project_name(
-                    entity.project, repo)
-                project = project_obj.name
-            except:
-                project = None
-            priority = entity.priority.name if hasattr(entity.priority,
-                                                       "name") else "UNKNOWN"
-            time_spent = self._calculate_time_spent(entity)
-            if entity.status.name in ("DELETED", "DONE"):
-                completed_tasks.append(entity)
-                completed_tasks_story_points.append(story_point)
-                continue
-            printable_entities += 1
-            entity_name = f"{entity.name}" if not comments else f"{entity.name} [blue][{len(comments)}][/blue]"
-            if entity.due_date and entity.due_date <= date.today():
-                entity_id = f"[red]{entity.id}[/red]"
-            elif (event_history := entity.history) and entity.status.name in (
-                    "TODO", "IN_PROGRESS", "REVIEW"):
-                if max([event.date for event in event_history
-                        ]) < (datetime.today() - timedelta(days=5)):
-                    entity_id = f"[yellow]{entity.id}[/yellow]"
-                else:
-                    entity_id = str(entity.id)
-            else:
-                entity_id = str(entity.id)
-            table.add_row(str(entity_id), entity_name, entity.description,
-                          str(story_point), entity.status.name, priority,
-                          project, str(entity.due_date), tag_string,
-                          collaborator_string, str(time_spent))
-        if table.row_count:
-            self.console.print(table)
-        if show_completed and completed_tasks:
-            table = Table(box=self.box)
-            for column in default_columns:
-                table.add_column(column)
-            self.console.print(f"[green]****COMPLETED TASKS*****[/green]")
-            for entity, story_point in zip(completed_tasks,
-                                           completed_tasks_story_points):
-                try:
-                    project_obj = services.lookup_project_name(
-                        entity.project, repo)
-                    project = project_obj.name
-                except:
-                    project = None
-                priority = entity.priority.name if hasattr(
-                    entity.priority, "name") else "UNKNOWN"
-                time_spent = self._calculate_time_spent(entity)
-                if tags := entity.tags:
-                    tag_texts = sorted(
-                        [tag.base_tag.text for tag in list(tags)])
-                    tag_string = ",".join(tag_texts)
-                else:
-                    tag_string = ""
-                if collaborators := entity.collaborators:
-                    collaborators_texts = sorted([
-                        collaborator.users.name
-                        for collaborator in list(collaborators)
-                    ])
-                    collaborator_string = ",".join(collaborators_texts)
-                else:
-                    collaborator_string = ""
-                table.add_row(str(entity.id), entity.name, entity.description,
-                              str(story_point), entity.status.name, priority,
-                              project, str(entity.due_date), tag_string,
-                              collaborator_string, str(time_spent))
-            if table.row_count:
-                self.console.print(table)
-        if len(entities) == 1 and printable_entities == 0:
-            table = Table(box=self.box)
-            for column in default_columns:
-                table.add_column(column)
-            for entity in entities:
-                table.add_row(str(entity.id), entity.name, entity.description,
-                              entity.status.name, priority, project,
-                              str(entity.due_date), tag_string,
-                              collaborator_string, str(time_spent))
-            if table.row_count:
-                self.console.print(table)
-
     def print_task(self,
                    entities,
                    repo,
                    print_options,
                    custom_sort=None,
                    show_window=True,
+                   story_points=None,
                    kwargs=None):
         table = Table(box=self.box, title="TASKS")
-        default_columns = ("id", "name", "description", "status", "priority",
-                           "project", "due_date", "tags", "collaborators",
-                           "time_spent")
+        if story_points:
+            default_columns = ("id", "name", "description", "story points",
+                               "status", "priority", "project", "due_date",
+                               "tags", "collaborators", "time_spent")
+        else:
+            default_columns = ("id", "name", "description", "status",
+                               "priority", "project", "due_date", "tags",
+                               "collaborators", "time_spent")
         #TODO: Add printing for only a single task
         # if (entities[0].status.name == "DONE"):
         #     console.print(f"[green]task is completed on [/green]")
         # else:
         #     active_in_days = datetime.now() - entities[0].creation_date
         #     console.print(f"[blue]task is active {active_in_days.days} days[/blue]")
-        for column in default_columns:
-            table.add_column(column)
         entities = list(entities)
         if kwargs:
             entities = self._get_filtered_entities(entities, kwargs)
-        completed_tasks = []
-        if custom_sort:
-            entities.sort(key=lambda c: getattr(c, custom_sort), reverse=False)
-        else:
-            entities.sort(key=lambda c: (c.status.value, c.priority.value),
-                          reverse=True)
-        printable_entities = 0
-        for entity in entities:
-            if tags := entity.tags:
-                tag_texts = sorted([tag.base_tag.text for tag in list(tags)])
-                tag_string = ",".join(tag_texts)
+        if not story_points:
+            if custom_sort:
+                entities.sort(key=lambda c: getattr(c, custom_sort),
+                              reverse=False)
             else:
-                tag_string = ""
-            if collaborators := entity.collaborators:
-                collaborators_texts = sorted([
-                    collaborator.users.name
-                    for collaborator in list(collaborators)
-                    if collaborator.users
-                ])
-                collaborator_string = ",".join(collaborators_texts)
-            else:
-                collaborator_string = ""
-            if comments := entity.commentaries:
-                comments.sort(key=lambda c: c.date, reverse=False)
-            if history := entity.history:
-                history.sort(key=lambda c: c.date, reverse=False)
-            try:
-                project_obj = services.lookup_project_name(
-                    entity.project, repo)
-                project = project_obj.name
-            except:
-                project = None
-            priority = entity.priority.name if hasattr(entity.priority,
-                                                       "name") else "UNKNOWN"
-            time_spent = self._calculate_time_spent(entity)
-            if entity.status.name in ("DELETED", "DONE"):
-                completed_tasks.append(entity)
-                continue
-            printable_entities += 1
-            entity_name = f"{entity.name}" if not comments else f"{entity.name} [blue][{len(comments)}][/blue]"
-            if entity.due_date and entity.due_date <= date.today():
-                entity_id = f"[red]{entity.id}[/red]"
-            elif (event_history := entity.history) and entity.status.name in (
-                    "TODO", "IN_PROGRESS", "REVIEW"):
-                if max([event.date for event in event_history
-                        ]) < (datetime.today() - timedelta(days=5)):
-                    entity_id = f"[yellow]{entity.id}[/yellow]"
-                else:
-                    entity_id = str(entity.id)
-            else:
-                entity_id = str(entity.id)
-            table.add_row(entity_id, entity_name, entity.description,
-                          entity.status.name, priority, project,
-                          str(entity.due_date), tag_string,
-                          collaborator_string, str(time_spent))
-        if printable_entities:
-            if printable_entities == 1 and show_window:
-                app = TerkaTask(entity=entity,
-                                project=project,
-                                history=history,
-                                commentaries=comments)
-                app.run()
-            if table.row_count:
-                self.console.print(table)
+                entities.sort(key=lambda c: (c.status.value, c.priority.value),
+                              reverse=True)
+        table, completed_tasks, completed_story_points = self._print_task(
+            table=table,
+            entities=entities,
+            default_columns=default_columns,
+            repo=repo,
+            story_points=story_points,
+            show_window=show_window)
+        if table.row_count:
+            self.console.print(table)
         if print_options.show_completed and completed_tasks:
             table = Table(box=self.box)
-            for column in default_columns:
-                table.add_column(column)
-            self.console.print(f"[green]****COMPLETED TASKS*****[/green]")
-            for entity in completed_tasks:
-                time_spent = self._calculate_time_spent(entity)
-                table.add_row(str(entity.id), entity.name, entity.description,
-                              entity.status.name, priority, project,
-                              str(entity.due_date), tag_string,
-                              collaborator_string, str(time_spent))
+            table, *rest = self._print_task(table=table,
+                                            entities=completed_tasks,
+                                            default_columns=default_columns,
+                                            repo=repo,
+                                            story_points=completed_story_points,
+                                            show_window=show_window,
+                                            all_tasks=False)
             if table.row_count:
+                self.console.print(
+                    f"[green]****COMPLETED TASKS*****[/green]")
                 self.console.print(table)
-        if len(entities) == 1 and printable_entities == 0:
-            table = Table(box=self.box)
-            app = TerkaTask(entity=entities[0],
-                            project=project,
-                            is_completed=True,
-                            history=history,
-                            commentaries=comments)
-            app.run()
-            exit()
+        # TODO: not working
         if print_options.show_commentaries and (commentaries :=
                                                 entity.commentaries):
             self.print_commentaries(commentaries)
         if print_options.show_history and (history := entity.history):
             self.print_history(history)
 
     def _get_attributes(self, obj) -> List[Tuple[str, str]]:
@@ -639,15 +471,16 @@
         if kwargs:
             filtering_attributes = set(list(kwargs))
             temp_entities = []
             attributes = [
                 name for name, value in inspect.getmembers(entities[0])
                 if not name.startswith("_") and not inspect.ismethod(value)
             ]
-            filtering_attributes = filtering_attributes.intersection(set(attributes))
+            filtering_attributes = filtering_attributes.intersection(
+                set(attributes))
             attribute_getter = attrgetter(*filtering_attributes)
             filtered_entities = []
             for entity in entities:
                 should_add = False
                 for key, value in kwargs.items():
                     if key in filtering_attributes:
                         attribute_value = getattr(entity, key)
@@ -664,7 +497,98 @@
                         else:
                             should_add = True
                             continue
                 if should_add:
                     filtered_entities.append(entity)
             entities = list(filtered_entities)
         return entities
+
+    def _print_task(self,
+                    table,
+                    entities,
+                    default_columns,
+                    repo,
+                    story_points=None,
+                    all_tasks=True,
+                    show_window=True):
+        if all_tasks:
+            completed_tasks = []
+        else:
+            completed_tasks = None
+            completed_story_points = None
+        if story_points:
+            completed_story_points = []
+            entities = [(entity, story_point) for entity, story_point in
+                        sorted(zip(entities, story_points),
+                               key=lambda x: x[0].status.value,
+                               reverse=True)]
+        else:
+            completed_story_points = None
+        for column in default_columns:
+            table.add_column(column)
+        for entity in entities:
+            if story_points:
+                story_point = entity[1]
+                entity = entity[0]
+            else:
+                story_point = None
+            if tags := entity.tags:
+                tag_texts = sorted([tag.base_tag.text for tag in list(tags)])
+                tag_string = ",".join(tag_texts)
+            else:
+                tag_string = ""
+            if collaborators := entity.collaborators:
+                collaborators_texts = sorted([
+                    collaborator.users.name
+                    for collaborator in list(collaborators)
+                    if collaborator.users
+                ])
+                collaborator_string = ",".join(collaborators_texts)
+            else:
+                collaborator_string = ""
+            if comments := entity.commentaries:
+                comments.sort(key=lambda c: c.date, reverse=False)
+            if history := entity.history:
+                history.sort(key=lambda c: c.date, reverse=False)
+            try:
+                project_obj = services.lookup_project_name(
+                    entity.project, repo)
+                project = project_obj.name
+            except:
+                project = None
+            priority = entity.priority.name if hasattr(entity.priority,
+                                                       "name") else "UNKNOWN"
+            time_spent = self._calculate_time_spent(entity)
+            if entity.status.name in ("DELETED", "DONE") and all_tasks:
+                completed_tasks.append(entity)
+                if story_points:
+                    completed_story_points.append(story_point)
+                continue
+            entity_name = f"{entity.name}" if not comments else f"{entity.name} [blue][{len(comments)}][/blue]"
+            if entity.due_date and entity.due_date <= date.today():
+                entity_id = f"[red]{entity.id}[/red]"
+            elif (event_history := entity.history) and entity.status.name in (
+                    "TODO", "IN_PROGRESS", "REVIEW"):
+                if max([event.date for event in event_history
+                        ]) < (datetime.today() - timedelta(days=5)):
+                    entity_id = f"[yellow]{entity.id}[/yellow]"
+                else:
+                    entity_id = str(entity.id)
+            else:
+                entity_id = str(entity.id)
+            if story_points:
+                table.add_row(entity_id, entity_name, entity.description,
+                              str(story_point), entity.status.name, priority,
+                              project, str(entity.due_date), tag_string,
+                              collaborator_string, str(time_spent))
+            else:
+                table.add_row(entity_id, entity_name, entity.description,
+                              entity.status.name, priority, project,
+                              str(entity.due_date), tag_string,
+                              collaborator_string, str(time_spent))
+        if table.row_count == 1 and show_window:
+            app = TerkaTask(entity=entities[0],
+                            project=project,
+                            history=history,
+                            commentaries=comments)
+            app.run()
+        return table, completed_tasks, completed_story_points
```

### Comparing `terka-1.6.0/src/service_layer/services.py` & `terka-1.6.1/src/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/service_layer/ui.py` & `terka-1.6.1/src/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/service_layer/vertical_layout.css` & `terka-1.6.1/src/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/src/utils.py` & `terka-1.6.1/src/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/terka.egg-info/PKG-INFO` & `terka-1.6.1/terka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.6.0
+Version: 1.6.1
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.6.0/terka.egg-info/SOURCES.txt` & `terka-1.6.1/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/tests/test_orm.py` & `terka-1.6.1/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/tests/test_task.py` & `terka-1.6.1/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.0/tests/test_user.py` & `terka-1.6.1/tests/test_user.py`

 * *Files identical despite different names*

