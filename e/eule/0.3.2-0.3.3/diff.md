# Comparing `tmp/eule-0.3.2.tar.gz` & `tmp/eule-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eule-0.3.2.tar", max compression
+gzip compressed data, was "eule-0.3.3.tar", max compression
```

## Comparing `eule-0.3.2.tar` & `eule-0.3.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-02-27 21:15:10.623533 eule-0.3.2/LICENSE
--rw-r--r--   0        0        0     1794 2023-03-19 15:49:57.253200 eule-0.3.2/README.md
--rw-r--r--   0        0        0      205 2023-03-27 14:19:19.843506 eule-0.3.2/eule/__init__.py
--rw-r--r--   0        0        0     4910 2023-03-12 23:04:37.552209 eule-0.3.2/eule/eule.py
--rw-r--r--   0        0        0     1470 2023-03-12 22:07:24.234825 eule-0.3.2/eule/utils.py
--rw-r--r--   0        0        0     1358 2023-04-04 13:13:36.394720 eule-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 eule-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-27 21:15:10.623533 eule-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1794 2023-03-19 15:49:57.253200 eule-0.3.3/README.md
+-rw-r--r--   0        0        0      205 2023-03-27 14:19:19.843506 eule-0.3.3/eule/__init__.py
+-rw-r--r--   0        0        0     5723 2023-04-17 20:44:39.812347 eule-0.3.3/eule/eule.py
+-rw-r--r--   0        0        0     2841 2023-04-17 20:46:01.004663 eule-0.3.3/eule/utils.py
+-rw-r--r--   0        0        0     1358 2023-04-17 20:56:06.487024 eule-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 eule-0.3.3/PKG-INFO
```

### Comparing `eule-0.3.2/LICENSE` & `eule-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eule-0.3.2/README.md` & `eule-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `eule-0.3.2/eule/eule.py` & `eule-0.3.3/eule/eule.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Main module."""
 
 from copy import deepcopy
 from warnings import warn
 
-from .utils import dsort, clear, reduc, uniq, areSpiderKeys
-
-delimiter = ','
+from .utils import update_tuple, clear, reduc, uniq, union, difference, intersection, tuplify
 
 def eulerGenerator(sets):
     """This generator function returns each tuple (key, elems) of the Euler diagram in a generator-wise fashion systematic:
     
     1. Begin with the available `sets` and their exclusive elements;
     2. Compute complementary elements to current key-set;
     3. In case complementary set-keys AND current set content are not empty, continue; Otherwise, go to next key-set;
@@ -22,109 +20,138 @@
     :rtype: tuple
     """
     sets_ = deepcopy(sets)
 
     # There are no sets
     if not isinstance(sets_, (list, dict)):
         msg_1 = 'Ill-conditioned input.'
-        msg_2 = 'It must be either a json-like or array of arrays object!'
+        msg_2 = 'It must be either a dict or array of arrays object!'
         raise TypeError(msg_1 + msg_2)
 
     is_unique_set_arr = [
         len(uniq(values)) == len(values) for values in sets_.values()
     ]
-    if not reduc(lambda a, b: a and b, is_unique_set_arr, True):
+
+    and_map = lambda a, b: a and b
+
+    if not reduc(and_map, is_unique_set_arr, True):
         warn('Each array MUST NOT have duplicates')
         sets = {key: uniq(values) for key, values in sets.items()}
 
     # Only a set
-    if len(sets_.values()) == 1:
+    if len(sets_.keys()) == 1:
         comb_key = list(sets_.keys())[0]
         comb_elements = list(sets_.values())[0]
-        yield (comb_key, comb_elements)
+        yield ((comb_key), comb_elements)
 
     else:
         # Sets with non-empty elements
         set_keys = clear(sets_)
 
         # Traverse the combination lattice
         for set_key in set_keys:
-            compl_sets_keys = list(set(set_keys) - {set_key})
+            compl_sets_keys = difference(set_keys, [set_key])
 
             # There are still sets to analyze
             if len(compl_sets_keys) != 0 and len(sets[set_key]) != 0:
                 # Complementary sets
                 csets = {cset_key: sets_[cset_key] for cset_key in compl_sets_keys}
 
                 # Instrospective recursion: Exclusive combination elements
-                for comb_str, celements in eulerGenerator(csets):
+                for euler_tuple, celements in eulerGenerator(csets):
 
                     # Remove current set_key elements
-                    comb_elems = list(set(celements) - set(sets_[set_key]))
+                    comb_elems = difference(celements, sets_[set_key])
 
                     # Non-empty combination exclusivity case
                     if len(comb_elems) != 0:
                         # Sort keys to assure deterministic behavior
-                        sorted_comb_key = dsort(comb_str, delimiter)
-
+                        sorted_comb_key = tuplify(sorted(tuplify(euler_tuple)))
+                        
                         # 1. Exclusive group elements except current analysis set
                         yield (sorted_comb_key, comb_elems)
 
                         # Remove comb_elems elements from its original sets
-                        for ckey in comb_str.split(delimiter):
-                            sets_[ckey] = list(set(sets_[ckey]) - set(comb_elems))
+                        for euler_set_key in euler_tuple:
+                            sets_[euler_set_key] = difference(sets_[euler_set_key], comb_elems)
+                    else:
+                        pass
 
                     # Retrieve intersection elements
-                    comb_elems = list(
-                        set(celements).intersection(set(sets[set_key])),
-                    )
-
+                    comb_elems = intersection(celements, sets[set_key]) 
+                    
                     # Non-empty intersection set
                     if len(comb_elems) != 0:
                         # 2. Intersection of analysis element and exclusive group:
                         # Sort keys to assure deterministic behavior
-                        comb_key = dsort(
-                            set_key + delimiter + comb_str, delimiter
-                        )
-
+                        comb_key = tuplify(sorted(update_tuple(euler_tuple, set_key)))
+                        
                         yield (comb_key, comb_elems)
 
                         # Remove intersection elements from current key-set and complementary sets
-                        for ckey in comb_str.split(delimiter):
-                            sets_[ckey] = list(set(sets_[ckey]) - set(comb_elems))
+                        for euler_set_key in euler_tuple:
+                            sets_[euler_set_key] = difference(sets_[euler_set_key], comb_elems)
+
+                        sets_[set_key] = difference(sets_[set_key], comb_elems)
 
-                        sets_[set_key] = list(set(sets_[set_key]) - set(comb_elems))
+                    else:
+                        pass
 
                     set_keys = clear(sets_)
 
                 # 3. Remaining exclusive elements
                 if len(sets_[set_key]) != 0:
                     # Load combination key
-                    comb_key = str(set_key)
-                    comb_elems = sets_[set_key]
+                    comb_key = tuplify([set_key])
+                    comb_elems = sets_[set_key]       
 
                     # Yield tuple
                     yield (comb_key, comb_elems)
 
                     # Remove remaining set elements
                     sets_[set_key] = []
+                
+                else:
+                    pass
 
                 set_keys = clear(sets_)
 
 
 def euler(sets):
     """Euler diagram dictionary of set-dictionary of non-repetitive elements
     
     :param dict sets: array/dict of arrays
     :returns: euler sets
     :rtype: dict
     """
+    print(list(eulerGenerator(sets)))
+
     return dict(eulerGenerator(sets))
 
 def eulerKeys(sets):
-    """Euler diagram dictionary of set-dictionary of non-repetitive elements
+    """Euler diagram keys
     
     :param dict sets: array/dict of arrays
-    :returns: euler sets
-    :rtype: dict
+    :returns: euler sets keys
+    :rtype: list
     """
     return list(euler(sets).keys())
+
+def eulerBoundaries(sets):
+    """Euler diagram set boundaries 
+    
+    :param dict sets: array/dict of arrays
+    :returns: euler boundary dict
+    :rtype: list
+    """
+
+    setsKeys = list(sets.keys())
+    eulerSetsKeys = eulerKeys(sets)
+
+    boundaries = dict(map(lambda key: (key, []), setsKeys))
+
+    for setKey in setsKeys:
+        for eulerSetKeys in eulerSetsKeys:
+            if setKey in eulerSetKeys:
+                boundaries[setKey] = union(boundaries[setKey], difference(eulerSetKeys, [setKey]))
+                
+    return {setKey: sorted(neighborsKeys) for setKey, neighborsKeys in boundaries.items()}
```

