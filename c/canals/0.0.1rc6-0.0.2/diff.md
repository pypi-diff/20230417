# Comparing `tmp/canals-0.0.1rc6.tar.gz` & `tmp/canals-0.0.2.tar.gz`

## Comparing `canals-0.0.1rc6.tar` & `canals-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,49 @@
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 canals-0.0.1rc6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.0.1rc6/.github/workflows/release.yml
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 canals-0.0.1rc6/.github/workflows/tests.yml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.0.1rc6/canals/__about__.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 canals-0.0.1rc6/canals/__init__.py
--rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 canals-0.0.1rc6/canals/node.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 canals-0.0.1rc6/canals/pipeline/__init__.py
--rw-r--r--   0        0        0    28327 2020-02-02 00:00:00.000000 canals-0.0.1rc6/canals/pipeline/pipeline.py
--rw-r--r--   0        0        0     9183 2020-02-02 00:00:00.000000 canals-0.0.1rc6/canals/pipeline/save_load.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/__init__.py
--rw-r--r--   0        0        0     7304 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/test_save_load.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/nodes/__init__.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/nodes/test_accumulate.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/nodes/test_add_value.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/nodes/test_below.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/nodes/test_double.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/nodes/test_greet.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/nodes/test_merge.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/nodes/test_remainder.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/nodes/test_rename.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/nodes/test_repeat.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/nodes/test_subtract.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/nodes/test_sum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/pipelines/__init__.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/pipelines/_test_looping_and_merge_pipeline.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/pipelines/test_complex_pipeline.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/pipelines/test_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/pipelines/test_decision_pipeline.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/pipelines/test_linear_pipeline.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/pipelines/test_looping_pipeline.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/pipelines/test_merging_pipeline.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 canals-0.0.1rc6/test/pipelines/test_parallel_branches_pipeline.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 canals-0.0.1rc6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.0.1rc6/LICENSE
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 canals-0.0.1rc6/README.md
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 canals-0.0.1rc6/pyproject.toml
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 canals-0.0.1rc6/PKG-INFO
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 canals-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 canals-0.0.2/mkdocs.yml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.0.2/.github/workflows/api-docs.yml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 canals-0.0.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 canals-0.0.2/canals/__about__.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 canals-0.0.2/canals/__init__.py
+-rw-r--r--   0        0        0     5852 2020-02-02 00:00:00.000000 canals-0.0.2/canals/component.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 canals-0.0.2/canals/pipeline/__init__.py
+-rw-r--r--   0        0        0    30093 2020-02-02 00:00:00.000000 canals-0.0.2/canals/pipeline/pipeline.py
+-rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 canals-0.0.2/canals/pipeline/save_load.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 canals-0.0.2/docs/index.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 canals-0.0.2/docs/api-docs/component.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 canals-0.0.2/docs/api-docs/pipeline.md
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 canals-0.0.2/docs/concepts/components.md
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 canals-0.0.2/docs/concepts/concepts.md
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 canals-0.0.2/docs/concepts/parameters.md
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 canals-0.0.2/docs/concepts/pipelines.md
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 canals-0.0.2/docs/concepts/save-load.md
+-rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.0.2/images/canals-logo-dark.png
+-rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.0.2/images/canals-logo-light.png
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 canals-0.0.2/test/__init__.py
+-rw-r--r--   0        0        0     7428 2020-02-02 00:00:00.000000 canals-0.0.2/test/test_save_load.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/__init__.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_accumulate.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_add_value.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_below.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_double.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_greet.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_merge.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_remainder.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_rename.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_repeat.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_subtract.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_sum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/__init__.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/_test_looping_and_merge_pipeline.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/test_complex_pipeline.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/test_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/test_decision_pipeline.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/test_linear_pipeline.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/test_looping_pipeline.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/test_merging_pipeline.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/test_parallel_branches_pipeline.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 canals-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 canals-0.0.2/README.md
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 canals-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 canals-0.0.2/PKG-INFO
```

### Comparing `canals-0.0.1rc6/.pre-commit-config.yaml` & `canals-0.0.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.2.0
   hooks:
     - id: check-ast   # checks Python syntax
     - id: check-json  # checks JSON syntax
-    - id: check-yaml  # checks YAML syntax
+#    - id: check-yaml  # checks YAML syntax
     - id: check-toml  # checks TOML syntax
     - id: end-of-file-fixer  # checks there is a newline at the end of the file
     - id: trailing-whitespace  # trims trailing whitespace
     - id: check-merge-conflict  # checks for no merge conflict strings
     - id: check-shebang-scripts-are-executable  # checks all shell scripts have executable permissions
     - id: mixed-line-ending  # normalizes line endings
     #- id: no-commit-to-branch  # prevents committing to main
```

### Comparing `canals-0.0.1rc6/.github/workflows/tests.yml` & `canals-0.0.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `canals-0.0.1rc6/canals/node.py` & `canals-0.0.2/canals/component.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,96 +1,96 @@
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
-class NodeError(Exception):
+class ComponentError(Exception):
     pass
 
 
-def node(class_):
+def component(class_):
     """
-    Marks a class as a node. Any class decorated with `@node`
+    Marks a class as a component. Any class decorated with `@component`
     can be picked up by a Pipeline, serialized, deserialized, etc.
 
-    All nodes MUST follow the contract below.
-    This docstring is the source of truth for nodes contract.
+    All components MUST follow the contract below.
+    This docstring is the source of truth for components contract.
 
     ```python
-    def __init__(self, [... nodes init parameters ...]):
+    def __init__(self, [... components init parameters ...]):
     ```
     Mandatory method.
 
-    Nodes should have an `__init__` method where they define:
+    Components should have an `__init__` method where they define:
 
-    - `self.inputs = [<expected_input_edge_name(s)>]`:
-        A list with all the edges they can possibly receive input from
+    - `self.inputs = [<expected_input_connection_name(s)>]`:
+        A list with all the connections they can possibly receive input from
 
-    - `self.outputs = [<expected_output_edge_name(s)>]`:
-        A list with the edges they might possibly produce as output
+    - `self.outputs = [<expected_output_connection_name(s)>]`:
+        A list with the connections they might possibly produce as output
 
     - `self.init_parameters = {<init parameters>}`:
         Any state they wish to be persisted when they are marshalled.
         These values will be given to the `__init__` method of a new instance
         when the pipeline is unmarshalled.
 
-    If nodes want to let users customize their input and output edges (be it
-    the edge name, the edge count, etc...) they should provide properly
+    If components want to let users customize their input and output connections (be it
+    the connection name, the connection count, etc...) they should provide properly
     named init parameters:
 
     - `input: str` or `inputs: List[str]` (always with proper defaults)
     - `output: str` or `outputs: List[str]` (always with proper defaults)
 
     All the rest is going to be interpreted as a regular init parameter that
-    has nothing to do with the node edges.
+    has nothing to do with the component connections.
 
     The `__init__` must be extrememly lightweight, because it's a frequent
-    operation during the construction and validation of the pipeline. If a node
+    operation during the construction and validation of the pipeline. If a component
     has some heavy state to initialize (models, backends, etc...) refer to the
     `warm_up()` method.
 
     ```
     def warm_up(self):
     ```
     Optional method.
 
     This method is called by Pipeline before the graph execution.
     Make sure to avoid double-initializations, because Pipeline will not keep
-    track of which nodes it called `warm_up()` on.
+    track of which components it called `warm_up()` on.
 
     ```
     def run(
         self,
         name: str,
         data: List[Tuple[str, Any]],
         parameters: Dict[str, Dict[str, Any]],
     ):
     ```
     Mandatory method.
 
-    This is the method where the main functionality of the node should be carried out.
+    This is the method where the main functionality of the component should be carried out.
     It's called by `Pipeline.run()`, which passes the following parameters to it:
 
-    - `name: str`: the name of the node. Allows the node to find its own parameters in
+    - `name: str`: the name of the component. Allows the component to find its own parameters in
         the `parameters` dictionary (see below).
 
     - `data: List[Tuple[str, Any]]`: the input data.
         Pipeline guarantees that the following assert always passes:
 
         `assert self.inputs == [name for name, value in data]`
 
         which means that:
         - `data` is of the same length as `self.inputs`.
         - `data` contains one tuple for each string stored in `self.inputs`.
         - no guarantee is given on the values of these tuples: notably, if there was a
-            decision node upstream, some values might be `None`.
+            decision component upstream, some values might be `None`.
 
-        For example, if a node declares `self.inputs = ["value", "value"]` (think of a
-        `Sum` node), `data` might look like:
+        For example, if a component declares `self.inputs = ["value", "value"]` (think of a
+        `Sum` component), `data` might look like:
 
         `[("value", 1), ("value", 10)]`
 
         `[("value", None), ("value", 10)]`
 
         `[("value", None), ("value", None)]`
 
@@ -101,43 +101,52 @@
         `[("value", 1), ("value", 10), ("value", 100)]`
 
         `[("value": 15)]`
 
         `[("value": 15), ("unexpected", 10)]`
 
     - `parameters: Dict[str, Dict[str, Any]]`: a dictionary of dictionaries with all
-        the parameters for all nodes.
-        Note that all nodes have access to all parameters for all other nodes: this
-        might come handy to nodes like `Agent`s, that want to influence the behavior
-        of nodes downstream.
-        Nodes can access their own parameters using `name`, but they must **not** assume
+        the parameters for all components.
+        Note that all components have access to all parameters for all other components: this
+        might come handy to components like `Agent`s, that want to influence the behavior
+        of components downstream.
+        Components can access their own parameters using `name`, but they must **not** assume
         their name is present in the dictionary.
         Therefore, the best way to get the parameters is with
         `my_parameters = parameters.get(name, {})`
 
     Pipeline expect the output of this function to be a tuple of two dictionaries.
     The first item is a dictionary that represents the output and it should always
     abide to the following format:
 
     `{output_name: output_value for output_name in <subset of self.expected_output>}`
 
     Which means that:
-    - Nodes are not forced to produce output on all the expected outputs: for example,
-        nodes taking a decision, like classifiers, can produce output on a subset of
-        the expected output edges and Pipeline will figure out the rest.
-    - Nodes must not add any key in the data dictionary that is not present in `self.outputs`.
+    - Components are not forced to produce output on all the expected outputs: for example,
+        components taking a decision, like classifiers, can produce output on a subset of
+        the expected output connections and Pipeline will figure out the rest.
+    - Components must not add any key in the data dictionary that is not present in `self.outputs`.
 
-    The second item of the tuple is the `parameters` dictionary. This allows node to
+    The second item of the tuple is the `parameters` dictionary. This allows component to
     propagate downstream any change they might have done to the `parameters` dictionary.
+
+    Args:
+        class_: the class that Canals should use as a component.
+
+    Returns:
+        A class that can be recognized by Canals as a component.
+
+    Raises:
+        ComponentError: if the class provided has no `run()` method.
     """
-    logger.debug("Registering %s as a node", class_)
+    logger.debug("Registering %s as a component", class_)
 
-    # '__canals_node__' is used to distinguish nodes from regular classes.
-    # Its value is set to the desired node name: normally it is the class name, but it can technically be customized.
-    class_.__canals_node__ = class_.__name__
+    # '__canals_component__' is used to distinguish components from regular classes.
+    # Its value is set to the desired component name: normally it is the class name, but it can technically be customized.
+    class_.__canals_component__ = class_.__name__
 
     # Check for run()
     if not hasattr(class_, "run"):
-        # TODO check the node signature too
-        raise NodeError("Nodes must have a 'run()' method. See the docs for more information.")
+        # TODO check the component signature too
+        raise ComponentError("Components must have a 'run()' method. See the docs for more information.")
 
     return class_
```

