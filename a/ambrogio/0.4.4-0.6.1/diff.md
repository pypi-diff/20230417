# Comparing `tmp/ambrogio-0.4.4.tar.gz` & `tmp/ambrogio-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambrogio-0.4.4.tar", last modified: Fri Feb 17 15:36:25 2023, max compression
+gzip compressed data, was "ambrogio-0.6.1.tar", last modified: Mon Apr 17 17:31:00 2023, max compression
```

## Comparing `ambrogio-0.4.4.tar` & `ambrogio-0.6.1.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:36:25.872026 ambrogio-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-02-17 15:36:16.000000 ambrogio-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-17 15:36:16.000000 ambrogio-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-02-17 15:36:25.872026 ambrogio-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-17 15:36:16.000000 ambrogio-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:36:25.868026 ambrogio-0.4.4/ambrogio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:36:25.872026 ambrogio-0.4.4/ambrogio/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/cli/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/cli/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/cli/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:36:25.872026 ambrogio-0.4.4/ambrogio/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:36:25.872026 ambrogio-0.4.4/ambrogio/procedures/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/procedures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/procedures/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/procedures/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/procedures/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:36:25.872026 ambrogio-0.4.4/ambrogio/procedures/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/procedures/templates/basic.py.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/procedures/templates/step.py.tmpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:36:25.872026 ambrogio-0.4.4/ambrogio/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/utils/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/utils/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-02-17 15:36:16.000000 ambrogio-0.4.4/ambrogio/utils/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:36:25.872026 ambrogio-0.4.4/ambrogio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-02-17 15:36:25.000000 ambrogio-0.4.4/ambrogio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-17 15:36:25.000000 ambrogio-0.4.4/ambrogio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 15:36:25.000000 ambrogio-0.4.4/ambrogio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-17 15:36:25.000000 ambrogio-0.4.4/ambrogio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 15:36:25.000000 ambrogio-0.4.4/ambrogio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-17 15:36:25.000000 ambrogio-0.4.4/ambrogio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-17 15:36:25.000000 ambrogio-0.4.4/ambrogio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 15:36:25.872026 ambrogio-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-02-17 15:36:16.000000 ambrogio-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:36:25.872026 ambrogio-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-17 15:36:16.000000 ambrogio-0.4.4/tests/test_basic_procedure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-02-17 15:36:16.000000 ambrogio-0.4.4/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-02-17 15:36:16.000000 ambrogio-0.4.4/tests/test_step_procedure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:00.480868 ambrogio-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-17 17:30:51.000000 ambrogio-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-17 17:30:51.000000 ambrogio-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-17 17:31:00.480868 ambrogio-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-04-17 17:30:51.000000 ambrogio-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:00.476868 ambrogio-0.6.1/ambrogio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:00.480868 ambrogio-0.6.1/ambrogio/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/cli/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/cli/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/cli/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/cli/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:00.480868 ambrogio-0.6.1/ambrogio/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:00.480868 ambrogio-0.6.1/ambrogio/procedures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/procedures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/procedures/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/procedures/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/procedures/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/procedures/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:00.480868 ambrogio-0.6.1/ambrogio/procedures/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/procedures/templates/basic.py.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/procedures/templates/step.py.tmpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:00.480868 ambrogio-0.6.1/ambrogio/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/utils/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/utils/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-17 17:30:51.000000 ambrogio-0.6.1/ambrogio/utils/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:00.480868 ambrogio-0.6.1/ambrogio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-17 17:31:00.000000 ambrogio-0.6.1/ambrogio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-17 17:31:00.000000 ambrogio-0.6.1/ambrogio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:31:00.000000 ambrogio-0.6.1/ambrogio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-17 17:31:00.000000 ambrogio-0.6.1/ambrogio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:31:00.000000 ambrogio-0.6.1/ambrogio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 17:31:00.000000 ambrogio-0.6.1/ambrogio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 17:31:00.000000 ambrogio-0.6.1/ambrogio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:31:00.480868 ambrogio-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-17 17:30:51.000000 ambrogio-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:00.480868 ambrogio-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-17 17:30:51.000000 ambrogio-0.6.1/tests/test_basic_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-17 17:30:51.000000 ambrogio-0.6.1/tests/test_procedure_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-17 17:30:51.000000 ambrogio-0.6.1/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-17 17:30:51.000000 ambrogio-0.6.1/tests/test_step_procedure.py
```

### Comparing `ambrogio-0.4.4/LICENSE` & `ambrogio-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ambrogio-0.4.4/ambrogio/cli/dashboard.py` & `ambrogio-0.6.1/ambrogio/cli/dashboard.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from rich.columns import Columns
 from rich.panel import Panel
 from rich.live import Live
 
 from ambrogio.procedures import Procedure
 from ambrogio.utils.memory import format_bytes
 from ambrogio.utils.time import Timer