### Comparing `eule-0.3.2/eule/utils.py` & `eule-0.3.3/eule/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,34 +27,84 @@
 
     :param str str_:  string with delimiter between elements 
     :returns: string with sorted elements delimited by given delimiter 
     :rtype: str
     """
     return delimiter.join(sorted(str_.split(delimiter)))
 
+def tuplify(candidate):
+    """This map returns a tuple element on given candidate
+
+    :param candidate: tuplification candidate
+    :returns: string with sorted elements delimited by given delimiter 
+    :rtype: str
+    """
+    return candidate if isinstance(candidate, tuple) \
+        else ( \
+            tuple(candidate) if isinstance(candidate, list) \
+            else (candidate)
+        )
+
 
 def clear(sets):
     """This map returns a set with non-empty values
 
     :param dict set:  
     :returns: a set universe with  
     :rtype: dict
     """
-    return list(
-        filter(
-            lambda key: len(sets[key]) != 0,
-            sets.keys(),
-        ),
-    )
+    non_empty_mask=lambda key: len(sets[key]) != 0
 
-def areSpiderKeys(arr):
-    """This map returns a boolean variable that type check a list of arrays
+    return list(filter(non_empty_mask, sets.keys(), ),)
 
-    :param dict set:  
-    :returns: a set universe with  
-    :rtype: boolean
+def update_tuple(tuple_, value):
+    """This map updates and sorts a tuple with a value
+
+    :param tuple of elements:
+    :param value: element to update
+    :returns: an ordered and updated tuple
+    :rtype: tuple
     """
