# Comparing `tmp/icepool-0.8.0.tar.gz` & `tmp/icepool-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icepool-0.8.0.tar", last modified: Sun Apr 24 06:26:06 2022, max compression
+gzip compressed data, was "icepool-0.9.0.tar", last modified: Fri Apr 29 06:48:01 2022, max compression
```

## Comparing `icepool-0.8.0.tar` & `icepool-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-04-24 06:26:06.413773 icepool-0.8.0/
--rw-rw-rw-   0        0        0     1111 2022-04-16 23:05:39.000000 icepool-0.8.0/LICENSE.md
--rw-rw-rw-   0        0        0     4467 2022-04-24 06:26:06.413773 icepool-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     3774 2022-04-18 08:12:54.000000 icepool-0.8.0/README.md
--rw-rw-rw-   0        0        0      110 2022-04-16 23:05:39.000000 icepool-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0      766 2022-04-24 06:26:06.414742 icepool-0.8.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-04-24 06:26:06.364875 icepool-0.8.0/src/
-drwxrwxrwx   0        0        0        0 2022-04-24 06:26:06.376844 icepool-0.8.0/src/icepool/
--rw-rw-rw-   0        0        0     2038 2022-04-23 07:22:40.000000 icepool-0.8.0/src/icepool/__init__.py
--rw-rw-rw-   0        0        0     1983 2022-04-18 04:20:10.000000 icepool-0.8.0/src/icepool/collections.py
-drwxrwxrwx   0        0        0        0 2022-04-24 06:26:06.406763 icepool-0.8.0/src/icepool/die/
--rw-rw-rw-   0        0        0        0 2022-04-16 23:05:39.000000 icepool-0.8.0/src/icepool/die/__init__.py
--rw-rw-rw-   0        0        0    39330 2022-04-24 06:11:01.000000 icepool-0.8.0/src/icepool/die/base.py
--rw-rw-rw-   0        0        0     9945 2022-04-18 04:20:37.000000 icepool-0.8.0/src/icepool/die/create.py
--rw-rw-rw-   0        0        0      800 2022-04-18 04:20:41.000000 icepool-0.8.0/src/icepool/die/empty.py
--rw-rw-rw-   0        0        0     5480 2022-04-23 06:24:20.000000 icepool-0.8.0/src/icepool/die/func.py
--rw-rw-rw-   0        0        0     9269 2022-04-18 04:20:45.000000 icepool-0.8.0/src/icepool/die/scalar.py
--rw-rw-rw-   0        0        0     7056 2022-04-18 04:20:48.000000 icepool-0.8.0/src/icepool/die/vector.py
--rw-rw-rw-   0        0        0      433 2022-04-16 23:05:39.000000 icepool-0.8.0/src/icepool/math.py
-drwxrwxrwx   0        0        0        0 2022-04-24 06:26:06.412747 icepool-0.8.0/src/icepool/pool/
--rw-rw-rw-   0        0        0        0 2022-04-17 22:24:24.000000 icepool-0.8.0/src/icepool/pool/__init__.py
--rw-rw-rw-   0        0        0     3059 2022-04-24 06:09:48.000000 icepool-0.8.0/src/icepool/pool/base.py
--rw-rw-rw-   0        0        0    18466 2022-04-24 06:09:48.000000 icepool-0.8.0/src/icepool/pool/eval.py
--rw-rw-rw-   0        0        0    26841 2022-04-24 06:14:48.000000 icepool-0.8.0/src/icepool/pool/pool.py
--rw-rw-rw-   0        0        0     2705 2022-04-24 06:09:49.000000 icepool-0.8.0/src/icepool/pool/roll.py
-drwxrwxrwx   0        0        0        0 2022-04-24 06:26:06.395792 icepool-0.8.0/src/icepool.egg-info/
--rw-rw-rw-   0        0        0     4467 2022-04-24 06:26:05.000000 icepool-0.8.0/src/icepool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      564 2022-04-24 06:26:06.000000 icepool-0.8.0/src/icepool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-24 06:26:06.000000 icepool-0.8.0/src/icepool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-04-24 06:26:06.000000 icepool-0.8.0/src/icepool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-04-29 06:48:01.884327 icepool-0.9.0/
+-rw-rw-rw-   0        0        0     1111 2022-04-16 23:05:39.000000 icepool-0.9.0/LICENSE.md
+-rw-rw-rw-   0        0        0     4572 2022-04-29 06:48:01.884327 icepool-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3879 2022-04-24 06:44:50.000000 icepool-0.9.0/README.md
+-rw-rw-rw-   0        0        0      110 2022-04-16 23:05:39.000000 icepool-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0      766 2022-04-29 06:48:01.896294 icepool-0.9.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-04-29 06:48:01.845431 icepool-0.9.0/src/
+drwxrwxrwx   0        0        0        0 2022-04-29 06:48:01.857399 icepool-0.9.0/src/icepool/
+-rw-rw-rw-   0        0        0     2313 2022-04-28 06:35:11.000000 icepool-0.9.0/src/icepool/__init__.py
+-rw-rw-rw-   0        0        0     1983 2022-04-18 04:20:10.000000 icepool-0.9.0/src/icepool/collections.py
+drwxrwxrwx   0        0        0        0 2022-04-29 06:48:01.877345 icepool-0.9.0/src/icepool/die/
+-rw-rw-rw-   0        0        0        0 2022-04-16 23:05:39.000000 icepool-0.9.0/src/icepool/die/__init__.py
+-rw-rw-rw-   0        0        0    39366 2022-04-29 06:38:50.000000 icepool-0.9.0/src/icepool/die/base.py
+-rw-rw-rw-   0        0        0    10773 2022-04-29 05:26:01.000000 icepool-0.9.0/src/icepool/die/create.py
+-rw-rw-rw-   0        0        0     1044 2022-04-28 07:04:05.000000 icepool-0.9.0/src/icepool/die/empty.py
+-rw-rw-rw-   0        0        0     5498 2022-04-28 06:33:19.000000 icepool-0.9.0/src/icepool/die/func.py
+-rw-rw-rw-   0        0        0     8374 2022-04-28 06:57:16.000000 icepool-0.9.0/src/icepool/die/scalar.py
+-rw-rw-rw-   0        0        0     7094 2022-04-28 06:57:17.000000 icepool-0.9.0/src/icepool/die/vector.py
+-rw-rw-rw-   0        0        0      433 2022-04-16 23:05:39.000000 icepool-0.9.0/src/icepool/math.py
+drwxrwxrwx   0        0        0        0 2022-04-29 06:48:01.883329 icepool-0.9.0/src/icepool/pool/
+-rw-rw-rw-   0        0        0        0 2022-04-17 22:24:24.000000 icepool-0.9.0/src/icepool/pool/__init__.py
+-rw-rw-rw-   0        0        0     3834 2022-04-25 04:17:29.000000 icepool-0.9.0/src/icepool/pool/base.py
+-rw-rw-rw-   0        0        0    18327 2022-04-25 04:11:13.000000 icepool-0.9.0/src/icepool/pool/eval.py
+-rw-rw-rw-   0        0        0    26877 2022-04-25 04:15:15.000000 icepool-0.9.0/src/icepool/pool/pool.py
+-rw-rw-rw-   0        0        0     2861 2022-04-25 04:13:58.000000 icepool-0.9.0/src/icepool/pool/roll.py
+drwxrwxrwx   0        0        0        0 2022-04-29 06:48:01.869366 icepool-0.9.0/src/icepool.egg-info/
+-rw-rw-rw-   0        0        0     4572 2022-04-29 06:48:01.000000 icepool-0.9.0/src/icepool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      564 2022-04-29 06:48:01.000000 icepool-0.9.0/src/icepool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-04-29 06:48:01.000000 icepool-0.9.0/src/icepool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2022-04-29 06:48:01.000000 icepool-0.9.0/src/icepool.egg-info/top_level.txt
```

### Comparing `icepool-0.8.0/LICENSE.md` & `icepool-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `icepool-0.8.0/PKG-INFO` & `icepool-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icepool
-Version: 0.8.0
+Version: 0.9.0
 Summary: A package for computing dice probabilities
 Home-page: https://github.com/HighDiceRoller/icepool
 Author: Albert Julius Liu
 Author-email: ajul1987+highdiceroller@gmail.com
 License: UNKNOWN
 Project-URL: Twitter, https://twitter.com/highdiceroller
 Platform: UNKNOWN
@@ -17,37 +17,39 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # <img width="32" height="32" src="https://highdiceroller.github.io/icepool/apps/favicon.png" /> Icepool
 
 A Python package for computing dice probabilities.
 
-[GitHub.](https://github.com/HighDiceRoller/icepool)
+[GitHub repository.](https://github.com/HighDiceRoller/icepool)
 
 ## Features
 
 * Pure Python implementation.
 * Exact fractional probabilities using Python `int`s.
-* Dice support all standard operators as well as an extensive library of functions.
-* Efficiently solves dice pool problems; depending on the problem, it can be more than 1000× as fast as multiset/sequence-based algorithms.
-* Supports multivariate distributions.
+* Dice support all standard operators (+, -, <, >, etc.) as well as an extensive library of functions (rerolling, exploding, etc.)
+* Can outperform sequence/multiset-based algorithms on many dice pool problems.
+    In some cases it may be thousands or millions of times faster.
 
 ## Installing
 
 ```
 pip install icepool
 ```
 
+The source is pure Python, so making a direct copy can work as well.
+
 ## Contact
 
 Feel free to open a [discussion](https://github.com/HighDiceRoller/icepool/discussions) or [issue](https://github.com/HighDiceRoller/icepool/issues) on GitHub. You can also find me on [Twitter](https://twitter.com/highdiceroller) or [Reddit](https://www.reddit.com/user/HighDiceRoller).
 
 ## API documentation
 
-[GitHub.](https://highdiceroller.github.io/icepool/apidoc/icepool.html)
+[pdoc on GitHub.](https://highdiceroller.github.io/icepool/apidoc/icepool.html)
 
 ## JupyterLite notebooks
 
 See this [JupyterLite distribution](https://highdiceroller.github.io/icepool/notebooks/lab/index.html) for a collection of interactive, editable examples. These include mechanics from published games, StackExchange, Reddit, and academic papers.
 
 ## Web applications
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `icepool-0.8.0/README.md` & `icepool-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # <img width="32" height="32" src="https://highdiceroller.github.io/icepool/apps/favicon.png" /> Icepool
 
 A Python package for computing dice probabilities.
 
