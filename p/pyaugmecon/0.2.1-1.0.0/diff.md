# Comparing `tmp/pyaugmecon-0.2.1.tar.gz` & `tmp/pyaugmecon-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaugmecon-0.2.1.tar", last modified: Tue Apr  4 17:32:03 2023, max compression
+gzip compressed data, was "pyaugmecon-1.0.0.tar", last modified: Mon Apr 17 13:16:57 2023, max compression
```

## Comparing `pyaugmecon-0.2.1.tar` & `pyaugmecon-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 whbles    (1000) whbles    (1000)        0 2023-04-04 17:32:03.365168 pyaugmecon-0.2.1/
--rw-r--r--   0 whbles    (1000) whbles    (1000)     1164 2021-10-16 20:28:36.000000 pyaugmecon-0.2.1/LICENSE
--rw-r--r--   0 whbles    (1000) whbles    (1000)    27360 2023-04-04 17:32:03.365168 pyaugmecon-0.2.1/PKG-INFO
--rw-r--r--   0 whbles    (1000) whbles    (1000)    25283 2023-04-04 17:14:23.000000 pyaugmecon-0.2.1/README.md
-drwxr-xr-x   0 whbles    (1000) whbles    (1000)        0 2023-04-04 17:32:03.325168 pyaugmecon-0.2.1/pyaugmecon/
--rw-r--r--   0 whbles    (1000) whbles    (1000)       45 2021-10-16 20:28:36.000000 pyaugmecon-0.2.1/pyaugmecon/__init__.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)      632 2023-04-04 17:14:23.000000 pyaugmecon-0.2.1/pyaugmecon/flag.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)     1569 2023-04-04 17:14:23.000000 pyaugmecon-0.2.1/pyaugmecon/helper.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)      778 2023-04-04 17:14:23.000000 pyaugmecon-0.2.1/pyaugmecon/logs.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)     5805 2023-04-04 17:14:23.000000 pyaugmecon-0.2.1/pyaugmecon/model.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)     2713 2023-04-04 17:14:23.000000 pyaugmecon-0.2.1/pyaugmecon/options.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)     1672 2023-04-04 17:14:23.000000 pyaugmecon-0.2.1/pyaugmecon/process_handler.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)     5260 2023-04-04 17:14:23.000000 pyaugmecon-0.2.1/pyaugmecon/pyaugmecon.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)     2206 2023-04-04 17:14:23.000000 pyaugmecon-0.2.1/pyaugmecon/queue_handler.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)     4172 2023-04-04 17:14:23.000000 pyaugmecon-0.2.1/pyaugmecon/solver_process.py
-drwxr-xr-x   0 whbles    (1000) whbles    (1000)        0 2023-04-04 17:32:03.355168 pyaugmecon-0.2.1/pyaugmecon.egg-info/
--rw-r--r--   0 whbles    (1000) whbles    (1000)    27360 2023-04-04 17:32:02.000000 pyaugmecon-0.2.1/pyaugmecon.egg-info/PKG-INFO
--rw-r--r--   0 whbles    (1000) whbles    (1000)      431 2023-04-04 17:32:03.000000 pyaugmecon-0.2.1/pyaugmecon.egg-info/SOURCES.txt
--rw-r--r--   0 whbles    (1000) whbles    (1000)        1 2023-04-04 17:32:02.000000 pyaugmecon-0.2.1/pyaugmecon.egg-info/dependency_links.txt
--rw-r--r--   0 whbles    (1000) whbles    (1000)      107 2023-04-04 17:32:02.000000 pyaugmecon-0.2.1/pyaugmecon.egg-info/requires.txt
--rw-r--r--   0 whbles    (1000) whbles    (1000)       11 2023-04-04 17:32:02.000000 pyaugmecon-0.2.1/pyaugmecon.egg-info/top_level.txt
--rw-r--r--   0 whbles    (1000) whbles    (1000)       38 2023-04-04 17:32:03.365168 pyaugmecon-0.2.1/setup.cfg
--rw-r--r--   0 whbles    (1000) whbles    (1000)     1843 2023-04-04 17:27:18.000000 pyaugmecon-0.2.1/setup.py
+drwxr-xr-x   0 whbles    (1000) whbles    (1000)        0 2023-04-17 13:16:57.217151 pyaugmecon-1.0.0/
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     1164 2021-10-16 20:28:36.000000 pyaugmecon-1.0.0/LICENSE
+-rw-r--r--   0 whbles    (1000) whbles    (1000)    28216 2023-04-17 13:16:57.217151 pyaugmecon-1.0.0/PKG-INFO
+-rw-r--r--   0 whbles    (1000) whbles    (1000)    26087 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/README.md
+drwxr-xr-x   0 whbles    (1000) whbles    (1000)        0 2023-04-17 13:16:57.217151 pyaugmecon-1.0.0/pyaugmecon/
+-rw-r--r--   0 whbles    (1000) whbles    (1000)       45 2021-10-16 20:28:36.000000 pyaugmecon-1.0.0/pyaugmecon/__init__.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     1349 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/flag.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     2483 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/helper.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     1295 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/logs.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)    11055 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/model.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     4029 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/options.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     2616 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/process_handler.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     9360 2023-04-17 13:10:50.000000 pyaugmecon-1.0.0/pyaugmecon/pyaugmecon.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     4230 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/queue_handler.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     6603 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/solver_process.py
+drwxr-xr-x   0 whbles    (1000) whbles    (1000)        0 2023-04-17 13:16:57.217151 pyaugmecon-1.0.0/pyaugmecon.egg-info/
+-rw-r--r--   0 whbles    (1000) whbles    (1000)    28216 2023-04-17 13:16:57.000000 pyaugmecon-1.0.0/pyaugmecon.egg-info/PKG-INFO
+-rw-r--r--   0 whbles    (1000) whbles    (1000)      431 2023-04-17 13:16:57.000000 pyaugmecon-1.0.0/pyaugmecon.egg-info/SOURCES.txt
+-rw-r--r--   0 whbles    (1000) whbles    (1000)        1 2023-04-17 13:16:57.000000 pyaugmecon-1.0.0/pyaugmecon.egg-info/dependency_links.txt
+-rw-r--r--   0 whbles    (1000) whbles    (1000)      107 2023-04-17 13:16:57.000000 pyaugmecon-1.0.0/pyaugmecon.egg-info/requires.txt
+-rw-r--r--   0 whbles    (1000) whbles    (1000)       11 2023-04-17 13:16:57.000000 pyaugmecon-1.0.0/pyaugmecon.egg-info/top_level.txt
+-rw-r--r--   0 whbles    (1000) whbles    (1000)       38 2023-04-17 13:16:57.217151 pyaugmecon-1.0.0/setup.cfg
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     1843 2023-04-17 13:13:24.000000 pyaugmecon-1.0.0/setup.py
```

### Comparing `pyaugmecon-0.2.1/LICENSE` & `pyaugmecon-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaugmecon-0.2.1/PKG-INFO` & `pyaugmecon-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaugmecon
-Version: 0.2.1
+Version: 1.0.0
 Home-page: https://github.com/wouterbles/pyaugmecon
 Author: Wouter Bles
 Author-email: whbles@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/wouterbles/pyaugmecon/blob/main/CHANGELOG.md
 Keywords: python,pyomo,optimization,multi-objective-optimization,augmecon
 Classifier: Development Status :: 3 - Alpha