### Comparing `canals-0.0.1rc6/canals/pipeline/pipeline.py` & `canals-0.0.2/canals/pipeline/pipeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,141 +41,166 @@
     pass
 
 
 class PipelineMaxLoops(PipelineError):
     pass
 
 
-def locate_pipeline_input_nodes(graph) -> List[str]:
+def locate_pipeline_input_components(graph) -> List[str]:
     """
-    Collect the nodes with no input edges: they receive directly the pipeline inputs.
+    Collect the components with no input connections: they receive directly the pipeline inputs.
+
+    Args:
+        graph: the pipeline graph.
+
+    Returns:
+        A list of components that should directly receive the user's inputs.
     """
-    return [node for node in graph.nodes if not graph.in_edges(node) or graph.nodes[node]["input_node"]]
+    return [node for node in graph.nodes if not graph.in_edges(node) or graph.nodes[node]["input_component"]]
 
 
-def locate_pipeline_output_nodes(graph) -> List[str]:
+def locate_pipeline_output_components(graph) -> List[str]:
     """
-    Collect the nodes with no output edges: these define the output of the pipeline.
+    Collect the components with no output connections: these define the output of the pipeline.
+
+    Args:
+        graph: the pipeline graph.
+
+    Returns:
+        A list of components whose output goes back to the user.
     """
-    return [node for node in graph.nodes if not graph.out_edges(node) or graph.nodes[node]["output_node"]]
+    return [node for node in graph.nodes if not graph.out_edges(node) or graph.nodes[node]["output_component"]]
 
 
 class Pipeline:
     """
-    Nodes orchestration engine.
+    Components orchestration engine.
 
-    Builds a graph of nodes and orchestrates their execution according to the execution graph.
+    Builds a graph of components and orchestrates their execution according to the execution graph.
     """
 
     def __init__(
         self,
         metadata: Optional[Dict[str, Any]] = None,
         max_loops_allowed: int = 100,
     ):
         """
         Creates the Pipeline.
 
-        :param metadata: arbitrary dictionary to store metadata about this pipeline. Make sure
-            all the values contained in this dictionary can be serialized and deserialized if you wish to save this
-            pipeline to file with `save_pipelines()/load_pipelines()`.
-        :param max_loops_allowed: how many times the pipeline can run the same node before throwing an exception.
+        Args:
+            metadata: arbitrary dictionary to store metadata about this pipeline. Make sure all the values contained in
+                this dictionary can be serialized and deserialized if you wish to save this pipeline to file with
+                `save_pipelines()/load_pipelines()`.
+            max_loops_allowed: how many times the pipeline can run the same node before throwing an exception.
         """
         self.metadata = metadata or {}
         self.max_loops_allowed = max_loops_allowed
         self.graph = nx.DiGraph()
 
     def __eq__(self, other) -> bool:
-        """
-        Equal pipelines share all nodes and metadata instances.
-        """
+        # Equal pipelines share all nodes and metadata instances.
         if not isinstance(other, type(self)):
             return False
         return (
             self.metadata == other.metadata
             and self.max_loops_allowed == other.max_loops_allowed
             and self.graph == other.graph
         )
 
