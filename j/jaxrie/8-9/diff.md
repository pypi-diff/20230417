# Comparing `tmp/jaxrie-8.tar.gz` & `tmp/jaxrie-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrie-8.tar", last modified: Thu Apr 13 18:34:57 2023, max compression
+gzip compressed data, was "jaxrie-9.tar", last modified: Sun Apr 16 04:46:30 2023, max compression
```

## Comparing `jaxrie-8.tar` & `jaxrie-9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      114 2023-04-11 06:28:18.666689 jaxrie-8/README.md
--rw-r--r--   0        0        0     3959 2023-04-13 18:34:57.659852 jaxrie-8/pyproject.toml
--rw-r--r--   0        0        0      321 2023-04-13 02:05:54.392649 jaxrie-8/src/jaxrie/__init__.py
--rw-r--r--   0        0        0       18 2023-04-13 18:34:34.058886 jaxrie-8/src/jaxrie/__version__.py
--rw-r--r--   0        0        0      274 2023-04-12 22:32:25.869284 jaxrie-8/src/jaxrie/manifold/__init__.py
--rw-r--r--   0        0        0     4120 2023-04-13 02:10:13.893763 jaxrie-8/src/jaxrie/manifold/base.py
--rw-r--r--   0        0        0     4567 2023-04-13 18:30:08.539578 jaxrie-8/src/jaxrie/manifold/euclidean.py
--rw-r--r--   0        0        0     1434 2023-04-13 18:31:44.775171 jaxrie-8/src/jaxrie/manifold/lorentz.py
--rw-r--r--   0        0        0    21849 2023-04-13 18:31:44.712690 jaxrie-8/src/jaxrie/manifold/math.py
--rw-r--r--   0        0        0     5122 2023-04-13 18:30:08.411332 jaxrie-8/src/jaxrie/manifold/stereographic.py
--rw-r--r--   0        0        0       93 2023-04-11 06:05:54.838637 jaxrie-8/src/jaxrie/modules/__init__.py
--rw-r--r--   0        0        0     4753 2023-04-13 17:54:44.533901 jaxrie-8/src/jaxrie/modules/basic.py
--rw-r--r--   0        0        0        0 2023-04-11 05:52:43.064397 jaxrie-8/src/jaxrie/nets/__init__.py
--rw-r--r--   0        0        0     2282 2023-04-12 22:18:13.252978 jaxrie-8/src/jaxrie/nets/basic.py
--rw-r--r--   0        0        0        0 2023-04-11 06:36:46.927134 jaxrie-8/src/jaxrie/py.typed
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 jaxrie-8/PKG-INFO
+-rw-r--r--   0        0        0      114 2023-04-11 06:28:18.666689 jaxrie-9/README.md
+-rw-r--r--   0        0        0     3959 2023-04-16 04:46:30.507992 jaxrie-9/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-04-16 04:42:20.234479 jaxrie-9/src/jaxrie/__init__.py
+-rw-r--r--   0        0        0       18 2023-04-16 04:45:53.592976 jaxrie-9/src/jaxrie/__version__.py
+-rw-r--r--   0        0        0      274 2023-04-12 22:32:25.869284 jaxrie-9/src/jaxrie/manifold/__init__.py
+-rw-r--r--   0        0        0     4248 2023-04-16 04:42:20.245070 jaxrie-9/src/jaxrie/manifold/base.py
+-rw-r--r--   0        0        0     4619 2023-04-16 04:42:20.246000 jaxrie-9/src/jaxrie/manifold/euclidean.py
+-rw-r--r--   0        0        0     1470 2023-04-16 04:42:20.240027 jaxrie-9/src/jaxrie/manifold/lorentz.py
+-rw-r--r--   0        0        0    21849 2023-04-13 18:31:44.712690 jaxrie-9/src/jaxrie/manifold/math.py
+-rw-r--r--   0        0        0     5130 2023-04-16 04:42:20.244140 jaxrie-9/src/jaxrie/manifold/stereographic.py
+-rw-r--r--   0        0        0      101 2023-04-16 04:42:20.247366 jaxrie-9/src/jaxrie/modules/__init__.py
+-rw-r--r--   0        0        0     4782 2023-04-16 04:43:26.933236 jaxrie-9/src/jaxrie/modules/basic.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:52:43.064397 jaxrie-9/src/jaxrie/nets/__init__.py
+-rw-r--r--   0        0        0     2282 2023-04-12 22:18:13.252978 jaxrie-9/src/jaxrie/nets/basic.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:36:46.927134 jaxrie-9/src/jaxrie/py.typed
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 jaxrie-9/PKG-INFO
```

### Comparing `jaxrie-8/pyproject.toml` & `jaxrie-9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
     "jaxlib>=0.4.6",
     "dm-haiku>=0.0.9",
     "optax>=0.1.4",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 dynamic = []
