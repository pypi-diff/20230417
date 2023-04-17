# Comparing `tmp/kronbinations-0.6.tar.gz` & `tmp/kronbinations-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kronbinations-0.6.tar", last modified: Tue Jan 10 17:23:44 2023, max compression
+gzip compressed data, was "kronbinations-1.0.tar", last modified: Mon Apr 17 14:07:09 2023, max compression
```

## Comparing `kronbinations-0.6.tar` & `kronbinations-1.0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-01-10 17:23:44.649735 kronbinations-0.6/
--rw-rw-rw-   0        0        0     1096 2023-01-09 15:45:38.000000 kronbinations-0.6/LICENSE
--rw-rw-rw-   0        0        0     1975 2023-01-10 17:23:44.649735 kronbinations-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1449 2023-01-10 16:52:02.000000 kronbinations-0.6/README.md
--rw-rw-rw-   0        0        0      539 2023-01-10 17:23:44.651734 kronbinations-0.6/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-01-10 17:20:09.000000 kronbinations-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-10 17:23:44.615736 kronbinations-0.6/src/
-drwxrwxrwx   0        0        0        0 2023-01-10 17:23:44.628737 kronbinations-0.6/src/kronbinations/
--rw-rw-rw-   0        0        0       68 2023-01-09 15:52:36.000000 kronbinations-0.6/src/kronbinations/__init__.py
--rw-rw-rw-   0        0        0     7165 2023-01-10 17:22:23.000000 kronbinations-0.6/src/kronbinations/kronbinations.py
-drwxrwxrwx   0        0        0        0 2023-01-10 17:23:44.646739 kronbinations-0.6/src/kronbinations.egg-info/
--rw-rw-rw-   0        0        0     1975 2023-01-10 17:23:44.000000 kronbinations-0.6/src/kronbinations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-01-10 17:23:44.000000 kronbinations-0.6/src/kronbinations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-10 17:23:44.000000 kronbinations-0.6/src/kronbinations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-01-10 17:23:44.000000 kronbinations-0.6/src/kronbinations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-01-10 17:23:44.000000 kronbinations-0.6/src/kronbinations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-10 17:23:44.647738 kronbinations-0.6/test/
--rw-rw-rw-   0        0        0     4043 2023-01-10 17:18:46.000000 kronbinations-0.6/test/test_kronbinations.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:09.633749 kronbinations-1.0/
+-rw-rw-rw-   0        0        0     1096 2023-04-17 14:06:49.000000 kronbinations-1.0/LICENSE
+-rw-rw-rw-   0        0        0     6252 2023-04-17 14:07:09.633749 kronbinations-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5724 2023-04-17 14:06:49.000000 kronbinations-1.0/README.md
+-rw-rw-rw-   0        0        0      523 2023-04-17 14:07:09.638802 kronbinations-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      872 2023-04-17 14:06:49.000000 kronbinations-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:09.583497 kronbinations-1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:09.615723 kronbinations-1.0/src/kronbinations/
+-rw-rw-rw-   0        0        0     9324 2023-04-17 10:40:53.000000 kronbinations-1.0/src/kronbinations/JIT_Array.py
+-rw-rw-rw-   0        0        0    14097 2023-04-17 13:54:15.000000 kronbinations-1.0/src/kronbinations/JIT_kronbinations.py
+-rw-rw-rw-   0        0        0     3087 2023-04-17 10:40:45.000000 kronbinations-1.0/src/kronbinations/Kron_Array.py
+-rw-rw-rw-   0        0        0    44564 2023-02-24 16:06:05.000000 kronbinations-1.0/src/kronbinations/Kron_Fun_Modifier.py
+-rw-rw-rw-   0        0        0      241 2023-02-27 13:26:54.000000 kronbinations-1.0/src/kronbinations/__init__.py
+-rw-rw-rw-   0        0        0    10708 2023-04-17 13:47:18.000000 kronbinations-1.0/src/kronbinations/kronbinations.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:09.623743 kronbinations-1.0/src/kronbinations.egg-info/
+-rw-rw-rw-   0        0        0     6252 2023-04-17 14:07:08.000000 kronbinations-1.0/src/kronbinations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-04-17 14:07:09.000000 kronbinations-1.0/src/kronbinations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 14:07:08.000000 kronbinations-1.0/src/kronbinations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-17 14:07:08.000000 kronbinations-1.0/src/kronbinations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-17 14:07:08.000000 kronbinations-1.0/src/kronbinations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:09.633749 kronbinations-1.0/test/
+-rw-rw-rw-   0        0        0     4602 2023-04-17 13:58:07.000000 kronbinations-1.0/test/test_JIT_kronbinations.py
+-rw-rw-rw-   0        0        0     3564 2023-04-17 13:58:07.000000 kronbinations-1.0/test/test_kronbinations.py
```

### Comparing `kronbinations-0.6/LICENSE` & `kronbinations-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kronbinations-0.6/setup.cfg` & `kronbinations-1.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206b 726f 6e62 696e 6174 696f 6e73   = kronbinations
-00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 360d  ..version = 0.6.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 300d  ..version = 1.0.
 00000030: 0a61 7574 686f 7220 3d20 4d69 6368 6165  .author = Michae
 00000040: 6c20 5363 6869 6c6c 696e 670d 0a61 7574  l Schilling..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6d69 6368  hor_email = mich
 00000060: 6165 6c40 6e74 726f 7069 632e 6465 0d0a  ael@ntropic.de..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 6b72  description = kr
 00000080: 6f6e 6269 6e61 7469 6f6e 7320 6973 2075  onbinations is u
 00000090: 7365 6420 746f 2072 656d 6f76 6520 6e65  sed to remove ne