-    def add_node(
+    def add_component(
         self,
         name: str,
         instance: Any,
         parameters: Optional[Dict[str, Any]] = None,
-        input_node: bool = False,
-        output_node: bool = False,
+        input_component: bool = False,
+        output_output: bool = False,
     ) -> None:
         """
-        Create a node for the given node. Nodes are not connected to anything by default:
-        use `Pipeline.connect()` to connect nodes together.
+        Create a component for the given component. Components are not connected to anything by default:
+        use `Pipeline.connect()` to connect components together.
 
-        Node names must be unique, but node instances can be reused if needed.
+        Component names must be unique, but component instances can be reused if needed.
 
-        :param name: the name of the node.
-        :param instance: the node instance.
-        :param parameters: default parameters to pass to this node's instance only then this
-            specific node is executed. These parameters are NOT shared across nodes that use
-            the same instance.
-        :param input_node: whether this node should receive the input data given to
-            `Pipeline.run()` directly, regardless of its location in the Pipeline.
-        :param output_node: whether the output of this node should be returned as output,
-            regardless of its location in the Pipeline.
-        :returns: None
+        Args:
+            name: the name of the component.
+            instance: the component instance.
+            parameters: default parameters to pass to this component's instance only then this specific component is
+                executed. These parameters are NOT shared across components that use the same instance.
+            input_component: whether this component should receive the input data given to `Pipeline.run()` directly, regardless
+                of its location in the Pipeline.
+            output_component: whether the output of this component should be returned as output, regardless of its
+                location in the Pipeline.
+
+        Returns:
+            None
+
+        Raises:
+            ValueError: if a component with the same name already exists or `parameters` is not a dictionary
+            PipelineValidationError: if the given instance is not a Canals component
         """
-        # Node names are unique
+        # Component names are unique
         if name in self.graph.nodes:
-            raise ValueError(f"Node named '{name}' already exists: choose another name.")
+            raise ValueError(f"Component named '{name}' already exists: choose another name.")
 
-        # Node instances must be nodes
-        if not hasattr(instance, "__canals_node__"):
+        # Component instances must be components
+        if not hasattr(instance, "__canals_component__"):
             raise PipelineValidationError(
-                f"'{type(instance)}' doesn't seem to be a node. Is this class decorated with @node?"
+                f"'{type(instance)}' doesn't seem to be a component. Is this class decorated with @component?"
             )
 
         # Params must be a dict
         if parameters and not isinstance(parameters, dict):
             raise ValueError("'parameters' must be a dictionary.")
 
-        # Add node to the graph, disconnected
-        logger.debug("Adding node '%s' (%s)", name, instance)
+        # Add component to the graph, disconnected
+        logger.debug("Adding component '%s' (%s)", name, instance)
         self.graph.add_node(
             name,
             instance=instance,
             visits=0,
             parameters=parameters,
-            input_node=input_node,
-            output_node=output_node,
+            input_component=input_component,
+            output_component=output_output,
         )
 
     def connect(self, connect_from: str, connect_to: str) -> None:
         """
-        Connect nodes together. All nodes to connect must exist in the pipeline.
-        If connecting to an node that has several output edges, specify its name with 'node_name.edge_name'.
-
-        :param connect_from: the node that deliver the values. This can be either a single node name or
-            can be in the format `node_name.edge_name` if the node has multiple outputs.
-        :param connect_to: the node that receives the values. This is always just the node name.
-        :returns: None
+        Connect components together. All components to connect must exist in the pipeline.
+        If connecting to an component that has several output connections, specify its name with
+        'component_name.connections_name'.
+
+        Args:
+            connect_from: the component that deliver the values. This can be either a single component name or can be
+                in the format `component_name.connection_name` if the component has multiple outputs.
+            connect_to: the component that receives the values. This is always just the component name.
+
+        Returns:
+            None
+
+        Raises:
+            PipelineConnectError: if the two components cannot be connected (for example if one of the components is
+                not present in the pipeline, or the connections don't match, and so on).
         """
         upstream_node_name = connect_from
         downstream_node_name = connect_to
 
-        # Find out the name of the edge
+        # Find out the name of the connection
         edge_name = None
         # Edges may be named explicitly by passing 'node_name.edge_name' to connect().
         # Specify the edge name for the upstream node only.
         if "." in upstream_node_name:
             upstream_node_name, edge_name = upstream_node_name.split(".", maxsplit=1)
             upstream_node = self.graph.nodes[upstream_node_name]["instance"]
         else:
             # If the edge had no explicit name and the upstream node has multiple outputs, raise an exception
             upstream_node = self.graph.nodes[upstream_node_name]["instance"]
             if len(upstream_node.outputs) != 1:
                 raise PipelineConnectError(
                     f"Please specify which output of '{upstream_node_name}' "
-                    f"'{downstream_node_name}' should connect to. Node '{upstream_node_name}' has the following "
+                    f"'{downstream_node_name}' should connect to. Component '{upstream_node_name}' has the following "
                     f"outputs: {upstream_node.outputs}"
                 )
             edge_name = upstream_node.outputs[0]
 
         # Remove edge name from downstream_node name (it's needed only when the node is upstream)
         downstream_node_name = downstream_node_name.split(".", maxsplit=2)[0]
         downstream_node = self.graph.nodes[downstream_node_name]["instance"]
@@ -188,15 +213,15 @@
 
         # Check if the edge with that name already exists between those two nodes
         if any(
             edge[1] == downstream_node_name and edge[2]["label"] == edge_name
             for edge in self.graph.edges.data(nbunch=upstream_node_name)
         ):
             logger.info(
-                "An edge called '%s' connecting node '%s' and node '%s' already exists: skipping.",
+                "A connection called '%s' between component '%s' and component '%s' already exists: skipping.",
                 edge_name,
                 upstream_node_name,
                 downstream_node_name,
             )
             return
 
         # Find all empty slots in the upstream and downstream nodes
@@ -224,57 +249,70 @@
                     " - " + edge[2]["label"] + f" (taken by {edge[1]})"
                     for edge in self.graph.out_edges(upstream_node_name, data=True)
                 ]
                 + [f" - {free_out_edge} (free)" for free_out_edge in free_upstream_outputs]
             )
             raise PipelineConnectError(
                 f"Cannot connect '{upstream_node_name}' with '{downstream_node_name}' "
-                f"with an edge named '{edge_name}': "
+                f"with an connection named '{edge_name}': "
                 f"their declared inputs and outputs do not match.\n"
-                f"Upstream node '{upstream_node_name}' declared these outputs:\n{outputs_string}\n"
-                f"Downstream node '{downstream_node_name}' declared these inputs:\n{inputs_string}\n"
+                f"Upstream component '{upstream_node_name}' declared these outputs:\n{outputs_string}\n"
+                f"Downstream component '{downstream_node_name}' declared these inputs:\n{inputs_string}\n"
             )
-        # Create the edge
+        # Create the connection
         logger.debug(
-            "Connecting node '%s' to node '%s' along edge '%s'",
+            "Connecting component '%s' to component '%s' with connection name '%s'",
             upstream_node_name,
             downstream_node_name,
             edge_name,
         )
         self.graph.add_edge(upstream_node_name, downstream_node_name, label=edge_name)
 
-    def get_node(self, name: str) -> Dict[str, Any]:
+    def get_component(self, name: str) -> Dict[str, Any]:
         """
-        Returns all the data associated with a node.
+        Returns all the data associated with a component.
+
+        Args:
+            name: the name of the component
 
-        :param name: the name of the node
-        :returns: a dictionary containing all data that was given to `add_node()` (except for `name`)
+        Returns:
+            A dictionary containing all data that was given to `add_component()` (except for `name`)
+
+        Raises:
+            ValueError: if a nocomponentde with that name is not present in the pipeline.
         """
         candidates = [node for node in self.graph.nodes if node == name]
         if not candidates:
-            raise ValueError(f"Node named {name} not found.")
+            raise ValueError(f"Component named {name} not found.")
         return self.graph.nodes[candidates[0]]
 
     def draw(self, path: Path) -> None:
         """
         Draws the pipeline. Requires `pygraphviz`.
         Run `pip install canals[draw]` to install missing dependencies.
 
-        :param path: where to save the drawing.
+        Args:
+            path: where to save the drawing.
+
+        Returns:
+            None
+
+        Raises:
+            ImportError: if pygraphviz is not installed.
         """
         if not PYGRAPHVIZ_IMPORTED:
             raise ImportError(
                 "Could not import `pygraphviz`. Please install via: \n"
                 "pip install pygraphviz\n"
                 "(You might need to run this first: apt install libgraphviz-dev graphviz )"
             )
         graph = deepcopy(self.graph)
 
-        input_nodes = locate_pipeline_input_nodes(graph)
-        output_nodes = locate_pipeline_output_nodes(graph)
+        input_nodes = locate_pipeline_input_components(graph)
+        output_nodes = locate_pipeline_output_components(graph)
 
         # Draw the input
         graph.add_node("input", shape="plain")
         for node in input_nodes:
             for edge in graph.nodes[node]["instance"].inputs:
                 graph.add_edge("input", node, label=edge)
 
@@ -305,18 +343,24 @@
         data: Union[Dict[str, Any], List[Tuple[str, Any]]],
         parameters: Optional[Dict[str, Dict[str, Any]]] = None,
         debug: bool = False,
     ) -> Dict[str, Any]:
         """
         Runs the pipeline.
 
-        :param data: the inputs to give to the input nodes of the Pipeline.
-        :param parameters: a dictionary with all the parameters of all the nodes, namespaced by node.
-        :param debug: whether to collect and return debug information.
-        :returns: a dictionary with the outputs of the output nodes of the Pipeline.
+        Args:
+            data: the inputs to give to the input components of the Pipeline.
+            parameters: a dictionary with all the parameters of all the components, namespaced by component.
+            debug: whether to collect and return debug information.
+
+        Returns:
+            A dictionary with the outputs of the output components of the Pipeline.
+
+        Raises:
+            PipelineRuntimeError: if the any of the components fail or return unexpected output.
         """
         parameters = self._validate_parameters(parameters=parameters)
         self.warm_up()
         self._validate_pipeline()
 
         # **** The Pipeline.run() algorithm ****
         #
@@ -341,35 +385,35 @@
         # - Node instance          # self.graph.nodes[node]["instance"]
         # - Input nodes            # [e[0] for e in self.graph.in_edges(node)]
         # - Output nodes           # [e[1] for e in self.graph.out_edges(node)]
         # - Output edges           # [e[2]["label"] for e in self.graph.out_edges(node, data=True)]
         logger.info("Pipeline execution started.")
         inputs_buffer: OrderedDict = OrderedDict()
 
-        for node_name in locate_pipeline_input_nodes(self.graph):
+        for node_name in locate_pipeline_input_components(self.graph):
             # NOTE: We allow users to pass dictionaries just for convenience.
             # The real input format is List[Tuple[str, Any]], to allow several input edges to have the same name.
             if isinstance(data, dict):
                 data = list(data.items())
             inputs_buffer[node_name] = {"data": data, "parameters": parameters}
 
         # *** PIPELINE EXECUTION LOOP ***
         # We select the nodes to run by checking which keys are set in the
         # inputs buffer. If the key exists, the node might be ready to run.
         pipeline_results: Dict[str, List[Dict[str, Any]]] = {}
         while inputs_buffer:
-            logger.debug("> Current node queue: %s", inputs_buffer.keys())
+            logger.debug("> Current component queue: %s", inputs_buffer.keys())
 
             node_name, node_inputs = inputs_buffer.popitem(last=False)  # FIFO
 
             # Check if we looped over this node too many times
             self._check_max_loops(node_name)
 
             ready_to_run, inputs_buffer = self._ready_to_run(
-                node_name=node_name, node_inputs=node_inputs, inputs_buffer=inputs_buffer
+                component_name=node_name, component_inputs=node_inputs, inputs_buffer=inputs_buffer
             )
             if not ready_to_run:
                 continue
 
             # **** RUN THE NODE ****
             # It is our turn! The node is ready to run and all inputs are ready
             #
@@ -414,17 +458,17 @@
             # Type-check the output
             if (
                 len(node_results) != 2
                 or not isinstance(node_results[0], dict)
                 or not isinstance(node_results[1], dict)
                 or not all(isinstance(params, dict) for params in node_results[1].values())
             ):
-                logger.debug("Node output is malformed!\n%s", node_results)
+                logger.debug("Component's output is malformed:\n%s", node_results)
                 raise PipelineRuntimeError(
-                    f"The node '{node_name}' did not return proper output. Check out the '@node' docstring."
+                    f"The component '{node_name}' did not return proper output. Check out the '@component' docstring."
                 )
 
             # Process the output of the node
             if not self.graph.out_edges(node_name):
                 # If there are no output edges, the output of this node is the output of the pipeline:
                 # store it in pipeline_results.
                 if not node_name in pipeline_results.keys():
@@ -449,62 +493,64 @@
         Validate the input parameters.
         """
         if not parameters:
             return {}
 
         if any(node not in self.graph.nodes for node in parameters.keys()):
             logging.warning(
-                "You passed parameters for one or more node(s) that do not exist in the pipeline: %s",
+                "You passed parameters for one or more component(s) that do not exist in the pipeline: %s",
                 [node for node in parameters.keys() if node not in self.graph.nodes],
             )
         return parameters
 
     def _validate_pipeline(self):
         """
-        Make sure the pipeline has at least one input node and one output node.
+        Make sure the pipeline has at least one input component and one output component.
         """
-        if not locate_pipeline_input_nodes(self.graph):
-            raise ValueError("This pipeline has no input nodes!")
+        if not locate_pipeline_input_components(self.graph):
+            raise ValueError("This pipeline has no input components!")
 
-        if not locate_pipeline_output_nodes(self.graph):
-            raise ValueError("This pipeline has no output nodes!")
+        if not locate_pipeline_output_components(self.graph):
+            raise ValueError("This pipeline has no output components!")
 
-    def _check_max_loops(self, node_name: str):
+    def _check_max_loops(self, component_name: str):
         """
-        Verify whether this node run too many times.
+        Verify whether this component run too many times.
         """
-        if self.graph.nodes[node_name]["visits"] > self.max_loops_allowed:
-            raise PipelineMaxLoops(f"Maximum loops count ({self.max_loops_allowed}) exceeded for node '{node_name}'.")
+        if self.graph.nodes[component_name]["visits"] > self.max_loops_allowed:
+            raise PipelineMaxLoops(
+                f"Maximum loops count ({self.max_loops_allowed}) exceeded for component '{component_name}'."
+            )
 
     def _ready_to_run(
-        self, node_name: str, node_inputs: Dict[str, Any], inputs_buffer: OrderedDict
+        self, component_name: str, component_inputs: Dict[str, Any], inputs_buffer: OrderedDict
     ) -> Tuple[bool, OrderedDict]:
         """
-        Verify whether a node is ready to run.
+        Verify whether a component is ready to run.
 
-        Returns true if the node should run, false otherwise, and the updated inputs buffer.
+        Returns true if the component should run, false otherwise, and the updated inputs buffer.
         """
         # List all the inputs the current node should be waiting for.
-        inputs_received = [i[0] for i in node_inputs["data"]]
+        inputs_received = [i[0] for i in component_inputs["data"]]
 
         # We should be wait on all edges except for the downstream ones, to support loops.
         # This downstream check is enabled only for nodes taking more than one input
         # (the "entrance" of the loop).
-        is_merge_node = len(self.graph.in_edges(node_name)) != 1
+        is_merge_node = len(self.graph.in_edges(component_name)) != 1
         data_to_wait_for = [
             (e[0], e[2]["label"])  # the node and the edge label
-            for e in self.graph.in_edges(node_name, data=True)  # for all input edges
+            for e in self.graph.in_edges(component_name, data=True)  # for all input edges
             # if there's a path in the graph leading back from the current node to the
             # input node, in case of multiple input nodes.
-            if not is_merge_node or not nx.has_path(self.graph, node_name, e[0])
+            if not is_merge_node or not nx.has_path(self.graph, component_name, e[0])
         ]
 
         if not data_to_wait_for:
             # This is an input node, so it's ready to run.
-            logger.debug("'%s' is an input node and it's ready to run.")
+            logger.debug("'%s' is an input component and it's ready to run.")
             return (True, inputs_buffer)
 
         # Do we have all the inputs we expect?
         nodes_to_wait_for, inputs_to_wait_for = zip(*data_to_wait_for)
         if sorted(inputs_to_wait_for) == sorted(inputs_received):
             return (True, inputs_buffer)
 
@@ -512,40 +558,40 @@
         #
         # Did all the upstream nodes run?
         if not all(self.graph.nodes[node_to_wait_for]["visits"] > 0 for node_to_wait_for in nodes_to_wait_for):
             # Some node upstream didn't run yet, so we should wait for them.
             logger.debug(
                 "Putting '%s' back in the queue, some inputs are missing "
                 "(inputs to wait for: %s, inputs_received: %s)",
-                node_name,
+                component_name,
                 inputs_to_wait_for,
                 inputs_received,
             )
             # Put back the node in the inputs buffer at the back...
-            inputs_buffer[node_name] = node_inputs
+            inputs_buffer[component_name] = component_inputs
             # ... and do not run this node (yet)
             return (False, inputs_buffer)
 
         # All upstream nodes run, so it **must** be our turn.
         #
         # Are we missing ALL inputs or just a few?
         if not inputs_received:
             # ALL upstream nodes have been skipped.
             #
             # Let's skip this node and add all downstream nodes to the queue.
-            self.graph.nodes[node_name]["visits"] += 1
+            self.graph.nodes[component_name]["visits"] += 1
             logger.debug(
-                "Skipping '%s', all input nodes were skipped and no inputs were received "
-                "(skipped nodes: %s, inputs: %s)",
-                node_name,
+                "Skipping '%s', all input components were skipped and no inputs were received "
+                "(skipped components: %s, inputs: %s)",
+                component_name,
                 nodes_to_wait_for,
                 inputs_to_wait_for,
             )
             # Put all downstream nodes in the inputs buffer...
-            downstream_nodes = [e[1] for e in self.graph.out_edges(node_name)]
+            downstream_nodes = [e[1] for e in self.graph.out_edges(component_name)]
             for downstream_node in downstream_nodes:
                 if not downstream_node in inputs_buffer:
                     inputs_buffer[downstream_node] = {
                         "data": [],
                         "parameters": {},
                     }
             # ... and never run this node
@@ -569,31 +615,31 @@
         # with 'value' and 'odd' only, because 'even' will never arrive.
         #
         inputs_to_wait_for = list(inputs_to_wait_for)
         for input_expected in inputs_to_wait_for:
             if input_expected in inputs_received:
                 inputs_to_wait_for.pop(inputs_to_wait_for.index(input_expected))
         logger.debug(
-            "Some nodes upstream of '%s' were skipped, so some inputs will be None (missing inputs: %s)",
-            node_name,
+            "Some components upstream of '%s' were skipped, so some inputs will be None (missing inputs: %s)",
+            component_name,
             inputs_to_wait_for,
         )
         for missing_input in inputs_to_wait_for:
-            node_inputs["data"].append((missing_input, None))
+            component_inputs["data"].append((missing_input, None))
 
         return (True, inputs_buffer)
 
     def _route_output(
         self,
         node_name: str,
         node_results: Tuple[Dict[str, Any], Dict[str, Dict[str, Any]]],
         inputs_buffer: OrderedDict,
     ) -> OrderedDict:
         """
-        Distrubute the outputs of the node into the input buffer of downstream nodes.
+        Distrubute the outputs of the component into the input buffer of downstream components.
 
         Returns the updated inputs buffer.
         """
         # This is not a terminal node: find out where the output goes, to which nodes and along which edge
         is_decision_node_for_loop = (
             any(nx.has_path(self.graph, edge[1], node_name) for edge in self.graph.out_edges(node_name))
             and len(self.graph.out_edges(node_name)) > 1
@@ -630,22 +676,22 @@
 
         return inputs_buffer
 
     def _unwrap_results(self, pipeline_results):
         """
         Simplifies the output of simple Pipelines:
 