@@ -121,33 +121,39 @@
 
 ```python
 from pyaugmecon import PyAugmecon
 from tests.optimization_models import three_kp_model
 
 # Multiprocessing requires this If statement (on Windows)
 if __name__ == "__main__":
-    model_type = '3kp40'
+    model_type = "3kp40"
 
     # AUGMECON related options
     opts = {
-        'name': model_type,
-        'grid_points': 540,
-        'nadir_points': [1031, 1069],
-        }
-
-    # Options passed to Gurobi
-    solver_opts = {}
-
-    A = PyAugmecon(three_kp_model(model_type), opts, solver_opts) # instantiate  PyAugmecon
-    A.solve() # solve PyAugmecon multi-objective optimization problem
-    print(A.model.payoff) # this prints the payoff table
-    print(A.unique_pareto_sols) # this prints the unique Pareto optimal solutions
+        "name": model_type,
+        "grid_points": 540,
+        "nadir_points": [1031, 1069],
+    }
+
+    pyaugmecon = PyAugmecon(three_kp_model(model_type), opts)  # instantiate  PyAugmecon
+    pyaugmecon.solve()  # solve PyAugmecon multi-objective optimization problem
+    sols = pyaugmecon.get_pareto_solutions()  # get all pareto solutions
+    payoff = pyaugmecon.get_payoff_table()  # get the payoff table
+    decision_vars = pyaugmecon.get_decision_variables(sols[0])  # get the decision variables
 ```
 