-from ambrogio.utils.threading import check_events
+from ambrogio.utils.threading import pause_event, wait_resume, check_events
 
 
 class Dashboard():
     """
     Show a dashboard with live performances monitoring.
 
     :param procedure: The procedure to monitor.
@@ -26,38 +26,42 @@
         'threads': 0
     }
     _procedure: Procedure
     _process: psutil.Process
     _timer: Timer
 
     def __init__(self, procedure: Procedure):
+        self._process = psutil.Process(os.getpid())
+        self._timer = Timer()
+
         self._procedure = procedure
 
     @property
     def procedure(self):
         return self._procedure
 
     @property
     def max_performances(self):
         return self._max_performances
 
     def show(self):
         """
         Show the dashboard.
         """
-        
-        self._process = psutil.Process(os.getpid())
-        self._timer = Timer()
 
-        with Live(self._generate_dashboard(), refresh_per_second=4) as live:
+        with Live(self._generate_dashboard(), refresh_per_second = 4) as live:
             while not self.procedure.finished and check_events():
                 live.update(self._generate_dashboard())
                 sleep(1/4)
             
             live.update(self._generate_dashboard())
+        
+        if pause_event.is_set():
+            wait_resume()
+            self.show()
 
     def _get_performances(self):
         """
         Get the performances of the current process.
 
         :return: A dict with the performances.
         """
@@ -78,38 +82,38 @@
         performances = self._get_performances()
         
         for key, value in performances.items():
             if value > self.max_performances[key]:
                 self.max_performances[key] = value
                 
         performance_table = Table(
-            show_header=True,
-            header_style='bold',
-            expand=True
+            show_header = True,
+            header_style = 'bold',
+            expand = True
         )
         
-        performance_table.add_column('Elapsed time', justify='right')
-        performance_table.add_column('Memory', justify='right')
-        performance_table.add_column('CPU', justify='right', min_width=10)
-        performance_table.add_column('Threads', justify='right')
+        performance_table.add_column('Elapsed time', justify = 'right')
+        performance_table.add_column('Memory', justify = 'right')
+        performance_table.add_column('CPU', justify = 'right', min_width = 10)
+        performance_table.add_column('Threads', justify = 'right')
 
         performance_table.add_row(
             self._timer.elapsed_time,
             format_bytes(performances['memory']),
             f"{performances['cpu']:.2f} %",
             f"{performances['threads']}",
-            end_section=True
+            end_section = True
         )
 
         performance_table.add_row(
             'Max',
             format_bytes(self.max_performances['memory']),
             f"{self.max_performances['cpu']:.2f} %",
             f"{self.max_performances['threads']}"
         )
 
         columns = Columns([
             Panel(performance_table, title='Performances'),
             *self.procedure._dashboard_widgets
-        ], expand=True)
+        ], expand = True)
 
         return columns
```

### Comparing `ambrogio-0.4.4/ambrogio/environment/__init__.py` & `ambrogio-0.6.1/ambrogio/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `ambrogio-0.4.4/ambrogio/procedures/basic.py` & `ambrogio-0.6.1/ambrogio/procedures/basic.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,20 +13,20 @@
         super().__init__(*args, **kwargs)
 
     def _execute(self) -> Any:
         """
         Execute the procedure.
         """
 
-        logging.info(f'Executing "{self.name}" procedure...')
+        self.logger.info(f'Executing "{self.name}" procedure...')
 
         result = self.execute()
         self._finished = True
         
-        logging.info(f'Procedure "{self.name}" executed successfully')
+        self.logger.info(f'Procedure "{self.name}" executed successfully')
 
         return result
 
     def execute(self) -> Any:
         """
         Execute the procedure.
         """
```

### Comparing `ambrogio-0.4.4/ambrogio/procedures/loader.py` & `ambrogio-0.6.1/ambrogio/procedures/loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import os
 from types import ModuleType
-from typing import List, Callable, Generator, Union
+from typing import TypeVar, List, Type, Generator, Union
 import inspect
 from importlib import import_module
 from pkgutil import iter_modules
 from configparser import ConfigParser
 
 from ambrogio.procedures import Procedure
+from ambrogio.procedures.basic import BasicProcedure
+from ambrogio.procedures.step import StepProcedure
+
+
+ProcedureType = TypeVar('ProcedureType', BasicProcedure, StepProcedure)
 
 
 def walk_modules(path: str) -> List[ModuleType]:
     """
     Loads a module and all its submodules from the given module path and
     returns them. If *any* module throws an exception while importing, that
     exception is thrown back.
