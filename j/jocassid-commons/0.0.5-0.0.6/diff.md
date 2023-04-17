# Comparing `tmp/jocassid_commons-0.0.5.tar.gz` & `tmp/jocassid_commons-0.0.6.tar.gz`

## Comparing `jocassid_commons-0.0.5.tar` & `jocassid_commons-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/Makefile
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/pytest.ini
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/requirements.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/.pytest_cache/README.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/src/jocassid_commons/__init__.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/src/jocassid_commons/accumulator_dict.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/src/jocassid_commons/dirf.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/src/jocassid_commons/json.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/tests/test_accumulator_dict.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/tests/test_dirf.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/tests/test_json.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/LICENSE
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/README.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 jocassid_commons-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/Makefile
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/pytest.ini
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/requirements.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/.pytest_cache/README.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/src/jocassid_commons/__init__.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/src/jocassid_commons/accumulator_dict.py
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/src/jocassid_commons/data_structures.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/src/jocassid_commons/dirf.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/src/jocassid_commons/json.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/tests/test_accumulator_dict.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/tests/test_data_structures.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/tests/test_dirf.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/tests/test_json.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/LICENSE
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/README.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 jocassid_commons-0.0.6/PKG-INFO
```

### Comparing `jocassid_commons-0.0.5/src/jocassid_commons/accumulator_dict.py` & `jocassid_commons-0.0.6/src/jocassid_commons/accumulator_dict.py`

 * *Files identical despite different names*

### Comparing `jocassid_commons-0.0.5/src/jocassid_commons/dirf.py` & `jocassid_commons-0.0.6/src/jocassid_commons/dirf.py`

 * *Files identical despite different names*

### Comparing `jocassid_commons-0.0.5/src/jocassid_commons/json.py` & `jocassid_commons-0.0.6/src/jocassid_commons/json.py`

 * *Files identical despite different names*

### Comparing `jocassid_commons-0.0.5/tests/test_accumulator_dict.py` & `jocassid_commons-0.0.6/tests/test_accumulator_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     d1['b'] = 3
     assert d1 == {
         'a': [1, 2],
         'b': [3],
     }
 
     d1['c'] = [4, 5]
-    assert d1  == {
+    assert d1 == {
         'a': [1, 2],
         'b': [3],
         'c': [4, 5]
     }
 
     d2 = AccumulatorDict(set)
```

### Comparing `jocassid_commons-0.0.5/tests/test_dirf.py` & `jocassid_commons-0.0.6/tests/test_dirf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,7 @@
     def test_case_sensitive_contains(self):
         expected = ['foo_bar']
         assert expected == dirf(dir(Thingy), 'bar', ignore_case=False)
 
     def test_startswith(self):
         expected = ['title', 'translate']
         assert expected == dirf(dir('a'), 't', starts_with=True)
-
```

### Comparing `jocassid_commons-0.0.5/tests/test_json.py` & `jocassid_commons-0.0.6/tests/test_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     # Top level is list
     assert json_get([], 42, 0) == 42
     
     # index outside of list bounds
     assert json_get([2, 2], 42, 2) == 42
     
     # 2nd level is list
-    assert json_get({'foo':[2,4,9]}, 42, 'foo', 1) == 4 
+    assert json_get({'foo': [2, 4, 9]}, 42, 'foo', 1) == 4
     
     # 3 levels of lists
     data = [
         [
             [1, 1, 2, 3, 5],
             [1, 1, 4, 9, 25]
         ],
```

### Comparing `jocassid_commons-0.0.5/LICENSE` & `jocassid_commons-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jocassid_commons-0.0.5/pyproject.toml` & `jocassid_commons-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jocassid-commons"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name="John Cassidy", email="author@example.com" },
 ]
 maintainers = [
     { name="John Cassidy", email="author@example.com" },
 ]
 description = "Miscellaneous utility functions"
```

