# Comparing `tmp/duplocloud-client-0.0.5.tar.gz` & `tmp/duplocloud-client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duplocloud-client-0.0.5.tar", last modified: Sat Apr  8 04:26:18 2023, max compression
+gzip compressed data, was "duplocloud-client-0.0.6.tar", last modified: Mon Apr 17 18:36:26 2023, max compression
```

## Comparing `duplocloud-client-0.0.5.tar` & `duplocloud-client-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:26:18.633487 duplocloud-client-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:26:18.629487 duplocloud-client-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:26:18.629487 duplocloud-client-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-08 04:26:18.633487 duplocloud-client-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-08 04:26:18.633487 duplocloud-client-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:26:18.629487 duplocloud-client-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:26:18.629487 duplocloud-client-0.0.5/src/duplo_resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/src/duplo_resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/src/duplo_resource/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/src/duplo_resource/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/src/duplo_resource/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:26:18.633487 duplocloud-client-0.0.5/src/duplocloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/src/duplocloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/src/duplocloud/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/src/duplocloud/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/src/duplocloud/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/src/duplocloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-08 04:25:43.000000 duplocloud-client-0.0.5/src/duplocloud/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:26:18.633487 duplocloud-client-0.0.5/src/duplocloud_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-08 04:26:18.000000 duplocloud-client-0.0.5/src/duplocloud_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-08 04:26:18.000000 duplocloud-client-0.0.5/src/duplocloud_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 04:26:18.000000 duplocloud-client-0.0.5/src/duplocloud_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-08 04:26:18.000000 duplocloud-client-0.0.5/src/duplocloud_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-08 04:26:18.000000 duplocloud-client-0.0.5/src/duplocloud_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-08 04:26:18.000000 duplocloud-client-0.0.5/src/duplocloud_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:36:26.415969 duplocloud-client-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:36:26.411969 duplocloud-client-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:36:26.411969 duplocloud-client-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-17 18:36:26.415969 duplocloud-client-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-17 18:36:26.415969 duplocloud-client-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:36:26.411969 duplocloud-client-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:36:26.411969 duplocloud-client-0.0.6/src/duplo_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplo_resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplo_resource/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplo_resource/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplo_resource/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:36:26.411969 duplocloud-client-0.0.6/src/duplocloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplocloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplocloud/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplocloud/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplocloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplocloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplocloud/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:36:26.415969 duplocloud-client-0.0.6/src/duplocloud_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-17 18:36:26.000000 duplocloud-client-0.0.6/src/duplocloud_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-17 18:36:26.000000 duplocloud-client-0.0.6/src/duplocloud_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:36:26.000000 duplocloud-client-0.0.6/src/duplocloud_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-17 18:36:26.000000 duplocloud-client-0.0.6/src/duplocloud_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-17 18:36:26.000000 duplocloud-client-0.0.6/src/duplocloud_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 18:36:26.000000 duplocloud-client-0.0.6/src/duplocloud_client.egg-info/top_level.txt
```

### Comparing `duplocloud-client-0.0.5/.github/workflows/publish.yaml` & `duplocloud-client-0.0.6/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.5/.github/workflows/test.yml` & `duplocloud-client-0.0.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.5/CONTRIBUTING.md` & `duplocloud-client-0.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.5/PKG-INFO` & `duplocloud-client-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplocloud-client
-Version: 0.0.5
+Version: 0.0.6
 Summary: Generic DuploClient for Python apps.
 Home-page: https://github.com/duplocloud/py-client
 Author: Kelly Ferrone
 Author-email: kelly@duplocloud.net
 Project-URL: Bug Tracker, https://github.com/duplocloud/py-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplocloud-client-0.0.5/setup.cfg` & `duplocloud-client-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.5/src/duplo_resource/service.py` & `duplocloud-client-0.0.6/src/duplo_resource/user.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from duplocloud.client import DuploClient
 from duplocloud.resource import DuploResource
 from duplocloud.errors import DuploError
 
-class DuploService(DuploResource):
-  
+class DuploUser(DuploResource):
   def __init__(self, duplo: DuploClient):
     super().__init__(duplo)
     self.tenent_svc = duplo.service('tenant')
   
