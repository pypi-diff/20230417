# Comparing `tmp/servox-2.2.3.tar.gz` & `tmp/servox-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servox-2.2.3.tar", max compression
+gzip compressed data, was "servox-2.2.4.tar", max compression
```

## Comparing `servox-2.2.3.tar` & `servox-2.2.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    35574 2023-04-03 18:16:31.365505 servox-2.2.3/CHANGELOG.md
--rw-r--r--   0        0        0    11385 2023-04-03 18:16:31.365505 servox-2.2.3/LICENSE
--rw-r--r--   0        0        0    51279 2023-04-03 18:16:31.365505 servox-2.2.3/README.md
--rw-r--r--   0        0        0     3639 2023-04-03 18:16:31.369506 servox-2.2.3/pyproject.toml
--rw-r--r--   0        0        0     1832 2023-04-03 18:16:31.369506 servox-2.2.3/servo/__init__.py
--rw-r--r--   0        0        0     9522 2023-04-03 18:16:31.369506 servox-2.2.3/servo/api.py
--rw-r--r--   0        0        0    15480 2023-04-03 18:16:31.369506 servox-2.2.3/servo/assembly.py
--rw-r--r--   0        0        0    43745 2023-04-03 18:16:31.369506 servox-2.2.3/servo/checks.py
--rw-r--r--   0        0        0    78505 2023-04-03 18:16:31.369506 servox-2.2.3/servo/cli.py
--rw-r--r--   0        0        0    27724 2023-04-03 18:16:31.369506 servox-2.2.3/servo/configuration.py
--rw-r--r--   0        0        0    16873 2023-04-03 18:16:31.369506 servox-2.2.3/servo/connector.py
--rw-r--r--   0        0        0      680 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/__init__.py
--rw-r--r--   0        0        0    31949 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/kube_metrics.py
--rw-r--r--   0        0        0    95520 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/kubernetes.py
--rw-r--r--   0        0        0      799 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/kubernetes_helpers/__init__.py
--rw-r--r--   0        0        0     2528 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/kubernetes_helpers/base.py
--rw-r--r--   0        0        0    11264 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/kubernetes_helpers/base_workload.py
--rw-r--r--   0        0        0     5158 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/kubernetes_helpers/container.py
--rw-r--r--   0        0        0    14837 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/kubernetes_helpers/deployment.py
--rw-r--r--   0        0        0     1195 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/kubernetes_helpers/namespace.py
--rw-r--r--   0        0        0    12193 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/kubernetes_helpers/pod.py
--rw-r--r--   0        0        0     1779 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/kubernetes_helpers/replicaset.py
--rw-r--r--   0        0        0     2722 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/kubernetes_helpers/service.py
--rw-r--r--   0        0        0     3702 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/kubernetes_helpers/statefulset.py
--rw-r--r--   0        0        0     1625 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/kubernetes_helpers/util.py
--rw-r--r--   0        0        0    47402 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/opsani_dev.py
--rw-r--r--   0        0        0    40511 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/prometheus.py
--rw-r--r--   0        0        0     1708 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/scripts.py
--rw-r--r--   0        0        0    19127 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/vegeta.py
--rw-r--r--   0        0        0      983 2023-04-03 18:16:31.373505 servox-2.2.3/servo/connectors/vegeta_target_schema.json
--rw-r--r--   0        0        0     2619 2023-04-03 18:16:31.377506 servox-2.2.3/servo/connectors/wait.py
--rw-r--r--   0        0        0      607 2023-04-03 18:16:31.377506 servox-2.2.3/servo/encoders.py
--rw-r--r--   0        0        0     1771 2023-04-03 18:16:31.377506 servox-2.2.3/servo/entry_points.py
--rw-r--r--   0        0        0     5335 2023-04-03 18:16:31.377506 servox-2.2.3/servo/errors.py
--rw-r--r--   0        0        0    38440 2023-04-03 18:16:31.377506 servox-2.2.3/servo/events.py
--rw-r--r--   0        0        0    10685 2023-04-03 18:16:31.377506 servox-2.2.3/servo/fast_fail.py
--rw-r--r--   0        0        0    14123 2023-04-03 18:16:31.377506 servox-2.2.3/servo/logging.py
--rw-r--r--   0        0        0    61151 2023-04-03 18:16:31.377506 servox-2.2.3/servo/pubsub.py
--rw-r--r--   0        0        0     6750 2023-04-03 18:16:31.377506 servox-2.2.3/servo/repeating.py
--rw-r--r--   0        0        0    26006 2023-04-03 18:16:31.377506 servox-2.2.3/servo/runner.py
--rw-r--r--   0        0        0    24633 2023-04-03 18:16:31.377506 servox-2.2.3/servo/servo.py
--rw-r--r--   0        0        0     7891 2023-04-03 18:16:31.377506 servox-2.2.3/servo/telemetry.py
--rw-r--r--   0        0        0      808 2023-04-03 18:16:31.377506 servox-2.2.3/servo/types/__init__.py
--rw-r--r--   0        0        0    10891 2023-04-03 18:16:31.377506 servox-2.2.3/servo/types/api.py
--rw-r--r--   0        0        0    31548 2023-04-03 18:16:31.377506 servox-2.2.3/servo/types/core.py
--rw-r--r--   0        0        0     2232 2023-04-03 18:16:31.377506 servox-2.2.3/servo/types/kubernetes.py
--rw-r--r--   0        0        0    23824 2023-04-03 18:16:31.377506 servox-2.2.3/servo/types/settings.py
--rw-r--r--   0        0        0     4575 2023-04-03 18:16:31.377506 servox-2.2.3/servo/types/slo.py
--rw-r--r--   0        0        0      777 2023-04-03 18:16:31.377506 servox-2.2.3/servo/utilities/__init__.py
--rw-r--r--   0        0        0     2854 2023-04-03 18:16:31.377506 servox-2.2.3/servo/utilities/associations.py
--rw-r--r--   0        0        0     5404 2023-04-03 18:16:31.377506 servox-2.2.3/servo/utilities/duration_str.py
--rw-r--r--   0        0        0     2314 2023-04-03 18:16:31.377506 servox-2.2.3/servo/utilities/hashing.py
--rw-r--r--   0        0        0    17660 2023-04-03 18:16:31.377506 servox-2.2.3/servo/utilities/inspect.py
--rw-r--r--   0        0        0     2116 2023-04-03 18:16:31.377506 servox-2.2.3/servo/utilities/key_paths.py
--rw-r--r--   0        0        0     2427 2023-04-03 18:16:31.377506 servox-2.2.3/servo/utilities/pydantic.py
--rw-r--r--   0        0        0     2529 2023-04-03 18:16:31.377506 servox-2.2.3/servo/utilities/strings.py
--rw-r--r--   0        0        0    15189 2023-04-03 18:16:31.377506 servox-2.2.3/servo/utilities/subprocess.py
--rw-r--r--   0        0        0     1016 2023-04-03 18:16:31.377506 servox-2.2.3/servo/utilities/yaml.py
--rw-r--r--   0        0        0    54592 2023-04-03 18:20:09.561790 servox-2.2.3/setup.py
--rw-r--r--   0        0        0    52862 2023-04-03 18:20:09.565895 servox-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35755 2023-04-17 20:31:46.899608 servox-2.2.4/CHANGELOG.md
+-rw-r--r--   0        0        0    11385 2023-04-17 20:31:46.899608 servox-2.2.4/LICENSE
+-rw-r--r--   0        0        0    51279 2023-04-17 20:31:46.903608 servox-2.2.4/README.md
+-rw-r--r--   0        0        0     3639 2023-04-17 20:31:46.903608 servox-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1832 2023-04-17 20:31:46.903608 servox-2.2.4/servo/__init__.py
+-rw-r--r--   0        0        0     9522 2023-04-17 20:31:46.903608 servox-2.2.4/servo/api.py
+-rw-r--r--   0        0        0    15480 2023-04-17 20:31:46.903608 servox-2.2.4/servo/assembly.py
+-rw-r--r--   0        0        0    43745 2023-04-17 20:31:46.903608 servox-2.2.4/servo/checks.py
+-rw-r--r--   0        0        0    78505 2023-04-17 20:31:46.907609 servox-2.2.4/servo/cli.py
+-rw-r--r--   0        0        0    27810 2023-04-17 20:31:46.907609 servox-2.2.4/servo/configuration.py
+-rw-r--r--   0        0        0    16873 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connector.py
+-rw-r--r--   0        0        0      680 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/__init__.py
+-rw-r--r--   0        0        0    31949 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/kube_metrics.py
+-rw-r--r--   0        0        0    95520 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/kubernetes.py
+-rw-r--r--   0        0        0      799 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/kubernetes_helpers/__init__.py
+-rw-r--r--   0        0        0     2528 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/kubernetes_helpers/base.py
+-rw-r--r--   0        0        0    11264 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/kubernetes_helpers/base_workload.py
+-rw-r--r--   0        0        0     5158 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/kubernetes_helpers/container.py
+-rw-r--r--   0        0        0    14837 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/kubernetes_helpers/deployment.py
+-rw-r--r--   0        0        0     1195 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/kubernetes_helpers/namespace.py
+-rw-r--r--   0        0        0    12193 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/kubernetes_helpers/pod.py
+-rw-r--r--   0        0        0     1779 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/kubernetes_helpers/replicaset.py
+-rw-r--r--   0        0        0     2722 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/kubernetes_helpers/service.py
+-rw-r--r--   0        0        0     3702 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/kubernetes_helpers/statefulset.py
+-rw-r--r--   0        0        0     1625 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/kubernetes_helpers/util.py
+-rw-r--r--   0        0        0    47402 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/opsani_dev.py
+-rw-r--r--   0        0        0    40511 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/prometheus.py
+-rw-r--r--   0        0        0     1708 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/scripts.py
+-rw-r--r--   0        0        0    19127 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/vegeta.py
+-rw-r--r--   0        0        0      983 2023-04-17 20:31:46.907609 servox-2.2.4/servo/connectors/vegeta_target_schema.json
+-rw-r--r--   0        0        0     2619 2023-04-17 20:31:46.911609 servox-2.2.4/servo/connectors/wait.py
+-rw-r--r--   0        0        0      607 2023-04-17 20:31:46.911609 servox-2.2.4/servo/encoders.py
+-rw-r--r--   0        0        0     1771 2023-04-17 20:31:46.911609 servox-2.2.4/servo/entry_points.py
+-rw-r--r--   0        0        0     5335 2023-04-17 20:31:46.911609 servox-2.2.4/servo/errors.py
+-rw-r--r--   0        0        0    38440 2023-04-17 20:31:46.911609 servox-2.2.4/servo/events.py
+-rw-r--r--   0        0        0    10685 2023-04-17 20:31:46.911609 servox-2.2.4/servo/fast_fail.py
+-rw-r--r--   0        0        0    14123 2023-04-17 20:31:46.911609 servox-2.2.4/servo/logging.py
+-rw-r--r--   0        0        0    61151 2023-04-17 20:31:46.911609 servox-2.2.4/servo/pubsub.py
+-rw-r--r--   0        0        0     6750 2023-04-17 20:31:46.911609 servox-2.2.4/servo/repeating.py
+-rw-r--r--   0        0        0    26006 2023-04-17 20:31:46.911609 servox-2.2.4/servo/runner.py
+-rw-r--r--   0        0        0    24633 2023-04-17 20:31:46.911609 servox-2.2.4/servo/servo.py
+-rw-r--r--   0        0        0     7891 2023-04-17 20:31:46.911609 servox-2.2.4/servo/telemetry.py
+-rw-r--r--   0        0        0      808 2023-04-17 20:31:46.911609 servox-2.2.4/servo/types/__init__.py
+-rw-r--r--   0        0        0    10891 2023-04-17 20:31:46.911609 servox-2.2.4/servo/types/api.py
+-rw-r--r--   0        0        0    32100 2023-04-17 20:31:46.911609 servox-2.2.4/servo/types/core.py
+-rw-r--r--   0        0        0     2232 2023-04-17 20:31:46.911609 servox-2.2.4/servo/types/kubernetes.py
+-rw-r--r--   0        0        0    23824 2023-04-17 20:31:46.911609 servox-2.2.4/servo/types/settings.py
+-rw-r--r--   0        0        0     4575 2023-04-17 20:31:46.911609 servox-2.2.4/servo/types/slo.py
+-rw-r--r--   0        0        0      777 2023-04-17 20:31:46.911609 servox-2.2.4/servo/utilities/__init__.py
+-rw-r--r--   0        0        0     2854 2023-04-17 20:31:46.911609 servox-2.2.4/servo/utilities/associations.py
+-rw-r--r--   0        0        0     5404 2023-04-17 20:31:46.911609 servox-2.2.4/servo/utilities/duration_str.py
+-rw-r--r--   0        0        0     2314 2023-04-17 20:31:46.911609 servox-2.2.4/servo/utilities/hashing.py
+-rw-r--r--   0        0        0    17660 2023-04-17 20:31:46.911609 servox-2.2.4/servo/utilities/inspect.py
+-rw-r--r--   0        0        0     2116 2023-04-17 20:31:46.911609 servox-2.2.4/servo/utilities/key_paths.py
+-rw-r--r--   0        0        0     2427 2023-04-17 20:31:46.911609 servox-2.2.4/servo/utilities/pydantic.py
+-rw-r--r--   0        0        0     2529 2023-04-17 20:31:46.911609 servox-2.2.4/servo/utilities/strings.py
+-rw-r--r--   0        0        0    15189 2023-04-17 20:31:46.911609 servox-2.2.4/servo/utilities/subprocess.py
+-rw-r--r--   0        0        0     1016 2023-04-17 20:31:46.911609 servox-2.2.4/servo/utilities/yaml.py
+-rw-r--r--   0        0        0    54592 2023-04-17 20:35:23.483669 servox-2.2.4/setup.py
+-rw-r--r--   0        0        0    52862 2023-04-17 20:35:23.487443 servox-2.2.4/PKG-INFO
```

### Comparing `servox-2.2.3/CHANGELOG.md` & `servox-2.2.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 Servo is distributed under the terms of the Apache 2.0 license.
 
 This changelog catalogs all notable changes made to the project. The format is
 based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/). Releases are
 versioned in accordance with [Semantic
 Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.2.4] "genesis" - 2023-04-14
