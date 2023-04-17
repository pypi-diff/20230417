# Comparing `tmp/terka-1.5.5.tar.gz` & `tmp/terka-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.5.5.tar", last modified: Sat Apr 15 20:21:57 2023, max compression
+gzip compressed data, was "terka-1.6.0.tar", last modified: Sun Apr 16 18:40:18 2023, max compression
```

## Comparing `terka-1.5.5.tar` & `terka-1.6.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 20:21:57.829262 terka-1.5.5/
--rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.5.5/LICENSE
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-15 20:21:57.825285 terka-1.5.5/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.5.5/README.md
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-15 20:21:57.829262 terka-1.5.5/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      872 2023-04-15 20:21:50.000000 terka-1.5.5/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 20:21:57.825285 terka-1.5.5/src/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.5/src/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 20:21:57.825285 terka-1.5.5/src/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.5/src/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    15295 2023-04-12 20:19:39.000000 terka-1.5.5/src/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.5.5/src/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 20:21:57.825285 terka-1.5.5/src/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.5/src/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.5.5/src/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    37330 2023-04-15 20:21:36.000000 terka-1.5.5/src/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.5.5/src/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.5.5/src/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.5.5/src/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.5.5/src/domain/event_history.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.5.5/src/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.5.5/src/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2177 2023-04-15 18:25:02.000000 terka-1.5.5/src/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.5.5/src/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.5.5/src/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.5.5/src/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.5.5/src/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.5.5/src/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 20:21:57.825285 terka-1.5.5/src/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.5.5/src/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     4257 2023-04-08 19:24:05.000000 terka-1.5.5/src/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 20:21:57.825285 terka-1.5.5/src/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.5/src/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    28173 2023-04-15 20:21:39.000000 terka-1.5.5/src/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.5.5/src/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.5.5/src/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.5.5/src/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     7181 2023-04-15 20:21:36.000000 terka-1.5.5/src/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 20:21:57.825285 terka-1.5.5/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-15 20:21:57.000000 terka-1.5.5/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      976 2023-04-15 20:21:57.000000 terka-1.5.5/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-15 20:21:57.000000 terka-1.5.5/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-15 20:21:57.000000 terka-1.5.5/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       37 2023-04-15 20:21:57.000000 terka-1.5.5/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-15 20:21:57.000000 terka-1.5.5/terka.egg-info/top_level.txt
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-15 20:21:57.825285 terka-1.5.5/tests/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.5/tests/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.5.5/tests/conftest.py
--rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.5.5/tests/test_commands.py
--rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.5.5/tests/test_orm.py
--rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.5.5/tests/test_task.py
--rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.5.5/tests/test_user.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.5.5/tests/test_utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.721919 terka-1.6.0/
+-rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.6.0/LICENSE
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-16 18:40:18.721919 terka-1.6.0/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.6.0/README.md
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-16 18:40:18.721919 terka-1.6.0/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      872 2023-04-16 18:39:09.000000 terka-1.6.0/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.717919 terka-1.6.0/src/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.0/src/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.717919 terka-1.6.0/src/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.0/src/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    15295 2023-04-12 20:19:39.000000 terka-1.6.0/src/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.6.0/src/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.721919 terka-1.6.0/src/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.0/src/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.0/src/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    37918 2023-04-16 18:32:21.000000 terka-1.6.0/src/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.0/src/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.0/src/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.6.0/src/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.0/src/domain/event_history.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.0/src/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.0/src/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2177 2023-04-15 18:25:02.000000 terka-1.6.0/src/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.6.0/src/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.0/src/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.6.0/src/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.0/src/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.6.0/src/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.721919 terka-1.6.0/src/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.0/src/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     5069 2023-04-16 07:51:14.000000 terka-1.6.0/src/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.721919 terka-1.6.0/src/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.0/src/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    30299 2023-04-16 18:29:06.000000 terka-1.6.0/src/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.6.0/src/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.0/src/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.0/src/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     7617 2023-04-16 08:47:06.000000 terka-1.6.0/src/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.721919 terka-1.6.0/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-16 18:40:18.000000 terka-1.6.0/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      976 2023-04-16 18:40:18.000000 terka-1.6.0/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-16 18:40:18.000000 terka-1.6.0/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-16 18:40:18.000000 terka-1.6.0/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       37 2023-04-16 18:40:18.000000 terka-1.6.0/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-16 18:40:18.000000 terka-1.6.0/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-16 18:40:18.721919 terka-1.6.0/tests/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.0/tests/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.6.0/tests/conftest.py
+-rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.6.0/tests/test_commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.6.0/tests/test_orm.py
+-rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.6.0/tests/test_task.py
+-rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.6.0/tests/test_user.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.6.0/tests/test_utils.py
```

### Comparing `terka-1.5.5/LICENSE` & `terka-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/PKG-INFO` & `terka-1.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.5.5
+Version: 1.6.0
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.5.5/README.md` & `terka-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/setup.py` & `terka-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.5.5",
+    version="1.6.0",
     description="CLI utility for creating and managing tasks in a terminal",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.5.5/src/adapters/orm.py` & `terka-1.6.0/src/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/adapters/repository.py` & `terka-1.6.0/src/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/domain/collaborators.py` & `terka-1.6.0/src/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/domain/commands.py` & `terka-1.6.0/src/domain/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,15 +368,16 @@
             self.execute("list", "tasks", kwargs)
         elif command == "log":
             table = Table(box=rich.box.SIMPLE)
             with open(f"{self.home_dir}/.terka/terka.log", "r") as f:
                 head = f.readlines()
             for column in ("date", "source", "level", "message"):
                 table.add_column(column)