-### PyAugmecon object attributes
+### PyAugmecon methods
+
+| Name                     | Description                                                                                                                                             |
+| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `get_pareto_solutions()`    | Get a list of Pareto-optimal solutions (`list[tuple]`) |
+| `get_decision_variables(pareto_solution)` | Get a dictionary of decision variables for a given Pareto-optimal solution. Where the key represents the decision variable name and the value is a pd.Series with the values. |
+| `get_payoff_table()`  | Get the payoff table from the model. |
+
+### PyAugmecon attributes
 
 After solving the model with `PyAugmecon.solve()`, the following object attributes are available:
 
 | Name                     | Description                                                                                                                                             |
 | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `sols`                   | Full unprocessed solutions, only checked for uniqueness                                                                                                 |
 | `unique_sols`            | Unique solutions, rounded to `round_decimals` and checked for uniqueness                                                                                |
@@ -341,14 +347,18 @@
 
 - Wouter Bles (current version of the package)
 - Nikolaos Paterakis (initial implementation)
 
 
 # Changelog
 
+## 1.0.0
+
+- Add new methods for solution retrieval
+
 ## 0.2.1
 
 - Add Python 3.10 to supported versions
 
 ## 0.2.0
 
 - Decision variables are now stored in a dictionary together with the objective values
```

### Comparing `pyaugmecon-0.2.1/README.md` & `pyaugmecon-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -93,33 +93,39 @@
 
 ```python
 from pyaugmecon import PyAugmecon
 from tests.optimization_models import three_kp_model
 
 # Multiprocessing requires this If statement (on Windows)
 if __name__ == "__main__":
-    model_type = '3kp40'
+    model_type = "3kp40"
 
     # AUGMECON related options
     opts = {
-        'name': model_type,
-        'grid_points': 540,
-        'nadir_points': [1031, 1069],
-        }
-
-    # Options passed to Gurobi
-    solver_opts = {}
-
-    A = PyAugmecon(three_kp_model(model_type), opts, solver_opts) # instantiate  PyAugmecon
-    A.solve() # solve PyAugmecon multi-objective optimization problem
-    print(A.model.payoff) # this prints the payoff table
-    print(A.unique_pareto_sols) # this prints the unique Pareto optimal solutions
+        "name": model_type,
+        "grid_points": 540,
+        "nadir_points": [1031, 1069],
+    }
+
+    pyaugmecon = PyAugmecon(three_kp_model(model_type), opts)  # instantiate  PyAugmecon
+    pyaugmecon.solve()  # solve PyAugmecon multi-objective optimization problem
+    sols = pyaugmecon.get_pareto_solutions()  # get all pareto solutions
+    payoff = pyaugmecon.get_payoff_table()  # get the payoff table
+    decision_vars = pyaugmecon.get_decision_variables(sols[0])  # get the decision variables
 ```
 
-### PyAugmecon object attributes
+### PyAugmecon methods
+
+| Name                     | Description                                                                                                                                             |
+| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `get_pareto_solutions()`    | Get a list of Pareto-optimal solutions (`list[tuple]`) |
+| `get_decision_variables(pareto_solution)` | Get a dictionary of decision variables for a given Pareto-optimal solution. Where the key represents the decision variable name and the value is a pd.Series with the values. |
+| `get_payoff_table()`  | Get the payoff table from the model. |
+
+### PyAugmecon attributes
 
 After solving the model with `PyAugmecon.solve()`, the following object attributes are available:
 
 | Name                     | Description                                                                                                                                             |
 | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `sols`                   | Full unprocessed solutions, only checked for uniqueness                                                                                                 |
 | `unique_sols`            | Unique solutions, rounded to `round_decimals` and checked for uniqueness                                                                                |
