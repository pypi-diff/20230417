# Comparing `tmp/tensortrax-0.8.5.tar.gz` & `tmp/tensortrax-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensortrax-0.8.5.tar", last modified: Mon Feb 13 22:18:36 2023, max compression
+gzip compressed data, was "tensortrax-0.9.0.tar", last modified: Wed Feb 15 22:31:34 2023, max compression
```

## Comparing `tensortrax-0.8.5.tar` & `tensortrax-0.9.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 22:18:36.782016 tensortrax-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35144 2023-02-13 22:18:27.000000 tensortrax-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    56921 2023-02-13 22:18:36.782016 tensortrax-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15182 2023-02-13 22:18:27.000000 tensortrax-0.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-02-13 22:18:27.000000 tensortrax-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 22:18:36.782016 tensortrax-0.8.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 22:18:36.778016 tensortrax-0.8.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 22:18:36.782016 tensortrax-0.8.5/src/tensortrax/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-13 22:18:27.000000 tensortrax-0.8.5/src/tensortrax/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-13 22:18:27.000000 tensortrax-0.8.5/src/tensortrax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10869 2023-02-13 22:18:27.000000 tensortrax-0.8.5/src/tensortrax/_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-02-13 22:18:27.000000 tensortrax-0.8.5/src/tensortrax/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17811 2023-02-13 22:18:27.000000 tensortrax-0.8.5/src/tensortrax/_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 22:18:36.782016 tensortrax-0.8.5/src/tensortrax/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-02-13 22:18:27.000000 tensortrax-0.8.5/src/tensortrax/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 22:18:36.782016 tensortrax-0.8.5/src/tensortrax/math/_linalg/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-13 22:18:27.000000 tensortrax-0.8.5/src/tensortrax/math/_linalg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-02-13 22:18:27.000000 tensortrax-0.8.5/src/tensortrax/math/_linalg/_linalg_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-02-13 22:18:27.000000 tensortrax-0.8.5/src/tensortrax/math/_linalg/_linalg_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-02-13 22:18:27.000000 tensortrax-0.8.5/src/tensortrax/math/_math_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-02-13 22:18:27.000000 tensortrax-0.8.5/src/tensortrax/math/_math_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 22:18:36.782016 tensortrax-0.8.5/src/tensortrax/math/_special/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-13 22:18:27.000000 tensortrax-0.8.5/src/tensortrax/math/_special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-02-13 22:18:27.000000 tensortrax-0.8.5/src/tensortrax/math/_special/_special_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 22:18:36.782016 tensortrax-0.8.5/src/tensortrax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    56921 2023-02-13 22:18:36.000000 tensortrax-0.8.5/src/tensortrax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-13 22:18:36.000000 tensortrax-0.8.5/src/tensortrax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 22:18:36.000000 tensortrax-0.8.5/src/tensortrax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-13 22:18:36.000000 tensortrax-0.8.5/src/tensortrax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-13 22:18:36.000000 tensortrax-0.8.5/src/tensortrax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 22:18:36.782016 tensortrax-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-02-13 22:18:27.000000 tensortrax-0.8.5/tests/test_hessian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-02-13 22:18:27.000000 tensortrax-0.8.5/tests/test_hessian_vector_product.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-02-13 22:18:27.000000 tensortrax-0.8.5/tests/test_jacobian.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-02-13 22:18:27.000000 tensortrax-0.8.5/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-02-13 22:18:27.000000 tensortrax-0.8.5/tests/test_mixed_partials.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-13 22:18:27.000000 tensortrax-0.8.5/tests/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-13 22:18:27.000000 tensortrax-0.8.5/tests/test_take.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:31:34.468262 tensortrax-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35144 2023-02-15 22:31:21.000000 tensortrax-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    56921 2023-02-15 22:31:34.468262 tensortrax-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15182 2023-02-15 22:31:21.000000 tensortrax-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-02-15 22:31:21.000000 tensortrax-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 22:31:34.468262 tensortrax-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:31:34.464262 tensortrax-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:31:34.464262 tensortrax-0.9.0/src/tensortrax/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-15 22:31:21.000000 tensortrax-0.9.0/src/tensortrax/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-15 22:31:21.000000 tensortrax-0.9.0/src/tensortrax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10869 2023-02-15 22:31:21.000000 tensortrax-0.9.0/src/tensortrax/_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-02-15 22:31:21.000000 tensortrax-0.9.0/src/tensortrax/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-02-15 22:31:21.000000 tensortrax-0.9.0/src/tensortrax/_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:31:34.464262 tensortrax-0.9.0/src/tensortrax/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-15 22:31:21.000000 tensortrax-0.9.0/src/tensortrax/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:31:34.464262 tensortrax-0.9.0/src/tensortrax/math/_linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-15 22:31:21.000000 tensortrax-0.9.0/src/tensortrax/math/_linalg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-02-15 22:31:21.000000 tensortrax-0.9.0/src/tensortrax/math/_linalg/_linalg_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-02-15 22:31:21.000000 tensortrax-0.9.0/src/tensortrax/math/_linalg/_linalg_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-02-15 22:31:21.000000 tensortrax-0.9.0/src/tensortrax/math/_math_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-02-15 22:31:21.000000 tensortrax-0.9.0/src/tensortrax/math/_math_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:31:34.464262 tensortrax-0.9.0/src/tensortrax/math/_special/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-15 22:31:21.000000 tensortrax-0.9.0/src/tensortrax/math/_special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-02-15 22:31:21.000000 tensortrax-0.9.0/src/tensortrax/math/_special/_special_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:31:34.464262 tensortrax-0.9.0/src/tensortrax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    56921 2023-02-15 22:31:34.000000 tensortrax-0.9.0/src/tensortrax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-02-15 22:31:34.000000 tensortrax-0.9.0/src/tensortrax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:31:34.000000 tensortrax-0.9.0/src/tensortrax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-15 22:31:34.000000 tensortrax-0.9.0/src/tensortrax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-15 22:31:34.000000 tensortrax-0.9.0/src/tensortrax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:31:34.468262 tensortrax-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-15 22:31:21.000000 tensortrax-0.9.0/tests/test_dual2real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-02-15 22:31:21.000000 tensortrax-0.9.0/tests/test_hessian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-02-15 22:31:21.000000 tensortrax-0.9.0/tests/test_hessian_vector_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-02-15 22:31:21.000000 tensortrax-0.9.0/tests/test_jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-02-15 22:31:21.000000 tensortrax-0.9.0/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-02-15 22:31:21.000000 tensortrax-0.9.0/tests/test_mixed_partials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-15 22:31:21.000000 tensortrax-0.9.0/tests/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-15 22:31:21.000000 tensortrax-0.9.0/tests/test_take.py
```

### Comparing `tensortrax-0.8.5/LICENSE` & `tensortrax-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/PKG-INFO` & `tensortrax-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensortrax
-Version: 0.8.5
+Version: 0.9.0
 Summary: Math on (Hyper-Dual) Tensors with Trailing Axes
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `tensortrax-0.8.5/README.md` & `tensortrax-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/pyproject.toml` & `tensortrax-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/src/tensortrax/_evaluate.py` & `tensortrax-0.9.0/src/tensortrax/_evaluate.py`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/src/tensortrax/_helpers.py` & `tensortrax-0.9.0/src/tensortrax/_helpers.py`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/src/tensortrax/_tensor.py` & `tensortrax-0.9.0/src/tensortrax/_tensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,51 +172,57 @@
     def __add__(self, B):
         A = self
         if isinstance(B, Tensor):
             x = f(A) + f(B)
             δx = δ(A) + δ(B)
             Δx = Δ(A) + Δ(B)
             Δδx = Δδ(A) + Δδ(B)
+            ntrax = min(A.ntrax, B.ntrax)
         else:
             x = f(A) + B
             δx = δ(A)
             Δx = Δ(A)
             Δδx = Δδ(A)
-        return Tensor(x=x, δx=δx, Δx=Δx, Δδx=Δδx, ntrax=A.ntrax)
+            ntrax = A.ntrax
+        return Tensor(x=x, δx=δx, Δx=Δx, Δδx=Δδx, ntrax=ntrax)
 
     def __sub__(self, B):
         A = self
         if isinstance(B, Tensor):
             x = f(A) - f(B)
             δx = δ(A) - δ(B)
             Δx = Δ(A) - Δ(B)
             Δδx = Δδ(A) - Δδ(B)
+            ntrax = min(A.ntrax, B.ntrax)
         else:
             x = f(A) - B
             δx = δ(A)
             Δx = Δ(A)
             Δδx = Δδ(A)
-        return Tensor(x=x, δx=δx, Δx=Δx, Δδx=Δδx, ntrax=A.ntrax)
+            ntrax = A.ntrax
+        return Tensor(x=x, δx=δx, Δx=Δx, Δδx=Δδx, ntrax=ntrax)
 
     def __rsub__(self, B):
         return -self.__sub__(B)
 
     def __mul__(self, B):
         A = self
         if isinstance(B, Tensor):
             x = f(A) * f(B)
             δx = δ(A) * f(B) + f(A) * δ(B)
             Δx = Δ(A) * f(B) + f(A) * Δ(B)
             Δδx = Δ(A) * δ(B) + δ(A) * Δ(B) + Δδ(A) * f(B) + f(A) * Δδ(B)
+            ntrax = min(A.ntrax, B.ntrax)
         else:
             x = f(A) * B
             δx = δ(A) * B
             Δx = Δ(A) * B
             Δδx = Δδ(A) * B
-        return Tensor(x=x, δx=δx, Δx=Δx, Δδx=Δδx, ntrax=A.ntrax)
+            ntrax = A.ntrax
+        return Tensor(x=x, δx=δx, Δx=Δx, Δδx=Δδx, ntrax=ntrax)
 
     def __truediv__(self, B):
         A = self
         return A * B**-1
 
     def __rtruediv__(self, B):
         A = self
@@ -299,14 +305,17 @@
 
     def reshape(self, *shape, order="C"):
         return reshape(self, newshape=shape, order=order)
 
     def squeeze(self, axis=None):
         return squeeze(self, axis=axis)
 
+    def dual2real(self, like):
+        return dual2real(self, like=like)
+
     __radd__ = __add__
     __rmul__ = __mul__
     __array_ufunc__ = None
 
 
 def broadcast_to(A, shape):
     "Broadcast Array or Tensor to a new shape."
@@ -321,14 +330,24 @@
             Δδx=_broadcast_to(Δδ(A)),
             ntrax=A.ntrax,
         )
     else:
         return _broadcast_to(A)
 
 
+def dual2real(A, like=None):
+    """Return a new Tensor with old-dual data as new-real values,
+    with `ntrax` derived by `like`."""
+
+    ndual = like.ndual - len(like.shape)
+    ntrax = A.ntrax - ndual
+
+    return Tensor(x=A.δx, δx=A.Δδx, Δx=A.Δδx, ndual=min(ndual, ntrax), ntrax=ntrax)
+
+
 def ravel(A, order="C"):
     if isinstance(A, Tensor):
         δtrax = δ(A).shape[len(A.shape) :]
         Δtrax = Δ(A).shape[len(A.shape) :]
         Δδtrax = Δδ(A).shape[len(A.shape) :]
         return Tensor(
             x=f(A).reshape(A.size, *A.trax, order=order),
@@ -399,15 +418,15 @@
             + _einsum(δ(A), Δ(B), f(C))
             + _einsum(Δ(A), δ(B), f(C))
             + _einsum(δ(A), f(B), Δ(C))
             + _einsum(Δ(A), f(B), δ(C))
             + _einsum(f(A), δ(B), Δ(C))
             + _einsum(f(A), Δ(B), δ(C))
         )
-        ntrax = A.ntrax
+        ntrax = min(A.ntrax, B.ntrax, C.ntrax)
     elif (
         isinstance(A, Tensor)
         and not isinstance(B, Tensor)
         and not isinstance(C, Tensor)
     ):
         x = _einsum(f(A), B, C)
         δx = _einsum(δ(A), B, C)
@@ -440,37 +459,37 @@
         Δx = _einsum(Δ(A), f(B), C) + _einsum(f(A), Δ(B), C)
         Δδx = (
             _einsum(Δδ(A), f(B), C)
             + _einsum(f(A), Δδ(B), C)
             + _einsum(δ(A), Δ(B), C)
             + _einsum(Δ(A), δ(B), C)
         )
-        ntrax = A.ntrax
+        ntrax = min(A.ntrax, B.ntrax)
     elif isinstance(A, Tensor) and not isinstance(B, Tensor) and isinstance(C, Tensor):
         x = _einsum(f(A), B, f(C))
         δx = _einsum(δ(A), B, f(C)) + _einsum(f(A), B, δ(C))
         Δx = _einsum(Δ(A), B, f(C)) + _einsum(f(A), B, Δ(C))
         Δδx = (
             _einsum(Δδ(A), B, f(C))
             + _einsum(f(A), B, Δδ(C))
             + _einsum(δ(A), B, Δ(C))
             + _einsum(Δ(A), B, δ(C))
         )
-        ntrax = A.ntrax
+        ntrax = min(A.ntrax, C.ntrax)
     elif not isinstance(A, Tensor) and isinstance(B, Tensor) and isinstance(C, Tensor):
         x = _einsum(A, f(B), f(C))
         δx = _einsum(A, δ(B), f(C)) + _einsum(A, f(B), δ(C))
         Δx = _einsum(A, Δ(B), f(C)) + _einsum(A, f(B), Δ(C))
         Δδx = (
             _einsum(A, Δδ(B), f(C))
             + _einsum(A, f(B), Δδ(C))
             + _einsum(A, δ(B), Δ(C))
             + _einsum(A, Δ(B), δ(C))
         )
-        ntrax = B.ntrax
+        ntrax = min(B.ntrax, C.ntrax)
     else:
         return _einsum(*operands)
 
     return Tensor(x=x, δx=δx, Δx=Δx, Δδx=Δδx, ntrax=ntrax)
 
 
 def einsum2(subscripts, *operands):
@@ -484,15 +503,15 @@
         Δx = _einsum(Δ(A), f(B)) + _einsum(f(A), Δ(B))
         Δδx = (
             _einsum(Δδ(A), f(B))
             + _einsum(f(A), Δδ(B))
             + _einsum(δ(A), Δ(B))
             + _einsum(Δ(A), δ(B))
         )
-        ntrax = A.ntrax
+        ntrax = min(A.ntrax, B.ntrax)
     elif isinstance(A, Tensor) and not isinstance(B, Tensor):
         x = _einsum(f(A), B)
         δx = _einsum(δ(A), B)
         Δx = _einsum(Δ(A), B)
         Δδx = _einsum(Δδ(A), B)
         ntrax = A.ntrax
     elif not isinstance(A, Tensor) and isinstance(B, Tensor):
```