-        - if the resuklt contains output of a single node, unwraps the dictionary to return the list only
+        - if the resuklt contains output of a single component, unwraps the dictionary to return the list only
         - if the resulting list is only composed of one dictionary, returns the internal dictionary only.
 
         So the output of `Pipeline.run()` might look like:
 
-        - Multi-node output: `{node: [{key: value, ... }, ... ], ... }`
-        - Single-node, repeated output: `[{key: value, ... }, ... ]`
-        - Single-node, single output: `{key: value, ... }`
+        - Multi-component output: `{component: [{key: value, ... }, ... ], ... }`
+        - Single-component, repeated output: `[{key: value, ... }, ... ]`
+        - Single-component, single output: `{key: value, ... }`
         """
         if len(pipeline_results.keys()) == 1:
             pipeline_results = pipeline_results[list(pipeline_results.keys())[0]]  # type: ignore
 
             if len(pipeline_results) == 1:
                 pipeline_results = pipeline_results[0]  # type: ignore
```

### Comparing `canals-0.0.1rc6/test/test_save_load.py` & `canals-0.0.2/test/test_save_load.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 from pathlib import Path
 
 import pytest
 
 from canals.pipeline import Pipeline, marshal_pipelines, unmarshal_pipelines
-from test.nodes import AddValue, Double
+from test.components import AddValue, Double
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_marshal():
     add_1 = AddValue(add=1)
     add_2 = AddValue(add=1)
 
     pipeline_1 = Pipeline(metadata={"type": "test pipeline", "author": "me"})
-    pipeline_1.add_node("first_addition", add_2, parameters={"add": 6})
-    pipeline_1.add_node("double", Double(input="value"))
-    pipeline_1.add_node("second_addition", add_1)
-    pipeline_1.add_node("third_addition", add_2)
+    pipeline_1.add_component("first_addition", add_2, parameters={"add": 6})
+    pipeline_1.add_component("double", Double(input="value"))
+    pipeline_1.add_component("second_addition", add_1)
+    pipeline_1.add_component("third_addition", add_2)
 
     pipeline_1.connect("first_addition", "double")
     pipeline_1.connect("double", "second_addition")
     pipeline_1.connect("second_addition", "third_addition")
 
     pipeline_2 = Pipeline(metadata={"type": "another test pipeline", "author": "you"})
-    pipeline_2.add_node("first_addition", add_2, parameters={"add": 4})
-    pipeline_2.add_node("double", Double(input="value"))
-    pipeline_2.add_node("second_addition", add_1)
+    pipeline_2.add_component("first_addition", add_2, parameters={"add": 4})
+    pipeline_2.add_component("double", Double(input="value"))
+    pipeline_2.add_component("second_addition", add_1)
 
     pipeline_2.connect("first_addition", "double")
     pipeline_2.connect("double", "second_addition")
 
     assert marshal_pipelines(pipelines={"pipe1": pipeline_1, "pipe2": pipeline_2}) == {
         "pipelines": {
             "pipe1": {
                 "metadata": {"type": "test pipeline", "author": "me"},
                 "max_loops_allowed": 100,
-                "nodes": {
+                "components": {
                     "first_addition": {
                         "type": "AddValue",
                         "init_parameters": {"add": 1, "input": "value", "output": "value"},
                         "run_parameters": {"add": 6},
                     },
                     "double": {"type": "Double", "init_parameters": {"input": "value", "output": "value"}},
                     "second_addition": {
                         "type": "AddValue",
                         "init_parameters": {"add": 1, "input": "value", "output": "value"},
                     },
                     "third_addition": {"refer_to": "pipe1.first_addition"},
                 },
-                "edges": [
+                "connections": [
                     ("first_addition", "double"),
                     ("double", "second_addition"),
                     ("second_addition", "third_addition"),
                 ],
             },
             "pipe2": {
                 "metadata": {"type": "another test pipeline", "author": "you"},
                 "max_loops_allowed": 100,
-                "nodes": {
+                "components": {
                     "first_addition": {"refer_to": "pipe1.first_addition", "run_parameters": {"add": 4}},
                     "double": {"type": "Double", "init_parameters": {"input": "value", "output": "value"}},
                     "second_addition": {"refer_to": "pipe1.second_addition"},
                 },
-                "edges": [
+                "connections": [
                     ("first_addition", "double"),
                     ("double", "second_addition"),
                 ],
             },
         },
         "dependencies": ["test", "canals"],
     }
@@ -77,101 +77,101 @@
 def test_unmarshal():
     pipelines = unmarshal_pipelines(
         {
             "pipelines": {
                 "pipe1": {
                     "metadata": {"type": "test pipeline", "author": "me"},
                     "max_loops_allowed": 100,
-                    "nodes": {
+                    "components": {
                         "first_addition": {
                             "type": "AddValue",
                             "init_parameters": {"add": 1, "input": "value", "output": "value"},
                             "run_parameters": {"add": 6},
                         },
                         "double": {"type": "Double", "init_parameters": {"input": "value", "output": "value"}},
                         "second_addition": {
                             "type": "AddValue",
                             "init_parameters": {"add": 1, "input": "value", "output": "value"},
                         },
                         "third_addition": {"refer_to": "pipe1.first_addition"},
                     },
-                    "edges": [
+                    "connections": [
                         ("first_addition", "double"),
                         ("double", "second_addition"),
                         ("second_addition", "third_addition"),
                     ],
                 },
                 "pipe2": {
                     "metadata": {"type": "another test pipeline", "author": "you"},
                     "max_loops_allowed": 100,
-                    "nodes": {
+                    "components": {
                         "first_addition": {"refer_to": "pipe1.first_addition", "run_parameters": {"add": 4}},
                         "double": {"type": "Double", "init_parameters": {"input": "value", "output": "value"}},
                         "second_addition": {"refer_to": "pipe1.second_addition"},
                     },
-                    "edges": [
+                    "connections": [
                         ("first_addition", "double"),
                         ("double", "second_addition"),
                     ],
                 },
             },
             "dependencies": ["test", "canals"],
         }
     )
 
     pipe1 = pipelines["pipe1"]
     assert pipe1.metadata == {"type": "test pipeline", "author": "me"}
 
-    first_addition = pipe1.get_node("first_addition")
+    first_addition = pipe1.get_component("first_addition")
     assert type(first_addition["instance"]) == AddValue
     assert first_addition["instance"].add == 1
     assert first_addition["parameters"] == {"add": 6}
 
-    second_addition = pipe1.get_node("second_addition")
+    second_addition = pipe1.get_component("second_addition")
     assert type(second_addition["instance"]) == AddValue
     assert second_addition["instance"].add == 1
     assert second_addition["parameters"] == {}
     assert second_addition["instance"] != first_addition["instance"]
 
-    third_addition = pipe1.get_node("third_addition")
+    third_addition = pipe1.get_component("third_addition")
     assert type(third_addition["instance"]) == AddValue
     assert third_addition["instance"].add == 1
     assert third_addition["parameters"] == {}
     assert third_addition["instance"] == first_addition["instance"]
 
-    double = pipe1.get_node("double")
+    double = pipe1.get_component("double")
     assert type(double["instance"]) == Double
     assert double["parameters"] == {}
 
     assert list(pipe1.graph.edges) == [
         ("first_addition", "double"),
         ("double", "second_addition"),
         ("second_addition", "third_addition"),
     ]
 
     pipe2 = pipelines["pipe2"]
     assert pipe2.metadata == {"type": "another test pipeline", "author": "you"}
 
-    first_addition_2 = pipe2.get_node("first_addition")
+    first_addition_2 = pipe2.get_component("first_addition")
     assert type(first_addition_2["instance"]) == AddValue
     assert first_addition_2["instance"].add == 1
     assert first_addition_2["parameters"] == {"add": 4}
     assert first_addition_2["instance"] == first_addition["instance"]
 
-    second_addition_2 = pipe2.get_node("second_addition")
+    second_addition_2 = pipe2.get_component("second_addition")
     assert type(second_addition_2["instance"]) == AddValue
     assert second_addition_2["instance"].add == 1
     assert second_addition_2["parameters"] == {}
     assert second_addition_2["instance"] != first_addition_2["instance"]
     assert second_addition_2["instance"] == second_addition["instance"]
 
     with pytest.raises(ValueError):
-        pipe2.get_node("third_addition")
+        pipe2.get_component("third_addition")
 
-    double_2 = pipe2.get_node("double")
+    double_2 = pipe2.get_component("double")
     assert type(double_2["instance"]) == Double
     assert double_2["parameters"] == {}
     assert double_2["instance"] != double["instance"]
 
     assert list(pipe2.graph.edges) == [
         ("first_addition", "double"),
         ("double", "second_addition"),
```

### Comparing `canals-0.0.1rc6/test/nodes/test_add_value.py` & `canals-0.0.2/test/components/test_add_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from typing import Dict, Any, List, Tuple
 
-from canals import node
+from canals import component
 
 
-@node
+@component
 class AddValue:
     def __init__(self, add: int = 1, input: str = "value", output: str = "value"):
         """