```

### Comparing `pyaugmecon-0.2.1/pyaugmecon/model.py` & `pyaugmecon-1.0.0/pyaugmecon/solver_process.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,180 +1,164 @@
 import logging
-import os
+from multiprocessing import Process
 
-import cloudpickle
-import numpy as np
-import pandas as pd
-import pyomo.environ as pyo
-from pyomo.core.base import (
-    Any,
-    ConstraintList,
-    NonNegativeReals,
-    Param,
-    Set,
-    Var,
-    maximize,
-    minimize,
-)
-
-from pyaugmecon.helper import Counter, ProgressBar
+from pyaugmecon.flag import Flag
+from pyaugmecon.model import Model
 from pyaugmecon.options import Options
+from pyaugmecon.queue_handler import QueueHandler
 
 
-class Model(object):
-    def __init__(self, model: pyo.ConcreteModel, opts: Options):
-        self.model = model
+class SolverProcess(Process):
+    def __init__(self, p_num, opts: Options, model: Model, queues: QueueHandler, flag: Flag):
+        """
+        Initialize the SolverProcess object.
+
+        Parameters
+        ----------
+        p_num : int
+            The process number.
+        opts : Options
+            The options object.
+        model : Model
+            The model object.
+        queues : QueueHandler
+            The queue handler object.
+        flag : Flag
+            The flag object.
+
+        """
+        super().__init__()
+        self.p_num = p_num
         self.opts = opts