-            tail = head[-10:]
+            num_log_entries = int(kwargs.get("num_log_entries", 10))
+            tail = head[-num_log_entries:]
             for row in tail[::-1]:
                 info, message = row.split("] ")
                 date, source, level = info.split("][")
                 table.add_row(re.sub("\[", "", date), source, level, message)
             self.console.print(table)
         elif command == "focus":
             if entity_type == "tasks":
@@ -788,36 +789,45 @@
                 task_params = {"id": task.id}
                 if task.status.name == "BACKLOG":
                     task_params.update({"status": "TODO"})
                 if not task.due_date or task.due_date > sprint.end_date:
                     task_params.update({"due_date": sprint.end_date})
                 self.execute("update", "tasks", task_params)
         elif command == "show":
+            if len(kwargs) == 1 and "project" in kwargs:
+                kwargs["id"] = kwargs["project"]
+                del kwargs["project"]
             print_options = printer.PrintOptions(
                 show_history=bool(kwargs.get("show_history")),
                 show_commentaries=bool(kwargs.get("show_commentaries")),
                 show_completed=bool(kwargs.get("show_completed")))
+            if kwargs.pop("partial_project_view", False):
+                print_options.show_epics = bool(kwargs.pop("epics", False))
+                print_options.show_tasks = bool(kwargs.pop("tasks", False))
+                print_options.show_stories = bool(kwargs.pop("stories", False))
             if not (task_id := kwargs.get("id")):
                 if entity_type == "sprints":
                     active_sprint = self.repo.list(Sprint,
                                                    {"status": "ACTIVE"})
                     if len(active_sprint) == 1:
                         task_id = active_sprint[0].id
                     else:
                         exit(
                             "More than 1 active sprint, please specify the sprint_id"
                         )
             tasks = get_ids(task_id)
