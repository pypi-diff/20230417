# Comparing `tmp/pysparkler-0.4.dev1681497870.tar.gz` & `tmp/pysparkler-0.4.dev1681747316.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.4.dev1681497870.tar", max compression
+gzip compressed data, was "pysparkler-0.4.dev1681747316.tar", max compression
```

## Comparing `pysparkler-0.4.dev1681497870.tar` & `pysparkler-0.4.dev1681747316.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     8895 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/README.md
--rw-r--r--   0        0        0     1203 2023-04-14 18:44:31.108843 pysparkler-0.4.dev1681497870/pyproject.toml
--rw-r--r--   0        0        0      807 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/__init__.py
--rw-r--r--   0        0        0     4374 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/api.py
--rw-r--r--   0        0        0     5879 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/base.py
--rw-r--r--   0        0        0     5734 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/cli.py
--rw-r--r--   0        0        0     2204 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/pyspark_23_to_24.py
--rw-r--r--   0        0        0    10520 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3967 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     4413 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/pyspark_32_to_33.py
--rw-r--r--   0        0        0     9774 1970-01-01 00:00:00.000000 pysparkler-0.4.dev1681497870/PKG-INFO
+-rw-r--r--   0        0        0     9111 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/README.md
+-rw-r--r--   0        0        0     1203 2023-04-17 16:01:57.251088 pysparkler-0.4.dev1681747316/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/__init__.py
+-rw-r--r--   0        0        0     4374 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/api.py
+-rw-r--r--   0        0        0     6057 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/base.py
+-rw-r--r--   0        0        0     5734 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/cli.py
+-rw-r--r--   0        0        0     2204 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/pyspark_23_to_24.py
+-rw-r--r--   0        0        0    10438 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3967 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     4263 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/pyspark_32_to_33.py
+-rw-r--r--   0        0        0     9990 1970-01-01 00:00:00.000000 pysparkler-0.4.dev1681747316/PKG-INFO
```

### Comparing `pysparkler-0.4.dev1681497870/README.md` & `pysparkler-0.4.dev1681747316/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # PySparkler
 