-version = "8"
+version = "9"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `jaxrie-8/src/jaxrie/manifold/base.py` & `jaxrie-9/src/jaxrie/manifold/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,23 +30,31 @@
 email    : Nasy <nasyxx+python@gmail.com>
 filename : base.py
 project  : jaxrie
 license  : MIT
 
 Manifold base.
 """
-import jax
+# Standard Library
+from abc import ABCMeta, abstractmethod
+
+# Types
 from jax.typing import ArrayLike
-from abc import abstractmethod, ABCMeta
+from typing import TypeVar
+
+# JAX
+import jax
+
+# Local
 from .math import EPS
 
 Array = jax.Array
 
 
-class Manifold(metaclass=ABCMeta):
+class BaseManifold(metaclass=ABCMeta):
   """Manifold base."""
 
   @property
   def name(self) -> str:
     """Name of the manifold."""
     return self.__class__.__name__
 
@@ -129,7 +137,10 @@
     raise NotImplementedError
 
   @staticmethod
   @abstractmethod
   def proj(x: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Projection on manifold with curvature k."""
     raise NotImplementedError
+
+
+Manifold = TypeVar("Manifold", bound=BaseManifold)
```

### Comparing `jaxrie-8/src/jaxrie/manifold/euclidean.py` & `jaxrie-9/src/jaxrie/manifold/euclidean.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,23 +30,30 @@
 email    : Nasy <nasyxx+python@gmail.com>
 filename : euclidean.py
 project  : jaxrie
 license  : GPL-3.0+
 
 This is the module for the Euclidean manifold.
 """
-from .base import Manifold, EPS
-import jax
-from jax.typing import ArrayLike
+# Standard Library
 from functools import partial
 
+# Types
+from jax.typing import ArrayLike
+
+# JAX
+import jax
+
+# Local
+from .base import EPS, BaseManifold
+
 Array = jax.Array
 
 
-class Euclidean(Manifold):
+class Euclidean(BaseManifold):
   """The universal Stereographic projection model."""
 
   @staticmethod
   @partial(jax.jit, static_argnames=("eps",))
   def add(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius addition on manifold with curvature k."""
     del k, eps
```

### Comparing `jaxrie-8/src/jaxrie/manifold/lorentz.py` & `jaxrie-9/src/jaxrie/manifold/lorentz.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,24 +31,31 @@
 filename : lorentz.py
 project  : jaxrie
 license  : GPL-3.0+
 
 Lorentz model.
 """
 
-from .base import Manifold
+# Standard Library
+from functools import partial
+
+# Types
+from jax.typing import ArrayLike
+
+# JAX
 import jax
 import jax.numpy as jnp
-from jax.typing import ArrayLike
-from functools import partial
+
+# Local
+from .base import BaseManifold
 
 Array = jax.Array
 
 
-class Lorentz(Manifold):
-    """Lorentz model."""
+class Lorentz(BaseManifold):
+  """Lorentz model."""
 
-    @staticmethod
-    @jax.jit
-    def add(x: Array, y: Array, k: ArrayLike) -> Array:
-        """Addition on manifold with curvature k."""
-        pass
+  @staticmethod
+  @jax.jit
+  def add(x: Array, y: Array, k: ArrayLike) -> Array:
+    """Addition on manifold with curvature k."""
+    pass
```

### Comparing `jaxrie-8/src/jaxrie/manifold/math.py` & `jaxrie-9/src/jaxrie/manifold/math.py`

 * *Files identical despite different names*

### Comparing `jaxrie-8/src/jaxrie/manifold/stereographic.py` & `jaxrie-9/src/jaxrie/manifold/stereographic.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,24 +43,24 @@
 # Types
 from jax.typing import ArrayLike
 
 # JAX
 import jax
 
 # Local
-from .base import Manifold
-from .math import (EPS, mobius_add, mobius_adde, mobius_matmulh, mobius_matmull,
-                   mobius_matmulr, mobius_matvec_mul, mobius_scala_mul,
-                   stereo_egrad2rgrad, stereo_expmap, stereo_expmap0,
-                   stereo_logmap, stereo_logmap0, stereo_proj)
+from .base import BaseManifold
+from .math import (EPS, mobius_add, mobius_adde, mobius_matmulh,
+                   mobius_matmull, mobius_matmulr, mobius_matvec_mul,
+                   mobius_scala_mul, stereo_egrad2rgrad, stereo_expmap,
+                   stereo_expmap0, stereo_logmap, stereo_logmap0, stereo_proj)
 
 Array = jax.Array
 
 
-class Stereographic(Manifold):
+class Stereographic(BaseManifold):
   """The universal Stereographic projection model."""
 
   @staticmethod
   @partial(jax.jit, static_argnames=("eps",))
   def add(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius addition on manifold with curvature k."""
     return mobius_add(x, y, k, eps)
```

### Comparing `jaxrie-8/src/jaxrie/modules/basic.py` & `jaxrie-9/src/jaxrie/modules/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,18 @@
 filename : basic.py
 project  : jaxrie
 license  : GPL-3.0+
 
 Basic
 """
 
+# Standard Library
+from collections.abc import Callable
+
 # Types
-from typing import Callable
 from jax.typing import ArrayLike
 
 # JAX
 import haiku as hk
 import jax
 import jax.numpy as jnp
```

### Comparing `jaxrie-8/src/jaxrie/nets/basic.py` & `jaxrie-9/src/jaxrie/nets/basic.py`

 * *Files identical despite different names*

