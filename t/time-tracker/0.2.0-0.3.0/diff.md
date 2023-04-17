# Comparing `tmp/time-tracker-0.2.0.tar.gz` & `tmp/time_tracker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time-tracker-0.2.0.tar", max compression
+gzip compressed data, was "time_tracker-0.3.0.tar", max compression
```

## Comparing `time-tracker-0.2.0.tar` & `time_tracker-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1069 2021-12-01 20:13:38.748888 time-tracker-0.2.0/LICENSE
--rw-r--r--   0        0        0     1256 2021-12-01 20:13:38.748888 time-tracker-0.2.0/README.md
--rw-r--r--   0        0        0      460 2021-12-01 20:13:38.748888 time-tracker-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-12-01 20:13:38.748888 time-tracker-0.2.0/time_tracker/__init__.py
--rw-r--r--   0        0        0     2739 2021-12-01 20:13:38.748888 time-tracker-0.2.0/time_tracker/log.py
--rw-r--r--   0        0        0     4826 2021-12-01 20:13:38.748888 time-tracker-0.2.0/time_tracker/main.py
--rw-r--r--   0        0        0     2027 2021-12-01 20:14:02.911772 time-tracker-0.2.0/setup.py
--rw-r--r--   0        0        0     1673 2021-12-01 20:14:02.912110 time-tracker-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-13 08:38:39.853413 time_tracker-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1256 2023-04-13 08:38:39.853577 time_tracker-0.3.0/README.md
+-rw-r--r--   0        0        0      536 2023-04-17 21:14:37.834140 time_tracker-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-13 08:38:39.855268 time_tracker-0.3.0/time_tracker/__init__.py
+-rw-r--r--   0        0        0     2739 2023-04-13 08:38:39.855527 time_tracker-0.3.0/time_tracker/log.py
+-rw-r--r--   0        0        0     4805 2023-04-13 08:43:50.542303 time_tracker-0.3.0/time_tracker/main.py
+-rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 time_tracker-0.3.0/PKG-INFO
```

### Comparing `time-tracker-0.2.0/LICENSE` & `time_tracker-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `time-tracker-0.2.0/README.md` & `time_tracker-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `time-tracker-0.2.0/time_tracker/log.py` & `time_tracker-0.3.0/time_tracker/log.py`

 * *Files identical despite different names*

### Comparing `time-tracker-0.2.0/time_tracker/main.py` & `time_tracker-0.3.0/time_tracker/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,16 +117,16 @@
 @app.command()
 def thoughts():
     """Retrieves all thoughts"""
     logger.retrieve_thoughts()
 
 
 @app.command()
-def log_folder():
-    """Prints the current log folder"""
+def info():
+    """Prints configs"""
 
     print(f"Log folder: {os.getenv('TT_LOG_FOLDER')}")
     print("To change log folder please set TT_LOG_FOLDER env var.")
 
 
 @app.command()
 def track(
```

### Comparing `time-tracker-0.2.0/setup.py` & `time_tracker-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,68 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: time-tracker
+Version: 0.3.0
+Summary: CLI to track time spent on tasks using pomodoro technique
+Author: Jose Cabeda
+Author-email: jecabeda@gmail.com
+Requires-Python: >=3.11,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Requires-Dist: python-dotenv (>=0.19.2,<0.20.0)
+Requires-Dist: typer (==0.7.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['time_tracker']
+# `time-tracker`
 
-package_data = \
-{'': ['*']}
+Time tracker cli
 
-install_requires = \
-['python-dotenv>=0.19.1,<0.20.0', 'typer==0.4.0']
-
-entry_points = \
-{'console_scripts': ['tt = time_tracker.main:app']}
-
-setup_kwargs = {
-    'name': 'time-tracker',
-    'version': '0.2.0',
-    'description': '',
-    'long_description': '# `time-tracker`\n\nTime tracker cli\n\n**Usage**:\n\n```console\n$ time-tracker [OPTIONS] COMMAND [ARGS]...\n```\n\n**Options**:\n\n* `--install-completion`: Install completion for the current shell.\n* `--show-completion`: Show completion for the current shell, to copy it or customize the installation.\n* `--help`: Show this message and exit.\n\n**Commands**:\n\n* `log`\n* `track`: Run depending on mode\n\n## `tt log`\n\n**Usage**:\n\n```console\n$ time-tracker log [OPTIONS]\n```\n\n**Options**:\n\n* `-l, --last`: Open last log file  [default: False]\n* `-o, --output`: Return log file content to terminal  [default: False]\n* `--help`: Show this message and exit.\n\n## `tt track`\n\nRun depending on mode\n\n**Usage**:\n\n```console\n$ tt track [OPTIONS]\n```\n\n**Options**:\n\n* `-w, --workDuration INTEGER`: Set work time (minutes)  [default: 25]\n* `-b, --breakDuration INTEGER`: Set break time (minutes)  [default: 5]\n* `-B, --bigBreakDuration INTEGER`: Set break time (minutes)  [default: 30]\n* `-m, --mode [manual|pomodoro]`: Set pomodoro mode. This will change the flow of work to 4 work sessions with small breaks and finish with a big Break  [default: pomodoro]\n* `-p, --prompt`: Set if it should prompt to go for next session  [default: True]\n* `--help`: Show this message and exit.\n',
-    'author': 'Jose Cabeda',
-    'author_email': 'jecabeda@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+**Usage**:
 
+```console
+$ time-tracker [OPTIONS] COMMAND [ARGS]...
+```
+
+**Options**:
+
+* `--install-completion`: Install completion for the current shell.
+* `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
+* `--help`: Show this message and exit.
+
+**Commands**:
+
+* `log`
+* `track`: Run depending on mode
+
+## `tt log`
+
+**Usage**:
+
+```console
+$ time-tracker log [OPTIONS]
+```
+
+**Options**:
+
+* `-l, --last`: Open last log file  [default: False]
+* `-o, --output`: Return log file content to terminal  [default: False]
+* `--help`: Show this message and exit.
+
+## `tt track`
+
+Run depending on mode
+
+**Usage**:
+
+```console
+$ tt track [OPTIONS]
+```
+
+**Options**:
+
+* `-w, --workDuration INTEGER`: Set work time (minutes)  [default: 25]
+* `-b, --breakDuration INTEGER`: Set break time (minutes)  [default: 5]
+* `-B, --bigBreakDuration INTEGER`: Set break time (minutes)  [default: 30]
+* `-m, --mode [manual|pomodoro]`: Set pomodoro mode. This will change the flow of work to 4 work sessions with small breaks and finish with a big Break  [default: pomodoro]
+* `-p, --prompt`: Set if it should prompt to go for next session  [default: True]
+* `--help`: Show this message and exit.
 
-setup(**setup_kwargs)
```