-        self.logger = logging.getLogger(opts.log_name)
-
-        self.n_obj = len(self.model.obj_list)
-        self.iter_obj = range(self.n_obj)
-        self.iter_obj2 = range(self.n_obj - 1)
-
-        # Setup progress bar
-        self.to_solve = self.opts.gp ** (self.n_obj - 1) + self.n_obj**2
-        self.progress = ProgressBar(Counter(), self.to_solve)
-
-        self.models_solved = Counter()
-        self.infeasibilities = Counter()
-
-        if self.n_obj < 2:
-            raise Exception("Too few objective functions provided")
-
-    def obj(self, i):
-        return self.model.obj_list[i + 1]
-
-    def obj_val(self, i):
-        return self.obj(i)()
-
-    def obj_expr(self, i):
-        return self.obj(i).expr
-
-    def obj_sense(self, i):
-        return self.obj(i).sense
-
-    def slack_val(self, i):
-        return self.model.Slack[i + 1].value
-
-    def obj_activate(self, i):
-        self.obj(i).activate()
-
-    def obj_deactivate(self, i):
-        self.obj(i).deactivate()
-
-    def solve(self):
-        opt = pyo.SolverFactory(self.opts.solver_name, solver_io=self.opts.solver_io)
-        opt.options.update(self.opts.solver_opts)
-        self.result = opt.solve(self.model)
-        self.term = self.result.solver.termination_condition
-        self.status = self.result.solver.status
-
-    def get_vars(self):
-        model_vars = self.model.component_map(ctype=Var, active=True)
-        vars_dict = {
-            v.name: pd.Series(v.extract_values(), index=v.extract_values().keys()) for v in model_vars.values()
-        }
-        return vars_dict
-
-    def pickle(self):
-        model_file = open(self.opts.model_fn, "wb")
-        cloudpickle.dump(self.model, model_file)
-        del self.model
-
-    def unpickle(self):
-        model_file = open(self.opts.model_fn, "rb")
-        self.model = cloudpickle.load(model_file)
-
-    def clean(self):
-        if os.path.exists(self.opts.model_fn):
-            os.remove(self.opts.model_fn)
-
-    def is_optimal(self):
-        return self.status == pyo.SolverStatus.ok and self.term == pyo.TerminationCondition.optimal
-
-    def is_infeasible(self):
-        return (
-            self.term == pyo.TerminationCondition.infeasible
-            or self.term == pyo.TerminationCondition.infeasibleOrUnbounded
-        )
-
-    def min_to_max(self):
-        self.obj_goal = [-1 if self.obj_sense(o) == minimize else 1 for o in self.iter_obj]
-
-        for o in self.iter_obj:
-            if self.obj_sense(o) == minimize:
-                self.model.obj_list[o + 1].sense = maximize
-                self.model.obj_list[o + 1].expr = -1 * self.model.obj_list[o + 1].expr
-
-    def construct_payoff(self):
-        self.logger.info("Constructing payoff")
-        self.progress.set_message("constructing payoff")
-
-        def set_payoff(i, j):
-            self.obj_activate(j)
-            self.solve()
-            self.progress.increment()
-            self.payoff[i, j] = self.obj_val(j)
-            self.obj_deactivate(j)
-
-        self.payoff = np.full((self.n_obj, self.n_obj), np.inf)
-        self.model.pcon_list = ConstraintList()
-
-        # Independently optimize each objective function (diagonal elements)
-        for i in self.iter_obj:
-            for j in self.iter_obj:
-                if i == j:
-                    set_payoff(i, j)
-
-        # Optimize j having all the i as constraints (off-diagonal elements)
-        for i in self.iter_obj:
-            self.model.pcon_list.add(expr=self.obj_expr(i) == self.payoff[i, i])
-
-            for j in self.iter_obj:
-                if i != j:
-                    set_payoff(i, j)
-                    self.model.pcon_list.add(expr=self.obj_expr(j) == self.payoff[i, j])
-
-            self.model.pcon_list.clear()
-
-    def find_obj_range(self):
-        self.logger.info("Finding objective function range")
-
-        # Gridpoints of p-1 objective functions that are used as constraints
-        self.e = np.zeros((self.n_obj - 1, self.opts.gp))
-        self.obj_range = np.zeros(self.n_obj - 1)
-
-        for i in self.iter_obj2:
-            if self.opts.nadir_p:
-                min = self.opts.nadir_p[i]
-            else:
-                min = self.opts.nadir_r * np.min(self.payoff[:, i + 1], 0)
-
-            max = np.max(self.payoff[:, i + 1], 0)
-            self.obj_range[i] = max - min
-            self.e[i] = [min + j * (self.obj_range[i] / (self.opts.gp - 1)) for j in range(0, self.opts.gp)]
-
-    def convert_prob(self):
-        self.logger.info("Converting optimization problem")
-
-        self.model.con_list = ConstraintList()
-
-        # Set of objective functions
-        self.model.Os = Set(ordered=True, initialize=[o + 2 for o in self.iter_obj2])
-
-        # Slack for objectives introduced as constraints
-        self.model.Slack = Var(self.model.Os, within=NonNegativeReals)
-        self.model.e = Param(
-            self.model.Os,
-            within=Any,
-            mutable=True,
-        )  # RHS of constraints
-
-        # Add p-1 objective functions as constraints
-        for o in range(1, self.n_obj):
-            self.model.obj_list[1].expr += self.opts.eps * (
-                10 ** (-1 * (o - 1)) * self.model.Slack[o + 1] / self.obj_range[o - 1]
-            )
-
-            self.model.con_list.add(
-                expr=self.model.obj_list[o + 1].expr - self.model.Slack[o + 1] == self.model.e[o + 1]
-            )
+        self.model = model
+        self.queues = queues
+        self.flag = flag
+        self.logger = None
+
+    def run(self):
+        """
+        Run the SolverProcess.
+
+        This function runs the SolverProcess. It retrieves work items from the queue and processes them until there is
+        no more work to do. For each work item, it sets up the model and solves it. If the `early_exit` flag is set to
+        True and the model is infeasible, the function sets the flag and jumps to the next work item. If the `bypass`
+        flag is set to True and the model is optimal, the function sets the flag and jumps to the next work item. If
+        the model is optimal, the function calculates the solutions and puts them in the result queue.
+
+        """
+        jump = 0  # Initialize variable 'jump' to zero
+
+        # Check if process logging is enabled
+        if self.opts.process_logging:
+            # If enabled, initialize logger with log name provided in 'self.opts.log_name'
+            self.logger = logging.getLogger(self.opts.log_name)
+            self.logger.setLevel(logging.INFO)  # Set log level to INFO
+
+        # Load pickled model
+        self.model.unpickle()
+
+        # Run indefinitely until there's no more work
+        while True:
+            # Get work from queue for this process number
+            work = self.queues.get_work(self.p_num)
+
+            # If no more work, break the loop
+            if not work:
+                break
+
+            # Process each job in the work list
+            for c in work:
+                log = f"Process: {self.p_num}, index: {c}, "  # Initialize logging string
+                cp_end = self.opts.gp - 1  # Set the end index for this job
+                self.model.progress.increment()  # Increment progress counter for this model
+
+                # Define helper functions to handle jump, bypass, and early exit scenarios
+                def do_jump(i, jump):
+                    return min(jump, abs(cp_end - i))
+
+                def bypass_range(i):
+                    if i == 0:
+                        return range(c[i], c[i] + 1)
+                    else:
+                        return range(c[i], c[i] + b[i] + 1)
+
+                def early_exit_range(i):
+                    if i == 0:
+                        return range(c[i], c[i] + 1)
+                    else:
+                        return range(c[i], cp_end)
+
+                # Check if flag is enabled and if the current job has a flag set
+                if self.opts.flag and self.flag.get(c) != 0 and jump == 0:
+                    # If jump is not set and there's a flag for this job, set jump
+                    jump = do_jump(c[0] - 1, self.flag.get(c))
+
+                # If jump is set, skip to the next iteration of the loop
+                if jump > 0:
+                    jump = jump - 1
+                    continue
+
+                # Log model progress for each objective
+                for o in self.model.iter_obj2:
+                    log += f"e{o + 1}: {self.model.e[o, c[o]]}, "
+                    self.model.model.e[o + 2] = self.model.e[o, c[o]]
+
+                # Activate objective 0 and solve the model
+                self.model.obj_activate(0)
+                self.model.solve()
+                self.model.models_solved.increment()
+
+                # Check if early exit is enabled and if the model is infeasible
+                if self.opts.early_exit and self.model.is_infeasible():
+                    # If so, increment infeasibilities counter
+                    self.model.infeasibilities.increment()
+
+                    # Set flag if flag is enabled
+                    if self.opts.flag:
+                        self.flag.set(early_exit_range, self.opts.gp, self.model.iter_obj2)
+
+                    jump = do_jump(c[0], self.opts.gp)  # Set jump
+                    log += "infeasible"  # Log infeasibility
+
+                    # Log progress if process logging is enabled
+                    if self.opts.process_logging:
+                        self.logger.info(log)
+
+                    continue  # Skip to next iteration of loop
+
+                # Calculate slack values and set jump if bypass is enabled
+                elif self.opts.bypass and self.model.is_optimal():
+                    b = []
+                    for i in self.model.iter_obj2:
+                        step = self.model.obj_range[i] / (self.opts.gp - 1)
+                        slack = round(self.model.slack_val(i + 1))
+                        b.append(int(slack / step))
+
+                    # Log jump and set flag if enabled
+                    log += f"jump: {b[0]}, "
+                    if self.opts.flag:
+                        self.flag.set(bypass_range, b[0] + 1, self.model.iter_obj2)
+                    jump = do_jump(c[0], b[0])
+
+                # If model is optimal, calculate and log solutions
+                sols = []
+                if self.model.is_optimal():
+                    sols.append(
+                        self.model.obj_val(0)
+                        - self.opts.eps
+                        * sum(
+                            10 ** (-1 * (o)) * self.model.slack_val(o + 1) / self.model.obj_range[o]
+                            for o in self.model.iter_obj2
+                        )
+                    )
+
+                    for o in self.model.iter_obj2:
+                        sols.append(self.model.obj_val(o + 1))
+
+                    # Put results into queue as a dictionary
+                    sols_dict = {tuple(sols): self.model.get_vars()}
+                    self.queues.put_result(sols_dict)
+
+                    # Log solutions if process logging is enabled
+                    log += f"solutions: {sols}"
+                    if self.opts.process_logging:
+                        self.logger.info(log)
```

### Comparing `pyaugmecon-0.2.1/pyaugmecon.egg-info/PKG-INFO` & `pyaugmecon-1.0.0/pyaugmecon.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaugmecon
-Version: 0.2.1
+Version: 1.0.0
 Home-page: https://github.com/wouterbles/pyaugmecon
 Author: Wouter Bles
 Author-email: whbles@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/wouterbles/pyaugmecon/blob/main/CHANGELOG.md
 Keywords: python,pyomo,optimization,multi-objective-optimization,augmecon
 Classifier: Development Status :: 3 - Alpha