@@ -89,15 +94,15 @@
         Return a list with the names of all procedures available in the project.
 
         :return: A list of procedure names.
         """
 
         return list(self._procedures.keys())
 
-    def load(self, procedure_name: str) -> Callable[[], Procedure]:
+    def load(self, procedure_name: str) -> Type[ProcedureType]:
         """
         Return the Procedure class for the given procedure name.
         If the procedure name is not found, raise a KeyError.
 
         :param procedure_name: The name of the procedure to load.
 
         :raises KeyError: If the procedure name is not found.
@@ -107,33 +112,35 @@
 
         try:
             return self._procedures[procedure_name]
 
         except KeyError:
             raise KeyError(f"Procedure not found: {procedure_name}")
 
-    def run(self, procedure_name: str):
+    def run(self, procedure_name: str) -> ProcedureType:
         """
         Run the Procedure execute method for the given procedure name.
         If the procedure name is not found, raise a KeyError.
 
         :param procedure_name: The name of the procedure to run.
 
         :raises KeyError: If the procedure name is not found.
 
-        :return: The Procedure class.
+        :return: The Procedure instance.
         """
 
-        procedure: Procedure = self.load(procedure_name)(self._project_path)
+        procedure: ProcedureType = self.load(procedure_name)(self.config)
         procedure._execute()
 
+        return procedure
+
     @staticmethod
     def iter_procedure_classes(
         module: ModuleType
-    ) -> Generator[Callable[[], Procedure], None, None]:
+    ) -> Generator[Type[Procedure], None, None]:
         """
         Return an iterator over all procedure classes defined in the given
         module that can be instantiated (i.e. which have name)
 
         :param module: The module to iterate over.
 
         :raises TypeError: If the module is not a module.
```

### Comparing `ambrogio-0.4.4/ambrogio/procedures/step.py` & `ambrogio-0.6.1/ambrogio/procedures/step.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import List, Optional, Callable, Any
 from threading import Thread
 import logging
 
 from rich.panel import Panel
-from rich.table import Column
 from rich.progress import Progress, TextColumn, BarColumn, TaskProgressColumn
 
 from ambrogio.procedures import Procedure
-from ambrogio.utils.threading import exit_event
+from ambrogio.utils.threading import exit_event, wait_resume
 
 
 class StepProcedure(Procedure):
     """
     Class for Ambrogio step procedures.
     """
 
     _steps: List[dict] = []
     _parallel_steps: List[Thread] = []
     _current_step: int = 0
     _completed_steps: int = 0
+    _failed_steps: int = 0
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     @property
     def current_step(self) -> Optional[dict]:
         """
