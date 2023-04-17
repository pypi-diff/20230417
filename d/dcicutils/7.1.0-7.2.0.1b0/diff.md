# Comparing `tmp/dcicutils-7.1.0.tar.gz` & `tmp/dcicutils-7.2.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.1.0.tar", max compression
+gzip compressed data, was "dcicutils-7.2.0.1b0.tar", max compression
```

## Comparing `dcicutils-7.1.0.tar` & `dcicutils-7.2.0.1b0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0     1166 2023-04-13 15:16:36.923706 dcicutils-7.1.0/README.rst
--rw-r--r--   0        0        0        0 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/base.py
--rwxr-xr-x   0        0        0    52659 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    13639 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/command_utils.py
--rw-r--r--   0        0        0     1649 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46318 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9257 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/exceptions.py
--rw-r--r--   0        0        0    37025 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    11502 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/log_utils.py
--rw-r--r--   0        0        0    87196 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    20232 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   120743 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28713 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    19745 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     1769 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3654 2023-04-13 15:16:36.927705 dcicutils-7.1.0/pyproject.toml
--rw-r--r--   0        0        0     2916 1970-01-01 00:00:00.000000 dcicutils-7.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1166 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/README.rst
+-rw-r--r--   0        0        0        0 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/base.py
+-rwxr-xr-x   0        0        0    52659 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    13639 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     1649 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46730 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9257 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    37025 2023-04-17 11:36:35.353539 dcicutils-7.2.0.1b0/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    11502 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    87196 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20232 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   120743 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28713 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    19745 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9633 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     1769 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3680 2023-04-17 11:36:35.357540 dcicutils-7.2.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 dcicutils-7.2.0.1b0/PKG-INFO
```

### Comparing `dcicutils-7.1.0/README.rst` & `dcicutils-7.2.0.1b0/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/base.py` & `dcicutils-7.2.0.1b0/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/beanstalk_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/cloudformation_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/codebuild_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/command_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/common.py` & `dcicutils-7.2.0.1b0/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/creds_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/data_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/deployment_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/diff_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/docker_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/ecr_scripts.py` & `dcicutils-7.2.0.1b0/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/ecr_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/ecs_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/env_base.py` & `dcicutils-7.2.0.1b0/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/env_manager.py` & `dcicutils-7.2.0.1b0/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/env_scripts.py` & `dcicutils-7.2.0.1b0/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/env_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/env_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -686,14 +686,24 @@
     entry = (find_association(EnvUtils.PUBLIC_URL_TABLE, **{p.NAME: envname}) or
              find_association(EnvUtils.PUBLIC_URL_TABLE, **{p.ENVIRONMENT: full_env_name(envname)}) or
              find_association(EnvUtils.PUBLIC_URL_TABLE, **{p.ENVIRONMENT: short_env_name(envname)}))
     if entry:
         return entry
 
 
+def get_portal_url(envname: EnvName) -> UrlString:
+    """
+    Returns the Portal URL for the given environment name.
+    Effectively same ase get_env_real_url (below) but does not actually access
+    the URL (to get the health page is that function does); i.e. so we can get
+    the URL without exception even if there is a problem with the Portal.
+    """
+    return get_env_real_url(full_env_name(envname))
+
+
 @if_orchestrated
 def get_env_real_url(envname: EnvName) -> UrlString:
 
     entry = _find_public_url_entry(envname)
     if entry:
         return entry.get('url')
```

### Comparing `dcicutils-7.1.0/dcicutils/env_utils_legacy.py` & `dcicutils-7.2.0.1b0/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/es_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/exceptions.py` & `dcicutils-7.2.0.1b0/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/ff_mocks.py` & `dcicutils-7.2.0.1b0/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/ff_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/jh_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/kibana/dashboards.json` & `dcicutils-7.2.0.1b0/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/kibana/readme.md` & `dcicutils-7.2.0.1b0/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/lang_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/log_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/misc_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/obfuscation_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/opensearch_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/qa_checkers.py` & `dcicutils-7.2.0.1b0/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/qa_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/redis_tools.py` & `dcicutils-7.2.0.1b0/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/redis_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/s3_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/secrets_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/snapshot_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/dcicutils/trace_utils.py` & `dcicutils-7.2.0.1b0/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.1.0/pyproject.toml` & `dcicutils-7.2.0.1b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.1.0"
+version = "7.2.0.1b0"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
@@ -52,14 +52,15 @@
 structlog = "^19.2.0"
 toml = ">=0.10.1,<1"
 typing-extensions = ">=3.8"  # Fourfront uses 3.8
 urllib3 = "^1.26.6"
 webtest = "^2.0.34"
 opensearch-py = "^2.0.1"
 redis = "^4.5.1"
+pyOpenSSL = "^23.1.1"
 PyJWT = "^2.6.0"
 
 
 [tool.poetry.dev-dependencies]
 botocore-stubs = "1.21.22"
 boto3-stubs = "1.18.23"
 coverage = ">=5.3.1"
```

### Comparing `dcicutils-7.1.0/PKG-INFO` & `dcicutils-7.2.0.1b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.1.0
+Version: 7.2.0.1b0
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
@@ -25,14 +25,15 @@
 Requires-Dist: aws-requests-auth (>=0.4.2,<1)
 Requires-Dist: boto3 (>=1.17.39,<2.0.0)
 Requires-Dist: botocore (>=1.20.39,<2.0.0)
 Requires-Dist: docker (>=4.4.4,<5.0.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: opensearch-py (>=2.0.1,<3.0.0)
+Requires-Dist: pyOpenSSL (>=23.1.1,<24.0.0)
 Requires-Dist: pytz (>=2020.4)
 Requires-Dist: redis (>=4.5.1,<5.0.0)
 Requires-Dist: requests (>=2.21.0,<3.0.0)
 Requires-Dist: rfc3986 (>=1.4.0,<2.0.0)
 Requires-Dist: structlog (>=19.2.0,<20.0.0)
 Requires-Dist: toml (>=0.10.1,<1)
 Requires-Dist: typing-extensions (>=3.8)
```

