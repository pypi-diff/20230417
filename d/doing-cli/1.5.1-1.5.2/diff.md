# Comparing `tmp/doing-cli-1.5.1.tar.gz` & `tmp/doing-cli-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doing-cli-1.5.1.tar", last modified: Wed Dec 28 12:36:41 2022, max compression
+gzip compressed data, was "doing-cli-1.5.2.tar", last modified: Mon Apr 17 18:40:29 2023, max compression
```

## Comparing `doing-cli-1.5.1.tar` & `doing-cli-1.5.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:36:41.633928 doing-cli-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2022-12-28 12:35:51.000000 doing-cli-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2022-12-28 12:36:41.633928 doing-cli-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2022-12-28 12:35:51.000000 doing-cli-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-28 12:36:41.633928 doing-cli-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2022-12-28 12:35:51.000000 doing-cli-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:36:41.629928 doing-cli-1.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:36:41.629928 doing-cli-1.5.1/src/doing/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:36:41.629928 doing-cli-1.5.1/src/doing/init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/init/_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/init/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:36:41.629928 doing-cli-1.5.1/src/doing/issue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/issue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/issue/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/issue/create_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/issue/open_issue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:36:41.629928 doing-cli-1.5.1/src/doing/list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9578 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/list/_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/list/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:36:41.629928 doing-cli-1.5.1/src/doing/open/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/open/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/open/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:36:41.633928 doing-cli-1.5.1/src/doing/pr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/pr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/pr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12509 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/pr/create_pr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/pr/list_pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/pr/open_pr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:36:41.633928 doing-cli-1.5.1/src/doing/workon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/workon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2022-12-28 12:35:51.000000 doing-cli-1.5.1/src/doing/workon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:36:41.633928 doing-cli-1.5.1/src/doing_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2022-12-28 12:36:41.000000 doing-cli-1.5.1/src/doing_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      863 2022-12-28 12:36:41.000000 doing-cli-1.5.1/src/doing_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 12:36:41.000000 doing-cli-1.5.1/src/doing_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-28 12:36:41.000000 doing-cli-1.5.1/src/doing_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2022-12-28 12:36:41.000000 doing-cli-1.5.1/src/doing_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-28 12:36:41.000000 doing-cli-1.5.1/src/doing_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-17 18:39:54.000000 doing-cli-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-17 18:40:29.755096 doing-cli-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-17 18:39:54.000000 doing-cli-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:40:29.755096 doing-cli-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-17 18:39:54.000000 doing-cli-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.751096 doing-cli-1.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.751096 doing-cli-1.5.2/src/doing/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/src/doing/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/init/_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/init/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/src/doing/issue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/issue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/issue/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/issue/create_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/issue/open_issue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/src/doing/list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/list/_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/list/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/src/doing/open/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/open/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/open/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/src/doing/pr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/pr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/pr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/pr/create_pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/pr/list_pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/pr/open_pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/src/doing/workon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/workon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/workon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/src/doing_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-17 18:40:29.000000 doing-cli-1.5.2/src/doing_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-17 18:40:29.000000 doing-cli-1.5.2/src/doing_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:40:29.000000 doing-cli-1.5.2/src/doing_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-17 18:40:29.000000 doing-cli-1.5.2/src/doing_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-17 18:40:29.000000 doing-cli-1.5.2/src/doing_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 18:40:29.000000 doing-cli-1.5.2/src/doing_cli.egg-info/top_level.txt
```

### Comparing `doing-cli-1.5.1/LICENSE` & `doing-cli-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.1/PKG-INFO` & `doing-cli-1.5.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doing-cli
-Version: 1.5.1
+Version: 1.5.2
 Summary: CLI tool to simplify the development workflow on azure devops
 Home-page: https://github.com/ing-bank/doing-cli
 Author: ING Bank N.V.
 Author-email: tim.vink@ing.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doing-cli-1.5.1/README.md` & `doing-cli-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.1/setup.py` & `doing-cli-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.1/src/doing/cli.py` & `doing-cli-1.5.2/src/doing/cli.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.1/src/doing/exceptions.py` & `doing-cli-1.5.2/src/doing/exceptions.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.1/src/doing/init/_init.py` & `doing-cli-1.5.2/src/doing/init/_init.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.1/src/doing/issue/commands.py` & `doing-cli-1.5.2/src/doing/issue/commands.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.1/src/doing/issue/create_issue.py` & `doing-cli-1.5.2/src/doing/issue/create_issue.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from rich.console import Console
 
 from doing.exceptions import InputError