@@ -59,23 +59,33 @@
 
         :return: The number of completed steps.
         """
 
         return self._completed_steps
 
     @property
+    def failed_steps(self) -> int:
+        """
+        The number of failed steps.
+
+        :return: The number of failed steps.
+        """
+
+        return self._failed_steps
+
+    @property
     def _dashboard_widgets(self) -> List[Panel]:
         """
         Additional widgets to be added to Ambrogio dashboard.
 
         :return: A list of Rich panels.
         """
 
         progress = Progress(
-            TextColumn("[progress.description]{task.description}"),
+            TextColumn('[progress.description]{task.description}'),
             BarColumn(),
             TaskProgressColumn(),
             expand=True,
             auto_refresh=False
         )
         
         progress.add_task(
@@ -88,131 +98,131 @@
         return [Panel(progress, title='Progress')]
 
     def _execute(self) -> Any:
         """
         Execute the procedure.
         """
 
-        logging.info(f'Executing "{self.name}" procedure...')
+        self.logger.info(f"Executing '{self.name}' procedure...")
 
-        self.setUp()
+        self.set_up()
 
         if not self.total_steps:
             raise ValueError('No steps added to the procedure')
 
         for step in self._steps:
             self._current_step += 1
 
             if step['parallel']:
                 parallel_step = Thread(
                     target=self._execute_step,
                     args=(step,)
                 )
                 
-                logging.debug(f'Starting parallel step "{step["name"]}"...')
+                self.logger.debug(f"Starting parallel step '{step['name']}'...")
                 parallel_step.start()
                 self._parallel_steps.append(parallel_step)
 
             else:
                 self._join_parallel_steps()
 
-                logging.debug(f'Executing step "{step["name"]}"...')
-                self._execute_step(step)
-
-            if exit_event.is_set():
-                break
-
-        self._join_parallel_steps()
+                wait_resume()
+                if not exit_event.is_set():
+                    self._execute_step(step)
+
+        wait_resume()
+        if not exit_event.is_set():
+            self._join_parallel_steps()
         
-        self._finished = True
+            self._finished = True
 
-        self.tearDown()
+            self.tear_down()
 
-        logging.info(f'Procedure "{self.name}" executed successfully')
+            self.logger.info(f"Procedure '{self.name}' executed successfully")
 
-    def setUp(self):
+    def set_up(self):
         """
         Method called before the execution of the procedure.
         Procedure steps can be added here.
         """
 
         pass
 
-    def tearDown(self):
+    def tear_down(self):
         """
         Method called after the execution of the procedure.
         """
 
         pass
 
     def add_step(
         self,
         function: Callable,
         name: Optional[str] = None,
         parallel: bool = False,
         blocking: bool = True,
-        *args,
-        **kwargs
+        params: Optional[dict] = None,
     ):
         """
         Add a step to the procedure.
 
         :param function: The function to be executed.
         :param name: The name of the step.
         :param parallel: If the step can be executed in a separate thread.
         :param blocking: If the step can block the execution of the procedure.