-        Adds the value of `add` to the value of the incoming edge.
+        Adds the value of `add` to the value of the incoming connection.
 
-        Single input, single output node.
+        Single input, single output component.
 
         :param add: the value to add. This is also a parameter.
-        :param input: name of the input edge
-        :param output: name of the output edge
+        :param input: name of the input connection
+        :param output: name of the output connection
         """
         self.add = add
 
         self.init_parameters = {"add": add, "input": input, "output": output}
         self.inputs = [input]
         self.outputs = [output]
 
     def run(self, name: str, data: List[Tuple[str, Any]], parameters: Dict[str, Any]):
         sum = parameters.get(name, {}).get("add", self.add)
         sum += data[0][1]
         return ({self.outputs[0]: sum}, parameters)
 
 
 def test_addvalue_default():
-    node = AddValue()
-    results = node.run(name="test_node", data=[("value", 10)], parameters={})
+    component = AddValue()
+    results = component.run(name="test_component", data=[("value", 10)], parameters={})
     assert results == ({"value": 11}, {})
-    assert node.init_parameters == {"add": 1, "input": "value", "output": "value"}
+    assert component.init_parameters == {"add": 1, "input": "value", "output": "value"}
 
 
 def test_addvalue_init_params():
-    node = AddValue(add=3, input="test_in", output="test_out")
-    results = node.run(name="test_node", data=[("test_in", 10)], parameters={})
+    component = AddValue(add=3, input="test_in", output="test_out")
+    results = component.run(name="test_component", data=[("test_in", 10)], parameters={})
     assert results == ({"test_out": 13}, {})
-    assert node.init_parameters == {"add": 3, "input": "test_in", "output": "test_out"}
+    assert component.init_parameters == {"add": 3, "input": "test_in", "output": "test_out"}
 
 
 def test_addvalue_runtime_params():
-    node = AddValue(add=3, input="test_in", output="test_out")
-    results = node.run(name="test_node", data=[("test_in", 10)], parameters={"test_node": {"add": 5}})
-    assert results == ({"test_out": 15}, {"test_node": {"add": 5}})
-    assert node.init_parameters == {"add": 3, "input": "test_in", "output": "test_out"}
+    component = AddValue(add=3, input="test_in", output="test_out")
+    results = component.run(name="test_component", data=[("test_in", 10)], parameters={"test_component": {"add": 5}})
+    assert results == ({"test_out": 15}, {"test_component": {"add": 5}})
+    assert component.init_parameters == {"add": 3, "input": "test_in", "output": "test_out"}
```

### Comparing `canals-0.0.1rc6/test/nodes/test_double.py` & `canals-0.0.2/test/components/test_double.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Dict, Any, List, Tuple
 
-from canals import node
+from canals import component
 
 
-@node
+@component
 class Double:
     def __init__(self, input: str = "value", output: str = "value"):
         """
         Doubles the value in input.
 
-        Single input single output node. Doesn't take parameters.
+        Single input single output component. Doesn't take parameters.
 
         :param input: the name of the input.
         :param output: the name of the output.
         """
         self.init_parameters = {"input": input, "output": output}
         self.inputs = [input]
         self.outputs = [output]
@@ -22,18 +22,18 @@
         for _, value in data:
             value *= 2
 
         return ({self.outputs[0]: value}, parameters)
 
 
 def test_double_default():
-    node = Double()
-    results = node.run(name="test_node", data=[("value", 10)], parameters={})
+    component = Double()
+    results = component.run(name="test_component", data=[("value", 10)], parameters={})
     assert results == ({"value": 20}, {})
-    assert node.init_parameters == {"input": "value", "output": "value"}
+    assert component.init_parameters == {"input": "value", "output": "value"}
 
 
 def test_double_init_params():
-    node = Double(input="test_in", output="test_out")
-    results = node.run(name="test_node", data=[("test_in", 10)], parameters={})
+    component = Double(input="test_in", output="test_out")
+    results = component.run(name="test_component", data=[("test_in", 10)], parameters={})
     assert results == ({"test_out": 20}, {})
-    assert node.init_parameters == {"input": "test_in", "output": "test_out"}
+    assert component.init_parameters == {"input": "test_in", "output": "test_out"}
```

### Comparing `canals-0.0.1rc6/test/nodes/test_merge.py` & `canals-0.0.2/test/components/test_merge.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Dict, Any, List, Tuple
 
-from canals import node
+from canals import component
 
 
-@node
+@component
 class Merge:
     def __init__(
         self,
         inputs: List[str] = ["value"],
         output: str = "value",
     ):
         """
-        Takes several input nodes and returns the first one that is not None.
-        If no input edges received any value, returns None as well.
+        Takes several input components and returns the first one that is not None.
+        If no input connections received any value, returns None as well.
 
-        Multi input, single output node. Doesn't take any parameter.
+        Multi input, single output component. Doesn't take any parameter.
 
         :param inputs: the inputs to expect.
-        :param output: the name of the output edge.
+        :param output: the name of the output connection.
         """
         self.output = output
         self.init_parameters = {
             "inputs": inputs,
             "output": output,
         }
         self.inputs = inputs
@@ -30,20 +30,20 @@
     def run(self, name: str, data: List[Tuple[str, Any]], parameters: Dict[str, Any]):
         for _, value in data:
             if value is not None:
                 return ({self.outputs[0]: value}, parameters)
 
 
 def test_merge_default():
-    node = Merge()
-    results = node.run(name="test_node", data=[("value", 5)], parameters={})
+    component = Merge()
+    results = component.run(name="test_component", data=[("value", 5)], parameters={})
     assert results == ({"value": 5}, {})
-    assert node.init_parameters == {
+    assert component.init_parameters == {
         "inputs": ["value"],
         "output": "value",
     }
 
 
 def test_merge_init_parameters():
-    node = Merge(inputs=["test1", "test2", "test3"], output="test")
-    results = node.run(name="test_node", data=[("test1", None), ("test2", 5), ("test3", 10)], parameters={})
+    component = Merge(inputs=["test1", "test2", "test3"], output="test")
+    results = component.run(name="test_component", data=[("test1", None), ("test2", 5), ("test3", 10)], parameters={})
     assert results == ({"test": 5}, {})
```

### Comparing `canals-0.0.1rc6/test/nodes/test_repeat.py` & `canals-0.0.2/test/components/test_sum.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-from typing import Dict, Any, List, Tuple, Set
+from typing import Dict, Any, List, Tuple
 
-from canals import node
+from canals import component
 
 
-@node
-class Repeat:
-    """
-    Repeats the input value on all outputs.
-
-    Single input, multi output node. Order of outputs is irrelevant.
-    Doesn't accept parameters.
-
-    :param input: the name of the input edge.
-    :param outputs: the list of the output edges.
-    """
-
-    def __init__(self, input: str = "value", outputs: Set[str] = {"first", "second"}):
-        self.init_parameters = {
-            "input": input,
-            "outputs": outputs,
-        }
-        self.inputs = [input]
-        self.outputs = outputs
+@component
+class Sum:
+    def __init__(self, inputs: List[str] = ["value"], output: str = "sum"):
+        """
+        Sums the values of all the input connections together.
+
+        Multi input, single output component. Order of input connections is irrelevant.
+         Doesn't have parameters.
+
+        :param inputs: list of connections to sum.
+        :param output: name of the output connection.
+        """
+        self.init_parameters = {"inputs": inputs, "output": output}
+        self.inputs = inputs
+        self.outputs = [output]
 
     def run(self, name: str, data: List[Tuple[str, Any]], parameters: Dict[str, Any]):
-        return ({output: data[0][1] for output in self.outputs}, parameters)
-
-
-def test_repeat_default():
-    node = Repeat()
-    results = node.run(name="test_node", data=[("value", 10)], parameters={})
-    assert results == ({"first": 10, "second": 10}, {})
-    assert node.init_parameters == {"input": "value", "outputs": {"first", "second"}}
-
-
-def test_repeat_init_params():
-    node = Repeat(input="test", outputs={"one", "two"})
-    results = node.run(name="test_node", data=[("test", 10)], parameters={})
-    assert results == ({"one": 10, "two": 10}, {})
-    assert node.init_parameters == {"input": "test", "outputs": {"one", "two"}}
+        sum = 0
+        for _, value in data:
+            if value:
+                sum += value
+
+        return ({self.outputs[0]: sum}, parameters)
+
+
+def test_sum_default():
+    component = Sum()
+    results = component.run(name="test_component", data=[("value", 10)], parameters={})
+    assert results == ({"sum": 10}, {})
+    assert component.init_parameters == {"inputs": ["value"], "output": "sum"}
+
+
+def test_sum_init_params():
+    component = Sum(inputs=["value", "value"], output="test_out")
+    results = component.run(name="test_component", data=[("value", 10), ("value", 4)], parameters={})
+    assert results == ({"test_out": 14}, {})
+    assert component.init_parameters == {"inputs": ["value", "value"], "output": "test_out"}
```

### Comparing `canals-0.0.1rc6/test/nodes/test_subtract.py` & `canals-0.0.2/test/components/test_subtract.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Dict, Any, List, Tuple
 
-from canals import node
+from canals import component
 
 
-@node
+@component
 class Subtract:
     def __init__(self, first_input: str, second_input: str, output: str = "diff"):
         """