+            if "id" in kwargs:
+                kwargs.pop("id")
             for task in tasks:
                 if task.isdigit():
                     entities = self.repo.list(entity, {"id": task})
                 else:
                     entities = self.repo.list(entity, {"name": task})
                 self.printer.print_entity(task, entity_type, entities,
-                                          self.repo, print_options)
+                                          self.repo, print_options, kwargs)
                 logger.info("<show> %s: %s", entity_type, task_id)
             return entities, None, None
         elif command == "done":
             if entity_type not in ("tasks", "sprints"):
                 raise ValueError("can complete only tasks and sprints")
             elif entity_type == "tasks":
                 kwargs.update({"status": "DONE"})
```

### Comparing `terka-1.5.5/src/domain/commentary.py` & `terka-1.6.0/src/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/domain/epic.py` & `terka-1.6.0/src/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/domain/event_history.py` & `terka-1.6.0/src/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/domain/project.py` & `terka-1.6.0/src/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/domain/sprint.py` & `terka-1.6.0/src/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/domain/story.py` & `terka-1.6.0/src/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/domain/tag.py` & `terka-1.6.0/src/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/domain/task.py` & `terka-1.6.0/src/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/domain/time_tracker.py` & `terka-1.6.0/src/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/domain/user.py` & `terka-1.6.0/src/domain/user.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/entrypoints/cli.py` & `terka-1.6.0/src/entrypoints/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -78,19 +78,15 @@
             datefmt="%Y-%m-%d %H:%M:%S")
 
         repo = SqlAlchemyRepository(session)
         command_handler = CommandHandler(repo)
         if args.command == "init":
             command_handler.execute("init")
 
-        try:
-            with open(f"{home_dir}/.terka/config.yaml", encoding="utf-8") as f:
-                config = yaml.safe_load(f)
-        except FileNotFoundError:
-            raise TerkaInitError("call `terka init` to initialize terka")
+        config = load_config(home_dir)
 
         task_id = config.get("task_id")
         project_name = config.get("project_name")
         if task_id or project_name:
             focus_type = "task" if task_id else "project"
             logger.warning("Using terka in focus mode")
             logger.warning(f"Current focus is {focus_type}: {task_id or project_name}")
@@ -99,26 +95,47 @@
         task_dict = update_task_dict(task_dict, repo)
         logger.debug(task_dict)
 
         command, entity = args.command, args.entity
         is_interactive = False
         if not command and not entity:
             is_interactive = True
-            console.print(f"[green]>>> Running terka in an interactive mode[/green]")
+            interactive_message = f"[green]>>> Running terka in an interactive mode[/green]"
+            if task_id:
+                interactive_message = f"{interactive_message} (focus task {task_id})"
+            elif project_name:
+                interactive_message = f"{interactive_message} (focus project {project_name})"
+            console.print(interactive_message)
             command = input("enter command: ")
             command, entity, task_dict = process_command(command, config, repo)
         try:
             command_handler.execute(command, entity, task_dict)
         except ValueError as e:
             console.print(f"[red]{e}[/red]")
 
         while is_interactive:
-            console.print(f"[green]>>> Running terka in an interactive mode[/green]")
+            interactive_message = f"[green]>>> Running terka in an interactive mode[/green]"
+            config = load_config(home_dir)
+            task_id = config.get("task_id")
+            project_name = config.get("project_name")
+            if task_id:
+                interactive_message = f"{interactive_message} (focus task {task_id})"
+            elif project_name:
+                interactive_message = f"{interactive_message} (focus project {project_name})"
+            console.print(interactive_message)
             command = input("enter command: ")
             command, entity, task_dict = process_command(command, config, repo)
             if command[0] == "q":
                 exit()
             command_handler.execute(command, entity, task_dict)
 