@@ -15,20 +15,19 @@
 000000e0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
 000000f0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
 00000100: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
 00000110: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
 00000120: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
 00000130: 622e 636f 6d2f 4e74 726f 7069 632f 6b72  b.com/Ntropic/kr
 00000140: 6f6e 6269 6e61 7469 6f6e 732f 6172 6368  onbinations/arch
-00000150: 6976 652f 7265 6673 2f74 6167 732f 7630  ive/refs/tags/v0
-00000160: 2e36 2e74 6172 2e67 7a0d 0a63 6c61 7373  .6.tar.gz..class
-00000170: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
-00000180: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000190: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
-000001a0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-000001b0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-000001c0: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
-000001d0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-000001e0: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
-000001f0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000200: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000210: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000150: 6976 652f 7265 6673 2f74 6167 732f 7631  ive/refs/tags/v1
+00000160: 2e30 2e74 6172 2e67 7a0d 0a50 726f 6772  .0.tar.gz..Progr
+00000170: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000180: 3d20 3a20 5079 7468 6f6e 203a 3a20 330d  = : Python :: 3.
+00000190: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
+000001a0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+000001b0: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
+000001c0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+000001d0: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
+000001e0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+000001f0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+00000200: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `kronbinations-0.6/setup.py` & `kronbinations-1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "kronbinations",
-    version = "0.6",
+    version      = "1.0",
     author = "Michael Schilling",
     author_email = "michael@ntropic.de",
     description  = "kronbinations is used to remove nested loops and perform parameter sweeps.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/Ntropic/kronbinations/archive/refs/tags/v0.6.tar.gz",
+    url = "https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.0.tar.gz",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `kronbinations-0.6/test/test_kronbinations.py` & `kronbinations-1.0/test/test_kronbinations.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,35 +9,27 @@
 strings = np.array(['a', 'b', 'c', 'd', 'e'])
 
 # Create a kronbinations object
 def test_kronbinations_matrices():
     # Create a kronbinations object
     # with the lists as values
     k = kronbinations(floats, ints, strings)
-    assert k.size() == 125
-    assert k.shape() == (5,5,5)
-    assert k.ndim() == 3
+    assert k.size == 125
+    assert k.shape == (5,5,5)
+    assert k.ndim == 3
     # Test the generation of matrices
     o = k.ones(dtype=int)
     z = k.zeros(dtype=int)
     e = k.empty()
     f = k.full(fill_value= 1.0/3.0)
-    r = k.random()
-    ri = k.randint(0,1)
-    rng = np.random.default_rng()
-    rr = k.rng(rng.random)
-    list_of_matrices = [o, z, e, f, r, ri, rr]
     assert o.shape == (5,5,5)
     assert z.shape == (5,5,5)
     assert e.shape == (5,5,5)
     assert f.shape == (5,5,5)
-    assert r.shape == (5,5,5)
-    assert ri.shape == (5,5,5)
-    assert rr.shape == (5,5,5)
-
+    
 def test_kronbinations_loop_outputs():
     k = kronbinations(floats, ints, strings)
     b = [False, True]
     # Check number of outputs
     for index in b:
         for change in b:
             for progress in b:
@@ -58,34 +50,29 @@
         for j in range(3):
             assert k.changed(j) == c[j]
             assert k.index(j) == i[j]
             assert k.value(j) == v[j]
 
 def test_krombinations_settings_and_changes_to_them():
     k = kronbinations(floats, ints, strings)
-    k.set(do_index=True, do_change=True, do_tqdm=True, return_as_dict=False)
+    k.set(do_index=True, do_change=True, do_tqdm=True)
     do_index, do_change, do_tqdm, return_as_dict = k.get('do_index', 'do_change', 'do_tqdm', 'return_as_dict')
     assert do_index
     assert do_change
     assert do_tqdm
-    assert not return_as_dict
-    k.set(do_index=False, do_change=False, do_tqdm=False, return_as_dict=False)
+    k.set(do_index=False, do_change=False, do_tqdm=False)
     do_index, do_change, do_tqdm, return_as_dict = k.get('index', 'do_change', 'do_tqdm', 'return_as_dict')
     assert not do_index
     assert not do_change
     assert not do_tqdm
-    assert not return_as_dict
 
 def test_kronbinations_illegal_dict_outputs():
     # Check the illegal dictionary outputs
     k = kronbinations(floats, ints, strings)
     with pytest.raises(ValueError):
-        for a in k.kronprod(index=True, change=True, progress=True, return_as_dict=True):
-            pass
-    with pytest.raises(ValueError):
         for i,v,c in k.kronprod(index=True, change=True, progress=False):
             k.value('floats')
     with pytest.raises(ValueError):
         for i,v,c in k.kronprod(index=True, change=True, progress=False):
             k.index('floats')
     with pytest.raises(ValueError):
         for i,v,c in k.kronprod(index=True, change=True, progress=False):
@@ -96,11 +83,12 @@
     # with the lists as a dictionary
     keys = ['floats', 'ints', 'strings']
     d = {'floats': floats, 'ints': ints, 'strings': strings}
     k = kronbinations(d)
     with pytest.raises(ValueError):
         k = kronbinations(d, d)
     for i,v,c in k.kronprod(index=True, change=True, progress=False):
-        for key in keys:
+        for j, key in enumerate(keys):
             assert k.changed(key) == c[key]
-            assert k.index(key) == i[key]
-            assert k.value(key) == v[key]
+            assert k.index(key) == i[j]
+            assert k.value(key) == v[key]
+
```

