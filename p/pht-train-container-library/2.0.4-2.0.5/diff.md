# Comparing `tmp/pht_train_container_library-2.0.4.tar.gz` & `tmp/pht_train_container_library-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pht_train_container_library-2.0.4.tar", max compression
+gzip compressed data, was "pht_train_container_library-2.0.5.tar", max compression
```

## Comparing `pht_train_container_library-2.0.4.tar` & `pht_train_container_library-2.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1068 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/LICENSE.txt
--rw-r--r--   0        0        0     5852 2023-03-07 12:16:53.453164 pht_train_container_library-2.0.4/README.md
--rw-r--r--   0        0        0     1848 2023-04-12 13:19:41.590587 pht_train_container_library-2.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/__init__.py
--rw-r--r--   0        0        0       32 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/clients/__init__.py
--rw-r--r--   0        0        0      107 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/clients/fhir/__init__.py
--rw-r--r--   0        0        0    19926 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/clients/fhir/fhir_client.py
--rw-r--r--   0        0        0     2509 2023-03-07 12:14:19.038419 pht_train_container_library-2.0.4/train_lib/clients/fhir/fhir_k_anonymity.py
--rw-r--r--   0        0        0     3788 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/clients/fhir/fhir_query_builder.py
--rw-r--r--   0        0        0      297 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/clients/fhir/minimal_query.json
--rw-r--r--   0        0        0      758 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/clients/fhir/query.json
--rw-r--r--   0        0        0       14 2023-04-12 10:34:43.891083 pht_train_container_library-2.0.4/train_lib/docker_util/__init__.py
--rw-r--r--   0        0        0     6596 2023-04-12 12:11:47.347039 pht_train_container_library-2.0.4/train_lib/docker_util/docker_ops.py
--rw-r--r--   0        0        0     6219 2023-03-30 14:41:16.691214 pht_train_container_library-2.0.4/train_lib/docker_util/validate_master_image.py
--rw-r--r--   0        0        0        1 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/security/__init__.py
--rw-r--r--   0        0        0      257 2023-04-12 13:21:36.885381 pht_train_container_library-2.0.4/train_lib/security/constants.py
--rw-r--r--   0        0        0     4436 2023-03-07 12:17:00.953436 pht_train_container_library-2.0.4/train_lib/security/encryption.py
--rw-r--r--   0        0        0      248 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/security/errors.py
--rw-r--r--   0        0        0     2543 2023-03-07 12:16:53.463164 pht_train_container_library-2.0.4/train_lib/security/hashing.py
--rw-r--r--   0        0        0     1483 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/security/homomorphic_addition.py
--rw-r--r--   0        0        0     6336 2023-03-07 12:16:53.463164 pht_train_container_library-2.0.4/train_lib/security/key_manager.py
--rw-r--r--   0        0        0     1772 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/security/primes.py
--rw-r--r--   0        0        0    32244 2023-04-12 12:11:47.497039 pht_train_container_library-2.0.4/train_lib/security/protocol.py
--rw-r--r--   0        0        0     2628 2023-03-07 12:41:46.414956 pht_train_container_library-2.0.4/train_lib/security/train_config.py
--rw-r--r--   0        0        0    11507 2023-03-30 14:41:16.301214 pht_train_container_library-2.0.4/train_lib/tests/conftest.py
--rw-r--r--   0        0        0    10607 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/tests/test_fhir_functionality.py
--rw-r--r--   0        0        0     2425 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/tests/test_homomorphic_addition.py
--rw-r--r--   0        0        0      116 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/tests/test_key_manager.py
--rw-r--r--   0        0        0     5127 2023-03-07 12:17:04.923592 pht_train_container_library-2.0.4/train_lib/tests/test_security_functions.py
--rw-r--r--   0        0        0    23503 2023-03-07 12:17:05.793630 pht_train_container_library-2.0.4/train_lib/tests/test_security_protocol.py
--rw-r--r--   0        0        0     7602 2023-03-27 15:40:16.372314 pht_train_container_library-2.0.4/train_lib/tests/test_validate_master_image.py
--rw-r--r--   0        0        0     6575 1970-01-01 00:00:00.000000 pht_train_container_library-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     5852 2023-03-07 12:16:53.453164 pht_train_container_library-2.0.5/README.md
+-rw-r--r--   0        0        0     1848 2023-04-17 18:07:22.070677 pht_train_container_library-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/__init__.py
+-rw-r--r--   0        0        0       32 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/clients/__init__.py
+-rw-r--r--   0        0        0      107 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/clients/fhir/__init__.py
+-rw-r--r--   0        0        0    19926 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/clients/fhir/fhir_client.py
+-rw-r--r--   0        0        0     2509 2023-03-07 12:14:19.038419 pht_train_container_library-2.0.5/train_lib/clients/fhir/fhir_k_anonymity.py
+-rw-r--r--   0        0        0     3788 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/clients/fhir/fhir_query_builder.py
+-rw-r--r--   0        0        0      297 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/clients/fhir/minimal_query.json
+-rw-r--r--   0        0        0      758 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/clients/fhir/query.json
+-rw-r--r--   0        0        0       14 2023-04-12 10:34:43.891083 pht_train_container_library-2.0.5/train_lib/docker_util/__init__.py
+-rw-r--r--   0        0        0     6213 2023-04-17 18:05:04.947429 pht_train_container_library-2.0.5/train_lib/docker_util/docker_ops.py
+-rw-r--r--   0        0        0     6219 2023-03-30 14:41:16.691214 pht_train_container_library-2.0.5/train_lib/docker_util/validate_master_image.py
+-rw-r--r--   0        0        0        1 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/security/__init__.py
+-rw-r--r--   0        0        0      257 2023-04-12 13:21:36.885381 pht_train_container_library-2.0.5/train_lib/security/constants.py
+-rw-r--r--   0        0        0     4436 2023-03-07 12:17:00.953436 pht_train_container_library-2.0.5/train_lib/security/encryption.py
+-rw-r--r--   0        0        0      248 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/security/errors.py
+-rw-r--r--   0        0        0     2543 2023-03-07 12:16:53.463164 pht_train_container_library-2.0.5/train_lib/security/hashing.py
+-rw-r--r--   0        0        0     1483 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/security/homomorphic_addition.py
+-rw-r--r--   0        0        0     6336 2023-03-07 12:16:53.463164 pht_train_container_library-2.0.5/train_lib/security/key_manager.py
+-rw-r--r--   0        0        0     1772 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/security/primes.py
+-rw-r--r--   0        0        0    32244 2023-04-12 12:11:47.497039 pht_train_container_library-2.0.5/train_lib/security/protocol.py
+-rw-r--r--   0        0        0     2628 2023-03-07 12:41:46.414956 pht_train_container_library-2.0.5/train_lib/security/train_config.py
+-rw-r--r--   0        0        0    11507 2023-03-30 14:41:16.301214 pht_train_container_library-2.0.5/train_lib/tests/conftest.py
+-rw-r--r--   0        0        0    10607 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/tests/test_fhir_functionality.py
+-rw-r--r--   0        0        0     2425 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/tests/test_homomorphic_addition.py
+-rw-r--r--   0        0        0      116 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.5/train_lib/tests/test_key_manager.py
+-rw-r--r--   0        0        0     5127 2023-03-07 12:17:04.923592 pht_train_container_library-2.0.5/train_lib/tests/test_security_functions.py
+-rw-r--r--   0        0        0    23503 2023-03-07 12:17:05.793630 pht_train_container_library-2.0.5/train_lib/tests/test_security_protocol.py
+-rw-r--r--   0        0        0     7602 2023-03-27 15:40:16.372314 pht_train_container_library-2.0.5/train_lib/tests/test_validate_master_image.py
+-rw-r--r--   0        0        0     6575 1970-01-01 00:00:00.000000 pht_train_container_library-2.0.5/PKG-INFO
```

### Comparing `pht_train_container_library-2.0.4/LICENSE.txt` & `pht_train_container_library-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/README.md` & `pht_train_container_library-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/pyproject.toml` & `pht_train_container_library-2.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pht-train-container-library"
-version = "2.0.4"
+version = "2.0.5"
 description = "Python library for handling containerized PHT trains"
 authors = ["Michael Graf <michael.graf@uni-tuebingen.com>"]
 readme = "README.md"
 packages = [{include = "train_lib"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pht_train_container_library-2.0.4/train_lib/clients/fhir/fhir_client.py` & `pht_train_container_library-2.0.5/train_lib/clients/fhir/fhir_client.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/clients/fhir/fhir_k_anonymity.py` & `pht_train_container_library-2.0.5/train_lib/clients/fhir/fhir_k_anonymity.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/clients/fhir/fhir_query_builder.py` & `pht_train_container_library-2.0.5/train_lib/clients/fhir/fhir_query_builder.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/clients/fhir/query.json` & `pht_train_container_library-2.0.5/train_lib/clients/fhir/query.json`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/docker_util/docker_ops.py` & `pht_train_container_library-2.0.5/train_lib/docker_util/docker_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import tarfile
 from io import BytesIO
 
 from loguru import logger
 
 import docker
-from docker.models.containers import Container
 from train_lib.docker_util import TIMEOUT
 from train_lib.security.constants import TrainTags
 from train_lib.security.train_config import TrainConfig
 
 
 def extract_train_config(img: str, config_path: str = "/opt/train_config.json"):
     """
@@ -148,31 +147,24 @@
     """
     Rebase the given image on the given base image
 
     :param base_image: the base image to rebase the new image on
     :param latest_image: the image to rebase
     """
     client = docker.from_env(timeout=TIMEOUT)
+    
+    
     latest_container = client.containers.create(train_image)
     base_container = client.containers.create(base_image)
 
-    def _copy(src: Container, dest: Container, path: str):
-        """
-        Copy the given file from the src container to the dest container
-
-        :param src: the source container
-        :param dest: the destination container
-        """
-        src_archive, stat = src.get_archive(path)
-        src.wait()
-        dest.put_archive(path, src_archive)
-        dest.wait()
 
-    # copy the archives from the PHT directories and commit the base image with under the latest tag
-    _copy(latest_container, base_container, "/opt")
+    src_archive, state = latest_container.get_archive("/opt")
+    logger.debug(f"Rebase copy state: {state}")
+    base_container.put_archive("/", src_archive)
+    base_container.wait()
 
     repo = repository_from_image(train_image)
     base_container.commit(repository=repo, tag=TrainTags.LATEST.value)
     base_container.wait()
 
     # remove the containers
     latest_container.remove()
```

### Comparing `pht_train_container_library-2.0.4/train_lib/docker_util/validate_master_image.py` & `pht_train_container_library-2.0.5/train_lib/docker_util/validate_master_image.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/security/encryption.py` & `pht_train_container_library-2.0.5/train_lib/security/encryption.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/security/hashing.py` & `pht_train_container_library-2.0.5/train_lib/security/hashing.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/security/homomorphic_addition.py` & `pht_train_container_library-2.0.5/train_lib/security/homomorphic_addition.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/security/key_manager.py` & `pht_train_container_library-2.0.5/train_lib/security/key_manager.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/security/primes.py` & `pht_train_container_library-2.0.5/train_lib/security/primes.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/security/protocol.py` & `pht_train_container_library-2.0.5/train_lib/security/protocol.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/security/train_config.py` & `pht_train_container_library-2.0.5/train_lib/security/train_config.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/tests/conftest.py` & `pht_train_container_library-2.0.5/train_lib/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/tests/test_fhir_functionality.py` & `pht_train_container_library-2.0.5/train_lib/tests/test_fhir_functionality.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/tests/test_homomorphic_addition.py` & `pht_train_container_library-2.0.5/train_lib/tests/test_homomorphic_addition.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/tests/test_security_functions.py` & `pht_train_container_library-2.0.5/train_lib/tests/test_security_functions.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/tests/test_security_protocol.py` & `pht_train_container_library-2.0.5/train_lib/tests/test_security_protocol.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/train_lib/tests/test_validate_master_image.py` & `pht_train_container_library-2.0.5/train_lib/tests/test_validate_master_image.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.4/PKG-INFO` & `pht_train_container_library-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pht-train-container-library
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python library for handling containerized PHT trains
 Author: Michael Graf
 Author-email: michael.graf@uni-tuebingen.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