+def load_config(home_dir):
+        try:
+            with open(f"{home_dir}/.terka/config.yaml", encoding="utf-8") as f:
+                config = yaml.safe_load(f)
+            return config
+        except FileNotFoundError:
+            raise TerkaInitError("call `terka init` to initialize terka")
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `terka-1.5.5/src/service_layer/printer.py` & `terka-1.6.0/src/service_layer/printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-from typing import Any, Dict, List, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 from dataclasses import dataclass
+from operator import attrgetter
+import inspect
+from copy import deepcopy
 
 from collections import defaultdict
 from datetime import datetime, date, timedelta
 import rich
 from rich.console import Console
 from rich.table import Table
 from statistics import mean, median
@@ -14,14 +17,16 @@
 
 @dataclass
 class PrintOptions:
     show_tasks: bool = True
     show_history: bool = False
     show_commentaries: bool = False
     show_completed: bool = False
+    show_epics: bool = True
+    show_stories: bool = True
 
 
 class Printer:
 
     def __init__(self, repo, box=rich.box.SIMPLE) -> None:
         self.console = Console()
         self.box = box
@@ -60,33 +65,34 @@
             self.console.print(table)
 
     def print_entity(self,
                      task,
                      entity_type,
                      entities,
                      repo,
-                     print_options: PrintOptions = PrintOptions()):
+                     print_options: PrintOptions = PrintOptions(),
+                     kwargs: Optional[Dict[str, Any]] = None):
         if entity_type == "sprints":
             if entities:
-                self.print_sprint(entities, repo, print_options)
+                self.print_sprint(entities, repo, print_options, kwargs)
             else:
                 exit(f"No sprint with id '{task}' found!")
         if entity_type == "epics":
             if entities:
                 self.print_epic(entities, repo, print_options)
             else:
                 exit(f"No epic with id '{task}' found!")
         if entity_type == "stories":
             if entities:
                 self.print_story(entities, repo, print_options)
             else:
                 exit(f"No story with id '{task}' found!")
         if entity_type == "projects":
             if entities:
-                self.print_project(entities, print_options)
+                self.print_project(entities, print_options, kwargs)
             else:
                 exit(f"No project '{task}' found!")
         if entity_type == "tasks":
             if entities:
                 self.print_task(entities, repo, print_options)
             else:
                 print(f"No task with id '{task}' found!")
@@ -213,15 +219,15 @@
                             repo=repo,
                             print_options=print_options,
                             show_window=False)
         if i == 0 and print_options.show_commentaries and (
                 commentaries := entity.commentaries):
             self.print_commentaries(commentaries)
 
-    def print_sprint(self, entities, repo, print_options):
+    def print_sprint(self, entities, repo, print_options, kwargs=None):
         table = Table(box=rich.box.SQUARE_DOUBLE_HEAD)
         for column in ("id", "start_date", "end_date", "goal", "status",
                        "open tasks", "tasks", "velocity", "collaborators",
                        "time_spent"):
             table.add_column(column)
         for i, entity in enumerate(entities):
             story_points = []
@@ -263,25 +269,21 @@
                           str(time_spent))
         if table.row_count:
             self.console.print(table)
         if print_options.show_tasks:
             self.print_sprint_task(entities=tasks,
                                    repo=repo,
                                    show_completed=print_options.show_completed,
-                                   story_points=story_points)
+                                   story_points=story_points,
+                                   kwargs=kwargs)
         if i == 0 and print_options.show_commentaries and (
                 commentaries := entity.commentaries):
             self.print_commentaries(commentaries)
 
-    def print_project(
-        self,
-        entities,
-        # zero_tasks: bool = False,
-        # zero_tasks_only: bool = False,
-        print_options):
+    def print_project(self, entities, print_options, kwargs=None):
         table = Table(box=rich.box.SQUARE_DOUBLE_HEAD, expand=True)
         non_active_projects = Table(box=rich.box.SQUARE_DOUBLE_HEAD)
         for column in ("id", "name", "description", "status", "open_tasks",
                        "overdue", "backlog", "todo", "in_progress", "review",
                        "done", "median_task_age"):
             table.add_column(column)
         for column in ("id", "name", "description", "status", "open_tasks"):
@@ -323,47 +325,52 @@
                                             str(open_tasks))
 
         if table.row_count:
             self.console.print(table)
         if non_active_projects.row_count:
             self.console.print("[green]Inactive projects[/green]")
             self.console.print(non_active_projects)
-        if print_options.show_tasks:
-            not_tasks_print_options = PrintOptions(show_tasks=False)
-            if epics := entity.epics:
-                self.console.print("")
-                self.print_epic(epics, self.repo, not_tasks_print_options)
-            if stories := entity.stories:
-                self.console.print("")
-                self.print_story(stories, self.repo, not_tasks_print_options)
-            if tasks := entity.tasks:
-                self.print_task(entities=tasks,
-                                repo=self.repo,
-                                print_options=print_options,
-                                show_window=False)
+        non_task_view_options = deepcopy(print_options)
+        non_task_view_options.show_tasks = False
+        if print_options.show_epics and (epics := entity.epics):
+            self.console.print("")
+            self.print_epic(epics, self.repo, non_task_view_options)
+        if print_options.show_stories and (stories := entity.stories):
+            self.console.print("")
+            self.print_story(stories, self.repo, non_task_view_options)
+        if print_options.show_tasks and (tasks := entity.tasks):
+            self.console.print("")
+            self.print_task(entities=tasks,
+                            repo=self.repo,
+                            print_options=print_options,
+                            show_window=False,
+                            kwargs=kwargs)
         if print_options.show_commentaries and (commentaries :=
                                                 entity.commentaries):
             self.print_commentaries(commentaries)
         if print_options.show_history and (history := entity.history):
             self.print_history(history)
 
     def print_sprint_task(self,
                           entities,
                           repo,
                           show_completed=False,
                           history=None,
                           comments=None,
-                          story_points=None):
+                          story_points=None,
+                          kwargs=None):
         table = Table(box=self.box)
         default_columns = ("id", "name", "description", "story points",
                            "status", "priority", "project", "due_date", "tags",
                            "collaborators", "time_spent")
         for column in default_columns:
             table.add_column(column)
         entities = list(entities)
+        if kwargs:
+            entities = self._get_filtered_entities(entities, kwargs)
         completed_tasks = []
         completed_tasks_story_points = []
         printable_entities = 0
         for entity, story_point in sorted(zip(entities, story_points),
                                           key=lambda x: x[0].status.value,
                                           reverse=True):
             if tags := entity.tags:
@@ -398,15 +405,16 @@
                 continue
             printable_entities += 1
             entity_name = f"{entity.name}" if not comments else f"{entity.name} [blue][{len(comments)}][/blue]"
             if entity.due_date and entity.due_date <= date.today():
                 entity_id = f"[red]{entity.id}[/red]"
             elif (event_history := entity.history) and entity.status.name in (
                     "TODO", "IN_PROGRESS", "REVIEW"):
-                if max([event.date for event in event_history]) < (datetime.today() - timedelta(days=5)):
+                if max([event.date for event in event_history
+                        ]) < (datetime.today() - timedelta(days=5)):
                     entity_id = f"[yellow]{entity.id}[/yellow]"
                 else:
                     entity_id = str(entity.id)
             else:
                 entity_id = str(entity.id)
             table.add_row(str(entity_id), entity_name, entity.description,
                           str(story_point), entity.status.name, priority,
@@ -463,28 +471,31 @@
                 self.console.print(table)
 
     def print_task(self,
                    entities,
                    repo,
                    print_options,
                    custom_sort=None,
-                   show_window=True):
+                   show_window=True,
+                   kwargs=None):
         table = Table(box=self.box, title="TASKS")
         default_columns = ("id", "name", "description", "status", "priority",
                            "project", "due_date", "tags", "collaborators",
                            "time_spent")
         #TODO: Add printing for only a single task
         # if (entities[0].status.name == "DONE"):
         #     console.print(f"[green]task is completed on [/green]")
         # else:
         #     active_in_days = datetime.now() - entities[0].creation_date
         #     console.print(f"[blue]task is active {active_in_days.days} days[/blue]")
         for column in default_columns:
             table.add_column(column)
         entities = list(entities)
+        if kwargs:
+            entities = self._get_filtered_entities(entities, kwargs)
         completed_tasks = []
         if custom_sort:
             entities.sort(key=lambda c: getattr(c, custom_sort), reverse=False)
         else:
             entities.sort(key=lambda c: (c.status.value, c.priority.value),
                           reverse=True)
         printable_entities = 0
@@ -521,15 +532,16 @@
                 continue
             printable_entities += 1
             entity_name = f"{entity.name}" if not comments else f"{entity.name} [blue][{len(comments)}][/blue]"
             if entity.due_date and entity.due_date <= date.today():
                 entity_id = f"[red]{entity.id}[/red]"
             elif (event_history := entity.history) and entity.status.name in (
                     "TODO", "IN_PROGRESS", "REVIEW"):
-                if max([event.date for event in event_history]) < (datetime.today() - timedelta(days=5)):
+                if max([event.date for event in event_history
+                        ]) < (datetime.today() - timedelta(days=5)):
                     entity_id = f"[yellow]{entity.id}[/yellow]"
                 else:
                     entity_id = str(entity.id)
             else:
                 entity_id = str(entity.id)
             table.add_row(entity_id, entity_name, entity.description,
                           entity.status.name, priority, project,
@@ -618,7 +630,41 @@
         elif time_spent_hours:
             time_spent = f"{time_spent_hours}H"
         elif time_spent_minutes:
             time_spent = f"{time_spent_minutes}M"
         else:
             time_spent = ""
         return time_spent
+
+    def _get_filtered_entities(self, entities, kwargs):
+        if kwargs:
+            filtering_attributes = set(list(kwargs))
+            temp_entities = []
+            attributes = [
+                name for name, value in inspect.getmembers(entities[0])
+                if not name.startswith("_") and not inspect.ismethod(value)
+            ]
+            filtering_attributes = filtering_attributes.intersection(set(attributes))
+            attribute_getter = attrgetter(*filtering_attributes)
+            filtered_entities = []
+            for entity in entities:
+                should_add = False
+                for key, value in kwargs.items():
+                    if key in filtering_attributes:
+                        attribute_value = getattr(entity, key)
+                        if hasattr(attribute_value, "name"):
+                            if attribute_value.name != value:
+                                should_add = False
+                                break
+                            else:
+                                should_add = True
+                                continue
+                        elif attribute_value != value:
+                            should_add = False
+                            break
+                        else:
+                            should_add = True
+                            continue
+                if should_add:
+                    filtered_entities.append(entity)
+            entities = list(filtered_entities)
+        return entities
```

