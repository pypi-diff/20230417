# Comparing `tmp/fractal-tokens-1.1.1.tar.gz` & `tmp/fractal-tokens-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal-tokens-1.1.1.tar", last modified: Fri Jan 20 10:12:23 2023, max compression
+gzip compressed data, was "fractal-tokens-1.2.0.tar", last modified: Mon Apr 17 12:32:25 2023, max compression
```

## Comparing `fractal-tokens-1.1.1.tar` & `fractal-tokens-1.2.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0      187 2023-01-20 10:12:08.321155 fractal-tokens-1.1.1/.coveragerc
--rw-r--r--   0        0        0      100 2023-01-20 10:12:08.321155 fractal-tokens-1.1.1/.flake8
--rw-r--r--   0        0        0      945 2023-01-20 10:12:08.321155 fractal-tokens-1.1.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-01-20 10:12:08.321155 fractal-tokens-1.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-01-20 10:12:08.321155 fractal-tokens-1.1.1/.gitignore
--rw-r--r--   0        0        0      161 2023-01-20 10:12:08.321155 fractal-tokens-1.1.1/.isort.cfg
--rw-r--r--   0        0        0     1708 2023-01-20 10:12:08.321155 fractal-tokens-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-01-20 10:12:08.321155 fractal-tokens-1.1.1/LICENSE
--rw-r--r--   0        0        0     1470 2023-01-20 10:12:08.321155 fractal-tokens-1.1.1/Makefile
--rw-r--r--   0        0        0    22752 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/README.md
--rw-r--r--   0        0        0      780 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/align_version.py
--rw-r--r--   0        0        0        0 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/asymmetric/__init__.py
--rw-r--r--   0        0        0      460 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/asymmetric/app.py
--rw-r--r--   0        0        0      589 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/asymmetric/utils.py
--rw-r--r--   0        0        0        0 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/automatic/__init__.py
--rw-r--r--   0        0        0     2077 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/automatic/app.py
--rw-r--r--   0        0        0      578 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/automatic/utils.py
--rw-r--r--   0        0        0        0 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/dummy/__init__.py
--rw-r--r--   0        0        0      507 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/dummy/app.py
--rw-r--r--   0        0        0        0 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/fastapi_demo/__init__.py
--rw-r--r--   0        0        0     1145 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/fastapi_demo/app.py
--rw-r--r--   0        0        0       33 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/fastapi_demo/requirements.txt
--rw-r--r--   0        0        0     1042 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/fastapi_demo/utils.py
--rw-r--r--   0        0        0        0 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/fastapi_roles_demo/__init__.py
--rw-r--r--   0        0        0     1419 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/fastapi_roles_demo/app.py
--rw-r--r--   0        0        0       47 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/fastapi_roles_demo/requirements.txt
--rw-r--r--   0        0        0     1634 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/fastapi_roles_demo/utils.py
--rw-r--r--   0        0        0        0 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/symmetric/__init__.py
--rw-r--r--   0        0        0      406 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/examples/symmetric/app.py
--rw-r--r--   0        0        0      132 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/fractal_tokens/__init__.py
--rw-r--r--   0        0        0      707 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/fractal_tokens/exceptions.py
--rw-r--r--   0        0        0        0 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/fractal_tokens/services/__init__.py
--rw-r--r--   0        0        0      898 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/fractal_tokens/services/dummy.py
--rw-r--r--   0        0        0     2907 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/fractal_tokens/services/generic.py
--rw-r--r--   0        0        0     1353 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/fractal_tokens/services/jwk.py
--rw-r--r--   0        0        0      782 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/fractal_tokens/services/jwt/__init__.py
--rw-r--r--   0        0        0     4037 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/fractal_tokens/services/jwt/asymmetric.py
--rw-r--r--   0        0        0     2582 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/fractal_tokens/services/jwt/automatic.py
--rw-r--r--   0        0        0     1008 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/fractal_tokens/services/jwt/symmetric.py
--rw-r--r--   0        0        0      113 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/fractal_tokens/settings.py
--rw-r--r--   0        0        0     1632 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       69 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/setup.py
--rw-r--r--   0        0        0        0 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/conftest.py
--rw-r--r--   0        0        0       89 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      152 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/fixtures/services/__init__.py
--rw-r--r--   0        0        0      162 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/fixtures/services/dummy.py
--rw-r--r--   0        0        0     1563 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/fixtures/services/jwk.py
--rw-r--r--   0        0        0      181 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/fixtures/services/jwt/__init__.py
--rw-r--r--   0        0        0     2269 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/fixtures/services/jwt/asymmetric.py
--rw-r--r--   0        0        0      655 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/fixtures/services/jwt/automatic.py
--rw-r--r--   0        0        0      253 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/fixtures/services/jwt/symmetric.py
--rw-r--r--   0        0        0       92 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/fixtures/utils.py
--rw-r--r--   0        0        0        0 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/services/__init__.py
--rw-r--r--   0        0        0        0 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/services/jwt/__init__.py
--rw-r--r--   0        0        0     2749 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/services/jwt/test_asymmetric.py
--rw-r--r--   0        0        0     2225 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/services/jwt/test_automatic.py
--rw-r--r--   0        0        0     1835 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/services/jwt/test_symmetric.py
--rw-r--r--   0        0        0      739 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/services/test_dummy.py
--rw-r--r--   0        0        0      719 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tests/services/test_jwk.py
--rw-r--r--   0        0        0      653 2023-01-20 10:12:08.325156 fractal-tokens-1.1.1/tox.ini
--rw-r--r--   0        0        0    23626 1970-01-01 00:00:00.000000 fractal-tokens-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/.coveragerc
+-rw-r--r--   0        0        0      100 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/.flake8
+-rw-r--r--   0        0        0      945 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/.gitignore
+-rw-r--r--   0        0        0      161 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/.isort.cfg
+-rw-r--r--   0        0        0     1708 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1470 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/Makefile
+-rw-r--r--   0        0        0    22752 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/README.md
+-rw-r--r--   0        0        0      780 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/align_version.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/asymmetric/__init__.py
+-rw-r--r--   0        0        0      460 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/asymmetric/app.py
+-rw-r--r--   0        0        0      589 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/asymmetric/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/automatic/__init__.py
+-rw-r--r--   0        0        0     2186 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/automatic/app.py
+-rw-r--r--   0        0        0      578 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/automatic/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/dummy/__init__.py
+-rw-r--r--   0        0        0      507 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/dummy/app.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_demo/__init__.py
+-rw-r--r--   0        0        0     1145 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_demo/app.py
+-rw-r--r--   0        0        0       33 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_demo/requirements.txt
+-rw-r--r--   0        0        0     1042 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_demo/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_roles_demo/__init__.py
+-rw-r--r--   0        0        0     1419 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_roles_demo/app.py
+-rw-r--r--   0        0        0       47 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_roles_demo/requirements.txt
+-rw-r--r--   0        0        0     1634 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_roles_demo/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/symmetric/__init__.py
+-rw-r--r--   0        0        0      406 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/symmetric/app.py
+-rw-r--r--   0        0        0      132 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/fractal_tokens/__init__.py
+-rw-r--r--   0        0        0      707 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/fractal_tokens/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/fractal_tokens/services/__init__.py
+-rw-r--r--   0        0        0      898 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/services/dummy.py
+-rw-r--r--   0        0        0     2907 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/services/generic.py
+-rw-r--r--   0        0        0     1471 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/services/jwk.py
+-rw-r--r--   0        0        0      782 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/services/jwt/__init__.py
+-rw-r--r--   0        0        0     4033 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/services/jwt/asymmetric.py
+-rw-r--r--   0        0        0     2582 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/services/jwt/automatic.py
+-rw-r--r--   0        0        0     1008 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/services/jwt/symmetric.py
+-rw-r--r--   0        0        0      113 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/settings.py
+-rw-r--r--   0        0        0     1632 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/setup.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/conftest.py
+-rw-r--r--   0        0        0       89 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      152 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/services/__init__.py
+-rw-r--r--   0        0        0      162 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/services/dummy.py
+-rw-r--r--   0        0        0     1676 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/services/jwk.py
+-rw-r--r--   0        0        0      181 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/services/jwt/__init__.py
+-rw-r--r--   0        0        0     2269 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/services/jwt/asymmetric.py
+-rw-r--r--   0        0        0      655 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/services/jwt/automatic.py
+-rw-r--r--   0        0        0      253 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/services/jwt/symmetric.py
+-rw-r--r--   0        0        0       92 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/services/jwt/__init__.py
+-rw-r--r--   0        0        0     2749 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/services/jwt/test_asymmetric.py
+-rw-r--r--   0        0        0     2225 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/services/jwt/test_automatic.py
+-rw-r--r--   0        0        0     1835 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/services/jwt/test_symmetric.py
+-rw-r--r--   0        0        0      739 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/services/test_dummy.py
+-rw-r--r--   0        0        0      719 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/services/test_jwk.py
+-rw-r--r--   0        0        0      653 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tox.ini
+-rw-r--r--   0        0        0    23626 1970-01-01 00:00:00.000000 fractal-tokens-1.2.0/PKG-INFO
```

### Comparing `fractal-tokens-1.1.1/.github/workflows/build.yml` & `fractal-tokens-1.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/.github/workflows/publish.yml` & `fractal-tokens-1.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/.gitignore` & `fractal-tokens-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/.pre-commit-config.yaml` & `fractal-tokens-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/LICENSE` & `fractal-tokens-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/Makefile` & `fractal-tokens-1.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/README.md` & `fractal-tokens-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/align_version.py` & `fractal-tokens-1.2.0/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/examples/asymmetric/utils.py` & `fractal-tokens-1.2.0/examples/asymmetric/utils.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/examples/automatic/app.py` & `fractal-tokens-1.2.0/examples/automatic/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import uuid
 
 from automatic.utils import rsa_key_pair
 from cryptography.hazmat.primitives import serialization
 