### Comparing `tensortrax-0.8.5/src/tensortrax/math/__init__.py` & `tensortrax-0.9.0/src/tensortrax/math/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     abs,
     array,
     broadcast_to,
     cos,
     cosh,
     diagonal,
     dot,
+    dual2real,
     einsum,
     exp,
     hstack,
     log,
     log10,
     matmul,
     ravel,
```

### Comparing `tensortrax-0.8.5/src/tensortrax/math/_linalg/__init__.py` & `tensortrax-0.9.0/src/tensortrax/math/_linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/src/tensortrax/math/_linalg/_linalg_array.py` & `tensortrax-0.9.0/src/tensortrax/math/_linalg/_linalg_array.py`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/src/tensortrax/math/_linalg/_linalg_tensor.py` & `tensortrax-0.9.0/src/tensortrax/math/_linalg/_linalg_tensor.py`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/src/tensortrax/math/_math_array.py` & `tensortrax-0.9.0/src/tensortrax/math/_math_array.py`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/src/tensortrax/math/_math_tensor.py` & `tensortrax-0.9.0/src/tensortrax/math/_math_tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import numpy as np
 
 from .._tensor import (
     Tensor,
     Δ,
     Δδ,
     broadcast_to,
+    dual2real,
     einsum,
     f,
     matmul,
     ravel,
     reshape,
     squeeze,
     δ,
@@ -42,15 +43,15 @@
     elif isinstance(object, list) or isinstance(object, tuple):
         if isinstance(object[0], Tensor):
             return Tensor(
                 x=np.array([f(o) for o in object], dtype=dtype),
                 δx=np.array([δ(o) for o in object], dtype=dtype),
                 Δx=np.array([Δ(o) for o in object], dtype=dtype),
                 Δδx=np.array([Δδ(o) for o in object], dtype=dtype),
-                ntrax=object[0].ntrax,
+                ntrax=min([o.ntrax for o in object]),
             )
         else:
             return np.array(object, dtype=dtype)
     else:
         return np.array(object, dtype=dtype)
 
 
@@ -282,45 +283,45 @@
 
     if isinstance(tup[0], Tensor):
         return Tensor(
             x=np.hstack([f(A) for A in tup]),
             δx=np.hstack([δ(A) for A in tup]),
             Δx=np.hstack([Δ(A) for A in tup]),
             Δδx=np.hstack([Δδ(A) for A in tup]),
-            ntrax=tup[0].ntrax,
+            ntrax=min([A.ntrax for A in tup]),
         )
     else:
         return np.hstack(tup)
 
 
 def vstack(tup):
     "Stack arrays in sequence vertically (row wise)."
 
     if isinstance(tup[0], Tensor):
         return Tensor(
             x=np.vstack([f(A) for A in tup]),
             δx=np.vstack([δ(A) for A in tup]),
             Δx=np.vstack([Δ(A) for A in tup]),
             Δδx=np.vstack([Δδ(A) for A in tup]),
-            ntrax=tup[0].ntrax,
+            ntrax=min([A.ntrax for A in tup]),
         )
     else:
         return np.vstack(tup)
 
 
 def stack(arrays, axis=0):
     "Join a sequence of arrays along a new axis."
 
     if isinstance(arrays[0], Tensor):
         return Tensor(
             x=np.stack([f(A) for A in arrays], axis=axis),
             δx=np.stack([δ(A) for A in arrays], axis=axis),
             Δx=np.stack([Δ(A) for A in arrays], axis=axis),
             Δδx=np.stack([Δδ(A) for A in arrays], axis=axis),
-            ntrax=arrays[0].ntrax,
+            ntrax=min([A.ntrax for A in arrays]),
         )
     else:
         return np.stack(arrays, axis=0)
 
 
 def split(ary, indices_or_sections, axis=0):
     "Split an array into multiple sub-arrays as views into ary."
```