-[GitHub.](https://github.com/HighDiceRoller/icepool)
+[GitHub repository.](https://github.com/HighDiceRoller/icepool)
 
 ## Features
 
 * Pure Python implementation.
 * Exact fractional probabilities using Python `int`s.
-* Dice support all standard operators as well as an extensive library of functions.
-* Efficiently solves dice pool problems; depending on the problem, it can be more than 1000× as fast as multiset/sequence-based algorithms.
-* Supports multivariate distributions.
+* Dice support all standard operators (+, -, <, >, etc.) as well as an extensive library of functions (rerolling, exploding, etc.)
+* Can outperform sequence/multiset-based algorithms on many dice pool problems.
+    In some cases it may be thousands or millions of times faster.
 
 ## Installing
 
 ```
 pip install icepool
 ```
 
+The source is pure Python, so making a direct copy can work as well.
+
 ## Contact
 
 Feel free to open a [discussion](https://github.com/HighDiceRoller/icepool/discussions) or [issue](https://github.com/HighDiceRoller/icepool/issues) on GitHub. You can also find me on [Twitter](https://twitter.com/highdiceroller) or [Reddit](https://www.reddit.com/user/HighDiceRoller).
 
 ## API documentation
 
-[GitHub.](https://highdiceroller.github.io/icepool/apidoc/icepool.html)
+[pdoc on GitHub.](https://highdiceroller.github.io/icepool/apidoc/icepool.html)
 
 ## JupyterLite notebooks
 
 See this [JupyterLite distribution](https://highdiceroller.github.io/icepool/notebooks/lab/index.html) for a collection of interactive, editable examples. These include mechanics from published games, StackExchange, Reddit, and academic papers.
 
 ## Web applications
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `icepool-0.8.0/setup.cfg` & `icepool-0.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 6365 706f 6f6c 0d0a 7665 7273   = icepool..vers
-00000020: 696f 6e20 3d20 302e 382e 300d 0a61 7574  ion = 0.8.0..aut
+00000020: 696f 6e20 3d20 302e 392e 300d 0a61 7574  ion = 0.9.0..aut
 00000030: 686f 7220 3d20 416c 6265 7274 204a 756c  hor = Albert Jul
 00000040: 6975 7320 4c69 750d 0a61 7574 686f 725f  ius Liu..author_
 00000050: 656d 6169 6c20 3d20 616a 756c 3139 3837  email = ajul1987
 00000060: 2b68 6967 6864 6963 6572 6f6c 6c65 7240  +highdiceroller@
 00000070: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000080: 6970 7469 6f6e 203d 2041 2070 6163 6b61  iption = A packa
 00000090: 6765 2066 6f72 2063 6f6d 7075 7469 6e67  ge for computing
```

### Comparing `icepool-0.8.0/src/icepool/__init__.py` & `icepool-0.9.0/src/icepool/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,23 +33,27 @@
 from icepool.pool.pool import Pool, standard_pool, DicePool
 from icepool.pool.roll import PoolRoll
 from icepool.pool.eval import EvalPool, WrapFuncEval, SumPool, sum_pool, FindBestSet, FindBestRun
 
 import enum
 
 class SpecialValue(enum.Enum):
-    Reroll = 'Reroll'
+    Reroll = 'Reroll'  # Indicates an outcome should be rerolled (with no max depth).
+    Scalar = 'Scalar'  # A `ndim` indicating a non-vector die.
+    Empty = 'Empty'    # A `ndim` indicating a die with no outcomes.
 
 Reroll = SpecialValue.Reroll
+Scalar = SpecialValue.Scalar
+Empty = SpecialValue.Empty
 
 __all__ = ['Die',
     'standard', 'd', '__getattr__', 'bernoulli', 'coin',
     'BaseDie', 'EmptyDie', 'ScalarDie', 'VectorDie',
     'from_cweights', 'from_sweights', 'from_rv', 'align', 'align_range',
     'lowest', 'highest', 'max_outcome', 'min_outcome',
     'apply', 'dice_with_common_ndim',
-    'Reroll',
+    'Reroll', 'Scalar', 'Empty',
     'BasePool',
     'Pool', 'standard_pool', 'DicePool',
     # 'PoolRoll',  # Not needed externally due to implicit casts
     'EvalPool', 'WrapFuncEval', 'SumPool', 'sum_pool', 'FindBestSet', 'FindBestRun',
     'd2', 'd3', 'd4', 'd6', 'd8', 'd10', 'd12', 'd20', 'd100']
```

### Comparing `icepool-0.8.0/src/icepool/collections.py` & `icepool-0.9.0/src/icepool/collections.py`

 * *Files identical despite different names*

### Comparing `icepool-0.8.0/src/icepool/die/base.py` & `icepool-0.9.0/src/icepool/die/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     though these have little use other than being sentinel values.
     """
     
     @abstractmethod
     def ndim(self):
         """ Returns the number of dimensions if this is a `VectorDie`.
         
-        Otherwise, returns `'scalar'` for a `ScalarDie` and `'empty'` for an `EmptyDie`.
+        Otherwise, returns `'icepool.Scalar'` for a `ScalarDie` and `'icepool.Empty'` for an `EmptyDie`.
         """
     
     # Abstract methods.
     
     @abstractmethod
     def _unary_op(self, op, *args, **kwargs):
         """ Returns a die representing the effect of performing the operation on the outcomes.
@@ -62,16 +62,15 @@
         This is used for the operators `+, -, *, /, //, %, **, <<, >>, &, |, ^, <, <=, >=, >, ==, !=`.
         Note that `*` multiplies outcomes directly; it is not the same as `@` or `d()`.
         
         Special operators:
             * The `@` operator rolls the left die, then rolls the right die that many times and sums the outcomes.
                 Only the left side will be cast to a die; the right side must already be a die.
             * `==` and `!=` are applied across outcomes like the other operators.
-                Unfortunately this means dice are not hashable by normal means.
-                Custom functions can use `key_tuple()`, `equals()` and `hash()` as workarounds.
+                They also set the truth value of the die according to whether the die themselves are the same.
         """
     
     @abstractmethod
     def _wrap_unpack(self, func):
         """ Possibly wraps `func` so that outcomes are unpacked before giving it to `func`. """
         
     @abstractmethod
@@ -390,31 +389,20 @@
                 data[min_outcome] += weight
             elif max_outcome is not None and outcome >= max_outcome:
                 data[max_outcome] += weight
             else:
                 data[outcome] += weight
         return icepool.Die(data, ndim=self.ndim())
     
-    def split(self, cond):
-        """ Splits this die's items into two pieces based on `cond(outcome)`.
+    def if_else(self, outcome_if_true, outcome_if_false, /):
+        """ Ternary conditional operator.
         
-        The left result is all outcome-weight pairs where `cond(outcome)` is `True`.
-        The right result is all outcome-weight pairs where `cond(outcome)` is `False`.
-        
-        `cond` will be supplied with one argument per `ndim` if this is a `VectorDie`.
+        This replaces truthy outcomes with the first argument and falsy outcomes with the second argument.
         """
-        cond = self._wrap_unpack(cond)
-        data_true = {}
-        data_false = {}
-        for outcome, weight in self.items():
-            if cond(outcome):
-                data_true[outcome] = weight
-            else:
-                data_false[outcome] = weight
-        return icepool.Die(data_true, ndim=self.ndim()), icepool.Die(data_false, ndim=self.ndim())
+        return self.bool().sub(lambda x: outcome_if_true if x else outcome_if_false)
     
     def set_outcomes(self, outcomes):
         """ Sets the set of outcomes to the argument.
         
         This may remove outcomes (if they are not present in the argument)
         and/or add zero-weight outcomes (if they are not present in this die).
         """
@@ -843,21 +831,27 @@
         other = icepool.Die(other, ndim=self.ndim())
         return self._binary_op(other, operator.ge)
         
     def __gt__(self, other):
         other = icepool.Die(other, ndim=self.ndim())
         return self._binary_op(other, operator.gt)
     
+    # Equality operators. These additionally set the truth value of the result.
+    
     def __eq__(self, other):
         other = icepool.Die(other, ndim=self.ndim())
-        return self._binary_op(other, operator.eq)
+        result = self._binary_op(other, operator.eq)
+        result._truth_value = self.equals(other)
+        return result
     
     def __ne__(self, other):
         other = icepool.Die(other, ndim=self.ndim())
-        return self._binary_op(other, operator.ne)
+        result = self._binary_op(other, operator.ne)
+        result._truth_value = not self.equals(other)
+        return result
     
     @staticmethod
     def _sign(x):
         z = BaseDie._zero(x)
         if x > z:
             return 1
         elif x < z:
@@ -908,56 +902,61 @@
         # We don't use random.choices since that is based on floats rather than ints.
         r = random.randrange(self.denominator())
         index = bisect.bisect_right(self.cweights(), r)
         return self.outcomes()[index]
     
     # Invalid operations.
     
-    def __bool__(self):
-        """ Dice are not considered to have truth values. 
-        
-        The result of a comparator operation is a die,
-        which if considered to have a truth value,
-        would imply that dice are sortable by that operator.
-        """
-        raise TypeError('A die does not have a truth value.')
-    
     def __reversed__(self):
         raise TypeError('A die cannot be reversed.')
     
     # Equality and hashing.
     
+    def __bool__(self):
+        if hasattr(self, '_truth_value'):
+            return self._truth_value
+        else:
+            raise ValueError('A die only has a truth value if it is the result of == or !=. If this is in the conditional of an if-statement, you probably want to use die.if_else() instead.')
+    
     @cached_property
     def _key_tuple(self):
         return tuple(self.items()), self.ndim()
         
     def key_tuple(self):
         """ Returns a tuple that uniquely (as `equals()`) identifies this die. """
         return self._key_tuple
 
-    def hash(self):
-        """ A true __hash__ doesn't work because we used the __eq__ operator 
-        for determining the chance two dice will roll equal to each other.
-        """
+    @cached_property
+    def _hash(self):
         return hash(self.key_tuple())
+        
+    def __hash__(self):
+        return self._hash
     
-    __hash__ = None
-    
-    def equals(self, other):
-        """ Returns `True` iff both dice have the same ndim, outcomes, and weights.
+    def equals(self, other, *, reduce=False):
+        """ Returns `True` iff both dice have the same ndim, outcomes, and weights. Truth value does NOT matter.
         
-        Note that dice are not reduced, e.g. a 2:2 coin is not `equals()` to a 1:1 coin. 
-        Also, if one die has a zero-weight outcome and the other die does not contain that outcome,
+        If one die has a zero-weight outcome and the other die does not contain that outcome,
         they are treated as unequal by this function.
         
-        For the chance of two dice rolling the same outcome, use the `==` operator.
+        The `==` and `!=` operators have a dual purpose; they return a die representing the result of the operator as normal,
+        but the die additionally has a truth value determined by this method.
+        Only dice returned by these methods have a truth value.
+        
+        Args:
+            reduce: If `True`, the dice will be reduced before comparing.
+                Otherwise, e.g. a 2:2 coin is not `equals()` to a 1:1 coin. 
         """
         try:
             other = icepool.Die(other, ndim=self.ndim())
         except ValueError:
             return False
-        return self.key_tuple() == other.key_tuple()
+        
+        if reduce:
+            return self.reduce().key_tuple() == other.reduce().key_tuple()
+        else:
+            return self.key_tuple() == other.key_tuple()
     
     # Strings.
     
     def __str__(self):
         return self.markdown(include_weights=self.denominator() < 10 ** 30)
```

### Comparing `icepool-0.8.0/src/icepool/die/create.py` & `icepool-0.9.0/src/icepool/die/create.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __docformat__ = 'google'
 
 import icepool
 from icepool.collections import Counts
 
 from collections import defaultdict
+import itertools
 import math
 
 def Die(*args, weights=None, min_outcome=None, ndim=None, denominator_method='lcm'):
     """ Factory for constructing a die.
     
     This is capitalized because it is the preferred way of getting a new instance,
     and so that you can use `from icepool import Die` while leaving the name `die` free.
@@ -25,218 +26,212 @@
     * Use a d6 that you already have: `Die(d6)`
     * Mix a d3 and a d3+3: `Die(d3, d3+3)`
     * Use a dict: `Die({1:1, 2:1, 3:1, 4:1, 5:1, 6:1})`
     * Give the faces as args: `Die(1, 2, 3, 4, 5, 6)`
     
     Args:
         *args: Each of these arguments can be one of the following:
+            * A die. Its current `ndim` will be ignored, but this may change in the future.
+                The outcomes of the die will be "flattened" into the result;
+                a die object will never contain a die as an outcome.
+            * A dict-like that maps outcomes to weights.
+                The outcomes of the dict-like will be "flattened" into the result.
+                This option will be taken in preference to treating the dict-like itself as an outcome
+                even if the dict-like itself is hashable and comparable.
+            * A tuple of outcomes. Any inner nested tuples will be treated as scalar.
+                Any arguments that are dice or dicts will expand the tuple
+                according to their independent joint distribution.
+                For example, (d6, d6) will expand to 36 ordered tuples with weight 1 each.
+                Use this sparingly since it may create a large number of outcomes.
+            * `icepool.Reroll`, which will drop itself
+                and the corresponding element of `weights` from consideration.
             * A single outcome, which must be hashable and comparable.
                 The same outcome can appear multiple times,
                 in which case it will be weighted proportionally higher.
             
                 Note: An argument that is a sequence will be treated as a single outcome.
                 If you want each element in the sequence to be a separate outcome,
                 you need to unpack it into separate arguments.
-            * A die. The `ndim` of the die must be preserved, or this is a `ValueError`.
-                The outcomes of the die will be "flattened" in the result die.
-            * A dict-like that maps outcomes to weights.
-                This option will be taken in preference to treating the dict-like itself as an outcome
-                even if the dict-like itself is hashable and comparable.
-                
-                Not recommended options:
-                
-                * If you want to use the dict-like itself as an outcome, wrap it in another dict.
-                * The dict itself can contain `icepool.Reroll`.
-                    This will only reroll within the dict, not the entire construction.
-            * `icepool.Reroll`, which will drop itself
-                and the corresponding element of `weights` from consideration.
         weights: Controls the relative weight of the arguments.
-            If not provided, each argument will end up with the same total weight,
-            unless they have zero weight to begin with.
+            If an argument expands into multiple outcomes, the weight is shared among those outcomes.
+            If not provided, each argument will end up with the same total weight.
             For example, `Die(d6, 7)` is the same as `Die(1, 2, 3, 4, 5, 6, 7, 7, 7, 7, 7, 7)`.
-        min_outcome: If used, there must be zero `*args` and `weights` must be provided.
+        min_outcome: If used, there must be zero `*args`, and `weights` must be provided.
             The outcomes of the result will be integers starting at `min_outcome`,
             one per weight in `weights` with that weight.
-        ndim: If set to `'scalar'`, the die will be forced to be scalar.
-            If set to an `int`, the die will be forced to be vector with that number of dimensions.
-            If not provided, this will be automatically detected.
+        ndim: If set to `icepool.Scalar`, the die will be scalar.
+            If set to an `int`, the die will have that many dimensions if the outcomes allow,
+                and raise `ValueError` otherwise.
+            If `None` (default), the number of dimensions will be automatically detected:
             If all arguments are `tuple`s of the same length,
             the result will have that many dimensions.
             Otherwise the result will be scalar.
+            Regardless of `ndim`, any inner nested tuples will be treated as scalar.
         denominator_method: How to determine the denominator of the result
-            if the arguments themselves contain weights.
+            if the arguments themselves contain weights. This is also used for dict-like arguments.
             From greatest to least:
             * 'prod': Product of the individual argument denominators, times the total of `weights`.
                 This is like rolling all of the possible dice, and then selecting a result.
             * 'lcm' (default): LCM of the individual argument denominators, times the total of `weights`.
                 This is like rolling `weights` first, then selecting an argument to roll.
             * 'lcm_weighted': LCM of the individual (argument denominators times corresponding element of `weights`).
                 This is like rolling the above, but the specific weight rolled
                 is used to help determine the result of the selected argument.
             * 'reduce': `reduce()` is called at the end.
     Raises:
-        `ValueError` if `ndim` is set but is not consistent with `*args`,
-            or there is a mismatch between the `ndim` of die arguments.
+        `ValueError` if `ndim` is set but is not consistent with `*args`.
             Furthermore, `None` is not a valid outcome for a die.
     """
     
+    # Special case: consecutive outcomes.
     if min_outcome is not None:
         if weights is None:
             raise ValueError('If min_outcome is provided, weights must also be provided.')
         if len(args) > 0:
             raise ValueError('If min_outcome is provided, no *args may be used.')
-        if ndim not in [None, 'scalar']:
+        if ndim not in [None, icepool.Scalar]:
             raise ValueError('If min_outcome is provided, the result may only be a scalar die.')
         data = Counts({i + min_outcome : weight for i, weight in enumerate(weights)})
         return icepool.ScalarDie(data)
     
     if weights is not None:
         if len(weights) != len(args):
             raise ValueError('If weights are provided, there must be exactly one weight per argument.')
     else:
         weights = (1,) * len(args)
     
-    # Remove rerolls.
-    args_weights = tuple(zip(*((arg, weight) for arg, weight in zip(args, weights) if arg is not icepool.Reroll)))
-    if len(args_weights) == 0:
-        args, weights = (), ()
-    else:
-        args, weights = args_weights
-    for arg in args:
-        if _is_dict(arg) and icepool.Reroll in arg:
-            del arg[icepool.Reroll]
-    
     # Special cases.
     if len(args) == 0:
         return icepool.EmptyDie()
     elif len(args) == 1 and _is_die(args[0]) and weights[0] == 1:
+        if ndim is not None and args[0].ndim() != ndim:
+            raise ValueError(f'Mismatch between requested ndim={ndim} and die with ndim={args[0].ndim()}')
         # Single unmodified die: just return the existing instance.
         return args[0]
     
-    # Total weights.
-    arg_denominators = [_arg_denominator(arg) for arg in args]
-    
-    if denominator_method == 'prod':
-        denominator_prod = math.prod(d for d in arg_denominators if d > 0)
-    elif denominator_method == 'lcm':
-        denominator_prod = math.lcm(*(d for d in arg_denominators if d > 0))
-    elif denominator_method in ['lcm_weighted', 'reduce']:
-        denominator_prod = math.lcm(*(d // math.gcd(d, w) for d, w in zip(arg_denominators, weights) if d > 0))
-    else:
-        raise ValueError(f'Invalid denominator_method {denominator_method}.')
-    
-    # Compute ndim.
-    ndim = _calc_ndim(*args, ndim=ndim)
-    
-    # Make data.
-    data = defaultdict(int)
-    for arg, arg_denominator, w in zip(args, arg_denominators, weights):
-        factor = denominator_prod * w // arg_denominator if arg_denominator else 0
-        if _is_die(arg) or _is_dict(arg):
-            for outcome, weight in arg.items():
-                data[outcome] += weight * factor
-        else:
-            data[arg] += factor
+    # Expand data.
+    subdatas = [_expand(arg, denominator_method) for arg in args]
+    data = _merge_subdatas(subdatas, weights, denominator_method)
     
     if len(data) == 0:
         return icepool.EmptyDie()
     
-    for arg in args:
-        ndim = _arg_ndim(arg, ndim)
+    # Compute ndim.
+    if ndim == None:
+        for outcome in data.keys():
+            if _is_tuple(outcome):
+                if ndim is None:
+                    ndim = len(outcome)
+                elif ndim != len(outcome):
+                    ndim = icepool.Scalar
+                    break
+            else:
+                ndim = icepool.Scalar
+                break
+    elif ndim != icepool.Scalar:
+        for outcome in data.keys():
+            if not _is_tuple(outcome) or len(outcome) != ndim:
+                raise ValueError(f'Outcome {outcome} is incompatible with requested ndim {ndim}')
     
-    if ndim == 'scalar':
+    if ndim == icepool.Scalar:
         data = Counts(data)
         result = icepool.ScalarDie(data)
     else:
-        data = Counts({ tuple(k) : v for k, v in data.items() })
+        data = Counts(data)
         result = icepool.VectorDie(data, ndim)
     
     if denominator_method == 'reduce':
         result = result.reduce()
     
     return result
 
+def _expand(arg, denominator_method):
+    """ Expands the argument to a dict mapping outcomes to weights.
+    
+    The outcomes are valid outcomes for a die.
+    """
+    if _is_die(arg):
+        return _expand_die(arg)
+    elif _is_dict(arg):
+        return _expand_dict(arg, denominator_method)
+    elif _is_tuple(arg):
+        return _expand_tuple(arg, denominator_method)
+    else:
+        return _expand_scalar(arg)
+
 def _is_die(arg):
     return isinstance(arg, icepool.BaseDie)
 
-def _is_dict(arg):
-    return hasattr(arg, 'keys') and hasattr(arg, 'items') and hasattr(arg, '__getitem__')
+def _expand_die(arg):
+    return arg._data
 
+def _is_dict(arg):
+    return hasattr(arg, 'keys') and hasattr(arg, 'values') and hasattr(arg, 'items') and hasattr(arg, '__getitem__')
+    
+def _expand_dict(arg, denominator_method):
+    subdatas = [_expand(k, denominator_method) for k, v in arg.items()]
+    weights = [x for x in arg.values()]
+    return _merge_subdatas(subdatas, weights, denominator_method)
+    
 def _is_tuple(arg):
     return type(arg) is tuple
 
-def _arg_denominator(arg):
-    if _is_die(arg):
-        return arg.denominator()
-    elif _is_dict(arg):
-        return sum(arg.values())
+def _expand_tuple(arg, denominator_method):
+    subdatas = [_expand(x, denominator_method) for x in arg]
+    data = defaultdict(int)
+    for t in itertools.product(*(subdata.items() for subdata in subdatas)):
+        outcomes, weights = zip(*t)
+        data[outcomes] += math.prod(weights)
+    return data
+    
+def _expand_scalar(arg):
+    if arg is icepool.Reroll:
+        return {}
     else:
-        return 1
+        return { arg : 1 }
 
-def _calc_ndim(*args, ndim):
-    """ Computes the common `ndim` of the arguments. 
+def _merge_subdatas(subdatas, weights, denominator_method):
+    subdata_denominators = [sum(subdata.values()) for subdata in subdatas]
     
-    Args:
-        *args: Args to find the common `ndim` of.
-        ndim: The required ndim of the results.
+    if denominator_method == 'prod':
+        denominator_prod = math.prod(d for d in subdata_denominators if d > 0)
+    elif denominator_method == 'lcm':
+        denominator_prod = math.lcm(*(d for d in subdata_denominators if d > 0))
+    elif denominator_method in ['lcm_weighted', 'reduce']:
+        denominator_prod = math.lcm(*(d // math.gcd(d, w) for d, w in zip(subdata_denominators, weights) if d > 0))
+    else:
+        raise ValueError(f'Invalid denominator_method {denominator_method}.')
     
-    Returns:
-        The common `ndim` of the arguments.  
-        May return `None` if no `ndim` is found.
+    data = defaultdict(int)
+    for subdata, subdata_denominator, w in zip(subdatas, subdata_denominators, weights):
+        factor = denominator_prod * w // subdata_denominator if subdata_denominator else 0
+        for outcome, weight in subdata.items():
+            data[outcome] += weight * factor
     
-    Raises:
-        `ValueError` if the arguments include conflicting `ndim`s.
-    """
-    for arg in args:
-        ndim = _arg_ndim(arg, ndim)
-    return ndim 
-
-def _arg_ndim(arg, ndim):
-    """ Checks the ndim of a single argument. """
-    if _is_die(arg):
-        if arg.is_empty():
-            return ndim
-        elif ndim is None:
-            return arg.ndim()
-        elif arg.ndim() != ndim:
-            raise ValueError(f'Argument die has ndim={arg.ndim()} inconsistent with other ndim={ndim}.')
-        return ndim
-    elif ndim == 'scalar':
-        return 'scalar'
-    elif _is_dict(arg):
-        for outcome in arg.keys():
-            # No recursion to nested dicts.
-            if _is_tuple(outcome):
-                if ndim is None:
-                    ndim = len(outcome)
-                elif len(outcome) != ndim:
-                    return 'scalar'
-            else:
-                return 'scalar'
-        return ndim
-    elif _is_tuple(arg):
-        # Arg is a sequence.
-        if ndim is None:
-            return len(arg)
-        elif len(arg) != ndim:
-            return 'scalar'
-        else:
-            return ndim
-    else:
-        # Arg is a scalar.
-        return 'scalar'
+    return data
 
 def dice_with_common_ndim(*args, ndim=None):
     """ Converts the arguments to dice with a common `ndim`.
     
     Args:
         *args: Args to be converted to dice.
         ndim: The required `ndim` of the results.
     
     Returns:
         dice, ndim: A tuple containing one die per arg, and the common `ndim`,
     
     Raises:
         `ValueError` if the arguments include conflicting `ndim`s.
     """
-    ndim = _calc_ndim(*args, ndim=ndim)
-    return tuple(Die(arg, ndim=ndim) for arg in args), ndim
+    if ndim is None:
+        if len(args) == 0:
+            return (), None
+        # First pass: All dice get to be vector if possible.
+        first_pass = tuple(Die(arg) for arg in args)
+        if all(die.ndim() == first_pass[0].ndim() for die in first_pass):
+            # If all dice end up with same ndim, return that.
+            return first_pass, first_pass[0].ndim()
+        else:
+            # Otherwise remake them as scalar.
+            return tuple(Die(arg, ndim=icepool.Scalar) for die in first_pass), icepool.Scalar
+    else:
+        return tuple(Die(arg, ndim=ndim) for arg in args), ndim
```

### Comparing `icepool-0.8.0/src/icepool/die/empty.py` & `icepool-0.9.0/src/icepool/die/empty.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,17 +4,23 @@
 import icepool.die.base
 from icepool.collections import Counts
 
 class EmptyDie(icepool.die.base.BaseDie):
     """ Die with no outcomes. """
     
     def ndim(self):
-        return 'empty'
+        return icepool.Empty
     
     def __init__(self):
+        """ Constructor.
+        
+        Dice should not be constructed directly;
+        instead, use one of the methods defined in `icepool.die.func` 
+        (which are imported into the top-level `icepool` module).
+        """
         self._data = Counts({})
         
     def _unary_op(self, op, *args, **kwargs):
         """ There are no outcomes, so nothing happens. """
         return self
     
     def _binary_op(self, other, op, *args, **kwargs):
```

### Comparing `icepool-0.8.0/src/icepool/die/func.py` & `icepool-0.9.0/src/icepool/die/func.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     * `icepool.Die(6)`: A die that always rolls the integer 6.
     * `icepool.d(6)`: A d6.
     """
     if not isinstance(num_sides, int):
         raise TypeError('Argument to standard() must be an int.')
     elif num_sides < 1:
         raise ValueError('Standard die must have at least one side.')
-    return icepool.Die(weights=[1] * num_sides, min_outcome=1, ndim='scalar')
+    return icepool.Die(weights=[1] * num_sides, min_outcome=1, ndim=icepool.Scalar)
     
 def d(arg):
     """ Converts the argument to a standard die if it is not already a die.
     
     Args:
         arg: Either:
             * An `int`, which produces a standard die.
@@ -50,15 +50,15 @@
             return standard(int(key[1:]))
         except ValueError:
             pass
     raise AttributeError(key)
 
 def bernoulli(n, d):
     """ A die that rolls `True` with chance `n / d`, and `False` otherwise. """
-    return icepool.Die({False : d - n, True : n}, ndim='scalar')
+    return icepool.Die({False : d - n, True : n}, ndim=icepool.Scalar)
 
 coin = bernoulli
 
 def from_cweights(outcomes, cweights, *, ndim=None):
     """ Constructs a die from cumulative weights. """
     prev = 0
     d = {}
@@ -110,15 +110,15 @@
     """
     dice, ndim = icepool.dice_with_common_ndim(*dice)
     outcomes = set(itertools.chain.from_iterable(die.outcomes() for die in dice))
     return tuple(die.set_outcomes(outcomes) for die in dice)
 
 def align_range(*dice):
     """Pads all the dice with zero weights so that all have the same set of consecutive `int` outcomes. """
-    dice, ndim = icepool.dice_with_common_ndim(*dice, ndim='scalar')
+    dice, ndim = icepool.dice_with_common_ndim(*dice, ndim=icepool.Scalar)
     outcomes = tuple(range(icepool.min_outcome(*dice), icepool.max_outcome(*dice) + 1))
     return tuple(die.set_outcomes(outcomes) for die in dice)
 
 def apply(func, *dice, ndim=None):
     """ Applies `func(outcome_of_die_0, outcome_of_die_1, ...)` for all possible outcomes of the dice.
     
     This is flexible but not very efficient for large numbers of dice.
```

### Comparing `icepool-0.8.0/src/icepool/die/scalar.py` & `icepool-0.9.0/src/icepool/die/scalar.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class ScalarDie(icepool.die.base.BaseDie):
     """ Univariate die.
     
     Outcomes are scalars and operations are performed directly on the outcomes.
     """
     
     def ndim(self):
-        return 'scalar'
+        return icepool.Scalar
     
     def __init__(self, data):
         """ Constructor.
         
         Dice should not be constructed directly;
         instead, use one of the methods defined in `icepool.die.func` 
         (which are imported into the top-level `icepool` module).
@@ -31,22 +31,22 @@
         self._data = data
     
     def _unary_op(self, op, *args, **kwargs):
         """ Returns a die representing the effect of performing the operation on the outcomes. """
         data = defaultdict(int)
         for outcome, weight in self.items():
             data[op(outcome, *args, **kwargs)] += weight
-        return icepool.Die(data, ndim='scalar')
+        return icepool.Die(data, ndim=icepool.Scalar)
     
     def _binary_op(self, other, op, *args, **kwargs):
         """ Returns a die representing the effect of performing the operation on pairs of outcomes from the two dice. """
         data = defaultdict(int)
         for (outcome_self, weight_self), (outcome_other, weight_other) in itertools.product(self.items(), other.items()):
             data[op(outcome_self, outcome_other, *args, **kwargs)] += weight_self * weight_other
-        return icepool.Die(data, ndim='scalar')
+        return icepool.Die(data, ndim=icepool.Scalar)
     
     def _wrap_unpack(self, func):
         return func
     
     # Special operators.
     
     def d(self, other, *, ndim=None):
@@ -168,37 +168,14 @@
     
     def skewness(self):
         return self.standardized_moment(3.0)
     
     def excess_kurtosis(self):
         return self.standardized_moment(4.0) - 3.0
     
-    def cartesian_product(*dice):
-        """
-        Produces a `VectorDie` from the Cartesian product of the input `ScalarDie`.
-        
-        This is usually not recommended, as it takes space and time exponential in the number of dice,
-        while not actually producing any additional information.
-        
-        Args:
-            *dice: Multiple dice or a single iterable of dice.
-        
-        Raises:
-            `TypeError` if any of the input dice are already `VectorDie`.
-        """
-        if any(die.ndim > 1 for die in dice):
-            raise TypeError('cartesian_product() is only valid on ScalarDie.')
-        
-        data = defaultdict(int)
-        for t in itertools.product(*(die.items() for die in dice)):
-            outcomes, weights = zip(*t)
-            data[outcomes] += math.prod(weights)
-        
-        return icepool.Die(data, ndim=len(dice))
-    
     def __repr__(self):
         return type(self).__qualname__ + f'({self._data.__repr__()})'
     
     def markdown(self, include_weights=True):
         outcome_length = max(tuple(len(str(outcome)) for outcome in self.outcomes()) + (len('Outcome'),))
         result = ''
         result += f'Denominator: {self.denominator()}\n\n'
```

### Comparing `icepool-0.8.0/src/icepool/die/vector.py` & `icepool-0.9.0/src/icepool/die/vector.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     
     def marginal(self, select):
         """ Returns the marginal distribution over selected dimensions of the die. """
         test_select = ([None] * self.ndim())[select]
         if hasattr(test_select, '__len__'):
             ndim = len(test_select)
         else:
-            ndim = 'scalar'
+            ndim = icepool.Scalar
         data = defaultdict(int)
         for outcome, weight in self.items():
             data[outcome[select]] += weight
         return icepool.Die(data, ndim=ndim)
     
     @cached_property
     def dim(self):
@@ -74,25 +74,25 @@
         
         For example, `die.dim[0]` will extract the 0th dimension.
         """
         return Slicer(self.marginal)
     
     def all(self):
         """ Returns a die representing whether all dimensions are true. """
-        return self.sub(lambda *outcome: all(outcome), ndim='scalar')
+        return self.sub(lambda *outcome: all(outcome), ndim=icepool.Scalar)
     
     def any(self):
         """ Returns a die representing whether any dimension is true. """
-        return self.sub(lambda *outcome: any(outcome), ndim='scalar')
+        return self.sub(lambda *outcome: any(outcome), ndim=icepool.Scalar)
     
     # Statistics.
     # These apply to a single dimension `i`.
     
     def _apply_to_dim(self, func, i, *args, **kwargs):
-        return func(self[i], *args, **kwargs)
+        return func(self.dim[i], *args, **kwargs)
     
     def median_left(self, i):
         return self._apply_to_dim(icepool.ScalarDie.median_left, i)
         
     def median_right(self, i):
         return self._apply_to_dim(icepool.ScalarDie.median_right, i)
     
@@ -127,21 +127,21 @@
         
     def excess_kurtosis(self, i):
         return self._apply_to_dim(icepool.ScalarDie.excess_kurtosis, i)
     
     # Joint statistics.
     
     def covariance(self, i, j):
-        mean_i = self[i].mean()
-        mean_j = self[j].mean()
+        mean_i = self.dim[i].mean()
+        mean_j = self.dim[j].mean()
         return sum((outcome[i] - mean_i) * (outcome[j] - mean_j) * weight for outcome, weight in self.items()) / self.denominator()
     
     def correlation(self, i, j):
-        sd_i = self[i].standard_deviation()
-        sd_j = self[j].standard_deviation()
+        sd_i = self.dim[i].standard_deviation()
+        sd_j = self.dim[j].standard_deviation()
         return self.covariance(i, j) / (sd_i * sd_j)
     
     def __repr__(self):
         return type(self).__qualname__ + f'({self._data.__repr__()}, ndim={self.ndim()})'
     
     def markdown(self, include_weights=True):
         """ Formats the die as a Markdown table. """
```

### Comparing `icepool-0.8.0/src/icepool/pool/base.py` & `icepool-0.9.0/src/icepool/pool/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,45 +18,67 @@
     """
     
     @abstractmethod
     def _is_single_roll(self):
         """ Returns `True` iff this is a single, fixed roll of a pool. """
     
     @abstractmethod
-    def _has_truncate_max(self):
-        """ Returns `True` iff the pool has right-truncation. """
-        
-    @abstractmethod
     def _has_truncate_min(self):
-        """ Returns `True` iff the pool has left-truncation. """
+        """ Returns `True` iff the pool has truncated min outcomes. """
+    
+    @abstractmethod
+    def _has_truncate_max(self):
+        """ Returns `True` iff the pool has truncated max outcomes. """
     
     @abstractmethod
     def outcomes(self):
         """ The outcomes of the fundamental die (including those with zero weight). """
-        
+    
+    @abstractmethod
+    def _min_outcome(self):
+        """ The minimum outcome of the fundamental die. """
+    
     @abstractmethod
     def _max_outcome(self):
         """ The maximum outcome of the fundamental die. """
         
     @abstractmethod
-    def _min_outcome(self):
-        """ The minimum outcome of the fundamental die. """
+    def _direction_score_ascending(self):
+        """ Returns a number indicating how preferred iterating in the ascending direction is.
+        
+        This is only called when there is no truncation.
+        
+        If the pool does not care at all about direction, the result is 0.
+        
+        The collective score is summed.
+        """
     
     @abstractmethod
-    def _pop_max(self):
-        """ Returns a sequence of pool, count, weight corresponding to removing the max outcome,
-        with count and weight corresponding to various numbers of dice rolling that outcome.
+    def _direction_score_descending(self):
+        """ Returns a number indicating how preferred iterating in the descending direction is.
+        
+        This is only called when there is no truncation.
+        
+        If the pool does not care at all about direction, the result is 0.
+        
+        The collective score is summed.
         """
     
     @abstractmethod
     def _pop_min(self):
         """ Returns a sequence of pool, count, weight corresponding to removing the min outcome,
         with count and weight corresponding to various numbers of dice rolling that outcome.
         """
     
+    @abstractmethod
+    def _pop_max(self):
+        """ Returns a sequence of pool, count, weight corresponding to removing the max outcome,
+        with count and weight corresponding to various numbers of dice rolling that outcome.
+        """
+    
     def eval(self, eval_or_func, /):
         """ Evaluates this pool using the given `EvalPool` or function.
         
         Note that each `EvalPool` instance carries its own cache;
         if you plan to use an evaluation multiple times,
         you may want to explicitly create an `EvalPool` instance
         rather than passing a function to this method directly.
```

### Comparing `icepool-0.8.0/src/icepool/pool/eval.py` & `icepool-0.9.0/src/icepool/pool/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,23 +218,21 @@
         direction = self.direction(*pools)
         
         if not direction:
             if has_truncate_max:
                 direction = 1
             elif has_truncate_min:
                 direction = -1
-            elif any(not pool._is_single_roll() for pool in pools):
-                num_drop_lowest = max(pool.num_drop_lowest() for pool in pools if not pool._is_single_roll())
-                num_drop_highest = max(pool.num_drop_highest() for pool in pools if not pool._is_single_roll())
-                if num_drop_lowest >= num_drop_highest:
-                    direction = 1
-                else:
-                    direction = -1
             else:
-                direction = 1
+                score_ascending = sum(pool._direction_score_ascending() for pool in pools)
+                score_descending = sum(pool._direction_score_descending() for pool in pools)
+                if score_ascending < score_descending:
+                    direction = -1
+                else:
+                    direction = 1
         
         if direction > 0 and has_truncate_min or direction < 0 and has_truncate_max:
             # Forced onto the less-preferred algorithm.
             return self._eval_internal_iterative, direction
         else:
             # Use the preferred algorithm.
             return self._eval_internal, direction
```

### Comparing `icepool-0.8.0/src/icepool/pool/pool.py` & `icepool-0.9.0/src/icepool/pool/pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,33 +344,33 @@
     __getitem__ = set_count_dice
     
     def __iter__(self):
         raise TypeError("'DicePool' object is not iterable")
     
     @cached_property
     def _num_drop_lowest(self):
+        """ How many elements of count_dice on the low side are falsy. """
         for i, count in enumerate(self.count_dice()):
             if count:
                 return i
         return self.num_dice()
     
-    def num_drop_lowest(self):
-        """ How many elements of count_dice on the low side have a false truth value. """
-        return self._num_drop_lowest
+    def _direction_score_ascending(self):
+        return self._num_drop_lowest * len(self.outcomes())
     
     @cached_property
     def _num_drop_highest(self):
+        """ How many elements of count_dice on the high side are falsy. """
         for i, count in enumerate(reversed(self.count_dice())):
             if count:
                 return i
         return self.num_dice()
     
-    def num_drop_highest(self):
-        """ How many elements of count_dice on the high side have a false truth value. """
-        return self._num_drop_highest
+    def _direction_score_descending(self):
+        return self._num_drop_highest * len(self.outcomes())
     
     def truncate_min(self, always_tuple=False):
         """ A sorted tuple of thresholds below which outcomes are truncated, one for each die in the pool. 
         
         Args:
             always_tuple: If `False`, this will return `None` if there are no die-specific `truncate_min`.
                 If `True` this will return a `tuple` even in this case.
@@ -425,15 +425,15 @@
         
         # Consider various numbers of dice rolling this outcome.
         popped_truncate_min = (popped_die.min_outcome(),) * num_possible_dice + truncate_min[num_possible_dice:]
         popped_count_dice = self.count_dice()
         count = 0
         
         comb_row = icepool.math.comb_row(num_possible_dice, single_weight)
-        end_counted = self.num_dice() - self.num_drop_highest()
+        end_counted = self.num_dice() - self._num_drop_highest
         for weight in comb_row[:min(num_possible_dice, end_counted)]:
             pool = _pool_cached_unchecked(popped_die, count_dice=popped_count_dice, truncate_min=popped_truncate_min)
             yield pool, count, weight
             count += popped_count_dice[0]
             popped_truncate_min = popped_truncate_min[1:]
             popped_count_dice = popped_count_dice[1:]
         
@@ -477,15 +477,15 @@
         
         # Consider various numbers of dice rolling this outcome.
         popped_truncate_max = truncate_max[:num_unused_dice] + (popped_die.max_outcome(),) * num_possible_dice
         popped_count_dice = self.count_dice()
         count = 0
         
         comb_row = icepool.math.comb_row(num_possible_dice, single_weight)
-        end_counted = self.num_dice() - self.num_drop_lowest()
+        end_counted = self.num_dice() - self._num_drop_lowest
         for weight in comb_row[:min(num_possible_dice, end_counted)]:
             pool = _pool_cached_unchecked(popped_die, count_dice=popped_count_dice, truncate_max=popped_truncate_max)
             yield pool, count, weight
             count += popped_count_dice[-1]
             popped_truncate_max = popped_truncate_max[:-1]
             popped_count_dice = popped_count_dice[:-1]
```

### Comparing `icepool-0.8.0/src/icepool/pool/roll.py` & `icepool-0.9.0/src/icepool/pool/roll.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __docformat__ = 'google'
 
 import icepool
 from icepool.collections import Counts
 
 from collections import defaultdict
 from functools import cached_property
+import math
 
 def _is_dict(arg):
     return hasattr(arg, 'keys') and hasattr(arg, 'items') and hasattr(arg, '__getitem__')
 
 class PoolRoll(icepool.BasePool):
     """ Represents a single, fixed roll of a dice pool.
     
@@ -33,40 +34,46 @@
             for outcome in arg:
                 data[outcome] += 1
         
         self._data = Counts(data)
 
     def _is_single_roll(self):
         return True
-    
-    def _has_truncate_max(self):
+        
+    def _has_truncate_min(self):
         return False
     
-    def _has_truncate_min(self):
+    def _has_truncate_max(self):
         return False
     
     def outcomes(self):
         return self._data.keys()
     
-    def _max_outcome(self):
-        return self._data.keys()[-1]
-    
     def _min_outcome(self):
         return self._data.keys()[0]
     
-    def _pop_max(self):
-        data = { outcome : count for outcome, count in self._data.items()[:-1] }
-        count = self._data.values()[-1]
-        return (PoolRoll(data), count, 1),
+    def _max_outcome(self):
+        return self._data.keys()[-1]
+        
+    def _direction_score_ascending(self):
+        return 0
+    
+    def _direction_score_descending(self):
+        return 0
     
     def _pop_min(self):
         data = { outcome : count for outcome, count in self._data.items()[1:] }
         count = self._data.values()[0]
         return (PoolRoll(data), count, 1),
     
+    def _pop_max(self):
+        data = { outcome : count for outcome, count in self._data.items()[:-1] }
+        count = self._data.values()[-1]
+        return (PoolRoll(data), count, 1),
+    
     # Forwarding dict-like methods.
     
     def keys(self):
         return self._data.keys()
         
     def items(self):
         return self._data.items()
```

### Comparing `icepool-0.8.0/src/icepool.egg-info/PKG-INFO` & `icepool-0.9.0/src/icepool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icepool
-Version: 0.8.0
+Version: 0.9.0
 Summary: A package for computing dice probabilities
 Home-page: https://github.com/HighDiceRoller/icepool
 Author: Albert Julius Liu
 Author-email: ajul1987+highdiceroller@gmail.com
 License: UNKNOWN
 Project-URL: Twitter, https://twitter.com/highdiceroller
 Platform: UNKNOWN
@@ -17,37 +17,39 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # <img width="32" height="32" src="https://highdiceroller.github.io/icepool/apps/favicon.png" /> Icepool
 
 A Python package for computing dice probabilities.
 
-[GitHub.](https://github.com/HighDiceRoller/icepool)
+[GitHub repository.](https://github.com/HighDiceRoller/icepool)
 
 ## Features
 
 * Pure Python implementation.
 * Exact fractional probabilities using Python `int`s.
-* Dice support all standard operators as well as an extensive library of functions.
-* Efficiently solves dice pool problems; depending on the problem, it can be more than 1000× as fast as multiset/sequence-based algorithms.
-* Supports multivariate distributions.
+* Dice support all standard operators (+, -, <, >, etc.) as well as an extensive library of functions (rerolling, exploding, etc.)
+* Can outperform sequence/multiset-based algorithms on many dice pool problems.
+    In some cases it may be thousands or millions of times faster.
 
 ## Installing
 
 ```
 pip install icepool
 ```
 
+The source is pure Python, so making a direct copy can work as well.
+
 ## Contact
 
 Feel free to open a [discussion](https://github.com/HighDiceRoller/icepool/discussions) or [issue](https://github.com/HighDiceRoller/icepool/issues) on GitHub. You can also find me on [Twitter](https://twitter.com/highdiceroller) or [Reddit](https://www.reddit.com/user/HighDiceRoller).
 
 ## API documentation
 
-[GitHub.](https://highdiceroller.github.io/icepool/apidoc/icepool.html)
+[pdoc on GitHub.](https://highdiceroller.github.io/icepool/apidoc/icepool.html)
 
 ## JupyterLite notebooks
 
 See this [JupyterLite distribution](https://highdiceroller.github.io/icepool/notebooks/lab/index.html) for a collection of interactive, editable examples. These include mechanics from published games, StackExchange, Reddit, and academic papers.
 
 ## Web applications
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `icepool-0.8.0/src/icepool.egg-info/SOURCES.txt` & `icepool-0.9.0/src/icepool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