-from doing.utils import get_az_devop_user_email, replace_user_aliases, run_command, validate_work_item_type
+from doing.utils import (
+    get_az_devop_user_email,
+    get_current_sprint,
+    replace_user_aliases,
+    run_command,
+    validate_work_item_type,
+)
 
 console = Console()
 
 
 def cmd_create_issue(
     title: str,
     mine: bool,
@@ -16,14 +22,15 @@
     parent: str,
     team: str,
     area: str,
     iteration: str,
     organization: str,
     project: str,
     story_points: str,
+    add_to_current_sprint: bool,
 ) -> int:
     """
     Create a new issue.
 
     Reference:
 
     - [`az boards work-item create]`(https://docs.microsoft.com/en-us/cli/azure/boards/work-item?view=azure-cli-latest#az-boards-work-item-create)
@@ -33,14 +40,17 @@
 
     if mine:
         assignee = get_az_devop_user_email()
 
     assignee = replace_user_aliases(assignee)
     validate_work_item_type(type)
 
+    if add_to_current_sprint:
+        iteration = get_current_sprint()
+
     cmd = "az boards work-item create "
     cmd += f'--title "{title}" '
     cmd += f'--type "{type}" '
     if assignee:
         cmd += f'--assigned-to "{assignee}" '
     if body:
         cmd += f'--description "{body}" '
```

### Comparing `doing-cli-1.5.1/src/doing/list/_list.py` & `doing-cli-1.5.2/src/doing/list/_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,14 @@
             iteration=iteration,
             last_build=False,
             show_state=show_state,
         ),
         refresh_per_second=4,
         console=console,
     ) as live:
-
         # For each PR, get linked work items. Note that "az repos pr list --include-links" does not work :(
         # Posted issue on bug here: https://github.com/Azure/azure-cli-extensions/issues/2946
         for pr_id in track(active_pullrequest_ids, description="Processing pull requests", transient=False):
             linked_workitems = run_command(
                 f'az repos pr work-item list --id {pr_id} --query "[].id" --org "{organization}"', allow_verbose=False
             )
             for work_item in linked_workitems:
```

### Comparing `doing-cli-1.5.1/src/doing/list/commands.py` & `doing-cli-1.5.2/src/doing/list/commands.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.1/src/doing/open/commands.py` & `doing-cli-1.5.2/src/doing/open/commands.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.1/src/doing/options.py` & `doing-cli-1.5.2/src/doing/options.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.1/src/doing/pr/commands.py` & `doing-cli-1.5.2/src/doing/pr/commands.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.1/src/doing/pr/create_pr.py` & `doing-cli-1.5.2/src/doing/pr/create_pr.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.1/src/doing/pr/list_pr.py` & `doing-cli-1.5.2/src/doing/pr/list_pr.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.1/src/doing/utils.py` & `doing-cli-1.5.2/src/doing/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -222,24 +222,25 @@
     if allow_verbose and verbose_shell():
         console.print(f"[bright_black]{command}[/bright_black]")
 
     encoding = get_config("encoding", "")
     if encoding == "":
         encoding = guess_shell_encoding()
 
+    timeout = int(get_config("timeout", 15))
     try:
         process = subprocess.run(
             command,
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             universal_newlines=True,
             encoding=encoding,
             shell=True,
-            timeout=15,
+            timeout=timeout,
         )
     except subprocess.TimeoutExpired as e:
         console.print(e)
         sys.exit(1)
 
     if process.returncode != 0:
         console.print(f"There was an error. Ran the following command with encoding '{encoding}':")
@@ -408,7 +409,26 @@
         "Risk",
     ]
 
     if type not in default_work_items:
         console.print(
             f"[dark_orange3]>[/dark_orange3] Warning: '[cyan]{type}[/cyan]' is not in the list of default work items"
         )
+
+
+def get_current_sprint():
+    organization = get_config("organization")
+    project = get_config("project")
+    team = get_config("team")
+    iteration = get_config("iteration")
+
+    cmd = "az boards iteration team list --timeframe current "
+    cmd += f'--project "{project}" --organization "{organization}" --team "{team}"'
+    iterations = run_command(cmd)
+    if len(iterations) == 0:
+        msg = "[dark_orange3]>[/dark_orange3] There is no current sprint, using default iteration: " + iteration
+        console.print(msg)
+        return iteration
+
+    current_sprint = str(iterations[0].get("path"))
+    console.print(current_sprint)
+    return current_sprint
```

### Comparing `doing-cli-1.5.1/src/doing/workon/commands.py` & `doing-cli-1.5.2/src/doing/workon/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,23 @@
     required=False,
     default="User Story",
     type=click.Choice(["Bug", "Epic", "Feature", "Issue", "Task", "Test Case", "User Story"]),
     help='Type of work item. Defaults to "User Story"',
     show_envvar=True,
 )
 @click.option(
+    "--label",
+    "-l",
+    required=False,
+    default="",
+    type=str,
+    help="Attach tags (labels) to work item. Comma separate multiple tags.",
+    show_envvar=True,
+)
+@click.option(
     "--parent",
     "-p",
     required=False,
     default="",
     type=str,
     help="To create a child work item, specify the ID of the parent work item.",
     show_envvar=True,
@@ -91,27 +100,37 @@
     "--branch-prefix",
     required=False,
     default="",
     type=str,
     help='The prefix to be prepended to the branch name. Defaults to ""',
     show_envvar=True,
 )
+@click.option(
+    "--add-to-current-sprint/--do-not-add-to-current-sprint",
+    required=False,
+    default=False,
+    type=bool,
+    help="If the item needs to be added to the current sprint. Defaults to false",
+    show_envvar=True,
+)
 def workon(
     issue,
     type,
+    label: str,
     parent,
     reviewers,
     draft: bool,
     auto_complete: bool,
     self_approve: bool,
     checkout: bool,
     delete_source_branch: bool,
     story_points,
     default_branch,
     branch_prefix: str,
+    add_to_current_sprint,
 ):
     """
     Create issue with PR and switch git branch.
 
     Create self-assigned issue, draft pull request and switch git branch all in one go.
 
     ISSUE is the title to be used for the new work item.
@@ -121,19 +140,20 @@
 
     # Create the issue. Note we changed some defaults:
     # - it's assigned to self (mine = True)
     work_item_id = cmd_create_issue(
         title=issue,
         mine=True,
         assignee="",
-        label="",
+        label=label,
         body="",
         type=type,
         parent=parent,
         story_points=story_points,
+        add_to_current_sprint=add_to_current_sprint,
         **get_common_options(),
     )
 
     # Open a PR.
     cmd_create_pr(
         work_item_id=str(work_item_id),
         draft=draft,  # Default true, note: `doing create pr` defaults to False
```

### Comparing `doing-cli-1.5.1/src/doing_cli.egg-info/PKG-INFO` & `doing-cli-1.5.2/src/doing_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doing-cli
-Version: 1.5.1
+Version: 1.5.2
 Summary: CLI tool to simplify the development workflow on azure devops
 Home-page: https://github.com/ing-bank/doing-cli
 Author: ING Bank N.V.
 Author-email: tim.vink@ing.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doing-cli-1.5.1/src/doing_cli.egg-info/SOURCES.txt` & `doing-cli-1.5.2/src/doing_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