### Comparing `terka-1.5.5/src/service_layer/services.py` & `terka-1.6.0/src/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/service_layer/ui.py` & `terka-1.6.0/src/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/service_layer/vertical_layout.css` & `terka-1.6.0/src/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/src/utils.py` & `terka-1.6.0/src/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,22 @@
 def format_task_dict(config, entity, kwargs) -> Dict[str, Optional[str]]:
     if len(kwargs) > 1:
         new_dict = create_task_dict(kwargs)
         task_dict = {
             "id":
             new_dict.get("id") if entity != "commentaries" else None,
             "task_id":
-            new_dict.get("id") if entity == "commentaries" else None,
+            new_dict.get("id") or new_dict.get("task_id") if entity == "commentaries" else None,
             "name":
             new_dict.get("n") or new_dict.get("name"),
+            "num_log_entries": new_dict.get("L") or new_dict.get("lines"),
             "status":
             new_dict.get("s") or new_dict.get("status"),
             "project":
-            new_dict.get("p") or new_dict.get("project"),
+            new_dict.get("p") or new_dict.get("project") or new_dict.get("project_name"),
             "assignee":
             new_dict.get("a") or new_dict.get("assignee"),
             "due_date":
             new_dict.get("d") or new_dict.get("due-date"),
             "description":
             new_dict.get("desc") or new_dict.get("description"),
             "text":
@@ -69,14 +70,17 @@
             "story_id": new_dict.get("to-story") or new_dict.get("from-story") or new_dict.get("story"),
             "epic_id": new_dict.get("to-epic") or new_dict.get("from-epic") or new_dict.get("epic"),
             "story_points": new_dict.get("story-points"),
             "hours": new_dict.get("H"),
             "minutes": new_dict.get("M"),
             "show_history": new_dict.get("show-history"),
             "show_commentaries": new_dict.get("show-commentaries") or new_dict.get("show-comments"),
+            "epics": new_dict.get("epics"),
+            "stories": new_dict.get("stories"),
+            "tasks": new_dict.get("tasks"),
         }
         if "--show-completed" in kwargs:
             task_dict.update({"show_completed": True})
         if "--sort" in kwargs:
             sort_statement = kwargs[kwargs.index("--sort"):]
             task_dict.update(create_task_dict(sort_statement))
     elif len(kwargs) == 1:
