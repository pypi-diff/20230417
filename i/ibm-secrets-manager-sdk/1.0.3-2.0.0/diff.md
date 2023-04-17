# Comparing `tmp/ibm-secrets-manager-sdk-1.0.3.tar.gz` & `tmp/ibm-secrets-manager-sdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm-secrets-manager-sdk-1.0.3.tar", last modified: Tue Feb  8 09:41:21 2022, max compression
+gzip compressed data, was "ibm-secrets-manager-sdk-2.0.0.tar", last modified: Mon Apr 17 18:22:43 2023, max compression
```

## Comparing `ibm-secrets-manager-sdk-1.0.3.tar` & `ibm-secrets-manager-sdk-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 09:41:21.646451 ibm-secrets-manager-sdk-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-02-08 09:41:11.000000 ibm-secrets-manager-sdk-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-02-08 09:41:11.000000 ibm-secrets-manager-sdk-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5822 2022-02-08 09:41:21.646451 ibm-secrets-manager-sdk-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4844 2022-02-08 09:41:11.000000 ibm-secrets-manager-sdk-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 09:41:21.646451 ibm-secrets-manager-sdk-1.0.3/ibm_secrets_manager_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-02-08 09:41:11.000000 ibm-secrets-manager-sdk-1.0.3/ibm_secrets_manager_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-02-08 09:41:11.000000 ibm-secrets-manager-sdk-1.0.3/ibm_secrets_manager_sdk/common.py
--rw-r--r--   0 runner    (1001) docker     (121)   411938 2022-02-08 09:41:11.000000 ibm-secrets-manager-sdk-1.0.3/ibm_secrets_manager_sdk/secrets_manager_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-02-08 09:41:11.000000 ibm-secrets-manager-sdk-1.0.3/ibm_secrets_manager_sdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 09:41:21.646451 ibm-secrets-manager-sdk-1.0.3/ibm_secrets_manager_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5822 2022-02-08 09:41:21.000000 ibm-secrets-manager-sdk-1.0.3/ibm_secrets_manager_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-02-08 09:41:21.000000 ibm-secrets-manager-sdk-1.0.3/ibm_secrets_manager_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-08 09:41:21.000000 ibm-secrets-manager-sdk-1.0.3/ibm_secrets_manager_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-02-08 09:41:21.000000 ibm-secrets-manager-sdk-1.0.3/ibm_secrets_manager_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-02-08 09:41:21.000000 ibm-secrets-manager-sdk-1.0.3/ibm_secrets_manager_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-08 09:41:21.000000 ibm-secrets-manager-sdk-1.0.3/ibm_secrets_manager_sdk.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-02-08 09:41:11.000000 ibm-secrets-manager-sdk-1.0.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-02-08 09:41:11.000000 ibm-secrets-manager-sdk-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-08 09:41:21.646451 ibm-secrets-manager-sdk-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3367 2022-02-08 09:41:11.000000 ibm-secrets-manager-sdk-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:22:43.713141 ibm-secrets-manager-sdk-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 18:22:34.000000 ibm-secrets-manager-sdk-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 18:22:34.000000 ibm-secrets-manager-sdk-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-04-17 18:22:43.713141 ibm-secrets-manager-sdk-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-04-17 18:22:34.000000 ibm-secrets-manager-sdk-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:22:43.713141 ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-17 18:22:34.000000 ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-17 18:22:34.000000 ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847137 2023-04-17 18:22:34.000000 ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk/secrets_manager_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1280844 2023-04-17 18:22:34.000000 ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk/secrets_manager_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-17 18:22:34.000000 ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:22:43.713141 ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-04-17 18:22:43.000000 ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-17 18:22:43.000000 ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:22:43.000000 ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 18:22:43.000000 ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 18:22:43.000000 ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:22:43.000000 ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-17 18:22:34.000000 ibm-secrets-manager-sdk-2.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 18:22:34.000000 ibm-secrets-manager-sdk-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:22:43.713141 ibm-secrets-manager-sdk-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-17 18:22:34.000000 ibm-secrets-manager-sdk-2.0.0/setup.py
```

### Comparing `ibm-secrets-manager-sdk-1.0.3/LICENSE` & `ibm-secrets-manager-sdk-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-secrets-manager-sdk-1.0.3/README.md` & `ibm-secrets-manager-sdk-2.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 </details>
 
 ## Overview
 
 The IBM Cloud Secrets Manager Python SDK allows developers to programmatically interact with the following IBM Cloud
 services:
 
-Service name | Imported class name
---- | ---
-[Secrets Manager](https://cloud.ibm.com/apidocs/secrets-manager) | SecretsManagerV1
+| Service name                                                     | Imported class name  |
+|------------------------------------------------------------------|----------------------|
+| [Secrets Manager](https://cloud.ibm.com/apidocs/secrets-manager) | SecretsManagerV1     |
 
 ## Prerequisites
 
 - An [IBM Cloud account](https://cloud.ibm.com/registration).
 - A [Secrets Manager service instance](https://cloud.ibm.com/catalog/services/secrets-manager).
 - An [IBM Cloud API key](https://cloud.ibm.com/iam/apikeys) that allows the SDK to access your account.
-- Python 3.5.3 or above.
+- Python 3.9 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
 pip install --upgrade "ibm-secrets-manager-sdk"
@@ -141,8 +141,10 @@
 
 ## Contributing
 
 For general contribution guidelines, see [CONTRIBUTING](CONTRIBUTING.md).
 
 ## License
 
-This SDK project is released under the Apache 2.0 license. The license's full text can be found in [LICENSE](LICENSE).
+This SDK project is released under the Apache 2.0 license. The license's full text can be found in [LICENSE](LICENSE). 
+
+dummy_PR #2
```

### Comparing `ibm-secrets-manager-sdk-1.0.3/ibm_secrets_manager_sdk/__init__.py` & `ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-secrets-manager-sdk-1.0.3/ibm_secrets_manager_sdk/common.py` & `ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk/common.py`

 * *Files identical despite different names*

### Comparing `ibm-secrets-manager-sdk-1.0.3/ibm_secrets_manager_sdk/version.py` & `ibm-secrets-manager-sdk-2.0.0/ibm_secrets_manager_sdk/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Version of ibm_secrets_manager_sdk
 """
-__version__ = '1.0.3'
+__version__ = '2.0.0'
```

### Comparing `ibm-secrets-manager-sdk-1.0.3/setup.py` & `ibm-secrets-manager-sdk-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '1.0.3'
+__version__ = '2.0.0'
 PACKAGE_NAME = 'ibm_secrets_manager_sdk'
 PACKAGE_DESC = 'IBM Cloud Secrets Manager Python SDK'
 
 with open('requirements.txt') as f:
     install_requires = [str(req) for req in pkg_resources.parse_requirements(f)]
 with open('requirements-dev.txt') as f:
     tests_require = [str(req) for req in pkg_resources.parse_requirements(f)]
```