### Comparing `tensortrax-0.8.5/src/tensortrax/math/_special/__init__.py` & `tensortrax-0.9.0/src/tensortrax/math/_special/__init__.py`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/src/tensortrax/math/_special/_special_tensor.py` & `tensortrax-0.9.0/src/tensortrax/math/_special/_special_tensor.py`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/src/tensortrax.egg-info/PKG-INFO` & `tensortrax-0.9.0/src/tensortrax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensortrax
-Version: 0.8.5
+Version: 0.9.0
 Summary: Math on (Hyper-Dual) Tensors with Trailing Axes
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `tensortrax-0.8.5/src/tensortrax.egg-info/SOURCES.txt` & `tensortrax-0.9.0/src/tensortrax.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/tensortrax/math/_math_array.py
 src/tensortrax/math/_math_tensor.py
 src/tensortrax/math/_linalg/__init__.py
 src/tensortrax/math/_linalg/_linalg_array.py
 src/tensortrax/math/_linalg/_linalg_tensor.py
 src/tensortrax/math/_special/__init__.py
 src/tensortrax/math/_special/_special_tensor.py
+tests/test_dual2real.py
 tests/test_hessian.py
 tests/test_hessian_vector_product.py
 tests/test_jacobian.py
 tests/test_math.py
 tests/test_mixed_partials.py
 tests/test_scalar.py
 tests/test_take.py
```

### Comparing `tensortrax-0.8.5/tests/test_hessian.py` & `tensortrax-0.9.0/tests/test_hessian.py`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/tests/test_hessian_vector_product.py` & `tensortrax-0.9.0/tests/test_hessian_vector_product.py`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/tests/test_jacobian.py` & `tensortrax-0.9.0/tests/test_jacobian.py`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/tests/test_math.py` & `tensortrax-0.9.0/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/tests/test_mixed_partials.py` & `tensortrax-0.9.0/tests/test_mixed_partials.py`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/tests/test_scalar.py` & `tensortrax-0.9.0/tests/test_scalar.py`

 * *Files identical despite different names*

### Comparing `tensortrax-0.8.5/tests/test_take.py` & `tensortrax-0.9.0/tests/test_take.py`

 * *Files identical despite different names*