@@ -121,33 +121,39 @@
 
 ```python
 from pyaugmecon import PyAugmecon
 from tests.optimization_models import three_kp_model
 
 # Multiprocessing requires this If statement (on Windows)
 if __name__ == "__main__":
-    model_type = '3kp40'
+    model_type = "3kp40"
 
     # AUGMECON related options
     opts = {
-        'name': model_type,
-        'grid_points': 540,
-        'nadir_points': [1031, 1069],
-        }
-
-    # Options passed to Gurobi
-    solver_opts = {}
-
-    A = PyAugmecon(three_kp_model(model_type), opts, solver_opts) # instantiate  PyAugmecon
-    A.solve() # solve PyAugmecon multi-objective optimization problem
-    print(A.model.payoff) # this prints the payoff table
-    print(A.unique_pareto_sols) # this prints the unique Pareto optimal solutions
+        "name": model_type,
+        "grid_points": 540,
+        "nadir_points": [1031, 1069],
+    }
+
+    pyaugmecon = PyAugmecon(three_kp_model(model_type), opts)  # instantiate  PyAugmecon
+    pyaugmecon.solve()  # solve PyAugmecon multi-objective optimization problem
+    sols = pyaugmecon.get_pareto_solutions()  # get all pareto solutions
+    payoff = pyaugmecon.get_payoff_table()  # get the payoff table
+    decision_vars = pyaugmecon.get_decision_variables(sols[0])  # get the decision variables
 ```
 