-from fractal_tokens.services.jwk import AutomaticJwkService, Jwk
+from fractal_tokens.services.jwk import AutomaticJwkService, Jwk, LocalJwkService
 from fractal_tokens.services.jwt.asymmetric import (
     AsymmetricJwtTokenService,
     ExtendedAsymmetricJwtTokenService,
 )
 from fractal_tokens.services.jwt.automatic import AutomaticJwtTokenService
 from fractal_tokens.services.jwt.symmetric import SymmetricJwtTokenService
 
 if __name__ == "__main__":
     private_key, public_key = rsa_key_pair()
     secret_key = "**SECRET**"
     kid = str(uuid.uuid4())
-    jwk_service = AutomaticJwkService(
+    local_jwk_service = LocalJwkService(
         jwks=[
             Jwk(
                 id=kid,
                 public_key=public_key.public_bytes(
                     serialization.Encoding.PEM,
                     serialization.PublicFormat.SubjectPublicKeyInfo,
                 ).decode("utf-8"),
             )
         ]
     )
+    jwk_service = AutomaticJwkService(
+        local_jwk_service=local_jwk_service,
+    )
 
     asymmetric_token_service = AsymmetricJwtTokenService(
         issuer="example", private_key=private_key, public_key=public_key
     )
     extended_asymmetric_token_service = ExtendedAsymmetricJwtTokenService(
         issuer="example",
         private_key=private_key,
```

### Comparing `fractal-tokens-1.1.1/examples/automatic/utils.py` & `fractal-tokens-1.2.0/examples/automatic/utils.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/examples/fastapi_demo/app.py` & `fractal-tokens-1.2.0/examples/fastapi_demo/app.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/examples/fastapi_demo/utils.py` & `fractal-tokens-1.2.0/examples/fastapi_demo/utils.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/examples/fastapi_roles_demo/app.py` & `fractal-tokens-1.2.0/examples/fastapi_roles_demo/app.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/examples/fastapi_roles_demo/utils.py` & `fractal-tokens-1.2.0/examples/fastapi_roles_demo/utils.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/fractal_tokens/exceptions.py` & `fractal-tokens-1.2.0/fractal_tokens/exceptions.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/fractal_tokens/services/dummy.py` & `fractal-tokens-1.2.0/fractal_tokens/services/dummy.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/fractal_tokens/services/generic.py` & `fractal-tokens-1.2.0/fractal_tokens/services/generic.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/fractal_tokens/services/jwk.py` & `fractal-tokens-1.2.0/fractal_tokens/services/jwk.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import List
+from typing import List, Optional
 
 
 @dataclass
 class Jwk:
     id: str
     public_key: str
 
@@ -13,16 +13,16 @@
 class JwkService(ABC):
     @abstractmethod
     def get_jwks(self, issuer: str = "") -> List[Jwk]:
         raise NotImplementedError
 
 
 class LocalJwkService(JwkService):
-    def __init__(self, jwks: List[Jwk]):
-        self.jwks = jwks
+    def __init__(self, jwks: Optional[List[Jwk]] = None):
+        self.jwks = jwks or []
 
     def get_jwks(self, issuer: str = "") -> List[Jwk]:
         return self.jwks
 
 
 class RemoteJwkService(JwkService):
     def __init__(self, endpoint: str = "/public/keys"):
@@ -34,16 +34,21 @@
         )
 
         jsonurl = urlopen(f"{issuer}{self.endpoint}")
         return [Jwk(**k) for k in json.loads(jsonurl.read())]
 
 
 class AutomaticJwkService(JwkService):
-    def __init__(self, jwks: List[Jwk], endpoint: str = "/public/keys"):
-        self.local_jwk_service = LocalJwkService(jwks)
-        self.remote_jwk_service = RemoteJwkService(endpoint)
+    def __init__(
+        self,
+        *,
+        local_jwk_service: JwkService = LocalJwkService(),
+        remote_jwk_service: JwkService = RemoteJwkService(),
+    ):
+        self.local_jwk_service = local_jwk_service
+        self.remote_jwk_service = remote_jwk_service
 
     def get_jwks(self, issuer: str = "") -> List[Jwk]:
         if issuer.startswith("http"):
             return self.remote_jwk_service.get_jwks(issuer)
         else:
             return self.local_jwk_service.get_jwks(issuer)
```

### Comparing `fractal-tokens-1.1.1/fractal_tokens/services/jwt/__init__.py` & `fractal-tokens-1.2.0/fractal_tokens/services/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/fractal_tokens/services/jwt/asymmetric.py` & `fractal-tokens-1.2.0/fractal_tokens/services/jwt/asymmetric.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
 from cryptography.hazmat.primitives import serialization
-from cryptography.hazmat.primitives.asymmetric.types import PUBLIC_KEY_TYPES
+from cryptography.hazmat.primitives.asymmetric.types import PublicKeyTypes
 from jose import jwt
 
 from fractal_tokens.exceptions import (
     NoPrivateKeyException,
     NoPublicKeyException,
     NotAllowedException,
 )
@@ -15,15 +15,15 @@
 
 
 class AsymmetricJwtTokenService(JwtTokenService):
     def __init__(
         self,
         issuer: str,
         private_key: str,
-        public_key: Optional[PUBLIC_KEY_TYPES] = None,
+        public_key: Optional[PublicKeyTypes] = None,
         options: Optional[dict] = None,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.issuer = issuer
         self.private_key = private_key
```

### Comparing `fractal-tokens-1.1.1/fractal_tokens/services/jwt/automatic.py` & `fractal-tokens-1.2.0/fractal_tokens/services/jwt/automatic.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/fractal_tokens/services/jwt/symmetric.py` & `fractal-tokens-1.2.0/fractal_tokens/services/jwt/symmetric.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/pyproject.toml` & `fractal-tokens-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-tokens"
-version = "1.1.1"
+version = "1.2.0"
 description = "Fractal Tokens provides a flexible way to generate and verify JWT tokens for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
```

### Comparing `fractal-tokens-1.1.1/tests/fixtures/services/jwk.py` & `fractal-tokens-1.2.0/tests/fixtures/services/jwk.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     )
 
 
 @pytest.fixture
 def empty_local_jwk_service():
     from fractal_tokens.services.jwk import LocalJwkService
 
-    yield LocalJwkService([])
+    yield LocalJwkService()
 
 
 @pytest.fixture
 def remote_jwk_service():
     from fractal_tokens.services.jwk import RemoteJwkService
 
     yield RemoteJwkService()
@@ -40,28 +40,32 @@
 
 @pytest.fixture
 def automatic_jwk_service(rsa_key_pair):
     kid, private_key, public_key = rsa_key_pair
 
     from cryptography.hazmat.primitives import serialization
 
-    from fractal_tokens.services.jwk import AutomaticJwkService
+    from fractal_tokens.services.jwk import AutomaticJwkService, LocalJwkService
 
-    yield AutomaticJwkService(
-        [
+    local_jwk_service = LocalJwkService(
+        jwks=[
             Jwk(
                 id=kid,
                 public_key=public_key.public_bytes(
                     serialization.Encoding.PEM,
                     serialization.PublicFormat.SubjectPublicKeyInfo,
                 ).decode("utf-8"),
             )
         ]
     )
 
+    yield AutomaticJwkService(
+        local_jwk_service=local_jwk_service,
+    )
+
 
 @pytest.fixture
 def mocked_urlopen():
     class HTTPResponse:
         def read(self):
             return "{}"
```

### Comparing `fractal-tokens-1.1.1/tests/fixtures/services/jwt/asymmetric.py` & `fractal-tokens-1.2.0/tests/fixtures/services/jwt/asymmetric.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/tests/fixtures/services/jwt/automatic.py` & `fractal-tokens-1.2.0/tests/fixtures/services/jwt/automatic.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/tests/services/jwt/test_asymmetric.py` & `fractal-tokens-1.2.0/tests/services/jwt/test_asymmetric.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/tests/services/jwt/test_automatic.py` & `fractal-tokens-1.2.0/tests/services/jwt/test_automatic.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/tests/services/jwt/test_symmetric.py` & `fractal-tokens-1.2.0/tests/services/jwt/test_symmetric.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/tests/services/test_dummy.py` & `fractal-tokens-1.2.0/tests/services/test_dummy.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/tests/services/test_jwk.py` & `fractal-tokens-1.2.0/tests/services/test_jwk.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/tox.ini` & `fractal-tokens-1.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.1.1/PKG-INFO` & `fractal-tokens-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-tokens
-Version: 1.1.1
+Version: 1.2.0
 Summary: Fractal Tokens provides a flexible way to generate and verify JWT tokens for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal-tokens
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