+    
+    return tuple(list(tuple_)+[value])
 
-    def isString(el): return isinstance(el, str)
-    def and_(a, b): return a and b
+def list_to_set(arr):
+    """This map converts a list into a set
+
+    :param list of elements:  
+    :returns: a set-converted list
+    :rtype: set
+    """
+    return {s for s in arr}
 
-    return reduce(and_, map(isString, arr)) if isinstance(arr, list) else False
+def union(listA, listB):
+    """This map returns the union of two lists without repetition
+
+    :param listA:
+    :param listB:
+    :returns: list with non-repeated elements
+    :rtype: list
+    """
+
+    return list(list_to_set(listA).union(list_to_set(listB)))
+
+def difference(listA, listB):
+    """This map returns the difference of a list respective to other, without repetition
+
+    :param listA:
+    :param listB:
+    :returns: difference list with non-repeated elements
+    :rtype: list
+    """
+    
+    return list(list_to_set(listA)-(list_to_set(listB)))
+
+def intersection(listA, listB):
+    """This map returns the intersection of a list respective to other, without repetition
+
+    :param listA:
+    :param listB:
+    :returns: intersection list with non-repeated elements
+    :rtype: list
+    """
+    
+    return list(list_to_set(listA).intersection(list_to_set(listB)))
```

### Comparing `eule-0.3.2/pyproject.toml` & `eule-0.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eule"
-version = "0.3.2"
+version = "0.3.3"
 description = "Euler diagrams in python"
 authors = ["Bruno Peixoto <brunolnetto@gmail.com>"]
 license = "MIT license"
 readme = "README.md"
 packages = [{include = "eule"}]
 homepage = "https://pypi.org/project/eule/"
 repository = "https://github.com/trouchet/eule"
```

### Comparing `eule-0.3.2/PKG-INFO` & `eule-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eule
-Version: 0.3.2
+Version: 0.3.3
 Summary: Euler diagrams in python
 Home-page: https://pypi.org/project/eule/
 License: MIT
 Keywords: euler-diagram,sets
 Author: Bruno Peixoto
 Author-email: brunolnetto@gmail.com
 Requires-Python: >=3.8.1,<4.0
```