-### PyAugmecon object attributes
+### PyAugmecon methods
+
+| Name                     | Description                                                                                                                                             |
+| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `get_pareto_solutions()`    | Get a list of Pareto-optimal solutions (`list[tuple]`) |
+| `get_decision_variables(pareto_solution)` | Get a dictionary of decision variables for a given Pareto-optimal solution. Where the key represents the decision variable name and the value is a pd.Series with the values. |
+| `get_payoff_table()`  | Get the payoff table from the model. |
+
+### PyAugmecon attributes
 
 After solving the model with `PyAugmecon.solve()`, the following object attributes are available:
 
 | Name                     | Description                                                                                                                                             |
 | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `sols`                   | Full unprocessed solutions, only checked for uniqueness                                                                                                 |
 | `unique_sols`            | Unique solutions, rounded to `round_decimals` and checked for uniqueness                                                                                |
@@ -341,14 +347,18 @@
 
 - Wouter Bles (current version of the package)
 - Nikolaos Paterakis (initial implementation)
 
 
 # Changelog
 
+## 1.0.0
+
+- Add new methods for solution retrieval
+
 ## 0.2.1
 
 - Add Python 3.10 to supported versions
 
 ## 0.2.0
 
 - Decision variables are now stored in a dictionary together with the objective values
```

### Comparing `pyaugmecon-0.2.1/setup.py` & `pyaugmecon-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         + "\n\n"
         + (CURRENT_DIR / "CHANGELOG.md").read_text(encoding="utf8")
     )
 
 
 setup(
     name="pyaugmecon",
-    version="0.2.1",
+    version="1.0.0",
     author="Wouter Bles",
     author_email="whbles@gmail.com",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     keywords="python, pyomo, optimization, multi-objective-optimization, augmecon",
     url="https://github.com/wouterbles/pyaugmecon",
     project_urls={"Changelog": "https://github.com/wouterbles/pyaugmecon/blob/main/CHANGELOG.md"},
```

