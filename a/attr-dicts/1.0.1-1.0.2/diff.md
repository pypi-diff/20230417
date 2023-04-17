# Comparing `tmp/attr_dicts-1.0.1.tar.gz` & `tmp/attr_dicts-1.0.2.tar.gz`

## Comparing `attr_dicts-1.0.1.tar` & `attr_dicts-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 attr_dicts-1.0.1/requirements.txt
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 attr_dicts-1.0.1/setup.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 attr_dicts-1.0.1/attrdict/__init__.py
--rw-r--r--   0        0        0    13925 2020-02-02 00:00:00.000000 attr_dicts-1.0.1/attrdict/_base.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 attr_dicts-1.0.1/attrdict/_base_utils.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 attr_dicts-1.0.1/attrdict/test.py
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 attr_dicts-1.0.1/attrdict/utils.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 attr_dicts-1.0.1/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 attr_dicts-1.0.1/LICENSE
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 attr_dicts-1.0.1/README.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 attr_dicts-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 attr_dicts-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 attr_dicts-1.0.2/requirements.txt
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 attr_dicts-1.0.2/setup.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 attr_dicts-1.0.2/attrdict/__init__.py
+-rw-r--r--   0        0        0    14336 2020-02-02 00:00:00.000000 attr_dicts-1.0.2/attrdict/_base.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 attr_dicts-1.0.2/attrdict/_base_utils.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 attr_dicts-1.0.2/attrdict/test.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 attr_dicts-1.0.2/attrdict/utils.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 attr_dicts-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 attr_dicts-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 attr_dicts-1.0.2/README.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 attr_dicts-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 attr_dicts-1.0.2/PKG-INFO
```

### Comparing `attr_dicts-1.0.1/attrdict/_base.py` & `attr_dicts-1.0.2/attrdict/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,21 @@
 
     def __setitem__(self, key, value):
         if isinstance(key, str) and '/' in key:
             # nested assignment
             key_split = key.split('/')
             curr_key = key_split[0]
             next_key = '/'.join(key_split[1:])
-            if curr_key not in self._map and curr_key != '_ipython_canary_method_should_not_exist_':
-                # automatically extend to new AttrDict on set
+            # reinitialize curr_key to an AttrDict() when...
+            # (1) the key is not present, and no ipy flag
+            # (2) the key is present but self[key] is not an AttrDict, and no ipy flag
+            if (curr_key not in self._map or
+                    not isinstance(self[curr_key], self.__class__)) \
+                    and curr_key != '_ipython_canary_method_should_not_exist_':
+                # automatically extend to new AttrDict on set,
                 self[curr_key] = self.__class__()
             self[curr_key][next_key] = value
         else:
             # dotmap based assignment.
             super(AttrDict, self).__setitem__(key, value)
 
     def pprint(self, str_max_len=30, ret_string=False):
@@ -129,14 +134,17 @@
 
     def leaf_filter_keys(self, names):
         return self.leaf_filter(lambda key, value: key in names)
 
     def node_leaf_filter_keys(self, names):
         return self.node_leaf_filter(lambda key, value: key in names)
 
+    def node_leaf_without_keys(self, keys):
+        return self.node_leaf_filter(lambda k, v: k not in keys)
+
     def node_leaf_filter_keys_required(self, names, copy_nodes=False):
         """ Filter with both leaf and node names.
 
         Parameters
         ----------
         names:
             keys to get, can include nodes
```

### Comparing `attr_dicts-1.0.1/attrdict/test.py` & `attr_dicts-1.0.2/attrdict/test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from attrdict import AttrDict
 from attrdict.utils import get_required
 
 if __name__ == '__main__':
     # just an example of how to instantiate
     dc = AttrDict(dict(
+        z='this should be removed',
         a=dict(
             b=1,
             c=2
         )
     ))
     print('dc:', dc.pprint(ret_string=True))
 
     dc_1 = AttrDict(
         a=AttrDict(
             e=4
+        ),
+        z=AttrDict(
+            test=1
         )
     )
     print('dc_1:', dc_1.pprint(ret_string=True))
 
     dc_dup = dc.copy()
 
     combined = dc_dup & dc_1
@@ -25,14 +29,16 @@
     print('dc (original):', dc.pprint(ret_string=True))
 
     assert 'a/b' in dc.leaf_keys()
     assert 'a' in dc.keys()
     assert 'a/e' in combined.leaf_keys()
     assert 'a/e' not in dc.leaf_keys()
 
+    assert 'z/test' in combined.leaf_keys()
+
     # raises a key error
     try:
         f = dc['a/f']
         raise AssertionError('Key a/f should not exist!')
     except KeyError:
         pass
```

### Comparing `attr_dicts-1.0.1/attrdict/utils.py` & `attr_dicts-1.0.2/attrdict/utils.py`

 * *Files identical despite different names*

### Comparing `attr_dicts-1.0.1/LICENSE` & `attr_dicts-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `attr_dicts-1.0.1/README.md` & `attr_dicts-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `attr_dicts-1.0.1/pyproject.toml` & `attr_dicts-1.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "attr-dicts"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Suneel Belkhale", email="belkhale@stanford.edu" },
 ]
 description = "AttrDict for nested dictionary processing and utilities"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `attr_dicts-1.0.1/PKG-INFO` & `attr_dicts-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attr-dicts
-Version: 1.0.1
+Version: 1.0.2
 Summary: AttrDict for nested dictionary processing and utilities
 Project-URL: Homepage, https://github.com/Stanford-ILIAD/attrdict
 Project-URL: Bug Tracker, https://github.com/Stanford-ILIAD/attrdict/issues
 Author-email: Suneel Belkhale <belkhale@stanford.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