-  def list(self):
-    """Retrieve a list of all services in a tenant."""
-    tenant_id = self.get_tenant()["TenantId"]
-    return self.duplo.get(f"subscriptions/{tenant_id}/GetReplicationControllers")
-  
-  def find(self, service_name):
-    """Find a service by name."""
+  def add_tenant(self, username, tenant):
+    """Retrieve a list of all users in the Duplo system."""
+    tenant_id = self.tenent_svc.find(tenant)["TenantId"]
+    res = self.duplo.post("admin/UpdateUserAccess", {
+      "Policy": { "IsReadOnly": None },
+      "Username": username,
+      "TenantId": tenant_id
+    })
+    # check http response is 204
+    if res.status_code != 204:
+      raise DuploError(f"Failed to add user '{username}' to tenant '{tenant}'", res["status_code"])
+    else:
+      return f"User '{username}' added to tenant '{tenant}'"
+
+  def find(self, username):
+    """Find a User by their username."""
     try:
-      return [s for s in self.list() if s["Name"] == service_name][0]
+      return [u for u in self.list() if u["Username"] == username][0]
     except IndexError:
-      raise DuploError(f"Service '{service_name}' not found", 404)
-
-  def update_image(self, service_name, image):
-    tenant_id = self.get_tenant()["TenantId"]
-    service = self.find(service_name)
-    allocation_tags = service["Template"]["AllocationTags"]
-    data = {
-      "Name": service_name,
-      "Image": image,
-      "AllocationTags": allocation_tags
-    }
-    return self.duplo.post(f"subscriptions/{tenant_id}/ReplicationControllerChange", data)
+      raise DuploError(f"User '{username}' not found", 404)
+    
+  def list(self):
+    """Retrieve a list of all users in the Duplo system."""
+    return self.duplo.get("admin/GetAllUserRoles")
```

### Comparing `duplocloud-client-0.0.5/src/duplo_resource/tenant.py` & `duplocloud-client-0.0.6/src/duplo_resource/tenant.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.5/src/duplocloud/cli.py` & `duplocloud-client-0.0.6/src/duplocloud/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 def main():
   env, args = load_env()
   client = DuploClient(
     host=env.host,
     token=env.token,
-    tenant=env.tenant
+    tenant_name=env.tenant,
   )
   service = client.service(env.service)
   service.exec(env.subcmd, args)
 
 def load_env():
   """Get the environment variables for the Duplo session."""
   parser = argparse.ArgumentParser(
```

### Comparing `duplocloud-client-0.0.5/src/duplocloud/client.py` & `duplocloud-client-0.0.6/src/duplocloud/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,19 +21,19 @@
       class DuploSomeService(DuploResource):
         def __init__(self, duplo: DuploClient):
           super().__init__(duplo)
           self.tenent_svc = duplo.service('tenant')
       ```
   """
     
-  def __init__(self, host, token, tenant="default", args=[]) -> None:
+  def __init__(self, host, token, tenant_name="default", args=[]) -> None:
     self.host = host
     self.timeout = 10
     self.args = args
-    self.tenant = tenant
+    self.tenant_name = tenant_name
     self.headers = {
       'Content-Type': 'application/json',
       'Authorization': f"Bearer {token}"
     }
   
   def __str__(self) -> str:
      return f"""
```

### Comparing `duplocloud-client-0.0.5/src/duplocloud/resource.py` & `duplocloud-client-0.0.6/src/duplocloud/resource.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.5/src/duplocloud_client.egg-info/PKG-INFO` & `duplocloud-client-0.0.6/src/duplocloud_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplocloud-client
-Version: 0.0.5
+Version: 0.0.6
 Summary: Generic DuploClient for Python apps.
 Home-page: https://github.com/duplocloud/py-client
 Author: Kelly Ferrone
 Author-email: kelly@duplocloud.net
 Project-URL: Bug Tracker, https://github.com/duplocloud/py-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplocloud-client-0.0.5/src/duplocloud_client.egg-info/SOURCES.txt` & `duplocloud-client-0.0.6/src/duplocloud_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

