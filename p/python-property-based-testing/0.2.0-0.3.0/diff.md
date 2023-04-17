# Comparing `tmp/python_property_based_testing-0.2.0.tar.gz` & `tmp/python_property_based_testing-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_property_based_testing-0.2.0.tar", max compression
+gzip compressed data, was "python_property_based_testing-0.3.0.tar", max compression
```

## Comparing `python_property_based_testing-0.2.0.tar` & `python_property_based_testing-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2023-04-16 11:55:27.759685 python_property_based_testing-0.2.0/LICENSE
--rw-r--r--   0        0        0     8116 2023-04-16 11:55:27.759685 python_property_based_testing-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-16 11:55:27.759685 python_property_based_testing-0.2.0/pybt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 11:55:27.759685 python_property_based_testing-0.2.0/pybt/core/__init__.py
--rw-r--r--   0        0        0     6720 2023-04-16 11:55:27.759685 python_property_based_testing-0.2.0/pybt/core/core.py
--rw-r--r--   0        0        0     3195 2023-04-16 11:55:27.759685 python_property_based_testing-0.2.0/pybt/core/util.py
--rw-r--r--   0        0        0        0 2023-04-16 11:55:27.759685 python_property_based_testing-0.2.0/pybt/tests/__init__.py
--rw-r--r--   0        0        0      575 2023-04-16 11:55:27.759685 python_property_based_testing-0.2.0/pybt/tests/simple_nonclass_test.py
--rw-r--r--   0        0        0      628 2023-04-16 11:55:27.759685 python_property_based_testing-0.2.0/pybt/tests/simple_unit_test.py
--rw-r--r--   0        0        0      433 2023-04-16 11:55:27.759685 python_property_based_testing-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8567 1970-01-01 00:00:00.000000 python_property_based_testing-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/LICENSE
+-rw-r--r--   0        0        0     8292 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pybt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pybt/core/__init__.py
+-rw-r--r--   0        0        0     6720 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pybt/core/core.py
+-rw-r--r--   0        0        0     3195 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pybt/core/util.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pybt/tests/__init__.py
+-rw-r--r--   0        0        0      575 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pybt/tests/simple_nonclass_test.py
+-rw-r--r--   0        0        0      628 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pybt/tests/simple_unit_test.py
+-rw-r--r--   0        0        0      425 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8634 1970-01-01 00:00:00.000000 python_property_based_testing-0.3.0/PKG-INFO
```

### Comparing `python_property_based_testing-0.2.0/LICENSE` & `python_property_based_testing-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.2.0/README.md` & `python_property_based_testing-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 ## PyBT
 
+## Installation 
+
+```python
+pip install python-property-based-testing 
+```
+
 ## Introduction 
 
+You can find a primer on property-based testing [here](https://vrindisbacher.github.io/pybt.pdf). 
+
 `PyBT` is a library for property based testing in python. The main idea, is to state and randomly test properties about functions at large scale. The main functionality `PyBT` provides is a decorator named `pybt`. 
 
 The parameter takes the following arguments:
 
 * **n**: the number of tests to run (defaults to 1000).
 
 * **generators**: user provided generators to be used to generate function arguments (defaults to None).
```

### Comparing `python_property_based_testing-0.2.0/pybt/core/core.py` & `python_property_based_testing-0.3.0/pybt/core/core.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.2.0/pybt/core/util.py` & `python_property_based_testing-0.3.0/pybt/core/util.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.2.0/pybt/tests/simple_nonclass_test.py` & `python_property_based_testing-0.3.0/pybt/tests/simple_nonclass_test.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.2.0/pybt/tests/simple_unit_test.py` & `python_property_based_testing-0.3.0/pybt/tests/simple_unit_test.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.2.0/PKG-INFO` & `python_property_based_testing-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: python-property-based-testing
-Version: 0.2.0
+Version: 0.3.0
 Summary: Property Based Testing in Python
 Author: vrindisbacher
 Author-email: vrindisbacher77@gmail.com
-Requires-Python: >=3.9,<=3.11.2
+Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 ## PyBT
 
+## Installation 
+
+```python
+pip install python-property-based-testing 
+```
+
 ## Introduction 
 
+You can find a primer on property-based testing [here](https://vrindisbacher.github.io/pybt.pdf). 
+
 `PyBT` is a library for property based testing in python. The main idea, is to state and randomly test properties about functions at large scale. The main functionality `PyBT` provides is a decorator named `pybt`. 
 
 The parameter takes the following arguments:
 
 * **n**: the number of tests to run (defaults to 1000).
 
 * **generators**: user provided generators to be used to generate function arguments (defaults to None).
```