+
+### Changed
+
+- Default interval of progress updates changed from 5 seconds to 60
+- Updated API path used for servo endpoint of optimize solution
+
 ## [2.2.3] "genesis" - 2023-03-31
 
 ### Changed
 
 - Update ID of appD config to use optimizerID instead of workloadID
 
 ## [2.2.2] "genesis" - 2023-03-20
```

### Comparing `servox-2.2.3/LICENSE` & `servox-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/README.md` & `servox-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/pyproject.toml` & `servox-2.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servox"
-version = "2.2.3"
+version = "2.2.4"
 description = "Opsani Servo: The Next Generation"
 homepage = "https://opsani.com/"
 repository = "https://github.com/opsani/servox"
 authors = ["Blake Watters <blake@opsani.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [
```

### Comparing `servox-2.2.3/servo/__init__.py` & `servox-2.2.4/servo/__init__.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/api.py` & `servox-2.2.4/servo/api.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/assembly.py` & `servox-2.2.4/servo/assembly.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/checks.py` & `servox-2.2.4/servo/checks.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/cli.py` & `servox-2.2.4/servo/cli.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/configuration.py` & `servox-2.2.4/servo/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     Endpoint: pydantic.AnyHttpUrl
     TenantId: str
 
 
 class AppdynamicsOptimizer(pydantic.BaseSettings):
     optimizer_id: str
     tenant_id: Optional[str] = None
-    base_url: pydantic.AnyHttpUrl = "https://optimize-ignite-test.saas.appd-test.com/"
+    base_url: Optional[pydantic.AnyHttpUrl] = None
     # static config properties
     client_id: Optional[str] = None
     client_secret: Optional[pydantic.SecretStr] = None
     # dynamic config properties
     connection_file: Optional[str] = None
     token: Optional[pydantic.SecretStr] = None
     # override properties
@@ -86,22 +86,23 @@
                 backoff.expo, FileNotFoundError, max_time=60
             )(self.load_connection_file)
             init_backoff()
         elif (
             self.client_id is None
             or self.client_secret is None
             or self.tenant_id is None
+            or self.base_url is None
         ):
             raise ValueError(
-                f"{self.__class__.__name__} must be configured with a connection file or specify client_id, client_secret, and tenant_id"
+                f"{self.__class__.__name__} must be configured with a connection file or specify base_url, client_id, client_secret, and tenant_id"
             )
 
         if not self.url:
             self.url = (
-                f"{self.base_url}/rest/optimize/co/v1/optimizer/{self.optimizer_id}/"
+                f"{self.base_url}/rest/optimize/co/v1/optimizers/{self.optimizer_id}/"
             )
         if not self.token_url:
             self.token_url = (
                 f"{self.base_url}/auth/{self.tenant_id}/default/oauth2/token"
             )
 
     def load_connection_file(self) -> None:
@@ -114,27 +115,30 @@
         validated_content = SidecarConnectionFile.parse_obj(content)
         self.token = validated_content.Authorization
         self.base_url = validated_content.Endpoint.rstrip("/")
         self.tenant_id = validated_content.TenantId
 
     @pydantic.validator("base_url")
     def _rstrip_slash(cls, url: str) -> str:
-        return url.rstrip("/")
+        if url:
+            return url.rstrip("/")
+        return url
 
     @property
     def id(self) -> str:
         return f"{self.tenant_id} - {self.optimizer_id}"
 
     @property
     def name(self) -> str:
         return f"{self.optimizer_id}"
 
     class Config:
         case_sensitive = True
         extra = pydantic.Extra.forbid
+        validate_assignment = True
         fields = {
             "optimizer_id": {"env": "APPD_OPTIMIZER_ID"},
             "tenant_id": {"env": "APPD_TENANT_ID"},
             "client_id": {"env": "APPD_CLIENT_ID"},
             "client_secret": {"env": "APPD_CLIENT_SECRET"},
             "base_url": {"env": "APPD_BASE_URL"},
             "url": {"env": "APPD_URL"},
```

### Comparing `servox-2.2.3/servo/connector.py` & `servox-2.2.4/servo/connector.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/__init__.py` & `servox-2.2.4/servo/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/kube_metrics.py` & `servox-2.2.4/servo/connectors/kube_metrics.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/kubernetes.py` & `servox-2.2.4/servo/connectors/kubernetes.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/kubernetes_helpers/__init__.py` & `servox-2.2.4/servo/connectors/kubernetes_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/kubernetes_helpers/base.py` & `servox-2.2.4/servo/connectors/kubernetes_helpers/base.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/kubernetes_helpers/base_workload.py` & `servox-2.2.4/servo/connectors/kubernetes_helpers/base_workload.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/kubernetes_helpers/container.py` & `servox-2.2.4/servo/connectors/kubernetes_helpers/container.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/kubernetes_helpers/deployment.py` & `servox-2.2.4/servo/connectors/kubernetes_helpers/deployment.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/kubernetes_helpers/namespace.py` & `servox-2.2.4/servo/connectors/kubernetes_helpers/namespace.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/kubernetes_helpers/pod.py` & `servox-2.2.4/servo/connectors/kubernetes_helpers/pod.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/kubernetes_helpers/replicaset.py` & `servox-2.2.4/servo/connectors/kubernetes_helpers/replicaset.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/kubernetes_helpers/service.py` & `servox-2.2.4/servo/connectors/kubernetes_helpers/service.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/kubernetes_helpers/statefulset.py` & `servox-2.2.4/servo/connectors/kubernetes_helpers/statefulset.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/kubernetes_helpers/util.py` & `servox-2.2.4/servo/connectors/kubernetes_helpers/util.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/opsani_dev.py` & `servox-2.2.4/servo/connectors/opsani_dev.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/prometheus.py` & `servox-2.2.4/servo/connectors/prometheus.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/scripts.py` & `servox-2.2.4/servo/connectors/scripts.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/vegeta.py` & `servox-2.2.4/servo/connectors/vegeta.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/vegeta_target_schema.json` & `servox-2.2.4/servo/connectors/vegeta_target_schema.json`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/connectors/wait.py` & `servox-2.2.4/servo/connectors/wait.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/encoders.py` & `servox-2.2.4/servo/encoders.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/entry_points.py` & `servox-2.2.4/servo/entry_points.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/errors.py` & `servox-2.2.4/servo/errors.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/events.py` & `servox-2.2.4/servo/events.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/fast_fail.py` & `servox-2.2.4/servo/fast_fail.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/logging.py` & `servox-2.2.4/servo/logging.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/pubsub.py` & `servox-2.2.4/servo/pubsub.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/repeating.py` & `servox-2.2.4/servo/repeating.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/runner.py` & `servox-2.2.4/servo/runner.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/servo.py` & `servox-2.2.4/servo/servo.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/telemetry.py` & `servox-2.2.4/servo/telemetry.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/types/__init__.py` & `servox-2.2.4/servo/types/__init__.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/types/api.py` & `servox-2.2.4/servo/types/api.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/types/core.py` & `servox-2.2.4/servo/types/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """The `servo.types` module defines the essential data types shared by all
 consumers of the servo package.
 """
 from __future__ import annotations
 
 import abc
 import asyncio
+import contextlib
 import datetime
 import enum
 import inspect
 import operator
 from typing import (
     Any,
     AsyncIterator,
@@ -579,19 +580,37 @@
         self,
         notify: Callable[["DurationProgress"], Union[None, Awaitable[None]]],
         every: Optional[Duration] = None,
     ) -> None:
         # NOTE: Handle the case where reporting interval < timeout (matters mostly for tests)
         if every is None:
             if self.timeout is None:
-                every = Duration("5s")
+                every = Duration("60s")
             else:
-                every = min(Duration("5s"), self.timeout)
+                every = min(Duration("60s"), self.timeout)
 
-        return await super().watch(notify, every)
+        # return await super().watch(notify, every)
+        async def async_notifier() -> None:
+            if asyncio.iscoroutinefunction(notify):
+                await notify(self)
+            else:
+                notify(self)
+
+        if not self.started:
+            self.start()
+
+        while True:
+            if self.finished:
+                break
+
+            with contextlib.suppress(asyncio.TimeoutError):
+                await asyncio.wait_for(
+                    self._event.wait(), timeout=every.total_seconds()
+                )
+            await async_notifier()
 
 
 class Unit(str, enum.Enum):
     """An enumeration of standard units of measure for metrics.
 
     Member names are the name of the unit and values are an abbreviation of the unit.
```

### Comparing `servox-2.2.3/servo/types/kubernetes.py` & `servox-2.2.4/servo/types/kubernetes.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/types/settings.py` & `servox-2.2.4/servo/types/settings.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/types/slo.py` & `servox-2.2.4/servo/types/slo.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/utilities/__init__.py` & `servox-2.2.4/servo/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/utilities/associations.py` & `servox-2.2.4/servo/utilities/associations.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/utilities/duration_str.py` & `servox-2.2.4/servo/utilities/duration_str.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/utilities/hashing.py` & `servox-2.2.4/servo/utilities/hashing.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/utilities/inspect.py` & `servox-2.2.4/servo/utilities/inspect.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/utilities/key_paths.py` & `servox-2.2.4/servo/utilities/key_paths.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/utilities/pydantic.py` & `servox-2.2.4/servo/utilities/pydantic.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/utilities/strings.py` & `servox-2.2.4/servo/utilities/strings.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/utilities/subprocess.py` & `servox-2.2.4/servo/utilities/subprocess.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/servo/utilities/yaml.py` & `servox-2.2.4/servo/utilities/yaml.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.3/setup.py` & `servox-2.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                       'servo.connectors.prometheus:PrometheusConnector',
                       'scripts = servo.connectors.scripts:ScriptsConnector',
                       'vegeta = servo.connectors.vegeta:VegetaConnector',
                       'wait = servo.connectors.wait:WaitConnector']}
 
 setup_kwargs = {
     'name': 'servox',
-    'version': '2.2.3',
+    'version': '2.2.4',
     'description': 'Opsani Servo: The Next Generation',
     'long_description': '# Opsani ServoX\n\n![Run Tests](https://github.com/opsani/servox/workflows/Run%20Tests/badge.svg)\n[![license](https://img.shields.io/github/license/opsani/servox.svg)](https://github.com/opsani/servox/blob/main/LICENSE)\n[![PyPI](https://img.shields.io/pypi/v/servox.svg)](https://pypi.org/project/servox/)\n[![release](https://img.shields.io/github/release/opsani/servox.svg)](https://github.com/opsani/servox/releases/latest)\n[![GitHub release\ndate](https://img.shields.io/github/release-date/opsani/servox.svg)](https://github.com/opsani/servox/releases)\n\nThis repository contains the source code of the Opsani Servo agent.\n\nThe servo connects applications to the Opsani cloud optimization engine\nto identify cost savings and performance enhancements by applying machine\nlearning technology. Servos are lightweight Python applications and are\ntypically deployed as a container under an orchestration layer such as\nKubernetes, ECS, or Docker Compose.\n\nServos are composed of connectors, which provide the core functionality for\nintegrating with metrics, orchestration, and load generation systems/utilities.\nThe ServoX codebase provides core functionality shared by all servos and a rich\nlibrary supporting the development of connectors.\n\n## Quick Start\n\nServoX is a modern Python application distributed as an installable Python\npackage. Development is done in a Python install managed with\n[Pyenv](https://github.com/pyenv/pyenv) and a virtual environment managed by\n[Poetry](https://python-poetry.org/). This is the path of least resistance but\nany Python package management system should work.\n\n* Clone the repo: `git clone git@github.com:opsani/servox`\n* Install required Python: `cd servox && pyenv install`\n* Install Poetry: `curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py |\n  python`\n* Link Poetry with pyenv version: ``poetry env use `cat .python-version` ``\n* Install dependencies: `poetry install`\n* Activate the venv: `poetry shell`\n* Initialize your environment: `servo init`\n* Start interacting with the servo: `servo --help`\n\n## Overview\n\n### Getting Started with Opsani\n\nAccess to an Opsani optimizer is required to deploy the servo and run the end to\nend integration tests. If you do not currently have access to an Opsani\nenvironment but are otherwise interested in working with the optimizer and\nServo, please reach out to us at [info@opsani.com](mailto:info@opsani.com) and\nwe will get back with you.\n\n### Usage\n\n#### Displaying Help\n\n```console\n❯ servo --help\n```\n\n#### Initializing an Assembly\n\n**NOTE**: A Dotenv file is recommended during development to keep the CLI\noptions under control. The init command will generate one for you.\n\n```console\n❯ servo init\n```\n\n#### Configuration\n\n```console\n# Generate a config file with all available connectors\n❯ servo generate\n\n# Validate a config file\n❯ servo validate\n\n# Display config schema\n❯ servo schema\n```\n\n#### Displaying Info\n\n```console\n# Display all available connectors\n❯ servo connectors\n\n# Display instance specific info (requires configuration)\n❯ servo show connectors\n❯ servo show events\n❯ servo show components\n❯ servo show metrics\n```\n\n#### Running Operations\n\n```console\n# Check servo readiness\n❯ servo run --dry-run\n\n# Describe application state\n❯ servo describe\n\n# Capture and display a measurement\n❯ servo measure\n\n# Adjust the memory of web-server to 512MB and cpu of gateway to 800 millicores\n❯ servo adjust web.mem=512 gateway.cpu=0.8\n\n# Run the servo to start optimizing\n❯ servo run\n```\n\n## Architecture\n\nServoX has been designed to provide a delightful experience for engineers\nintegrating cloud optimization into their systems and workflow. Developer\nergonomics and operator efficiency are primary concerns as integrating and\norchestrating disparate components can quickly become tiresome and complex. As a\nlibrary, ServoX aspires to be as "batteries included" as possible and support\ndevelopers with well designed, implemented, and tested solutions for common\nconcerns. As a tool, ServoX strives to support system operators and devops\nengineers with strong support for common tasks and a high-velocity workflow.\n\nThere are a few key components that form the foundation of the architecture:\n\n* **Connectors** - Connectors are pluggable components that enable the servo to\n  interact with external systems such as metrics providers (Prometheus, Datadog,\n  New Relic, etc), orchestration technologies (Kubernetes, cloud provider APIs,\n  etc), or load generators. Every major functional component (including the\n  servo itself) is a connector that inherits from the `Connector` base class.\n  Connectors can process events dispatched from the servo (see Events below),\n  provide services to the user (see CLI below), and interact with other\n  connectors.\n* **Servo** - The Servo class models the active set of connectors and\n  configuration that is executing. The servo handles connectivity with the\n  Opsani Optimizer API (see Optimizer below) and is responsible for the primary\n  concerns of connectivity management and event handling.\n* **Configuration** - Configuration is a major shared concern in tools such as\n  Opsani that are designed to integrate with arbitrary systems. Ensuring that\n  configuration is valid, complete, and functional is a non-trivial task for any\n  component with more than a few knobs and levers. ServoX provides a rich\n  configuration subsystem built on Pydantic that makes modeling and processing\n  configuration very straightforward. Out of the box support is provided for\n  common needs such as environment variables and dotenv files. Configuration is\n  strongly validated using JSON Schema and support is provided for generating\n  config files directly from the connectors.\n* **Optimizer** - The Optimizer class represents an Opsani optimization engine\n  that the servo interacts with via an API. The optimizer can be configured via\n  config file or from the environment; both of these support Kubernetes secrets.\n* **Events** - The Event subsystem provides the primary interaction point\n  between the Servo and Connectors in a loosely coupled manner. Events are\n  simple string values that have connector defined semantics and can optionally\n  return a result. The Servo base class defines the primary events of\n  `DESCRIBE`, `MEASURE`, `ADJUST`, and `PROMOTE` which correspond to declaring\n  the metrics & components that the connector is interested in, taking\n  measurements and returning aggregated scalar or time series data points,\n  making changes to the application under optimization, or promoting an\n  optimized configuration to the broader system.\n* **Checks** - Checks provide a mechanism for verifying the correctness and\n  health of connector configuration and operations. They are designed to support\n  a high throughput integration and debugging experience by providing feedback\n  loop driven workflow. Checks are implemented on top of the events subsystem\n  and can be executed alongside an actual run via the `servo run --check` CLI command,\n  or by themselves via `servo run --dry-run` The design of the checks subsystem\n  is covered in depth [in the docs](docs/checks.md).\n* **Assembly** - The Servo Assembly models the runtime environment of the servo\n  outside of a particular configuration. The assembly is the parent of the servo\n  and is responsible for "assembling" it by instantiating connectors as\n  configured by the operator. Connectors can be used multiple times (e.g. you\n  may want to connect to multiple discrete Prometheus services) or may not be\n  used at all (e.g. you have a New Relic connector in the container image but\n  aren\'t using it).\n* **CLI** - The CLI provides the primary interface for interacting with the\n  servo. The CLI is modular and contains a number of root level commands and\n  connectors can optionally register additional commands. Most of the root level\n  commands are driven through the event subsystem and connectors which respond\n  to the relevant events will automatically become accessible through the CLI.\n  For example, executing `servo schema` will emit a complete JSON Schema\n  document for the assembly while `servo schema kubernetes` will emit a JSON\n  Schema specific to the Kubernetes connector.\n\n### Understanding Events\n\nThe servo is built around an event driven architecture and utilizes a\nlightweight eventing system to pass messages between connectors. Eventing is\nimplemented in asynchronous Python on top of asyncio. Events are simple strings\nidentifiers that are bound to a Python\n[inspect.Signature](https://docs.python.org/3/library/inspect.html#inspect.Signature)\nobject. The signature is used when event handlers are registered to enforce a\ncontract around the parameter and return types, method arity, etc.\n\nAny connector can define an event provided that no other connector has already\nregistered an event with the desired name. The `Servo` class defines several\nbasic events covering essential functionality such as declaring metrics and\ncomponents, capturing measurements, and performing adjustments. These events are\nintegrated into the CLI and readily accessible. For example, executing `servo\nshow metrics` dispatches the `metrics` event to all active connectors and\ndisplays the aggregate results in a table. More substantial commands such as\n`measure` and `adjust` work in the same manner -- dispatching events and\nvisualizing the results. Whenever possible functionality is implemented via\neventing.\n\nWhen the servo is run, it connects to the Opsani optimizer via the API and\nreceives instructions about which actions to take to facilitate the optimization\nactivity. These commands are dispatched to the connectors via events.\n\nThe default events are available on the `servo.servo.Events` enumeration and\ninclude:\n\n| Event      | Category      | Description                                                                                                            |\n| ---------- | ------------- | ---------------------------------------------------------------------------------------------------------------------- |\n| startup    | Lifecycle     | Dispatched when the servo is assembled.                                                                                |\n| shutdown   | Lifecycle     | Dispatched when the servo is being shutdown.                                                                           |\n| metrics    | Informational | Dispatched to gather the metrics being measured.                                                                       |\n| components | Informational | Dispatched to gather the components & settings available for adjustment.                                               |\n| check      | Operational   | Asks connectors to check if they are ready to run by validating settings, etc.                                         |\n| describe   | Operational   | Gathers the current state of the application under optimization.                                                       |\n| measure    | Operational   | Takes a measurement of target metrics and reports them to the optimizer.                                               |\n| adjust     | Operational   | Applies a change to the components/settings of the application under optimization and reports status to the optimizer. |\n\n#### Event Handlers & Prepositions\n\nEvent handlers are easily registered via a set of method decorators available on\nthe `servo.connector` module. Handlers are registered with a *preposition* which\ndetermines if it is invoked before, on, or after the event has been processed.\nHandlers are invoked when the servo or another connector dispatches an event.\nEvent handlers can be implemented either synchronously or asynchronously\ndepending on if the method is a coroutine declared with the async prefix.\n\n```python\nfrom typing import List\nimport servo\n\n\nclass SomeConnector(servo.BaseConnector):\n    @servo.before_event(\'measure\')\n    def notify_before_measure(self) -> None:\n        self.logger.info("We are about to measure...")\n\n    @servo.on_event(\'metrics\')\n    def metrics(self) -> List[servo.Metric]:\n        return [servo.Metric(\'throughput\', servo.Unit.REQUESTS_PER_MINUTE)]\n\n    @servo.after_event(\'adjust\')\n    def analyze_results(self, results: List[servo.EventResult]) -> None:\n        self.logger.info(f"We got some results: {results}")\n```\n\nEach preposition has different capabilities available to it. Before event\nhandlers can cancel the execution of the event by raising a `EventCancelledError`.\nOn event handlers can return results that are aggregated and available for\nprocessing. After event handlers get access to all of the results returned by\nactive connectors via the on event handlers.\n\n#### Creating a new Event\n\nEvents can be created either programmatically via the `Connector.create_event()`\nclass method or declaratively via the `event()` decorator:\n\n```python\nimport servo\n\n\nclass EventExample(servo.BaseConnector):\n    @servo.event()\n    async def trace(self, url: str) -> str:\n        ...\n```\n\nThe `event` decorator uses the parameters and return type of the decorated\nmethod to define the signature requirements for on event handlers registered\nagainst the event. The body of the decorated method must be `...`, `pass`, or an\nasync generator that yields `None` exactly once.\n\nThe body of the decorated method can be used to define setup and tear-down\nactivities around on event handlers. This allows for common setup and tear-down\nfunctionality to be defined by the event creator. This is achieved by\nimplementing the body of the decorated method as an async generator that yields\ncontrol to the on event handler:\n\n```python\nfrom typing import AsyncIterator\nimport servo\n\n\nclass SetupAndTearDownExample(servo.BaseConnector):\n    @servo.event()\n    async def trace(self, url: str) -> AsyncIterator[str]:\n        print("Entering event handler...")\n        yield\n        print("Exited event handler.")\n```\n\nThe event decorator can also be used to create an event and register a handler\nfor the event at the same time. In this example, the `handler=True` keyword\nargument is provided to created the event **and** register the decorated method\nas an on event handler for the new event.\n\n```python\nimport servo\n\n\nclass AnotherConnector(servo.BaseConnector):\n    @servo.event(\'load_test\', handler=True)\n    async def run_load_test(self, url: str, duration: int = 60) -> str:\n        return "Do something..."\n```\n\nOnce an event is created, the connector can dispatch against it to notify other\nconnectors of changes in state or to request data from them.\n\n#### Dispatching an Event\n\nConnectors can notify or interact with other connectors by dispatching an event.\nWhen the servo is assembled, an event bus is transparently established between\nthe connectors to facilitate event driven interaction.\n\n```python\nfrom typing import List\nimport servo\n\n\nclass ExampleConnector(servo.BaseConnector):\n    async def do_something(self) -> None:\n        # Gather metrics from other connectors\n        results: List[servo.EventResult] = await self.dispatch_event("metrics")\n        for result in results:\n            print(f"Gathered metrics: {result.value}")\n```\n\n### Environment Variables & Dotenv\n\nPay attention to the output of `servo --help` and `servo schema` to identify\nenvironment variables that can be used for configuration. The servo handles\nconfiguration of deeply nested attributes by building the environment variable\nmapping on the fly at assembly time.\n\nFor convenience, the `servo` CLI utility automatically supports `.env` files for\nloading configuration and is already in the `.gitignore`. Interacting with the\nCLI is much cleaner if you drop in a dotenv file to avoid having to deal with\nthe options to configure the optimizer. The `servo init` command will help set\nthis up interactively.\n\n### Logging\n\nThe servo base library provides logging services for all connectors and core\ncomponents. By default, the `servo` CLI utility runs at the `INFO` log level\nwhich is designed to provide balanced output that informs you of what is\nhappening operationally without becoming overwhelming and pedantic. During\ndevelopment, debugging, or troubleshooting it may become desirable to run at an\nelevated log level. The log level can be set via a commandline option on the\n`servo` utility or via the `SERVO_LOG_LEVEL` environment variable. The servo\nwill emit ANSI colored output to `stderr` when the terminal is a TTY. Coloring\ncan be suppressed via the `--no-color` commandline option or with the\n`SERVO_NO_COLOR` or `NO_COLOR` environment variables.\n\n```console\n  -l, --log-level [TRACE|DEBUG|INFO|SUCCESS|WARNING|ERROR|CRITICAL]\n                                  Set the log level  [env var:\n                                  SERVO_LOG_LEVEL; default: INFO]\n  --no-color                      Disable colored output  [env var:\n                                  SERVO_NO_COLOR, NO_COLOR]\n```\n\nBy default, log messages are written to `stderr` and a file sink at the `logs/`\nsubdirectory relative to the servo root. Backtraces are preformatted and as much\ncontext as possible is provided when an exception is logged.\n\nThe `servo.logging` module exposes some interesting functionality for operators\nand developers alike. Logging is aware of the eventing subsystem and will\nautomatically attribute log messages to the currently executing connector and\nevent context. Long running operations can be automatically reported to the\nOpsani API by including a `progress` key with a numeric percentage value ranging\nfrom 0.0 to 100.0. There are several function decorators available that can\nprovide automatic logging output for entry and exit, execution timing, etc.\n\nDependent libraries such as `backoff` have been configured to emit their logs\ninto the servo logging module. Every component that has logging support is\nintercepted and handled by the logging subsystem and conforms to the log levels\noutlined above.\n\n### Connector Discovery\n\nConnectors are set up to be auto-discovered using the setuptools entry point\nfunctionality available from the Python standard library. When a new connector\nis installed into the assembly, it will be automatically discovered and become\navailable for interaction.\n\nThe specific of how this mechanism works is discussed in detail on the [Python\nPackaging\nGuide](https://packaging.python.org/guides/creating-and-discovering-plugins/).\n\nThe bundled connectors are registered and discovered using this mechanism via\nentries in the `pyproject.toml` file under the\n`[tool.poetry.plugins."servo.connectors"]` stanza.\n\nIf you\'re writing your own connector in an external package, you need to include\n```yaml\n[tool.poetry.plugins."servo.connectors"]\n"my_connector" = "my_project.foo:MyConnector"\n```\nin your `pyproject.toml` to add your connector as an entry point.\nand you _must_ name your connector `class MyConnector(servo.BaseConnector):` to have it discoverable.\nDiscovery is performed via the `servo.connector:_name_for_connector_class()` function. It matches\nthe `My` in the connector class name to the top level connector key in the `servo.yaml`.\nSo, for example, your `servo.yaml` could be as follows:\n```yaml\n...\nmy:\n  foo: bar\n  baz: bat\n...\n```\n\n### Running Multiple Connector Instances\n\nServoX is designed to support assemblies that contain an arbitrary number of\nconnectors that may or may not be active and enable the use of multiple\ninstances of a connector with different settings. This introduces a few modes of\nconfiguration.\n\nThe servo looks to a `connectors` configuration key that explicitly declares\nwhich connectors are active within the assembly. If a `connectors` key is not\npresent in the config file, then all available connectors become optionally\navailable based on the presence or absence of their default configuration key.\nFor example, an assembly that includes New Relic, Datadog, and SignalFX\nconnectors installed as Python packages with the following configuration would\nonly activate Datadog due to the presence of its configuration stanza:\n\n```yaml\ndatadog:\n  setting_1: some value\n  setting_2: another value\n```\n\nThis mode supports the general case of utilizing a small number of connectors in\n"off the shelf" configurations.\n\nFrom time to time, it may become necessary to connect to multiple instances of a\ngiven service -- we have seen this a few times with Prometheus in canary mode\ndeployments where metrics are scattered across a few instances. In these cases,\nit can become necessary to explicitly alias a connector and utilize it under two\nor more configurations. In such cases, the `connectors` key becomes required in\norder to disambiguate aliases from configuration errors. In such cases, the\n`connectors` key can be configured as a dictionary where the key identifies the\nalias and the value identifies the connector:\n\n```yaml\nconnectors:\n  prom1: prometheus\n  prom2: prometheus\n\nprom1:\n  setting_1: some value\n  setting_2: another value\n\nprom2:\n  setting_1: some value\n  setting_2: another value\n```\n\nIt is also possible to utilize the `connectors` key in order to exclude\nconnectors from the active set. This can be done with the dictionary syntax\nreferenced above or using an array syntax if aliasing is not being utilized. For\nexample, given a configuration with New Relic and Prometheus active but some\nsort of issue warranting the isolation of Prometheus from the active set, the\nconfig file might be configured like:\n\n```yaml\nconnectors:\n  - new_relic\n\nprometheus:\n  setting_1: some value\n  setting_2: another value\n\nnew_relic:\n  setting_1: some value\n  setting_2: another value\n```\n\nThese configurations can be generated for you by providing arguments to `servo\ngenerate`. A space delimited list of connector names will explicitly populate\nthe `connectors` key and a syntax of `alias:connector` will configure aliases:\n\n```console\n❯ servo generate foo:vegeta bar:kubernetes\nbar:\n  description: Update the namespace, deployment, etc. to match your Kubernetes cluster\n  namespace: default\nconnectors:\n  bar: kubernetes\n  foo: vegeta\nfoo:\n  description: Update the rate and target/targets to match your load profile\n  duration: 5m\n  rate: 50/1s\n  target: https://example.com/\n\nGenerated servo.yaml\n```\n\n### Running Multiple Servos\n\nServoX is capable of running multiple servos within the same assembly and servos\ncan be added and removed dynamically at runtime. This is useful for optimizing\nseveral applications at one time from a single servo deployment to simplify\noperations or more interestingly to support the integration and automation of\noptimization into CI and CD pipelines. For example, it is possible to configure\nthe build system to trigger optimization for apps as they head into staging or\nupon emergence into production.\n\nMulti-servo execution mode is straightforward. When the `servo.yaml` config file\nis found to contain multiple documents (delimited by `---`), a servo instance is\nconstructed for each entry in the file and added to the assembly. There are\nhowever a few differences in configuration options.\n\nWhen multi-servo mode is enabled, the `--optimizer`, `--token`, `--token-file`,\n`--base-url`, and `--url` options are unavailable. The optimizer and\nconnectivity configuration must be provided via the `optimizer` stanza within\neach configuration *document* in the config file. The CLI will raise errors if\nthese options are utilized with a multi-servo configuration because they are\nambiguous. This does not preclude a single servo being promoted into a\nmulti-servo configuration at runtime -- it is a configuration resolution\nconcern.\n\nWhen running multi-servo, logging is changed to provide context about the servo\nthat is active and generating the output. The `servo.current_servo()` method\nreturns the active servo at runtime.\n\nBecause ServoX is based on `asyncio` and functions as an orchestrator, it is\ncapable of managing a large number of optimizations in parallel (we have tested\ninto the thousands). Most operations performed are I/O bound and asynchronous\nbut the specifics of the connectors used in a multi-servo configuration will\nhave a significant impact on the upper bounds of concurrency.\n\n#### Configuring Multi-servo Mode\n\nBasically all that you need to do is use the `---` delimiter to create multiple\ndocuments within the `servo.yaml` file and configure an `optimizer` within\neach one. For example:\n\n```yaml\n---\noptimizer:\n  id: newco.com/awesome-app1\n  token: 00000000-0000-0000-0000-000000000000\nconnectors: [vegeta]\nvegeta:\n  duration: 5m\n  rate: 50/1s\n  target: GET https://app1.example.com/\n---\noptimizer:\n  id: newco.com/awesome-app2\n  token: 00000000-0000-0000-0000-000000000000\nconnectors: [vegeta]\nvegeta:\n  duration: 5m\n  rate: 50/1s\n  target: GET https://app2.example.com/\n```\n\n#### Adding & Removing Servos at Runtime\n\nServos can be added and removed from the assembly at runtime via methods on the\n`servo.Assembly` class:\n\n```python\nimport servo\n\nassembly = servo.current_assembly()\nnew_servo = servo.Servo()\nassembly.add_servo(new_servo)\nassembly.remove_servo(new_servo)\n```\n\n### Extending the CLI\n\nShould your connector wish to expose additional commands to the CLI, it can do\nso via the `ConnectorCLI` class. Instances are automatically registred with the\nCLI and the `Context` is configured appropriately when commands are invoked. All\nCLI extensions are namespaced as subcommands to keep things tidy and avoid\nnaming conflicts.\n\nA simple example of a CLI extension that will register `servo vegeta attack` is:\n\n```python\nimport servo\nimport servo.cli\nimport servo.connectors.vegeta\n\n\ncli = servo.cli.ConnectorCLI(servo.connectors.vegeta.VegetaConnector, help="Load testing with Vegeta")\n\n\n@cli.command()\ndef attack(context: servo.cli.Context):\n    """\n    Run an adhoc load generation\n    """\n    context.connector.measure()\n```\n\n### Requirements & Dependencies\n\nServoX is implemented in Python and supported by a handful of excellent\nlibraries from the Python Open Source community. Additional dependencies in the\nform of Python packages or system utilities are imposed by connectors (see\nbelow).\n\n* [Python](https://www.python.org/) 3.6+ - ServoX makes liberal use of type\n  hints to annotate the code and drive some functionality.\n* [Pydantic](https://pydantic-docs.helpmanual.io/) - Pydantic is a fantastic\n  parsing and validation library that underlies most classes within ServoX. It\n  enables the strong modeling and validation that forms the core of the\n  configuration module.\n* [Typer](https://typer.tiangolo.com/) - Typer provides a nice, lightweight\n  enhancement on top of [Click](https://click.palletsprojects.com/en/7.x/) for\n  building CLIs in Python. The CLI is built out on top of Typer.\n* [httpx](https://www.python-httpx.org/) - httpx is a (mostly) requests\n  compatible HTTP library that provides support for HTTP/2, is type annotated,\n  has extensive test coverage, and supports async interactions on top of\n  asyncio.\n* [loguru](https://loguru.readthedocs.io/en/stable/index.html) - A rich Python\n  logging library that builds on the foundation of the standard library logging\n  module and provides a number of enhancements.\n\n## Development\n\n### Contributing to ServoX\n\nOpen Source contributions are always appreciated. Should you wish to get\ninvolved, drop us a line via GitHub issues or email to coordinate efforts.\n\nIt is expected that most Open Source contributions will come in the form of new\nconnectors. Should you wish to develop a connector, reach out to us at Opsani as\nwe have connector developer guides that are in pre-release while ServoX matures.\n\n### Visual Studio Code\n\nThe core development team typically works in VSCode. Poetry and VSCode have not\nquite yet become seamlessly integrated. For your convenience, there are a couple\nof Makefile tasks that can simplify configuration:\n\n* `make init` - Initialize a Poetry environment, configure `.vscode/settings.json`,\n  and then run the `servo initialize command.\n* `make vscode` - Export the Poetry environment variables and then open the\n  local working copy within VSCode. The built-in terminal and Python extension\n  should auto-detect the Poetry environment and behave.\n\n### Pre-commit Hook\n\nThe project is configured with a [pre-commit](https://pre-commit.com/) hook to\nenforce as much of the coding standards and style guide as possible. To install\nit into your working copy, run:\n\n```console\npoetry run pre-commit install\n```\n\n### Developing with Local Packages\n\nWhen developing against dependencies or building out new connectors, it can be\nuseful to utilize a local package so that development can be done in the\ndependency and within the servox package at the same time.\n\nTo do so, utilize Poetry Path based dependencies with the `develop = true` flag\nby adding a path reference to the package into the to `tool.poetry.dev-dependencies`\nstanza of the `pyproject.toml` file, and then run `poetry update [dependency name]`.\n\nFor example, if developing on servox and the statesman state machine library in\na working copy in the parent directory, you would add:\n\n```toml\n[tool.poetry.dev-dependencies]\n# ...\nstatesman = {path = "../statesman", develop = true}\n```\n\nAnd then run `poetry update statesman`.\n\nChanges made to the dependency are immediately visible to servox, making it\neasy to develop across package boundaries efficiently.\n\n### Linting and Formatting\n\nThe project is structured to support and enforce consistent, idiomatic code. A\nnumber of tools have been integrated to provide linting and automatic\nreformatting when possible/appropriate.\n\nThis functionality is exposed via tasks in the `Makefile`, Git commit hooks, and\nGitHub Actions.\n\nDuring local development, you may wish to invoke these tools as follows:\n\n* `make lint` - Run the linters and output actionable feedback for conformance\n  with the engineering standards and style of the project.\n* `make format` - Automatically apply changes to the working copy to conform\n  with project standards where possible (e.g., reformatting imports).\n* `make pre-commit` - Run all pre-commit hooks in the manual hook stage. There\n  are a number of standards that are currently soft enforced in the interest of\n  pragmatism. Eventually the set of pre-commit and lint checks will form a\n  perfect union but we are not there yet. Most hooks set in manual mode have to\n  do with fit and finish concerns such as docstring tone/formatting.\n* `make test` - Execute the test suite and generate a code coverage report.\n\nLinting is automatically performed when a new branch is pushed or a PR is opened\nand conformance can be remediated during post-implementation code review.\n\n### Connecting to Optimization APIs\n\nOptimizer API and authentication can configured be inline with your config yaml (servo.yaml)\n\n```\noptimizer:\n  base_url: some_url\n  id: org.domain/app\n  ...\n```\n\nThese details can also be configured via environment variables as highlighted in the following sections.\nNote these sections are mutually exclusive: Opsani API refers to Opsani managed endpoints wheras the Appdynamics\nAPI refers to upcoming FSO Optimization. Which API type is used is dynamically derived during configuration/env var parsing by\nthe [pydantic configuration model (see BaseServoConfiguration.optimizer)](https://github.com/opsani/servox/blob/main/servo/configuration.py).\n\n#### Opsani API\n\nBy default, the servo will connect to the primary Opsani API hosted on\n[https://api.opsani.com](https://api.opsani.com). This behavior can be\noverridden via CLI options and environment variables:\n\n| Config Option        | Environment Variable | Description                                                                                                                                                                | Example                                                         |\n| -------------------- | -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- |\n| `optimizer.base-url` | `OPSANI_BASE_URL`    | Sets an alternate base URL. The path is computed using the provided optimizer id. Useful for staging deployments and integration tests.                                    | `OPSANI_BASE_URL=https://staging-api.opsani.com:3456 servo run` |\n| `optimizer.url`      | `OPSANI_URL`         | Sets an explicit URL target. When given, the base URL is ignored and paths are not computed. Useful in unit tests and workstation development with a partial server stack. | `OPSANI_URL=http://localhost:1234 servo run`                    |\n| `optimizer.id`       | `OPSANI_ID`          | Identifier of the application as provided by the Opsani optimizer provisioned for your application                                                                         | `OPSANI_ID=newco.com/awesome-app1 servo run`                    |\n| `optimizer.token`    | `OPSANI_TOKEN`       | Authentication token as provided by the Opsani optimizer provisioned for your application                                                                                  | `OPSANI_TOKEN=00000000-0000-0000-0000-000000000000 servo run`   |\n\n#### AppDynamics API\n\n| Config Option             | Environment Variable | Description                                                                                                                                                                | Example                                                                    |\n| ------------------------- | -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |\n| `optimizer.base-url`      | `APPD_BASE_URL`      | Sets an alternate base URL. The path is computed using the provided workload and tenant ids.                                                                               | `APPD_BASE_URL=https://optimize-ignite-test.saas.appd-test.com/ servo run` |\n| `optimizer.url`           | `APPD_URL`           | Sets an explicit URL target. When given, the base URL is ignored and paths are not computed. Useful in unit tests and workstation development with a partial server stack. | `APPD_URL=http://localhost:1234 servo run`                                 |\n| `optimizer.tenant_id`     | `APPD_TENANT_ID`     | Identifier of the application tenant                                                                                                                                       | `APPD_TENANT_ID=00000000-0000-0000-0000-000000000000 servo run`            |\n| `optimizer.optimizer_id`  | `APPD_OPTIMIZER_ID`  | Base64 encoded identifier of the workload to be optimized as provided by the provisioned optimizer tenant                                                                  | `APPD_OPTIMIZER_ID=AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA==== servo run`     |\n| `optimizer.client_id`     | `APPD_CLIENT_ID`     | Authentication client ID as provided by the Opsani optimizer provisioned for your application                                                                              | `APPD_CLIENT_ID=<client id text> servo run`                                |\n| `optimizer.client_secret` | `APPD_CLIENT_SECRET` | Authentication client secret as provided by the Opsani optimizer provisioned for your application                                                                          | `APPD_CLIENT_SECRET=<client secret text> servo run`                        |\n\n### Docker & Compose\n\n`Dockerfile` and `docker-compose.yaml` configurations are available in the\nrepository and have been designed to support both development and deployment\nworkflows. Configuration file mounts and environment variables can be used to\ninfluence the behavior of the servo within the container.\n\nThe `SERVO_ENV` build argument controls the target environment for the built\nimage. Building with `SERVO_ENV=production` excludes development packages from\nthe image to reduce size and build time.\n\nPre-built Docker images are available on\n[opsani/servox](https://hub.docker.com/repository/docker/opsani/servox) on\nDocker Hub. The documentation for these images is available within this\nrepository at [docs/README-DOCKER_HUB.md](docs/README-DOCKER_HUB.md).\n\nThe latest release version is available under the `opsani/servox:latest` tag.\nThe `main` development branch is published as the `opsani/servox:edge` tag.\n\nDocker images are built and published to Docker Hub via the\n[Docker GitHub Actions Workflow](.github/workflows/docker.yaml). The workflow\nbuilds branches, published releases, and the `main` integration branch. Pull\nRequests are not published to Docker Hub because as a publicly available\nrepository it could become an attack vector.\n\nGit branches and Docker images have differing naming constraints that impact how\ntag names are computed. For example, Docker tags cannot contain slashes, which\nis a common practice for namespacing branches and tags in Git. As such, slashes\nare converted to hyphens when computing tag names for branches and tags. The\nfull naming constraints on Docker image tags is covered in the [`docker\ntag`](https://docs.docker.com/engine/reference/commandline/tag/#extended-description)\ndocumentation.\n\nPre-built images are built using BuildKit and can be used as the basis for very\nfast customized builds:\n\n```console\n❯ DOCKER_BUILDKIT=1 docker build -t servox --build-arg BUILDKIT_INLINE_CACHE=1 --cache-from opsani/servox:edge .\n```\n\n### Switching Python Interpreters\n\nAfter changing Python interpreter versions you may find that you are "stuck" in\nthe existing virtual environment rather than your new desired version.\n\nThe problem is that Poetry is linked against the previous environment and needs\na nudge to select the new interpreter.\n\nThe project is bound to a local Python version via the `.python-version` file.\nTell Poetry to bind against the locally selected environment via:\n``poetry env use `cat .python-version` ``\n\nWhen upgrading between point releases of the Python interpreter, you may need\nto tear down and recreate your venv:\n``poetry env remove `cat .python-version` && poetry install``\n\n## Testing\n\nTests are implemented using [pytest](https://docs.pytest.org/en/stable/) and\nlive in the `tests` subdirectory. Tests can be executed directly via the\n`pytest` CLI interface (e.g., `pytest tests`) or via `make test`, which\nwill also compute coverage details.\n\nServoX is developed with a heavily test-driven workflow and philosophy. The\nframework strives to provide as much support for robust testing as possible\nand make things that you would think are very hard to test programmatically\nvery simple. You will want to familiarize yourself with what is available,\nthere are tools that can dramatically accelerate your development.\n\n### Test Types\n\nServoX divides the test suite into three types: **Unit**, **Integration**, and\n**System** tests.\n\nTests are identified within the suite in two ways:\n\n1. Use of pytest markers to annotate the tests in code.\n2. File location within the tests/ subdirectory.\n\nUnit tests are the default type and make up the bulk of the suite. They either\nexercise code that carries no outside dependencies or utilize isolation\ntechniques such as mocks and fakes. They are fast and highly effective for\nvalidating defined behavior and catching regressions.\n\nIntegration tests do not interact with an Opsani Optimizer but do interact with\nexternal systems and services such as Kubernetes and Prometheus. It is common to\nutilize a local environment (such as Docker, Compose, kind, or Minikube) or a\ndedicated cloud instance to host the services to interact with. But the focus of\nthe tests are on implementing and verifying the correct behaviors in a\nsupportive environment.\n\nSystem tests are much like integration tests except that theyn are highly\nprescriptive about the environment they are runnuing in and interact with a real\noptimizer backend as much as is practical. System tests sit at the top of the\npyramid and it is expected that there are comparatively few of them, buit they\ndeliver immense value late in a development cycle when code correctness has been\nestablished and deployment environments and compatibility concerns come to the\nforefront.\n\nAll test types can be implemented within any test module as appropriate by\nannotating the tests with pytest markers:\n\n```python\nimport pytest\n\n\n@pytest.mark.integration\nclass TestSomething:\n    ...\n```\n\nTests without a type mark are implicitly designated as unit tests for\nconvenience. When multiple type marks are in effect due to hierarchy, the\nclosest mark to the test node has precedence.\n\nThere are also dedicated directories for integration and system tests at\n`tests/integration` and `tests/system` respectively. These dedicated directories\nare home to cross cutting concerns and scenarios that do not clearly belong to a\nspecific module. Tests in these directories that are marked with other types\nwill trigger an error.\n\n### Running Tests\n\nA key part of any testing workflow is, well, running tests. pytest provides a\nwealth of capabilities out of the box and these have been further augmented with\ncustom pytest-plugins within the suite.\n\nLet\'s start with the basics: executing `pytest` standalone will execute the unit\ntests in `tests`. Running `pytest --verbose` (or -v) will provide a one test per\nline output which can be easier to follow in slower runs.\n\nIndividual files can be run by targetting them by name: `pytest\ntests/connector_test.py`. Individual test functions and container test classes\nwithin the file (known as nodes in pytest parlance) can be addressed with the\n`tests/path/to/test_something.py::TestSomething::test_name` syntax.\n\nTests can also be flexibly selected by marks and naming patterns. Invoking\n`pytest -m asyncio -k sleep` will select all tests with the asyncio mark and\nhave the word "sleep" in their name. These arguments support a matching syntax,\nlook into the pytest docs for details.\n\nThe ServoX test types have specific affordances exposed through pytest. Running\n`pytest -T integration` will select and run all integration tests, but deselect\nall other types. The `-T` also known as `--type` flag supports stem matching for\nbrevity: `pytest -T u` will select the unit tests.\n\nBecause they are slow and require supplemental configuration, integration and\nsystem tests are skipped by default. They can be enabled via the\n`-I, --integration` and `-S, --system` switches, respectively. Note the difference\nin behavior between the flags: `pytest -I -S` will result in all the tests being\nselected for run whereas `pytest -T sys` targets the system tests exclusively.\nOnce the `-I, -S` flags have been used to enable the tests, they can be further\nfiltered using `-m` and `-k`. If you are thoughtful about how you name your\ntests and leverage marks when it makes sense, it can become very easy to run\ninteresting subsets of the suite.\n\nBy default, pytest uses output buffering techniques to capture what is written\nto stdout and stderr. This can become annoying if you are trying to introspect\nstate, print debugging info, or get a look at the servo logs. You can suppress\noutput capture via the `-s` switch. This is typically only recommended when\nrunning a small number of tests because the output quickly becomes\nincomprehensible.\n\nIf you are working through a set of failures, you can rerun the tests that\nfailed on the last run via the `--lf, --last-failed` flag. The `--ff,\n--failed-first` flag will rerun all of the tests, but run the previously failed\ntests first. Similarly, `--nf, --new-first` will run the full suite but\nprioritize new files. The `pytest-picked` plugin provides additional targeting\nbased on git working copy status -- running `pytest --picked` will find unstaged\nfiles to run.\n\nFinally, the `--sw, --stepwise` and `--sw-skip, --stepwise-skip` flags allow you\nto methodically working through a stack of failures by resuming from your last\nfailure and then halting at the next one.\n\n### Makefile Tasks\n\nTest automation tasks are centralized into the `Makefile`. There are a number of\ntesting  tasks availble including:\n\n* `make test` - Run all available tests.\n* `make test-unit` - Run unit tests.\n* `make test-integration` - Run integration tests.\n* `make test-system` - Run system tests.\n* `make test-coverage` - Run all available tests and generate code coverage\n  report.\n* `make test-kubeconfig` - Generate a kubeconfig file at tests/kubeconfig. See\n  details in [Integration Testing](#integration-testing) below.\n* `make autotest` - Automatically run tests based on filesystem changes.\n\nTesting tasks will run in subprocess distributed mode by default (see below).\n\n### Integration Testing\n\nThe test suite includes support for integration tests for running tests against\nremote system components such as a Kubernetes cluster or Prometheus deployment.\nIntegration tests require a [kubeconfig](https://kubernetes.io/docs/concepts/configuration/organize-cluster-access-kubeconfig/)\nfile at `tests/kubeconfig`.\n\nBy convention, the default integration testing cluster is named `kubetest`\nand the `make test-kubeconfig` task is provided to export the cluster details\nfrom your primary kubeconfig, ensuring isolation.\n\nInteraction with the Kubernetes cluster is supported by the most excellent\n[kubetest](https://kubetest.readthedocs.io/en/latest/) library that provides\nfixtures, markers, and various testing utilities on top of pytest.\n\nTo run the integration tests, execute `pytest -I` to enable the\nmarker. Integration tests are much slower than the unit test suite\nand should be designed to balance coverage and execution time.\n\nSystem tests are enabled by running `pytest -S`. Systems tests are very similar\nto integration tests in implementation and performance, but differ in that they\nare prescriptively bound to particular deployment environments and interact with\nan actual\n\nTests can also be run in cluster by packaging a development container and\ndeploying it. The testing harness will detect the in-cluster state and utilize\nthe active service account.\n\n### Continuous Integration\n\nThe project is configured to run CI on unit tests for all branches, tags, and\npull requests opened against the repository. CI for integration and system tests\nis constrained by a few rules because they are so resource intensive and may be\nundesirable during experimental developmenmt or integrating multiple branches\ntogether.\n\nIntegration and system tests are run if any of the following conditions are\nmet:\n\n* A push is made to `main`.\n* A push is made to a branch prefixed with `release/`.\n* A push is made to a branch prefixed with `bugfix/`.\n* A tag is pushed.\n* A push is made to a branch with an open pull request.\n* The commit message includes `#test:integration` and/or\n  `#test:system`.\n\nThe default unit test job that is executed for all pushes generates code\ncoverage reports and XML/HTML report artifacts that are attached to the run. The\nintegration and system test jobs report on the runtime duration of the tests to\nhelp identify and manage runtime creep.\n\nThe unit, integration, and system test jobs all utilize the `pytest-xdist`\nplugin to split the test suite up across a set of subprocesses. This is\ndiscussed in the [Distributed Testing](#distributed-testing) section.\n\nDocker images are built and pushed to Docker Hub automatically for all\npushed refs. Release tags are handled automatically and the\n`opsani/servox:latest` tag is advanced when a new version is released. The\n`main` branch is built and pushed to the `opsani/servox:edge` tag.\n\n#### Distributed Testing\n\nThe project is configured to leverage locally distributed test execution by\ndefault. Servo workloads are heavily I/O bound and spend quite a bit\nof time awaiting data from external services. This characteristic makes tests\ninherently slower but also makes them very well suited for parallel execution.\nThe `Makefile` tasks and GitHub actions are configured to leverage a subprocess\ndivide & conquer strategy to speed things up.\n\nThis functionality is provided by [pytest-xdist](https://docs.pytest.org/en/3.0.1/xdist.html).\n\n### Manifest Templating\n\nAll manifests loaded through kubetest support Mustache templating.\nA context dictionary is provided to the template that includes references to all\nKubernetes resources that have been loaded at render time. The `namespace` and\n`objs` are likely to be the most interesting.\n\n### Startup Banner\n\nJust for fun, ServoX generates an ASCII art banner at startup. The font is\nrandomized from a painstakingly selected set of style that represent the ServoX\nvibe. The output color is then randomized and has a 50/50 shot of being rendered\nas a rainbow or a randomly selected flat output color.\n\nDon\'t like serendipity?\n\nYou can take control of the banner output with two environment variables:\n\n* `SERVO_BANNER_FONT`: Name of the [Figlet](http://www.figlet.org/fontdb.cgi)\n  font to render the banner in.\n* `SERVO_BANNER_COLOR`: The color to use when rendering the banner. Valid\n  options are:\n  * `RED`\n  * `GREEN`\n  * `YELLOW`\n  * `BLUE`\n  * `MAGENTA`\n  * `CYAN`\n  * `RAINBOW`\n\n## Release Process\n\n1. Use [Semantic Versioning](https://semver.org/) to choose a release number.\n   Run `poetry version [major | minor | patch]` to increment the version. This\n   will update the version number as `version` in  section `[tool.poetry]` of\n   the [pyproject.toml](pyproject.toml) file.\n1. Minor version release series each have a unique cryptonym. If incrementing\n   the major or minor version, choose a new cryptonym for the release series and\n   set it as the value of `__cryptonym__` in\n   [servo/\\_\\_init\\_\\_.py](servo/__init__.py).\n1. Update [CHANGELOG.md](CHANGELOG.md) with the notable changes of the release.\n   See the introduction for guidance on the form and format. Follow the pattern\n   of prior releases for the release title, generally `[x.y.z] "cryptonym" -\n   YYYY-MM-DD`.\n1. Commit changes and make sure all tests pass.\n1. [Draft a new release on\n   GitHub](https://github.com/opsani/servox/releases/new) with the following\n   settings:\n    * Tag version: set to vX.Y.Z (e.g., `v0.9.5`) again the `main` branch.\n    * Release title: set to `vX.Y.Z "<cryptonym>"`\n    * Description: judiciously paste the change log since the prior release\n1. Publish the release, wait for CI actions to complete. Release artifacts are\n   automatically created and published via the GitHub Actions `release.yml`\n   workflow. The framework is packaged into a Python library and published to\n   [PyPi](https://pypi.org/project/servox/) and Docker images are built and\n   published to\n   [Docker Hub](https://hub.docker.com/repository/docker/opsani/servox).\n1. Verify the new image, with tag `vX.Y.Z`, has been published in [Docker\n   Hub](https://hub.docker.com/repository/docker/opsani/servox/tags).\n\n## Contributing\n\nPlease reach out to support at opsani.com.\n\n## License\n\nServoX is distributed under the terms of the Apache 2.0 Open Source license.\n\nA copy of the license is provided in the [LICENSE](LICENSE) file at the root of\nthe repository.\n',
     'author': 'Blake Watters',
     'author_email': 'blake@opsani.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://opsani.com/',
```

### Comparing `servox-2.2.3/PKG-INFO` & `servox-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servox
-Version: 2.2.3
+Version: 2.2.4
 Summary: Opsani Servo: The Next Generation
 Home-page: https://opsani.com/
 License: Apache-2.0
 Author: Blake Watters
 Author-email: blake@opsani.com
 Requires-Python: >=3.8.1,<=3.9.11
 Classifier: License :: OSI Approved :: Apache Software License
```