-        :param args: The arguments to pass to the function.
-        :param kwargs: The keyword arguments to pass to the function.
+        :param params: The parameters to be passed to the function.
 
         :raises ValueError: If the function is not callable.
         """
 
-        logging.debug(f'Adding step "{name}" to procedure "{self.name}"')
-
         if name is None:
             name = function.__name__
 
+        self.logger.debug(f"Adding step '{name}' to procedure '{self.name}'")
+
         self._steps.append({
             'function': function,
             'name': name,
             'parallel': parallel,
             'blocking': blocking,
-            'args': args,
-            'kwargs': kwargs
+            'params': params or {}
         })
 
     def _execute_step(self, step: dict):
         """
         Execute a step.
 
         If the step is blocking and it raises an exception the procedure
         execution will be stopped and the exit event will be set.
 
         :param step: The step to execute.
 
         :raises Exception: If the step raises an exception.
         """
 
+        self.logger.debug(f"Executing step '{step['name']}'...")
+
         try:
-            step['function'](*step['args'], **step['kwargs'])
+            step['function'](**step['params'])
             self._completed_steps += 1
 
+            self.logger.debug(f"Step '{step['name']}' executed successfully")
+
         except Exception as e:
-            logging.error(f'Step "{step["name"]}" raised an exception: {e}')
+            self.logger.error(f"Step '{step['name']}' raised an exception: {e}")
+            self._failed_steps += 1
 
             if step['blocking']:
-                logging.error('Stopping procedure execution')
+                self.logger.error('Stopping procedure execution')
                 exit_event.set()
                 raise e
 
-            raise e
-
     def _join_parallel_steps(self):
         """
         Join the parallel steps.
         """
 
-        logging.debug('Joining parallel steps...')
+        self.logger.debug('Joining parallel steps...')
 
         for step in self._parallel_steps:
             if step.is_alive():
                 step.join()
```

### Comparing `ambrogio-0.4.4/ambrogio/utils/project.py` & `ambrogio-0.6.1/ambrogio/utils/project.py`

 * *Files identical despite different names*

### Comparing `ambrogio-0.4.4/ambrogio/utils/time.py` & `ambrogio-0.6.1/ambrogio/utils/time.py`

 * *Files identical despite different names*

### Comparing `ambrogio-0.4.4/ambrogio.egg-info/SOURCES.txt` & `ambrogio-0.6.1/ambrogio.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,24 +9,27 @@
 ambrogio.egg-info/dependency_links.txt
 ambrogio.egg-info/entry_points.txt
 ambrogio.egg-info/not-zip-safe
 ambrogio.egg-info/requires.txt
 ambrogio.egg-info/top_level.txt
 ambrogio/cli/__init__.py
 ambrogio/cli/dashboard.py
+ambrogio/cli/logger.py
 ambrogio/cli/prompt.py
 ambrogio/cli/start.py
 ambrogio/environment/__init__.py
 ambrogio/procedures/__init__.py
 ambrogio/procedures/basic.py
 ambrogio/procedures/loader.py
+ambrogio/procedures/param.py
 ambrogio/procedures/step.py
 ambrogio/procedures/templates/basic.py.tmpl
 ambrogio/procedures/templates/step.py.tmpl
 ambrogio/utils/__init__.py
 ambrogio/utils/memory.py
 ambrogio/utils/project.py
 ambrogio/utils/threading.py
 ambrogio/utils/time.py
 tests/test_basic_procedure.py
+tests/test_procedure_params.py
 tests/test_project.py
 tests/test_step_procedure.py
```

### Comparing `ambrogio-0.4.4/setup.py` & `ambrogio-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 project_directory = Path(__file__).parent
 long_description = (project_directory / "README.md").read_text()
 
 setup(
     name='ambrogio',
-    version='0.4.4',
+    version='0.6.1',
 
     description='A simple framework to handle complex scripts.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     
     url='https://github.com/officinaMusci/ambrogio',
     project_urls={
```

### Comparing `ambrogio-0.4.4/tests/test_basic_procedure.py` & `ambrogio-0.6.1/tests/test_basic_procedure.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,21 +10,23 @@
     Test the basic procedure.
     """
 
     def test_basic_procedure(self):
         """
         Test the basic procedure.
         """
+
+        name = 'Test basic procedure'
         
         create_procedure(
-            'Basic procedure',
+            name,
             'basic',
             self.project_path
         )
 
         self.procedure_loader._load_all_procedures()
 
-        self.procedure_loader.run('Basic procedure')
+        self.procedure_loader.run(name)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ambrogio-0.4.4/tests/test_project.py` & `ambrogio-0.6.1/tests/test_project.py`

 * *Files identical despite different names*