-## About
+[![PyPI version](https://badge.fury.io/py/pysparkler.svg)](https://badge.fury.io/py/pysparkler)
+[![License: Apache-2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 PySparkler is a tool that upgrades your PySpark scripts to latest Spark version. It is a command line tool that takes a
 PySpark script as input and outputs a latest Spark version compatible script. It is written in Python and uses the
 [LibCST](https://github.com/Instagram/LibCST) module to parse the input script and generate the output script.
 
 ## Basic Usage
```

### Comparing `pysparkler-0.4.dev1681497870/pyproject.toml` & `pysparkler-0.4.dev1681747316/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.4.dev1681497870"
+version = "0.4.dev1681747316"
 description = "A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
```

### Comparing `pysparkler-0.4.dev1681497870/pysparkler/__init__.py` & `pysparkler-0.4.dev1681747316/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681497870/pysparkler/api.py` & `pysparkler-0.4.dev1681747316/pysparkler/api.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681497870/pysparkler/base.py` & `pysparkler-0.4.dev1681747316/pysparkler/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,25 +45,29 @@
         self._comment = comment
         self.match_found = False
 
     @property
     def comment(self):
         return self._comment
 
-    def leave_SimpleStatementLine(self, original_node, updated_node):
-        """Add a comment where to Pandas is being used"""
+    def leave_SimpleStatementLine(
+        self,
+        original_node: cst.SimpleStatementLine,  # pylint: disable=unused-argument
+        updated_node: cst.SimpleStatementLine,
+    ) -> cst.SimpleStatementLine:
+        """Add a comment to the end of the statement line if a matching condition is found"""
         if self.match_found:
             self.match_found = False
             return add_comment_to_end_of_a_simple_statement_line(
                 updated_node,
                 self.transformer_id,
                 f"# {self.transformer_id}: {self.comment}",
             )
         else:
-            return original_node
+            return updated_node
 
 
 class RequiredDependencyVersionCommentWriter(StatementLineCommentWriter):
     """Base class for adding comments to the import statements of required dependencies version of PySpark"""
 
     def __init__(
         self,
```

### Comparing `pysparkler-0.4.dev1681497870/pysparkler/cli.py` & `pysparkler-0.4.dev1681747316/pysparkler/cli.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681497870/pysparkler/pyspark_23_to_24.py` & `pysparkler-0.4.dev1681747316/pysparkler/pyspark_23_to_24.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681497870/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.4.dev1681747316/pysparkler/pyspark_24_to_30.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,40 +185,36 @@
         pyspark_version: str = "3.0",
     ):
         super().__init__(
             transformer_id="PY24-30-007",
             comment=f"Sorting Row fields by name alphabetically since as of Spark {pyspark_version}, they are no longer when constructed with named arguments.",
         )
 
-    def visit_Call(self, node: cst.Call) -> None:
-        """Check if Row(...) is being called with named arguments"""
+    def leave_Call(self, original_node: cst.Call, updated_node: cst.Call) -> cst.Call:
+        """Check if Row(...) is being called with named arguments and sort Dataframe Row fields by name alphabetically
+        when constructed with named arguments for backwards compatibility"""
         if m.matches(
-            node,
+            original_node,
             m.Call(
                 func=m.Name("Row"),
                 args=[
                     m.ZeroOrMore(),
                     m.Arg(keyword=m.Name()),
                     m.ZeroOrMore(),
                 ],
             ),
         ):
             self.match_found = True
-
-    def leave_Call(self, original_node: cst.Call, updated_node: cst.Call) -> cst.Call:
-        """Sort Dataframe Row fields by name alphabetically when constructed with named arguments for backwards
-        compatibility"""
-        if self.match_found:
             row_fields = sorted(
                 updated_node.args,
                 key=lambda arg: arg.keyword.value,
             )
             return updated_node.with_changes(args=row_fields)
         else:
-            return original_node
+            return updated_node
 
 
 class MlParamMixinsSetterCommentWriter(StatementLineCommentWriter):
     """In Spark 3.0, pyspark.ml.param.shared.Has* mixins do not provide any set*(self, value) setter methods anymore,
     use the respective self.set(self.*, value) instead. See SPARK-29093 for details.
     """
```

### Comparing `pysparkler-0.4.dev1681497870/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.4.dev1681747316/pysparkler/pyspark_31_to_32.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681497870/pysparkler/pyspark_32_to_33.py` & `pysparkler-0.4.dev1681747316/pysparkler/pyspark_32_to_33.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,44 +33,41 @@
         self,
         pyspark_version: str = "3.3",
     ):
         super().__init__(
             transformer_id="PY32-33-001",
             comment=f"As of PySpark {pyspark_version}, the drop method of pandas API on Spark DataFrame supports dropping rows by index, and sets dropping by index instead of column by default.",
         )
+        self.inside_drop_call = False
 
-    def visit_Call(self, node: cst.Call) -> None:
-        """Check if the drop method of pandas API on Spark DataFrame is called with only one positional argument"""
+    def leave_Call(self, original_node: cst.Call, updated_node: cst.Call) -> cst.Call:
+        """Specify the axis argument to 1 if it is not specified to maintain the behavior of dropping columns"""
         if m.matches(
-            node,
+            original_node,
             m.Call(
                 func=m.Attribute(
                     attr=m.Name("drop"),
                 ),
                 args=[
                     m.OneOf(
                         m.Arg(keyword=m.Name("labels")),
                         m.Arg(keyword=None),
                     )
                 ],
             ),
         ):
             self.match_found = True
-
-    def leave_Call(self, original_node: cst.Call, updated_node: cst.Call) -> cst.Call:
-        """Specify the axis argument to 1 if it is not specified to maintain the behavior of dropping columns"""
-        if self.match_found:
             return updated_node.with_changes(
                 args=[
                     *updated_node.args,
                     cst.Arg(keyword=cst.Name("axis"), value=cst.Integer("1")),
                 ]
             )
         else:
-            return original_node
+            return updated_node
 
 
 class RequiredPandasVersionCommentWriter(RequiredDependencyVersionCommentWriter):
     """In Spark 3.3, PySpark upgrades Pandas version, the new minimum required version changes from 0.23.2 to 1.0.5."""
 
     def __init__(
         self,
```

### Comparing `pysparkler-0.4.dev1681497870/PKG-INFO` & `pysparkler-0.4.dev1681747316/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.4.dev1681497870
+Version: 0.4.dev1681747316
 Summary: A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
@@ -18,15 +18,16 @@
 Requires-Dist: nbformat (>=5.8.0,<6.0.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Project-URL: Repository, https://github.com/holdenk/spark-upgrade
 Description-Content-Type: text/markdown
 
 # PySparkler
 
-## About
+[![PyPI version](https://badge.fury.io/py/pysparkler.svg)](https://badge.fury.io/py/pysparkler)
+[![License: Apache-2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 PySparkler is a tool that upgrades your PySpark scripts to latest Spark version. It is a command line tool that takes a
 PySpark script as input and outputs a latest Spark version compatible script. It is written in Python and uses the
 [LibCST](https://github.com/Instagram/LibCST) module to parse the input script and generate the output script.
 
 ## Basic Usage
```

