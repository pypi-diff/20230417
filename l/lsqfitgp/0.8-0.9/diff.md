# Comparing `tmp/lsqfitgp-0.8.tar.gz` & `tmp/lsqfitgp-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsqfitgp-0.8.tar", last modified: Thu May  5 12:11:49 2022, max compression
+gzip compressed data, was "lsqfitgp-0.9.tar", last modified: Sun May 15 21:40:21 2022, max compression
```

## Comparing `lsqfitgp-0.8.tar` & `lsqfitgp-0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 giacomo    (503) staff       (20)        0 2022-05-05 12:11:49.163124 lsqfitgp-0.8/
--rw-r--r--   0 giacomo    (503) staff       (20)    35149 2022-04-26 13:06:09.000000 lsqfitgp-0.8/LICENSE
--rw-r--r--   0 giacomo    (503) staff       (20)     3024 2022-05-05 12:11:49.162998 lsqfitgp-0.8/PKG-INFO
--rw-r--r--   0 giacomo    (503) staff       (20)     2461 2022-04-27 15:22:42.000000 lsqfitgp-0.8/README.md
-drwxr-xr-x   0 giacomo    (503) staff       (20)        0 2022-05-05 12:11:49.162192 lsqfitgp-0.8/lsqfitgp/
--rw-r--r--   0 giacomo    (503) staff       (20)     4498 2022-05-04 09:08:22.000000 lsqfitgp-0.8/lsqfitgp/_Deriv.py
--rw-r--r--   0 giacomo    (503) staff       (20)    56827 2022-05-05 09:26:23.000000 lsqfitgp-0.8/lsqfitgp/_GP.py
--rw-r--r--   0 giacomo    (503) staff       (20)    34861 2022-05-04 19:53:22.000000 lsqfitgp-0.8/lsqfitgp/_Kernel.py
--rw-r--r--   0 giacomo    (503) staff       (20)     4903 2022-05-03 11:42:10.000000 lsqfitgp-0.8/lsqfitgp/__init__.py
--rw-r--r--   0 giacomo    (503) staff       (20)     7167 2022-04-27 15:34:38.000000 lsqfitgp-0.8/lsqfitgp/_array.py
--rw-r--r--   0 giacomo    (503) staff       (20)     3515 2022-04-27 20:38:48.000000 lsqfitgp-0.8/lsqfitgp/_fastraniter.py
--rw-r--r--   0 giacomo    (503) staff       (20)     7476 2022-05-05 10:13:53.000000 lsqfitgp-0.8/lsqfitgp/_fit.py
--rw-r--r--   0 giacomo    (503) staff       (20)     3449 2022-04-27 15:42:24.000000 lsqfitgp-0.8/lsqfitgp/_gvar_autograd.py
--rw-r--r--   0 giacomo    (503) staff       (20)    28032 2022-05-05 09:49:01.000000 lsqfitgp-0.8/lsqfitgp/_kernels.py
--rw-r--r--   0 giacomo    (503) staff       (20)    27687 2022-05-03 13:52:14.000000 lsqfitgp-0.8/lsqfitgp/_linalg.py
--rw-r--r--   0 giacomo    (503) staff       (20)     2082 2022-04-27 15:40:03.000000 lsqfitgp-0.8/lsqfitgp/_patch_autograd.py
--rw-r--r--   0 giacomo    (503) staff       (20)     3369 2022-04-26 13:06:09.000000 lsqfitgp-0.8/lsqfitgp/_toeplitz_linalg.py
-drwxr-xr-x   0 giacomo    (503) staff       (20)        0 2022-05-05 12:11:49.162825 lsqfitgp-0.8/lsqfitgp.egg-info/
--rw-r--r--   0 giacomo    (503) staff       (20)     3024 2022-05-05 12:11:49.000000 lsqfitgp-0.8/lsqfitgp.egg-info/PKG-INFO
--rw-r--r--   0 giacomo    (503) staff       (20)      447 2022-05-05 12:11:49.000000 lsqfitgp-0.8/lsqfitgp.egg-info/SOURCES.txt
--rw-r--r--   0 giacomo    (503) staff       (20)        1 2022-05-05 12:11:49.000000 lsqfitgp-0.8/lsqfitgp.egg-info/dependency_links.txt
--rw-r--r--   0 giacomo    (503) staff       (20)       26 2022-05-05 12:11:49.000000 lsqfitgp-0.8/lsqfitgp.egg-info/requires.txt
--rw-r--r--   0 giacomo    (503) staff       (20)        9 2022-05-05 12:11:49.000000 lsqfitgp-0.8/lsqfitgp.egg-info/top_level.txt
--rw-r--r--   0 giacomo    (503) staff       (20)       38 2022-05-05 12:11:49.163165 lsqfitgp-0.8/setup.cfg
--rw-r--r--   0 giacomo    (503) staff       (20)     1597 2022-04-26 13:06:09.000000 lsqfitgp-0.8/setup.py
+drwxr-xr-x   0 giacomo    (503) staff       (20)        0 2022-05-15 21:40:21.068558 lsqfitgp-0.9/
+-rw-r--r--   0 giacomo    (503) staff       (20)    35149 2022-05-11 18:05:44.000000 lsqfitgp-0.9/LICENSE
+-rw-r--r--   0 giacomo    (503) staff       (20)     2865 2022-05-15 21:40:21.068435 lsqfitgp-0.9/PKG-INFO
+-rw-r--r--   0 giacomo    (503) staff       (20)     2302 2022-05-11 18:05:44.000000 lsqfitgp-0.9/README.md
+drwxr-xr-x   0 giacomo    (503) staff       (20)        0 2022-05-15 21:40:21.067622 lsqfitgp-0.9/lsqfitgp/
+-rw-r--r--   0 giacomo    (503) staff       (20)     4498 2022-05-11 18:05:44.000000 lsqfitgp-0.9/lsqfitgp/_Deriv.py
+-rw-r--r--   0 giacomo    (503) staff       (20)    56718 2022-05-15 20:35:28.000000 lsqfitgp-0.9/lsqfitgp/_GP.py
+-rw-r--r--   0 giacomo    (503) staff       (20)    34861 2022-05-11 18:05:44.000000 lsqfitgp-0.9/lsqfitgp/_Kernel.py
+-rw-r--r--   0 giacomo    (503) staff       (20)     4903 2022-05-11 18:05:44.000000 lsqfitgp-0.9/lsqfitgp/__init__.py
+-rw-r--r--   0 giacomo    (503) staff       (20)     7167 2022-05-11 18:05:44.000000 lsqfitgp-0.9/lsqfitgp/_array.py
+-rw-r--r--   0 giacomo    (503) staff       (20)     3515 2022-05-11 18:05:44.000000 lsqfitgp-0.9/lsqfitgp/_fastraniter.py
+-rw-r--r--   0 giacomo    (503) staff       (20)     7476 2022-05-11 18:05:44.000000 lsqfitgp-0.9/lsqfitgp/_fit.py
+-rw-r--r--   0 giacomo    (503) staff       (20)     3449 2022-05-11 18:05:44.000000 lsqfitgp-0.9/lsqfitgp/_gvar_autograd.py
+-rw-r--r--   0 giacomo    (503) staff       (20)    28032 2022-05-11 18:05:44.000000 lsqfitgp-0.9/lsqfitgp/_kernels.py
+-rw-r--r--   0 giacomo    (503) staff       (20)    27687 2022-05-11 18:05:44.000000 lsqfitgp-0.9/lsqfitgp/_linalg.py
+-rw-r--r--   0 giacomo    (503) staff       (20)     2082 2022-05-11 18:05:44.000000 lsqfitgp-0.9/lsqfitgp/_patch_autograd.py
+-rw-r--r--   0 giacomo    (503) staff       (20)     3369 2022-05-11 18:05:44.000000 lsqfitgp-0.9/lsqfitgp/_toeplitz_linalg.py
+drwxr-xr-x   0 giacomo    (503) staff       (20)        0 2022-05-15 21:40:21.068285 lsqfitgp-0.9/lsqfitgp.egg-info/
+-rw-r--r--   0 giacomo    (503) staff       (20)     2865 2022-05-15 21:40:20.000000 lsqfitgp-0.9/lsqfitgp.egg-info/PKG-INFO
+-rw-r--r--   0 giacomo    (503) staff       (20)      447 2022-05-15 21:40:21.000000 lsqfitgp-0.9/lsqfitgp.egg-info/SOURCES.txt
+-rw-r--r--   0 giacomo    (503) staff       (20)        1 2022-05-15 21:40:20.000000 lsqfitgp-0.9/lsqfitgp.egg-info/dependency_links.txt
+-rw-r--r--   0 giacomo    (503) staff       (20)       26 2022-05-15 21:40:20.000000 lsqfitgp-0.9/lsqfitgp.egg-info/requires.txt
+-rw-r--r--   0 giacomo    (503) staff       (20)        9 2022-05-15 21:40:20.000000 lsqfitgp-0.9/lsqfitgp.egg-info/top_level.txt
+-rw-r--r--   0 giacomo    (503) staff       (20)       38 2022-05-15 21:40:21.068600 lsqfitgp-0.9/setup.cfg
+-rw-r--r--   0 giacomo    (503) staff       (20)     1597 2022-05-11 18:05:44.000000 lsqfitgp-0.9/setup.py
```

### Comparing `lsqfitgp-0.8/LICENSE` & `lsqfitgp-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lsqfitgp-0.8/PKG-INFO` & `lsqfitgp-0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsqfitgp
-Version: 0.8
+Version: 0.9
 Summary: Gaussian processes in nonlinear least-squares fits
 Home-page: https://github.com/Gattocrucco/lsqfitgp
 Author: Giacomo Petrillo
 Author-email: info@giacomopetrillo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,14 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI](https://img.shields.io/pypi/v/lsqfitgp)](https://pypi.org/project/lsqfitgp/)
-[![Tests](https://github.com/Gattocrucco/lsqfitgp/actions/workflows/tests.yml/badge.svg)](https://github.com/Gattocrucco/lsqfitgp/actions/workflows/tests.yml)
 
 # lsqfitgp
 
 Python module for manipulating gaussian processes. Features:
 
   * Use [gvar](https://github.com/gplepage/gvar) to keep track transparently of
     correlations between prior, data and posterior.
```

### Comparing `lsqfitgp-0.8/README.md` & `lsqfitgp-0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 [![PyPI](https://img.shields.io/pypi/v/lsqfitgp)](https://pypi.org/project/lsqfitgp/)
-[![Tests](https://github.com/Gattocrucco/lsqfitgp/actions/workflows/tests.yml/badge.svg)](https://github.com/Gattocrucco/lsqfitgp/actions/workflows/tests.yml)
 
 # lsqfitgp
 
 Python module for manipulating gaussian processes. Features:
 
   * Use [gvar](https://github.com/gplepage/gvar) to keep track transparently of
     correlations between prior, data and posterior.
```

### Comparing `lsqfitgp-0.8/lsqfitgp/_Deriv.py` & `lsqfitgp-0.9/lsqfitgp/_Deriv.py`

 * *Files identical despite different names*

### Comparing `lsqfitgp-0.8/lsqfitgp/_GP.py` & `lsqfitgp-0.9/lsqfitgp/_GP.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,20 +201,30 @@
     
     def __init__(self, proc, method, arg):
         """proc = proc key, method = Kernel method, arg = argument to method"""
         self.proc = proc
         self.method = method
         self.arg = arg
         
-class DefaultProcess:
-    """Object used as key for the default process in GP objects"""
+class _SingletonMeta(type):
+    
+    def __repr__(cls):
+        return cls.__name__
+
+class _Singleton(metaclass=_SingletonMeta):
+    
+    def __new__(cls):
+        raise NotImplementedError(f"{cls.__name__} can not be instantiated")
+
+class DefaultProcess(_Singleton):
+    """Singleton used as key for the default process in GP objects"""
     pass
 
-class _ZeroKernel:
-    """Object representing a null kernel"""
+class _ZeroKernel(_Singleton):
+    """Singleton representing a null kernel"""
     pass
 
 class GP:
     """
     
     Object that represents a Gaussian process over arbitrary input.
     
@@ -273,24 +283,26 @@
             algorithms are O(n^3). Slow for small sizes.
         'chol'
             Cholesky decomposition after regularizing the matrix with a
             Gershgorin estimate of the maximum eigenvalue. The fastest of the
             O(n^3) algorithms.
     
     checkpos : bool
-        If True (default), raise a `LinAlgError` if the prior covariance
-        matrix turns out non positive within numerical error. The check
-        will be done only if you use in some way the `gvar` prior. With
-        the Cholesky solvers the check will be done in all cases.
+        If True (default), raise a `LinAlgError` if the prior covariance matrix
+        turns out non positive within numerical error. With the Cholesky
+        solvers the check will be done in all cases.
     checksym : bool
         If True (default), check that the prior covariance matrix is
         symmetric. If False, only half of the matrix is computed.
     checkfinite : bool
         If True (default), check that the prior covariance matrix does not
         contain infs or nans.
+    posepsfac : number
+        The threshold used to check if the prior covariance matrix is positive
+        definite is multiplied by this factor (default 1).
     **kw
         Additional keyword arguments are passed to the solver.
         
         eps : positive float
             For solvers 'eigcut+', 'eigcut-', 'svdcut+', 'svdcut-', 'chol'.
             Specifies the threshold for considering small the eigenvalues,
             relative to the maximum eigenvalue. The default is matrix size *
@@ -311,40 +323,42 @@
     # not a problem. Alternative 4: check diagonal blocks.
     # Current behaviour: only the covariance of things added with addx is
     # checked, and only if gvars are used at some point
     # Alternative 5: do the check in _solver only on things to be solved
     # => Idea: do the full check even when not using gvars, only on
     # non-transformed variables, but issue a warning if the system is large
     
-    # TODO maybe the default should be solver='eigcut-' because it adds less
-    # noise. It is moot anyway if the plot is done sampling with gvar.raniter
-    # or lgp.raninter because they do add their own noise. But this will be
-    # solved when I add GP sampling methods.
+    # TODO maybe the default should be solver='eigcut-' (or 'svdcut-'?) because
+    # it adds less noise. It is moot anyway if the plot is done sampling with
+    # gvar.raniter or lgp.raninter because they do add their own noise. But this
+    # will be solved when I add GP sampling methods.
     
-    def __init__(self, covfun=None, solver='eigcut+', checkpos=True, checksym=True, checkfinite=True, **kw):
+    def __init__(self, covfun=None, solver='eigcut+', checkpos=True, checksym=True, checkfinite=True, posepsfac=1, **kw):
         self._elements = dict() # key -> _Element
         self._covblocks = dict() # (key, key) -> matrix
+        self._priordict = gvar.BufferDict({}, dtype=object) # key -> gvar array (shaped)
         self._decompcache = dict() # tuple of keys -> Decomposition
         self._procs = dict() # proc key -> _Proc
         self._kernels = dict() # (proc key, proc key) -> _KernelBase
         if covfun is not None:
             if not isinstance(covfun, _Kernel.Kernel):
                 raise TypeError('covariance function must be of class Kernel')
             self._procs[DefaultProcess] = _ProcKernel(covfun)
-        self._canaddx = True
         decomp = {
             'eigcut+': _linalg.EigCutFullRank,
             'eigcut-': _linalg.EigCutLowRank,
             'svdcut+': _linalg.SVDCutFullRank,
             'svdcut-': _linalg.SVDCutLowRank,
             'lowrank': _linalg.ReduceRank,
             'chol'   : _linalg.CholGersh,
         }[solver]
         self._decompclass = lambda K, **kwargs: decomp(K, **kwargs, **kw)
         self._checkpositive = bool(checkpos)
+        self._checkpositive_todo = True
+        self._posepsfac = float(posepsfac)
         self._checksym = bool(checksym)
         self._checkfinite = bool(checkfinite)
     
     def addproc(self, kernel=None, key=DefaultProcess, deriv=0):
         """
         
         Add an independent process.
@@ -520,18 +534,14 @@
         the process itself should be evaluated, use the parameter `deriv`.
         
         `addx` never copies the input arrays if they are numpy arrays, so if
         you change their contents before doing something with the GP, the
         change will be reflected on the result. However, after the GP has
         computed internally its covariance matrix, the x are ignored.
         
-        If you use in some way the `gvar` prior, e.g., by calling `prior` or
-        `pred` using gvars, you can't call `addx` any more, due to a
-        limitation in gvar.
-        
         Parameters
         ----------
         x : array or dictionary of arrays
             The points to be added.
         key : hashable
             If `x` is an array, the dictionary key under which `x` is added.
             Can not be specified if `x` is a dictionary.
@@ -546,18 +556,14 @@
         
         # TODO after I implement block solving, add per-key solver option. It
         # may not be possible to respect the setting if it is not the sole
         # key used as data.
         
         # TODO add `copy` parameter, default False, to copy the input arrays.
         
-        if not self._canaddx:
-            raise RuntimeError('can not add x any more to this process')
-            # TODO remove if I implement the lazy gvar prior.
-        
         deriv = _Deriv.Deriv(deriv)
 
         if proc not in self._procs:
             raise KeyError(f'process named {proc!r} not found')
                 
         if _isarraylike(x):
             if key is None:
@@ -708,17 +714,17 @@
         self._elements[key] = _Transf(tens, shape, axes)
     
     def addcov(self, covblocks, key=None):
         """
         
         Add user-defined prior covariance matrix blocks.
         
-        Covariance matrices defined with `addcov` represent arbitrary finite
-        zero-mean Gaussian variables, assumed independent from all other
-        variables in the GP object.
+        Covariance matrices defined with `addcov` represent arbitrary
+        finite-dimensional zero-mean Gaussian variables, assumed independent
+        from all other variables in the GP object.
                 
         Parameters
         ----------
         covblocks : array or dictionary of arrays
             If an array: a covariance matrix (or tensor) to be added under key
             `key`. If a dictionary: a mapping from pairs of keys to the
             corresponding covariance matrix blocks. A missing off-diagonal
@@ -733,17 +739,16 @@
         RuntimeError :
             A key is already used in the GP.
         ValueError :
             `covblocks` and/or `key` are malformed or inconsistent.
         
         """
         
-        if not self._canaddx:
-            raise RuntimeError('can not add x any more to this process')
-            # TODO remove if I implement the lazy gvar prior.
+        # TODO maybe allow passing only the lower/upper triangular part for
+        # the diagonal blocks, like I meta-allow for out of diagonal blocks?
         
         # Check type of `covblocks` and standardize it to dictionary.
         if _isarraylike(covblocks):
             if key is None:
                 raise ValueError('covblocks is array but key is None')
             covblocks = {(key, key): covblocks}
         elif _isdictlike(covblocks):
@@ -755,14 +760,15 @@
             raise TypeError('covblocks must be array or dict')
         
         # Convert blocks to numpy arrays and determine shapes from diagonal
         # blocks.
         shapes = {}
         preblocks = {}
         for keys, block in covblocks.items():
+            # TODO maybe check that keys is a 2-tuple
             for key in keys:
                 if key in self._elements:
                     raise KeyError(f'key {key!r} already in GP')
             xkey, ykey = keys
             block = np.asarray(block)
             if xkey == ykey:
                 if block.ndim % 2 == 1:
@@ -887,15 +893,15 @@
         xp = self._procs[xpkey]
         yp = self._procs[ypkey]
         
         if xp is yp:
             basekernel = self._crosskernel(xp.proc, xp.proc)
             # In principle I could avoid handling this case separately but it
             # will probably allow simplifications in how I implement nontrivial
-            # transformations in Kernel, I won't need to support taking a
+            # transformations in Kernel: I won't need to support taking a
             # transformation in two steps.
         else:
             basekernel = self._crosskernel(xp.proc, ypkey)
         
         if basekernel is _ZeroKernel:
             return _ZeroKernel
         elif xp is yp:
@@ -967,18 +973,29 @@
         if self._checkfinite and not np.all(np.isfinite(cov)):
             raise RuntimeError('covariance block {!r} is not finite'.format((xkey, ykey)))
         if self._checksym and xkey == ykey and not np.allclose(cov, cov.T):
             raise RuntimeError('covariance block {!r} is not symmetric'.format((xkey, ykey)))
 
         return cov
 
-    def _covblock(self, row, col):        
+    def _covblock(self, row, col):
+        
+        if self._checkpositive and self._checkpositive_todo:
+            self._checkpositive_todo = False
+            keys = [
+                k for k, v in self._elements.items()
+                if isinstance(v, (_Points, _Cov))
+            ]
+            fullcov = self._assemblecovblocks(list(keys))
+            self._checkpos(fullcov)
+            
         if (row, col) not in self._covblocks:
             block = self._makecovblock(row, col)
-            _linalg.noautograd(block).flags['WRITEABLE'] = False
+            # _linalg.noautograd(block).flags['WRITEABLE'] = False
+            # TODO gives problems to gvar.gvar, ask Lepage to solve the bug
             if row != col:
                 if self._checksym:
                     blockT = self._makecovblock(col, row)
                     if not np.allclose(block.T, blockT):
                         msg = 'covariance block {!r} is not symmetric'
                         raise RuntimeError(msg.format((row, col)))
                 self._covblocks[col, row] = block.T
@@ -1000,20 +1017,14 @@
         Return a decomposition of the covariance matrix of the keys in `keys`
         plus the matrix ycov.
         """
         
         # TODO Block matrix solving. Example: solve a subproblem with kronecker,
         # another plain.
         
-        # TODO Cache decompositions of blocks. Caching is effective
-        # with data if I can reuse the decomposition of Kxx to compute the
-        # decomposition of Kxx + ycov, i.e., it works in all cases if ycov is
-        # scalar, and in some cases if ycov is diagonal. Is there an efficient
-        # way to update a Cholesky decomposition if I add a diagonal matrix?
-        
         # TODO Check if the matrix is block diagonal. It's O(n^2). It is often
         # not needed but when it is it makes a difference. A faster and less
         # thorough check can be done only on off-diagonal key-key blocks being
         # zero, which may be useful with multi-output or split components.
         
         keys = tuple(keys)
         
@@ -1042,56 +1053,50 @@
         # faster but less trivial options for checking positivity:
         # 1) cholesky + eps, if fails it's not positive
         # 2) ldlt, check each 2x2 block     <--- probably best? is it stable?
         # 3) QR, check diagonal of R
         eigv = linalg.eigvalsh(_linalg.noautograd(cov))
         mineigv = np.min(eigv)
         if mineigv < 0:
-            bound = -len(cov) * np.finfo(float).eps * np.max(eigv)
+            bound = -len(cov) * np.finfo(float).eps * np.max(eigv) * self._posepsfac
             if mineigv < bound:
                 msg = 'covariance matrix is not positive definite: '
                 msg += 'mineigv = {:.4g} < {:.4g}'.format(mineigv, bound)
                 raise np.linalg.LinAlgError(msg)
     
     def _priorpointscov(self, key):
         
-        # TODO I think that gvar internals would let me build the prior
-        # one block at a time although everything is correlated, but I don't
-        # know how to do it. If I do that, remove _canaddx. => Lepage is
-        # working on it.
-        
-        assert not hasattr(self, '_priordict')
-        # caching is managed by _prior and since we have to create all gvars
-        # at once this method can be called only the first time
-        
-        if self._checkpositive:
-            keys = [
-                k for k, v in self._elements.items()
-                if isinstance(v, (_Points, _Cov))
-            ]
-            fullcov = self._assemblecovblocks(list(keys))
-            self._checkpos(fullcov)
-        items = [
-            (k, v) for k, v in self._elements.items()
-            if isinstance(v, (_Points, _Cov))
+        x = self._elements[key]
+        classes = (_Points, _Cov)
+        assert isinstance(x, classes)
+        mean = np.zeros(x.size)
+        cov = self._covblock(key, key).astype(float, copy=False)
+        assert cov.shape == 2 * mean.shape, cov.shape
+
+        # get preexisting primary gvars to be correlated with the new ones
+        preitems = [
+            k
+            for k, px in self._elements.items()
+            if isinstance(px, classes)
+            and k in self._priordict
         ]
-        mean = {
-            key: np.zeros(x.shape)
-            for key, x in items
-        }
-        cov = {
-            (row, col): self._covblock(row, col).reshape(x.shape + y.shape)
-            for row, x in items
-            for col, y in items
-        }
-        self._priordict = gvar.gvar(mean, cov, fast=True)
-        self._priordict.buf.flags['WRITEABLE'] = False
-        self._canaddx = False
+        if preitems:
+            prex = _concatenate_noop([
+                np.reshape(self._priordict[k], -1)
+                for k in preitems
+            ])
+            precov = _concatenate_noop([
+                self._covblock(k, key).astype(float, copy=False)
+                for k in preitems
+            ])
+            g = gvar.gvar(mean, cov, prex, precov, fast=True)
+        else:
+            g = gvar.gvar(mean, cov, fast=True)
         
-        return self._priordict[key]
+        return g.reshape(x.shape)
     
     def _priortransf(self, key):
         x = self._elements[key]
         assert isinstance(x, _Transf)
         out = None
         for k, tensor in x.tensors.items():
             prior = self._prior(k)
@@ -1099,25 +1104,24 @@
             if out is None:
                 out = transf
             else:
                 out = out + transf
         return out
     
     def _prior(self, key):
-        prior = getattr(self, '_priordict', {}).get(key, None)
+        prior = self._priordict.get(key, None)
         if prior is None:
             x = self._elements[key]
             if isinstance(x, (_Points, _Cov)):
                 prior = self._priorpointscov(key)
-                # _priorpoints already caches the result
             elif isinstance(x, _Transf):
                 prior = self._priortransf(key)
-                self._priordict[key] = prior
             else:
                 raise TypeError(type(x))
+            self._priordict[key] = prior
         return prior
     
     def prior(self, key=None, raw=False):
         """
         
         Return an array or a dictionary of arrays of gvars representing the
         prior for the Gaussian process. The returned object is not unique but
```

### Comparing `lsqfitgp-0.8/lsqfitgp/_Kernel.py` & `lsqfitgp-0.9/lsqfitgp/_Kernel.py`

 * *Files identical despite different names*

### Comparing `lsqfitgp-0.8/lsqfitgp/__init__.py` & `lsqfitgp-0.9/lsqfitgp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from ._Kernel import *
 from ._kernels import *
 from ._array import *
 from ._fit import *
 from ._Deriv import *
 from ._fastraniter import *
 
-__version__ = '0.8'
+__version__ = '0.9'
 
 __doc__ = """
 
 Module to fit Gaussian processes with gvar/lsqfit.
 
 Manual: https://gattocrucco.github.io/lsqfitgp/docs
```

### Comparing `lsqfitgp-0.8/lsqfitgp/_array.py` & `lsqfitgp-0.9/lsqfitgp/_array.py`

 * *Files identical despite different names*

### Comparing `lsqfitgp-0.8/lsqfitgp/_fastraniter.py` & `lsqfitgp-0.9/lsqfitgp/_fastraniter.py`

 * *Files identical despite different names*

### Comparing `lsqfitgp-0.8/lsqfitgp/_fit.py` & `lsqfitgp-0.9/lsqfitgp/_fit.py`

 * *Files identical despite different names*

### Comparing `lsqfitgp-0.8/lsqfitgp/_gvar_autograd.py` & `lsqfitgp-0.9/lsqfitgp/_gvar_autograd.py`

 * *Files identical despite different names*

### Comparing `lsqfitgp-0.8/lsqfitgp/_kernels.py` & `lsqfitgp-0.9/lsqfitgp/_kernels.py`

 * *Files identical despite different names*

### Comparing `lsqfitgp-0.8/lsqfitgp/_linalg.py` & `lsqfitgp-0.9/lsqfitgp/_linalg.py`

 * *Files identical despite different names*

### Comparing `lsqfitgp-0.8/lsqfitgp/_patch_autograd.py` & `lsqfitgp-0.9/lsqfitgp/_patch_autograd.py`

 * *Files identical despite different names*

### Comparing `lsqfitgp-0.8/lsqfitgp/_toeplitz_linalg.py` & `lsqfitgp-0.9/lsqfitgp/_toeplitz_linalg.py`

 * *Files identical despite different names*

### Comparing `lsqfitgp-0.8/lsqfitgp.egg-info/PKG-INFO` & `lsqfitgp-0.9/lsqfitgp.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsqfitgp
-Version: 0.8
+Version: 0.9
 Summary: Gaussian processes in nonlinear least-squares fits
 Home-page: https://github.com/Gattocrucco/lsqfitgp
 Author: Giacomo Petrillo
 Author-email: info@giacomopetrillo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,14 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI](https://img.shields.io/pypi/v/lsqfitgp)](https://pypi.org/project/lsqfitgp/)
-[![Tests](https://github.com/Gattocrucco/lsqfitgp/actions/workflows/tests.yml/badge.svg)](https://github.com/Gattocrucco/lsqfitgp/actions/workflows/tests.yml)
 
 # lsqfitgp
 
 Python module for manipulating gaussian processes. Features:
 
   * Use [gvar](https://github.com/gplepage/gvar) to keep track transparently of
     correlations between prior, data and posterior.
```

### Comparing `lsqfitgp-0.8/setup.py` & `lsqfitgp-0.9/setup.py`

 * *Files identical despite different names*