-        Subtracts the second edge's value from the first.
+        Subtracts the second connection's value from the first.
 
-        Double input, single output node. Order of input edges is critical.
+        Double input, single output component. Order of input connections is critical.
         Doesn't have parameters.
 
-        :param first_input: name of the edge carrying the value to subtract from.
-        :param second_input: name of the edge carrying the value to subtract.
-        :param output: name of the output edge.
+        :param first_input: name of the connection carrying the value to subtract from.
+        :param second_input: name of the connection carrying the value to subtract.
+        :param output: name of the output connection.
         """
         self.init_parameters = {"first_input": first_input, "second_input": second_input, "output": output}
         self.inputs = [first_input, second_input]
         self.outputs = [output]
 
     def run(self, name: str, data: List[Tuple[str, Any]], parameters: Dict[str, Any]):
         first_value = [value for name, value in data if name == self.inputs[0]][0]
         second_value = [value for name, value in data if name == self.inputs[1]][0]
 
         return ({"diff": first_value - second_value}, parameters)
 
 
 def test_subtract():
-    node = Subtract(first_input="first", second_input="second", output="diff")
-    results = node.run(name="test_node", data=[("second", 7), ("first", 10)], parameters={})
+    component = Subtract(first_input="first", second_input="second", output="diff")
+    results = component.run(name="test_component", data=[("second", 7), ("first", 10)], parameters={})
     assert results == ({"diff": 3}, {})
-    assert node.init_parameters == {"first_input": "first", "second_input": "second", "output": "diff"}
+    assert component.init_parameters == {"first_input": "first", "second_input": "second", "output": "diff"}
```

### Comparing `canals-0.0.1rc6/test/pipelines/_test_looping_and_merge_pipeline.py` & `canals-0.0.2/test/pipelines/test_looping_pipeline.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 from typing import *
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.nodes import Accumulate, AddValue, Below, Merge, Sum
+from test.components import Accumulate, AddValue, Below, Merge
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
-    accumulator = Accumulate(edge="value")
+    accumulator = Accumulate(connection="value")
 
     pipeline = Pipeline(max_loops_allowed=10)
-    pipeline.add_node("merge", Merge(), input_node=True)
-    pipeline.add_node("sum", Sum(inputs=["value", "value"]), input_node=True)
-    pipeline.add_node("below_10", Below(threshold=10))
-    pipeline.add_node("add_one", AddValue(add=1, input="below"))
-    pipeline.add_node("counter", accumulator)
-    pipeline.add_node("add_two", AddValue(add=2, input="above"))
+    pipeline.add_component("merge", Merge(inputs=["value", "value"]), input_component=True)
+    pipeline.add_component("below_10", Below(threshold=10))
+    pipeline.add_component("add_one", AddValue(add=1, input="below"))
+    pipeline.add_component("accumulator", accumulator)
+    pipeline.add_component("add_two", AddValue(add=2, input="above"))
 
     pipeline.connect("merge", "below_10")
     pipeline.connect("below_10.below", "add_one")
-    pipeline.connect("add_one", "counter")
-    pipeline.connect("counter", "merge")
+    pipeline.connect("add_one", "accumulator")
+    pipeline.connect("accumulator", "merge")
     pipeline.connect("below_10.above", "add_two")
-    pipeline.connect("add_two", "sum")
 
-    pipeline.draw(tmp_path / "looping_and_merge_pipeline.png")
+    try:
+        pipeline.draw(tmp_path / "looping_pipeline.png")
+    except ImportError:
+        logging.warning("pygraphviz not found, pipeline is not being drawn.")
 
     results = pipeline.run(
         {"value": 3},
     )
     pprint(results)
-    print("accumulate: ", accumulator.state)
+    print("accumulator: ", accumulator.state)
 
-    assert results == {"sum": 15}
-    assert accumulator.state == 7
+    assert results == {"value": 12}
+    assert accumulator.state == 49
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.0.1rc6/test/pipelines/test_decision_and_merge_pipeline.py` & `canals-0.0.2/test/pipelines/test_decision_and_merge_pipeline.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import logging
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.nodes import AddValue, Remainder, Double, Sum
+from test.components import AddValue, Remainder, Double, Sum
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
     add_one = AddValue(add=1, input="value")
 
     pipeline = Pipeline()
-    pipeline.add_node("add_one", add_one)
-    pipeline.add_node("remainder", Remainder(input="value", divisor=3))
-    pipeline.add_node("add_ten", AddValue(add=10, input="0"))
-    pipeline.add_node("double", Double(input="1", output="value"))
-    pipeline.add_node("add_three", AddValue(add=3, input="2"))
-    pipeline.add_node("add_one_again", add_one)
-    pipeline.add_node("sum", Sum(inputs=["value"] * 4), input_node=True)
+    pipeline.add_component("add_one", add_one)
+    pipeline.add_component("remainder", Remainder(input="value", divisor=3))
+    pipeline.add_component("add_ten", AddValue(add=10, input="0"))
+    pipeline.add_component("double", Double(input="1", output="value"))
+    pipeline.add_component("add_three", AddValue(add=3, input="2"))
+    pipeline.add_component("add_one_again", add_one)
+    pipeline.add_component("sum", Sum(inputs=["value"] * 4), input_component=True)
 
     pipeline.connect("add_one", "remainder")
     pipeline.connect("remainder.0", "add_ten")
     pipeline.connect("remainder.1", "double")
     pipeline.connect("add_ten", "sum")
     pipeline.connect("double", "sum")
     pipeline.connect("remainder.2", "add_three")
```

### Comparing `canals-0.0.1rc6/test/pipelines/test_decision_pipeline.py` & `canals-0.0.2/test/pipelines/test_decision_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.nodes import AddValue, Remainder, Double
+from test.components import AddValue, Remainder, Double
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
     add_one = AddValue(add=1)
 
     pipeline = Pipeline()
-    pipeline.add_node("add_one", add_one)
-    pipeline.add_node("remainder", Remainder(input="value", divisor=3))
-    pipeline.add_node("add_ten", AddValue(add=10, input="0"))
-    pipeline.add_node("double", Double(input="1", output="value"))
-    pipeline.add_node("add_three", AddValue(add=3, input="2"))
-    pipeline.add_node("add_one_again", add_one)
+    pipeline.add_component("add_one", add_one)
+    pipeline.add_component("remainder", Remainder(input="value", divisor=3))
+    pipeline.add_component("add_ten", AddValue(add=10, input="0"))
+    pipeline.add_component("double", Double(input="1", output="value"))
+    pipeline.add_component("add_three", AddValue(add=3, input="2"))
+    pipeline.add_component("add_one_again", add_one)
 
     pipeline.connect("add_one", "remainder")
     pipeline.connect("remainder.0", "add_ten")
     pipeline.connect("remainder.1", "double")
     pipeline.connect("remainder.2", "add_three")
     pipeline.connect("add_three", "add_one_again")
```

### Comparing `canals-0.0.1rc6/test/pipelines/test_linear_pipeline.py` & `canals-0.0.2/test/pipelines/test_linear_pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.nodes import AddValue, Double
+from test.components import AddValue, Double
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
     pipeline = Pipeline()
-    pipeline.add_node("first_addition", AddValue(add=2))
-    pipeline.add_node("second_addition", AddValue(add=1))
-    pipeline.add_node("double", Double(input="value"))
+    pipeline.add_component("first_addition", AddValue(add=2))
+    pipeline.add_component("second_addition", AddValue(add=1))
+    pipeline.add_component("double", Double(input="value"))
     pipeline.connect("first_addition", "double")
     pipeline.connect("double", "second_addition")
 
     try:
         pipeline.draw(tmp_path / "linear_pipeline.png")
     except ImportError:
         logging.warning("pygraphviz not found, pipeline is not being drawn.")
```

### Comparing `canals-0.0.1rc6/test/pipelines/test_looping_pipeline.py` & `canals-0.0.2/test/pipelines/_test_looping_and_merge_pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 from typing import *
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.nodes import Accumulate, AddValue, Below, Merge
+from test.components import Accumulate, AddValue, Below, Merge, Sum
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
-    accumulator = Accumulate(edge="value")
+    accumulator = Accumulate(connection="value")
 
     pipeline = Pipeline(max_loops_allowed=10)
-    pipeline.add_node("merge", Merge(inputs=["value", "value"]), input_node=True)
-    pipeline.add_node("below_10", Below(threshold=10))
-    pipeline.add_node("add_one", AddValue(add=1, input="below"))
-    pipeline.add_node("accumulator", accumulator)
-    pipeline.add_node("add_two", AddValue(add=2, input="above"))
+    pipeline.add_component("merge", Merge(), input_component=True)
+    pipeline.add_component("sum", Sum(inputs=["value", "value"]), input_component=True)
+    pipeline.add_component("below_10", Below(threshold=10))
+    pipeline.add_component("add_one", AddValue(add=1, input="below"))
+    pipeline.add_component("counter", accumulator)
+    pipeline.add_component("add_two", AddValue(add=2, input="above"))
 
     pipeline.connect("merge", "below_10")
     pipeline.connect("below_10.below", "add_one")
-    pipeline.connect("add_one", "accumulator")
-    pipeline.connect("accumulator", "merge")
+    pipeline.connect("add_one", "counter")
+    pipeline.connect("counter", "merge")
     pipeline.connect("below_10.above", "add_two")
+    pipeline.connect("add_two", "sum")
 
-    try:
-        pipeline.draw(tmp_path / "looping_pipeline.png")
-    except ImportError:
-        logging.warning("pygraphviz not found, pipeline is not being drawn.")
+    pipeline.draw(tmp_path / "looping_and_merge_pipeline.png")
 
     results = pipeline.run(
         {"value": 3},
     )
     pprint(results)
-    print("accumulator: ", accumulator.state)
+    print("accumulate: ", accumulator.state)
 
-    assert results == {"value": 12}
-    assert accumulator.state == 49
+    assert results == {"sum": 15}
+    assert accumulator.state == 7
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.0.1rc6/test/pipelines/test_merging_pipeline.py` & `canals-0.0.2/test/pipelines/test_merging_pipeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.nodes import AddValue, Sum
+from test.components import AddValue, Sum
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
 
     add_two = AddValue(add=2)
     make_the_sum = Sum(inputs=["value"] * 2)
 
     pipeline = Pipeline()
-    pipeline.add_node("first_addition", add_two)
-    pipeline.add_node("second_addition", add_two)
-    pipeline.add_node("third_addition", add_two)
-    pipeline.add_node("sum", make_the_sum)
-    pipeline.add_node("fourth_addition", AddValue(add=1, input="sum"))
+    pipeline.add_component("first_addition", add_two)
+    pipeline.add_component("second_addition", add_two)
+    pipeline.add_component("third_addition", add_two)
+    pipeline.add_component("sum", make_the_sum)
+    pipeline.add_component("fourth_addition", AddValue(add=1, input="sum"))
 
     pipeline.connect("first_addition", "second_addition")
     pipeline.connect("second_addition", "sum")
     pipeline.connect("third_addition", "sum")
     pipeline.connect("sum", "fourth_addition")
 
     try:
```

### Comparing `canals-0.0.1rc6/.gitignore` & `canals-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `canals-0.0.1rc6/LICENSE` & `canals-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `canals-0.0.1rc6/README.md` & `canals-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# 🌊 Canals 🌊
+# Canals
 
 <p align="center" float="left">
-  <img alt="" src="https://raw.githubusercontent.com/deepset-ai/.github/main/deepset-logo-colored.png" width="30%"/>
-  <img alt="" src="https://raw.githubusercontent.com/deepset-ai/.github/main/haystack-logo-colored-on-dark.png#gh-dark-mode-only" width="30%"/>
-  <img alt="" src="https://raw.githubusercontent.com/deepset-ai/.github/main/haystack-logo-colored.png#gh-light-mode-only" width="30%"/>
+  <img alt="" src="https://raw.githubusercontent.com/deepset-ai/canals/main/images/canals-logo-light.png#gh-dark-mode-only"/>
+  <img alt="" src="https://raw.githubusercontent.com/deepset-ai/canals/main/images/canals-logo-dark.png#gh-light-mode-only"/>
 </p>
 
 [![PyPI - Version](https://img.shields.io/pypi/v/canals.svg)](https://pypi.org/project/canals)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/canals.svg)](https://pypi.org/project/canals)
 
-Canals is a **node orchestration engine**. Nodes are Python objects that can execute a task, like reading a file, performing calculations, or making API calls. Canals connects these objects together: it builds a graph of nodes and takes care of managing their execution order, making sure that each object receives the input it expects from the other nodes of the pipeline.
+Canals is a **component orchestration engine**. Components are Python objects that can execute a task, like reading a file, performing calculations, or making API calls. Canals connects these objects together: it builds a graph of components and takes care of managing their execution order, making sure that each object receives the input it expects from the other components of the pipeline.
 
 Canals powers version 2.0 of the [Haystack framework](https://github.com/deepset-ai/haystack).
 
 ## Installation
 
 Running:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `canals-0.0.1rc6/pyproject.toml` & `canals-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "canals"
-description = 'A node orchestration engine for Haystack'
+description = 'A component orchestration engine for Haystack'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "ZanSara", email = "sara.zanzottera@deepset.ai" },
 ]
@@ -38,14 +38,20 @@
   "pre-commit",
   "mypy",
   "pylint==2.15.10",
   "black[jupyter]==22.6.0",
   "pytest",
   "coverage",
 ]
+docs = [
+  "mkdocs-material",
+  "mkdocstrings[python]",
+  "mkdocs-mermaid2-plugin"
+
+]
 all = ["canals[draw,dev]"]
 
 
 [project.urls]
 Documentation = "https://github.com/deepset-ai/canals#readme"
 Issues = "https://github.com/deepset-ai/canals/issues"
 Source = "https://github.com/deepset-ai/canals"
```

### Comparing `canals-0.0.1rc6/PKG-INFO` & `canals-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: canals
-Version: 0.0.1rc6
-Summary: A node orchestration engine for Haystack
+Version: 0.0.2
+Summary: A component orchestration engine for Haystack
 Project-URL: Documentation, https://github.com/deepset-ai/canals#readme
 Project-URL: Issues, https://github.com/deepset-ai/canals/issues
 Project-URL: Source, https://github.com/deepset-ai/canals
 Author-email: ZanSara <sara.zanzottera@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -26,30 +26,33 @@
 Requires-Dist: black[jupyter]==22.6.0; extra == 'dev'
 Requires-Dist: coverage; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pylint==2.15.10; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: mkdocs-material; extra == 'docs'
+Requires-Dist: mkdocs-mermaid2-plugin; extra == 'docs'
+Requires-Dist: mkdocstrings[python]; extra == 'docs'
 Provides-Extra: draw
 Requires-Dist: pygraphviz; extra == 'draw'
 Description-Content-Type: text/markdown
 
-# 🌊 Canals 🌊
+# Canals
 
 <p align="center" float="left">
-  <img alt="" src="https://raw.githubusercontent.com/deepset-ai/.github/main/deepset-logo-colored.png" width="30%"/>
-  <img alt="" src="https://raw.githubusercontent.com/deepset-ai/.github/main/haystack-logo-colored-on-dark.png#gh-dark-mode-only" width="30%"/>
-  <img alt="" src="https://raw.githubusercontent.com/deepset-ai/.github/main/haystack-logo-colored.png#gh-light-mode-only" width="30%"/>
+  <img alt="" src="https://raw.githubusercontent.com/deepset-ai/canals/main/images/canals-logo-light.png#gh-dark-mode-only"/>
+  <img alt="" src="https://raw.githubusercontent.com/deepset-ai/canals/main/images/canals-logo-dark.png#gh-light-mode-only"/>
 </p>
 
 [![PyPI - Version](https://img.shields.io/pypi/v/canals.svg)](https://pypi.org/project/canals)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/canals.svg)](https://pypi.org/project/canals)
 
-Canals is a **node orchestration engine**. Nodes are Python objects that can execute a task, like reading a file, performing calculations, or making API calls. Canals connects these objects together: it builds a graph of nodes and takes care of managing their execution order, making sure that each object receives the input it expects from the other nodes of the pipeline.
+Canals is a **component orchestration engine**. Components are Python objects that can execute a task, like reading a file, performing calculations, or making API calls. Canals connects these objects together: it builds a graph of components and takes care of managing their execution order, making sure that each object receives the input it expects from the other components of the pipeline.
 
 Canals powers version 2.0 of the [Haystack framework](https://github.com/deepset-ai/haystack).
 
 ## Installation
 
 Running:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