@@ -105,14 +109,16 @@
             if entity != "commentaries":
                 task_dict["id"] = str(config.get("task_id"))
             if entity == "commentaries":
                 task_dict["task_id"] = str(config.get("task_id"))
 
     if not task_dict.get("project") and config.get("project_name"):
         task_dict["project"] = config.get("project_name")
+    if any(key in task_dict.keys() for key in ("epics", "stories", "tasks")):
+        task_dict["partial_project_view"] = True
     return task_dict
 
 
 def convert_status(status: str):
     conversion_dict = {
         "b": "BACKLOG",
         "t": "TODO",
@@ -135,37 +141,39 @@
         return due_date.strftime("%Y-%m-%d")
     return date
 
 
 def process_command(command: str, config: Dict[str, Any],
                     repo: AbsRepository) -> Tuple[str, str, Dict[Any, Any]]:
     task_dict = {}
+    task_list = []
     entity = None
     command, *rest = command.split(" ", maxsplit=2)
     if command[0] == "q":
         exit()
     if rest:
         entity, *task_dict = rest
         if task_dict:
             task_list = re.split(r'\s+(?=[^"]*(?:"[^"]*"[^"]*)*$)',
                                  task_dict[0])
             task_list = [
                 re.sub("['|\"]", "", element) for element in task_list
             ]
-            task_dict = format_task_dict(config, entity, task_list)
-        else:
-            task_dict = {}
+        task_dict = format_task_dict(config, entity, task_list)
+    else:
+        task_dict = {}
     task_dict = update_task_dict(task_dict, repo)
     return command, entity, task_dict
 
 
 def update_task_dict(task_dict: Dict[str, str],
                      repo: AbsRepository) -> Dict[str, str]:
     if (project := task_dict.get("project")):
-        task_dict["project"] = services.lookup_project_id(project, repo)
+        project_id = services.lookup_project_id(project, repo)
+        task_dict["project"] = project_id
     if (assignee := task_dict.get("assignee")):
         task_dict["assignee"] = services.lookup_user_id(assignee, repo)
     task_dict = convert_date_in_task_dict(task_dict)
     return task_dict
 
 
 def convert_date_in_task_dict(task_dict):
```

### Comparing `terka-1.5.5/terka.egg-info/PKG-INFO` & `terka-1.6.0/terka.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.5.5
+Version: 1.6.0
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.5.5/terka.egg-info/SOURCES.txt` & `terka-1.6.0/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/tests/test_orm.py` & `terka-1.6.0/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/tests/test_task.py` & `terka-1.6.0/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `terka-1.5.5/tests/test_user.py` & `terka-1.6.0/tests/test_user.py`

 * *Files identical despite different names*

