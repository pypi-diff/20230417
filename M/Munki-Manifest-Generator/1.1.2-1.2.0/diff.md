# Comparing `tmp/Munki-Manifest-Generator-1.1.2.tar.gz` & `tmp/Munki-Manifest-Generator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Munki-Manifest-Generator-1.1.2.tar", last modified: Fri Mar  3 13:14:24 2023, max compression
+gzip compressed data, was "Munki-Manifest-Generator-1.2.0.tar", last modified: Mon Apr 17 08:37:15 2023, max compression
```

## Comparing `Munki-Manifest-Generator-1.1.2.tar` & `Munki-Manifest-Generator-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:14:24.341097 Munki-Manifest-Generator-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-03 13:14:11.000000 Munki-Manifest-Generator-1.1.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:14:24.341097 Munki-Manifest-Generator-1.1.2/Munki_Manifest_Generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-03-03 13:14:24.000000 Munki-Manifest-Generator-1.1.2/Munki_Manifest_Generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-03 13:14:24.000000 Munki-Manifest-Generator-1.1.2/Munki_Manifest_Generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 13:14:24.000000 Munki-Manifest-Generator-1.1.2/Munki_Manifest_Generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-03 13:14:24.000000 Munki-Manifest-Generator-1.1.2/Munki_Manifest_Generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-03 13:14:24.000000 Munki-Manifest-Generator-1.1.2/Munki_Manifest_Generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-03 13:14:24.000000 Munki-Manifest-Generator-1.1.2/Munki_Manifest_Generator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-03-03 13:14:24.341097 Munki-Manifest-Generator-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-03-03 13:14:11.000000 Munki-Manifest-Generator-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:14:24.341097 Munki-Manifest-Generator-1.1.2/munki_manifest_generator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:14:24.341097 Munki-Manifest-Generator-1.1.2/munki_manifest_generator/azstorage/
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-03-03 13:14:11.000000 Munki-Manifest-Generator-1.1.2/munki_manifest_generator/azstorage/az_storage_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-03-03 13:14:11.000000 Munki-Manifest-Generator-1.1.2/munki_manifest_generator/azstorage/az_storage_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-03 13:14:11.000000 Munki-Manifest-Generator-1.1.2/munki_manifest_generator/get_device_catalogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:14:24.341097 Munki-Manifest-Generator-1.1.2/munki_manifest_generator/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-03 13:14:11.000000 Munki-Manifest-Generator-1.1.2/munki_manifest_generator/graph/get_authentication_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-03-03 13:14:11.000000 Munki-Manifest-Generator-1.1.2/munki_manifest_generator/graph/get_device_group_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-03-03 13:14:11.000000 Munki-Manifest-Generator-1.1.2/munki_manifest_generator/graph/get_user_group_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-03-03 13:14:11.000000 Munki-Manifest-Generator-1.1.2/munki_manifest_generator/graph/make_api_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-03-03 13:14:11.000000 Munki-Manifest-Generator-1.1.2/munki_manifest_generator/graph/obtain_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-03-03 13:14:11.000000 Munki-Manifest-Generator-1.1.2/munki_manifest_generator/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-03 13:14:11.000000 Munki-Manifest-Generator-1.1.2/munki_manifest_generator/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-03 13:14:11.000000 Munki-Manifest-Generator-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-03 13:14:24.341097 Munki-Manifest-Generator-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:37:15.130853 Munki-Manifest-Generator-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-17 08:37:03.000000 Munki-Manifest-Generator-1.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:37:15.130853 Munki-Manifest-Generator-1.2.0/Munki_Manifest_Generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-04-17 08:37:15.000000 Munki-Manifest-Generator-1.2.0/Munki_Manifest_Generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-17 08:37:15.000000 Munki-Manifest-Generator-1.2.0/Munki_Manifest_Generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:37:15.000000 Munki-Manifest-Generator-1.2.0/Munki_Manifest_Generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-17 08:37:15.000000 Munki-Manifest-Generator-1.2.0/Munki_Manifest_Generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 08:37:15.000000 Munki-Manifest-Generator-1.2.0/Munki_Manifest_Generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-17 08:37:15.000000 Munki-Manifest-Generator-1.2.0/Munki_Manifest_Generator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-04-17 08:37:15.130853 Munki-Manifest-Generator-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-04-17 08:37:03.000000 Munki-Manifest-Generator-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:37:15.130853 Munki-Manifest-Generator-1.2.0/munki_manifest_generator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:37:15.130853 Munki-Manifest-Generator-1.2.0/munki_manifest_generator/azstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-04-17 08:37:03.000000 Munki-Manifest-Generator-1.2.0/munki_manifest_generator/azstorage/az_storage_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-17 08:37:03.000000 Munki-Manifest-Generator-1.2.0/munki_manifest_generator/azstorage/az_storage_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-17 08:37:03.000000 Munki-Manifest-Generator-1.2.0/munki_manifest_generator/get_device_catalogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:37:15.130853 Munki-Manifest-Generator-1.2.0/munki_manifest_generator/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-04-17 08:37:03.000000 Munki-Manifest-Generator-1.2.0/munki_manifest_generator/graph/concurrent_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-17 08:37:03.000000 Munki-Manifest-Generator-1.2.0/munki_manifest_generator/graph/get_authentication_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-17 08:37:03.000000 Munki-Manifest-Generator-1.2.0/munki_manifest_generator/graph/get_device_group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-17 08:37:03.000000 Munki-Manifest-Generator-1.2.0/munki_manifest_generator/graph/get_user_group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-17 08:37:03.000000 Munki-Manifest-Generator-1.2.0/munki_manifest_generator/graph/make_api_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-17 08:37:03.000000 Munki-Manifest-Generator-1.2.0/munki_manifest_generator/graph/obtain_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-17 08:37:03.000000 Munki-Manifest-Generator-1.2.0/munki_manifest_generator/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-04-17 08:37:03.000000 Munki-Manifest-Generator-1.2.0/munki_manifest_generator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-17 08:37:03.000000 Munki-Manifest-Generator-1.2.0/munki_manifest_generator/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-17 08:37:03.000000 Munki-Manifest-Generator-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-17 08:37:15.134853 Munki-Manifest-Generator-1.2.0/setup.cfg
```

### Comparing `Munki-Manifest-Generator-1.1.2/LICENSE` & `Munki-Manifest-Generator-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Munki-Manifest-Generator-1.1.2/Munki_Manifest_Generator.egg-info/PKG-INFO` & `Munki-Manifest-Generator-1.2.0/Munki_Manifest_Generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: Munki-Manifest-Generator
-Version: 1.1.2
+Version: 1.2.0
 Summary: Tool to create and update Munki manifests for devices managed in Intune
 Home-page: https://github.com/almenscorner/munki-manifest-generator
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/munki-manifest-generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/78877636/191977945-eb1c4e6f-85f7-429d-afa9-9acfc43d33c1.png" alt="mmg logo"/>
 </p>
 <p align="center">
```

### Comparing `Munki-Manifest-Generator-1.1.2/Munki_Manifest_Generator.egg-info/SOURCES.txt` & `Munki-Manifest-Generator-1.2.0/Munki_Manifest_Generator.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 Munki_Manifest_Generator.egg-info/PKG-INFO
 Munki_Manifest_Generator.egg-info/SOURCES.txt
 Munki_Manifest_Generator.egg-info/dependency_links.txt
 Munki_Manifest_Generator.egg-info/entry_points.txt
 Munki_Manifest_Generator.egg-info/requires.txt
 Munki_Manifest_Generator.egg-info/top_level.txt
 munki_manifest_generator/get_device_catalogs.py
+munki_manifest_generator/logger.py
 munki_manifest_generator/main.py
 munki_manifest_generator/manifest.py
 munki_manifest_generator/azstorage/az_storage_actions.py
 munki_manifest_generator/azstorage/az_storage_clients.py
+munki_manifest_generator/graph/concurrent_batch.py
 munki_manifest_generator/graph/get_authentication_token.py
 munki_manifest_generator/graph/get_device_group_membership.py
 munki_manifest_generator/graph/get_user_group_membership.py
 munki_manifest_generator/graph/make_api_request.py
 munki_manifest_generator/graph/obtain_access_token.py
```

### Comparing `Munki-Manifest-Generator-1.1.2/PKG-INFO` & `Munki-Manifest-Generator-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: Munki-Manifest-Generator
-Version: 1.1.2
+Version: 1.2.0
 Summary: Tool to create and update Munki manifests for devices managed in Intune
 Home-page: https://github.com/almenscorner/munki-manifest-generator
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/munki-manifest-generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/78877636/191977945-eb1c4e6f-85f7-429d-afa9-9acfc43d33c1.png" alt="mmg logo"/>
 </p>
 <p align="center">
```

### Comparing `Munki-Manifest-Generator-1.1.2/README.md` & `Munki-Manifest-Generator-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `Munki-Manifest-Generator-1.1.2/munki_manifest_generator/azstorage/az_storage_actions.py` & `Munki-Manifest-Generator-1.2.0/munki_manifest_generator/azstorage/az_storage_actions.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,98 +8,135 @@
 import plistlib
 
 from munki_manifest_generator.azstorage.az_storage_clients import (
     az_blob_client,
     az_container_client,
 )
 from munki_manifest_generator.get_device_catalogs import get_device_catalogs
+from munki_manifest_generator.logger import logger
 
 
-def get_current_manifest_blobs(connection_string, container_name):
+def get_current_manifest_blobs(connection_string: str, container_name: str) -> list:
     """Returns a list of the blob names in the container."""
     CURRENT_MANIFESTS = []
     try:
         # Create the BlobServiceClient object which will be used to create a container client
         container_client = az_container_client(connection_string, container_name)
         # List the blobs in the container
         source_blob_list = container_client.list_blobs(name_starts_with="manifests/")
         # Get the name of each blob
         for blob in source_blob_list:
             blob_name = blob.name.rsplit("/", 1)[1]
             CURRENT_MANIFESTS.append(blob_name)
 
     except Exception as ex:
-        print("Error: " + str(ex))
+        logger.error("Error: " + str(ex))
 
     return CURRENT_MANIFESTS
 
 
-def create_manifest_blob(connection_string, container_name, file_name, device, test):
+def create_manifest_blob(connection_string: str, container_name: str, file_name: str, device: dict, test: bool):
     """Creates a blob with the given file name and data."""
     try:
         local_path = "./"
         upload_file_path = os.path.join(local_path, file_name)
 
         with open(upload_file_path, "wb") as _f:
             plistlib.dump(device.__dict__, _f)
 
         blob_client = az_blob_client(connection_string, container_name, file_name)
 
         if not test:
             with open(upload_file_path, "rb") as data:
-                blob_client.upload_blob(data)
+                blob_client.upload_blob(data, overwrite=True)
         os.remove(upload_file_path)
 
     except Exception as ex:
-        print("Error: " + str(ex))
+        logger.error("Error: " + str(ex))
 
 
 def delete_manifest_blob(
-    connection_string, container_name, groups, serial_numbers, safe_manifest, test
+    connection_string: str,
+    container_name: str,
+    groups: list,
+    serial_numbers: list,
+    safe_manifest: str,
+    test: bool,
+    current_manifest_list: list,
 ):
     """Deletes blobs in the container if the device is not in Intune."""
+
     try:
-        # Get the list of blobs in the container
-        current_manifests = get_current_manifest_blobs(
-            connection_string, container_name
-        )
         # Get list of group names
-        groups = [val for list in groups for key, val in list.items() if key == "name"]
+        groups = [val for val in groups for key, val in val.items() if key == "name"]
         delete_manifests = []
         if safe_manifest:
             do_not_delete_manifest = safe_manifest.lower().split(",")
         else:
             do_not_delete_manifest = []
 
-        for manifest in current_manifests:
-            # If the manifest is not in the list of serial numbers, is not in the list of groups, is not site_defualt, and is not in the list of safe manifests, add it to the list of manifests to delete
+        for manifest in current_manifest_list:
+            # If the manifest is not in the list of serial numbers,
+            # is not in the list of groups, is not site_default,
+            # and is not in the list of safe manifests, add it to the list of manifests to delete
             if (
                 (manifest not in serial_numbers)
                 and (manifest not in groups)
                 and (manifest != "site_default")
                 and (manifest.lower() not in do_not_delete_manifest)
             ):
                 delete_manifests.append(manifest)
 
-                blob_client = az_blob_client(
-                    connection_string, container_name, manifest
-                )
+                blob_client = az_blob_client(connection_string, container_name, manifest)
                 if not test:
                     blob_client.delete_blob()
 
         if delete_manifests:
-            print(("{0:-^{1}}".format(str(len(delete_manifests)) + " deleted manifests", 90)))
-            print("\n".join(delete_manifests))
+            logger.info(("{0:-^{1}}".format(str(len(delete_manifests)) + " deleted manifests", 90)))
+            logger.info(", ".join(delete_manifests))
+            logger.info("-" * 90)
 
     except Exception as ex:
-        print("Error: " + str(ex))
+        logger.error("Error: " + str(ex))
+
+
+def update_current_upn(connection_string: str, container_name: str, serial_number: str, upn: str, old_user: str, test: bool):
+    """Updates the UPN in the manifest for the given serial number."""
+
+    try:
+        logger.info("[%s] Updating user to %s from %s", serial_number, upn, old_user)
+        local_path = "./"
+        download_file_path = os.path.join(local_path, serial_number)
+        blob_client = az_blob_client(connection_string, container_name, serial_number)
 
+        with open(download_file_path, "wb") as _f:
+            blob_data = blob_client.download_blob()
+            data = blob_data.readall()
+            plist_data = plistlib.loads(data)
+
+        plist_data["user"] = upn
+
+        with open(download_file_path, "wb") as _f:
+            plistlib.dump(plist_data, _f)
 
-def get_current_device_manifest(connection_string, container_name, serial_number):
+        blob_client = az_blob_client(connection_string, container_name, serial_number)
+
+        if not test:
+            with open(download_file_path, "rb") as data:
+                blob_client.upload_blob(data, overwrite=True)
+
+        os.remove(download_file_path)
+
+    except Exception as ex:
+        logger.error("Error: " + str(ex))
+
+
+def get_current_device_manifest(connection_string: str, container_name: str, serial_number: str) -> dict:
     """Returns the current manifest for the given serial number."""
+
     try:
         local_path = "./"
         download_file_path = os.path.join(local_path, serial_number)
         blob_client = az_blob_client(connection_string, container_name, serial_number)
 
         with open(download_file_path, "wb") as _f:
             blob_data = blob_client.download_blob()
@@ -107,105 +144,99 @@
             plist_data = plistlib.loads(data)
 
         os.remove(download_file_path)
 
         return plist_data
 
     except Exception as ex:
-        print("Error: " + str(ex))
+        logger.error("Error: " + str(ex))
 
 
 def update_manifest_blob(
-    connection_string,
-    container_name,
-    file_name,
-    device_manifest,
-    group_membership,
-    groups,
-    test,
-    default_catalog,
-):
+    connection_string: str,
+    container_name: str,
+    file_name: str,
+    device_manifest: dict,
+    group_membership: list,
+    groups: list,
+    test: bool,
+    default_catalog: str,
+    current_manifest_list: list,
+) -> list:
     """Updates the manifest with the given file name and data."""
+
     try:
         local_path = "./"
         download_file_path = os.path.join(local_path, file_name)
 
-        current_manifests = get_current_manifest_blobs(
-            connection_string, container_name
-        )
-
         blob_client = az_blob_client(connection_string, container_name, file_name)
 
         with open(download_file_path, "wb") as _f:
             blob_data = blob_client.download_blob()
             data = blob_data.readall()
             plist_data = plistlib.loads(data)
             add_catalogs = False
             add_manifests = []
             remove_manifests = []
 
             # Get updates to device catalogs
-            add_catalog = get_device_catalogs(
-                groups, device_manifest, default_catalog, add_catalogs=True
-            )
+            add_catalog = get_device_catalogs(groups, device_manifest, default_catalog, add_catalogs=True)
             # If updated catalogs are not equal to the current catalogs, update the manifest
             if add_catalog != device_manifest.catalogs:
                 device_manifest.catalogs = add_catalog
                 add_catalogs = True
 
             # Get updates to device manifests
             for manifest in device_manifest.included_manifests:
                 # If manifest is not in the device's current manifest list, add it to the list of manifests to add
                 if manifest not in plist_data["included_manifests"]:
                     add_manifests.append(manifest)
                 # If manifest is in the current manifest list, remove it from the list of manifests to add
-                if manifest not in current_manifests:
-                    print("Manifest " + manifest + " not found, skipping")
-                    # If the manifest not in the current manifest list, but in the device manifest list, add it to the list of manifests to remove
+                if manifest not in current_manifest_list:
+                    logger.info("[%s] Manifest %s not found, skipping", file_name, manifest)
+                    # If the manifest not in the current manifest list,
+                    # but in the device manifest list, add it to the list of manifests to remove
                     if manifest in device_manifest.included_manifests:
                         device_manifest.included_manifests.remove(manifest)
                         remove_manifests.append(manifest)
-                    # If the manifest is not in the current manifest list, but in the add manifest list, remove it from the add manifest list
+                    # If the manifest is not in the current manifest list, but in the add manifest list,
+                    # remove it from the add manifest list
                     if manifest in add_manifests:
                         add_manifests.remove(manifest)
 
             # Check if the device is a member of any AAD group based included manifest but not the AAD group
             for group_manifest in plist_data["included_manifests"]:
-                # If the AAD group based manifest is not in the device's membership list, add it to the list of manifests to remove
-                if (group_manifest not in group_membership) and (
-                    group_manifest != "site_default"
-                ):
+                # If the AAD group based manifest is not in the device's membership list,
+                # add it to the list of manifests to remove
+                if (group_manifest not in group_membership) and (group_manifest != "site_default"):
                     remove_manifests.append(group_manifest)
 
             # If there are manifests to remove, remove them
             if remove_manifests:
                 for manifest in remove_manifests:
                     plist_data["included_manifests"].remove(manifest)
-                    device_manifest.included_manifests = plist_data[
-                        "included_manifests"
-                    ]
+                    device_manifest.included_manifests = plist_data["included_manifests"]
 
             # Check if there are catalogs to remove
-            remove_catalogs = get_device_catalogs(
-                groups, device_manifest, default_catalog, remove_catalogs=True
-            )
+            remove_catalogs = get_device_catalogs(groups, device_manifest, default_catalog, remove_catalogs=True)
 
             plistlib.dump(device_manifest.__dict__, _f)
 
         if add_manifests or add_catalogs or remove_manifests or remove_catalogs:
-            print("Manifests or catalogs changed, updating")
+            # logger.info("[%s] Manifests or catalogs changed, updating..." % file_name)
             if add_manifests:
-                print("Manifests: \n" + " - " + "\n - ".join(add_manifests))
+                logger.info("[%s] " % file_name + "New manifest list: " + ", ".join(add_manifests))
             if add_catalogs:
-                print("Catalogs: \n" + " - " + "\n - ".join(add_catalog))
+                logger.info("[%s] " % file_name + "New catalog list: " + ", ".join(add_catalog))
             if remove_manifests:
-                print("Manifests removed: \n" + " - " + "\n - ".join(remove_manifests))
+                logger.info("[%s] " % file_name + "Manifests removed: " + ", ".join(remove_manifests))
             if remove_catalogs:
-                print("Catalogs removed: \n" + " - " + "\n - ".join(remove_catalogs))
+                logger.info("[%s] " % file_name + "Catalogs removed: " + ", ".join(remove_catalogs))
+
             if not test:
                 with open(download_file_path, "rb") as data:
                     blob_client.upload_blob(data, overwrite=True)
 
         os.remove(download_file_path)
 
     except Exception as ex:
-        print("Error: " + str(ex))
+        logger.error("Error: " + str(ex))
```

### Comparing `Munki-Manifest-Generator-1.1.2/munki_manifest_generator/azstorage/az_storage_clients.py` & `Munki-Manifest-Generator-1.2.0/munki_manifest_generator/azstorage/az_storage_clients.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 #!/usr/bin/env python3
 
 """
 This module is used to create clients for Azure Storage.
 """
 
-from azure.storage.blob import BlobServiceClient
+from azure.storage.blob import BlobServiceClient, ContainerClient
+from munki_manifest_generator.logger import logger
 
 
-def az_container_client(connection_string, container_name):
+def az_container_client(connection_string: str, container_name: str) -> ContainerClient:
     """Create a container client to get the list of files in the container."""
     try:
-        blob_source_service_client = BlobServiceClient.from_connection_string(
-            connection_string
-        )
-        container_client = blob_source_service_client.get_container_client(
-            container_name
-        )
+        blob_source_service_client = BlobServiceClient.from_connection_string(connection_string)
+        container_client = blob_source_service_client.get_container_client(container_name)
 
         return container_client
 
     except Exception as ex:
-        print("Error: " + str(ex))
+        logger.error("Error: " + str(ex))
 
 
-def az_blob_client(connection_string, container_name, file_name):
+def az_blob_client(connection_string: str, container_name: str, file_name: str) -> BlobServiceClient:
     """Create a blob client to get the file from the container."""
     try:
-        blob_service_client = BlobServiceClient.from_connection_string(
-            connection_string
-        )
-
-        blob_client = blob_service_client.get_blob_client(
-            container=container_name + "/manifests", blob=file_name
-        )
+        blob_service_client = BlobServiceClient.from_connection_string(connection_string)
+
+        blob_client = blob_service_client.get_blob_client(container=container_name + "/manifests", blob=file_name)
 
         return blob_client
 
     except Exception as ex:
-        print("Error: " + str(ex))
+        logger.error("Error: " + str(ex))
```

### Comparing `Munki-Manifest-Generator-1.1.2/munki_manifest_generator/get_device_catalogs.py` & `Munki-Manifest-Generator-1.2.0/munki_manifest_generator/get_device_catalogs.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,25 +3,18 @@
 """
 This module is used to get the catalogs that should be added or removed from a device.
 """
 
 from collections import defaultdict
 
 
-def get_device_catalogs(
-    groups, device_manifest, default_catalog, add_catalogs=False, remove_catalogs=False
-):
-
-    GROUP_CATALOGS = [
-        val
-        for list in groups
-        for key, val in list.items()
-        if "catalog" in key
-        if val is not None
-    ]
+def get_device_catalogs(groups, device_manifest, default_catalog, add_catalogs=False, remove_catalogs=False) -> list:
+    """Get the catalogs that should be added or removed from a device."""
+
+    GROUP_CATALOGS = [val for list in groups for key, val in list.items() if "catalog" in key if val is not None]
 
     if add_catalogs:
         catalogs = [default_catalog]
 
         for group in groups:
             if group["catalog"] is not None:
                 if group["name"] in device_manifest.included_manifests:
@@ -30,32 +23,30 @@
         return catalogs
 
     if remove_catalogs:
         catalogs_to_remove = []
 
         grouped_by_catalog = defaultdict(list)
         for item in groups:
-            grouped_by_catalog[item['catalog']].append(item)
+            grouped_by_catalog[item["catalog"]].append(item)
 
         multiple_result = dict(grouped_by_catalog)
 
         for catalog in device_manifest.catalogs:
             if catalog not in GROUP_CATALOGS and catalog != default_catalog:
                 device_manifest.catalogs.remove(catalog)
                 catalogs_to_remove.append(catalog)
 
         for group in groups:
-            if group["catalog"] is not None:
-                if (group["catalog"] in multiple_result):
-                    # get group names
-                    group_names = [item["name"] for item in multiple_result[group["catalog"]]]
-                    if group["name"] not in group_names:
-                        device_manifest.catalogs.remove(group["catalog"])
-                        catalogs_to_remove.append(group["catalog"])
-                elif (
-                    group["name"] not in device_manifest.included_manifests
-                    and group["catalog"] in device_manifest.catalogs
-                ):
+            if group["catalog"] is None:
+                continue
+            if group["catalog"] in multiple_result:
+                # get group names
+                group_names = [item["name"] for item in multiple_result[group["catalog"]]]
+                if group["name"] not in group_names:
                     device_manifest.catalogs.remove(group["catalog"])
                     catalogs_to_remove.append(group["catalog"])
+            elif group["name"] not in device_manifest.included_manifests and group["catalog"] in device_manifest.catalogs:
+                device_manifest.catalogs.remove(group["catalog"])
+                catalogs_to_remove.append(group["catalog"])
 
         return catalogs_to_remove
```

### Comparing `Munki-Manifest-Generator-1.1.2/munki_manifest_generator/graph/get_authentication_token.py` & `Munki-Manifest-Generator-1.2.0/munki_manifest_generator/graph/get_authentication_token.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,28 @@
 """
 This module is used to get the access token for the tenant.
 """
 
 import os
 import json
 
-from munki_manifest_generator.graph.obtain_access_token import obtain_accesstoken_app, obtain_accesstoken_cert, obtain_accesstoken_interactive
+from munki_manifest_generator.graph.obtain_access_token import (
+    obtain_accesstoken_app,
+    obtain_accesstoken_cert,
+    obtain_accesstoken_interactive,
+)
 
-def getAuth(app, certauth, interactiveauth):
+
+def getAuth(app: bool, certauth: bool, interactiveauth: bool) -> dict:
     """
     This function authenticates to MS Graph and returns the access token.
 
-    :param mode: The mode used when using this tool
-    :param localauth: Path to dict with keys to authenticate
-    :param tenant: Which tenant to authenticate to, PROD or DEV
+    :param app: Boolean to indicate if the app authentication method should be used
+    :param certauth: Boolean to indicate if the certificate authentication method should be used
+    :param interactiveauth: Boolean to indicate if the interactive authentication method should be used
     :return: The access token
     """
 
     if certauth:
         KEY_FILE = os.environ.get("KEY_FILE")
         THUMBPRINT = os.environ.get("THUMBPRINT")
         TENANT_NAME = os.environ.get("TENANT_NAME")
```

### Comparing `Munki-Manifest-Generator-1.1.2/munki_manifest_generator/graph/get_user_group_membership.py` & `Munki-Manifest-Generator-1.2.0/munki_manifest_generator/graph/get_user_group_membership.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,67 @@
 #!/usr/bin/env python3
 
+import logging
+
+from munki_manifest_generator.logger import logger
+
 """
 This module is used to get the user group membership and update included manifests.
 """
 
-from munki_manifest_generator.graph.make_api_request import make_api_request
 
 ENDPOINT = "https://graph.microsoft.com/v1.0/users"
 
 
-def get_user_group_membership(token, upn, groups, current_manifests, device_manifest):
+def get_user_group_membership(responses, groups, current_manifests, device_manifest):
     """Returns a list of group names the user is a member of and updates the included manifests."""
 
-    aad_user_object_id = None
-    q_param_user = {"$filter": "userPrincipalName eq '%s'" % upn}
-    user_object = make_api_request(ENDPOINT, token, q_param_user)
-
-    for id in user_object["value"]:
-        object_id = id["id"]
-        aad_user_object_id = object_id
-    q_param_group = {"$select": "id,displayName"}
-
-    # If Azure AD user id is none, skip getting groups
-    if aad_user_object_id is None:
-        print("AAD User ID is null, skipping user group memberships")
-
-    else:
-        memberOf = make_api_request(
-            ENDPOINT + "/" + aad_user_object_id + "/transitiveMemberOf", token, q_param_group
-        )
+    user = device_manifest.__dict__["user"]
+    serial_number = device_manifest.__dict__["serialnumber"]
+    memberOf = [val for val in responses if user in val["userPrincipalName"] for val in val["value"]]
 
+    if memberOf:
         user_groups = []
         user_groups_name = []
 
-        for group_id in memberOf["value"]:
+        for group_id in memberOf:
             id = group_id["id"]
             user_groups.append(id)
             user_groups_name.append(group_id["displayName"])
 
+        if logger.isEnabledFor(logging.DEBUG):
+            logger.debug(
+                "[%s] User found in groups: %s",
+                serial_number,
+                ", ".join(user_groups_name),
+            )
+            logger.debug(
+                "[%s] Groups from JSON or list: %s",
+                serial_number,
+                str(groups),
+            )
+
         for group in groups:
             if group["type"] == "user":
                 if group["id"] in user_groups:
                     if group["name"] in current_manifests:
                         if group["name"] not in device_manifest.included_manifests:
-                            print(
-                                "User found in group for "
-                                + group["name"]
-                                + ", adding included manifest for group"
+                            logger.info(
+                                "[%s] User found in group for %s, adding included manifest for group",
+                                serial_number,
+                                group["name"],
                             )
                             device_manifest.included_manifests.append(group["name"])
                     else:
-                        print(
-                            "User found in group for "
-                            + (group["name"])
-                            + " but manifest does not exist, skipping"
+                        logger.info(
+                            "[%s] User found in group for %s but manifest does not exist, skipping",
+                            serial_number,
+                            group["name"],
                         )
 
         return user_groups_name
+
+    else:
+        logger.warning(
+            "[%s] User not found in any groups",
+            serial_number,
+        )
```

### Comparing `Munki-Manifest-Generator-1.1.2/munki_manifest_generator/graph/make_api_request.py` & `Munki-Manifest-Generator-1.2.0/munki_manifest_generator/graph/make_api_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 """
 This module is used to make API requests to the Graph API.
 """
 
 import requests
 import json
 
+from retrying import retry
+
 
 def make_api_request(endpoint, token, q_param=None):
     """Makes a get request and returns the response."""
     # Create a valid header using the provided access token
 
     headers = {
         "Content-Type": "application/json",
@@ -38,10 +40,44 @@
             count = 0
             while count < entries:
                 json_data["value"].append(record["value"][count])
                 count += 1
         return json_data
 
     else:
-        raise Exception(
-            "Request failed with ", response.status_code, " - ", response.text
-        )
+        raise Exception("Request failed with ", response.status_code, " - ", response.text)
+
+
+@retry(
+    wait_exponential_multiplier=1000,
+    wait_exponential_max=10000,
+    stop_max_attempt_number=5,
+)
+def make_api_request_Post(endpoint, token, q_param=None, jdata=None, status_code=200):
+    """
+    This function makes a POST request to the Microsoft Graph API.
+
+    :param patchEndpoint: The endpoint to make the request to.
+    :param token: The token to use for authenticating the request.
+    :param q_param: The query parameters to use for the request.
+    :param jdata: The JSON data to use for the request.
+    :param status_code: The status code to expect from the request.
+    """
+
+    headers = {
+        "Content-Type": "application/json",
+        "Authorization": "Bearer {0}".format(token["access_token"]),
+    }
+
+    if q_param is not None:
+        response = requests.post(endpoint, headers=headers, params=q_param, data=jdata)
+    else:
+        response = requests.post(endpoint, headers=headers, data=jdata)
+    if response.status_code == status_code:
+        if response.text:
+            json_data = json.loads(response.text)
+            return json_data
+        else:
+            pass
+
+    else:
+        raise Exception("Request failed with ", response.status_code, " - ", response.text)
```

### Comparing `Munki-Manifest-Generator-1.1.2/munki_manifest_generator/graph/obtain_access_token.py` & `Munki-Manifest-Generator-1.2.0/munki_manifest_generator/graph/obtain_access_token.py`

 * *Files identical despite different names*

### Comparing `Munki-Manifest-Generator-1.1.2/munki_manifest_generator/main.py` & `Munki-Manifest-Generator-1.2.0/munki_manifest_generator/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,303 +2,433 @@
 
 """
 This module creates and updates manifests for macOS devices in Intune.
 """
 
 import os
 import json
+import time
 import argparse
+import threading
 
 from operator import itemgetter
+from concurrent.futures import ThreadPoolExecutor, as_completed
 from munki_manifest_generator.manifest import Manifest
 from munki_manifest_generator.graph.get_authentication_token import getAuth
 from munki_manifest_generator.graph.make_api_request import make_api_request
 from munki_manifest_generator.graph.get_device_group_membership import (
     get_device_group_membership,
 )
 from munki_manifest_generator.graph.get_user_group_membership import (
     get_user_group_membership,
 )
 from munki_manifest_generator.get_device_catalogs import get_device_catalogs
+from munki_manifest_generator.graph.concurrent_batch import batch_request
+
+from munki_manifest_generator.logger import logger
 from munki_manifest_generator.azstorage.az_storage_actions import (
     get_current_manifest_blobs,
     delete_manifest_blob,
     update_manifest_blob,
+    update_current_upn,
     get_current_device_manifest,
     create_manifest_blob,
 )
 
 
 def main(**kwargs):
+    # Start timer
+    startTime = time.time()
 
+    # Set variables to None
     j = None
-    l = None
+    g = None
     s = None
     t = None
     d = None
     c = None
     i = None
+    l = None
 
+    # If no kwargs are passed, parse arguments
     if not kwargs:
         argparser = argparse.ArgumentParser()
         argparser.add_argument(
             "-s",
             "--serial_number",
             help="Serial number to create or update a manifest for",
         )
         argparser.add_argument(
             "-j",
             "--json",
             help="Path to JSON file containing AzureAD groups specifying manifests devices should be in.",
         )
         argparser.add_argument(
-            "-l",
+            "-g",
             "--group_list",
             help="List of dicts containing AzureAD groups specifying manifests devices should be in.",
         )
         argparser.add_argument(
             "-sm",
             "--safe_manifest",
             help="Manifests specified here are safe from deletion, site_default does not have to be specified.",
         )
         argparser.add_argument(
             "-t",
-           "--test",
+            "--test",
             help="Enable testing, no changes will be made to manifests on Azure Storage.",
             action="store_true",
         )
         argparser.add_argument(
-            "-d", "--default_catalog", 
-            help="Default catalog for all devices. If not specified, the default catalog will be 'Production'."
-            
+            "-d",
+            "--default_catalog",
+            help="Default catalog for all devices. If not specified, the default catalog will be 'Production'.",
         )
         argparser.add_argument(
             "-c",
             "--certauth",
             help="When using certificate auth, the following ENV variables is required: TENANT_NAME, CLIENT_ID, THUMBPRINT, KEY_FILE",
             action="store_true",
         )
         argparser.add_argument(
             "-i",
             "--interactiveauth",
             help="When using interactive auth, the following ENV variables is required: TENANT_NAME, CLIENT_ID",
             action="store_true",
         )
+        argparser.add_argument(
+            "-v",
+            "--version",
+            action="version",
+            version="%(prog)s (version {version})".format(version="0.0.1"),
+        )
+        argparser.add_argument(
+            "-l",
+            "--log",
+            help="Log level, default is INFO",
+            default="INFO",
+            choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
+        )
 
         args = argparser.parse_args()
 
+        if args.log:
+            for handler in logger.handlers:
+                handler.setLevel(args.log.upper())
+
         if args.test:
-            print(
-                "*****Testing mode enabled, no changes will be made to manifests on Azure Storage*****"
-            )
+            logger.info("*****Testing mode enabled, no changes will be made to manifests on Azure Storage*****")
 
+    # Else, set variables to kwargs
     else:
         s = kwargs.get("serial_number")
         j = kwargs.get("json_file")
-        l = kwargs.get("group_list")
+        g = kwargs.get("group_list")
         sm = kwargs.get("safe_manifest")
         t = kwargs.get("test")
         d = kwargs.get("default_catalog")
         c = kwargs.get("certauth")
         i = kwargs.get("interactiveauth")
+        l = kwargs.get("log")
 
-        if t:
-            print(
-                "*****Testing mode enabled, no changes will be made to manifests on Azure Storage*****"
-            )
-
+        # If log level is passed, set it
+        if l:
+            choices = ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
+            if l in choices:
+                for handler in logger.handlers:
+                    handler.setLevel(l.upper())
+            else:
+                raise Exception("Invalid log level, choose from: DEBUG, INFO, WARNING, ERROR, CRITICAL")
 
-    def run(json_file, group_list, serial_number, SAFE_MANIFEST, TEST, DEFAULT_CATALOG, CERTAUTH, INTERACTIVEAUTH):
+        # If testing is enabled, log it
+        if t:
+            logger.info("*****Testing mode enabled, no changes will be made to manifests on Azure Storage*****")
 
-        if not all([os.environ.get("CONTAINER_NAME"), os.environ.get("AZURE_STORAGE_CONNECTION_STRING")]):
+    def run(
+        json_file,
+        group_list,
+        serial_number,
+        SAFE_MANIFEST,
+        TEST,
+        DEFAULT_CATALOG,
+        CERTAUTH,
+        INTERACTIVEAUTH,
+    ):
+        # Check if required environment variables are set
+        if not all(
+            [
+                os.environ.get("CONTAINER_NAME"),
+                os.environ.get("AZURE_STORAGE_CONNECTION_STRING"),
+            ]
+        ):
             raise Exception("Missing required environment variables, stopping...")
+
+        # Set variables
         CONTAINER_NAME = os.environ.get("CONTAINER_NAME")
         CONNECTION_STRING = os.environ.get("AZURE_STORAGE_CONNECTION_STRING")
         ENDPOINT = "https://graph.microsoft.com/v1.0/deviceManagement/managedDevices"
-        if not CERTAUTH and not INTERACTIVEAUTH:
-            APP = True
-        else:
+
+        # If certificate or interactive auth is enabled, set APP to False
+        if CERTAUTH or INTERACTIVEAUTH:
             APP = False
-        TOKEN = getAuth(APP, CERTAUTH, INTERACTIVEAUTH)
-        CURRENT_MANIFESTS = get_current_manifest_blobs(
-            CONNECTION_STRING, CONTAINER_NAME
-        )
+        else:
+            APP = True
 
+        # Get authentication token
+        TOKEN = getAuth(APP, CERTAUTH, INTERACTIVEAUTH)
+        # Get current manifests from Azure Storage
+        CURRENT_MANIFESTS = get_current_manifest_blobs(CONNECTION_STRING, CONTAINER_NAME)
+        # If custom default catalog is passed, set it
         if DEFAULT_CATALOG:
             DEFAULT_CATALOG = DEFAULT_CATALOG
         else:
             DEFAULT_CATALOG = "Production"
-
         # If a serial number is passed, create or update a manifest for that device
         if serial_number:
             Q_PARAM = {"$filter": "serialNumber eq '%s'" % serial_number}
             DEVICES = make_api_request(ENDPOINT, TOKEN, Q_PARAM)
 
             # If two objects are found, get the latest enrolled device
             if DEVICES["@odata.count"] > 1:
-                latest_enrolled = max(
-                    DEVICES["value"], key=lambda x: x["enrolledDateTime"]
-                )
+                latest_enrolled = max(DEVICES["value"], key=lambda x: x["enrolledDateTime"])
                 DEVICES["value"] = [latest_enrolled]
                 DEVICES["@odata.count"] = 1
 
             # If no device is returned, stop script
             if DEVICES["@odata.count"] == 0:
-                print(f"Device with serial {serial_number} not found, stopping...")
+                logger.error(f"Device with serial {serial_number} not found, stopping...")
                 quit()
 
         # Else, create or update manifests for all devices
         else:
             Q_PARAM = {"$filter": "operatingSystem eq 'macOS'"}
             DEVICES = make_api_request(ENDPOINT, TOKEN, Q_PARAM)
             # Check if there are duplicate entries for a device
-            for d in DEVICES['value']:
-                for index, value in enumerate(DEVICES['value']):
-                    if d['serialNumber'] == value['serialNumber']:
+            for d in DEVICES["value"]:
+                for index, value in enumerate(DEVICES["value"]):
+                    if d["serialNumber"] == value["serialNumber"]:
                         # If the device is enrolled more than once, get the latest enrolled device
-                        if d['enrolledDateTime'] > value['enrolledDateTime']:
+                        if d["enrolledDateTime"] > value["enrolledDateTime"]:
                             # Remove the older device from the list
-                            DEVICES['value'].remove(DEVICES['value'][index])
+                            DEVICES["value"].remove(DEVICES["value"][index])
+
+            import re
+            def contains_random_uuid(upn):
+                # Construct a regular expression pattern that matches the specified format
+                pattern = re.compile(r"[A-Za-z]+([0-9]+([A-Za-z]+[0-9]+)+).*@.*", re.IGNORECASE)
 
-            print("-" * 90)
-            print(f"Found {len(CURRENT_MANIFESTS)} current manifests")
-            print(f"Found {DEVICES['@odata.count']} devices")
-
-        SERIAL_NUMBERS = [
-            val
-            for d in DEVICES["value"]
-            for key, val in d.items()
-            if "serialNumber" in key
-            if val is not None
+                # Use the re module to search for the pattern in the input string
+                match = re.search(pattern, upn)
+
+                # If a match is found, return True; otherwise, return False
+                if match:
+                    return True
+                else:
+                    return False
+
+            # Remove devices that have a UPN that contains a random UUID
+            DEVICES["value"] = [d for d in DEVICES["value"] for key, val in d.items() if "userPrincipalName" in key if val is not None if not contains_random_uuid(val)]
+
+            logger.info("-" * 90)
+            logger.info(f"Found {len(CURRENT_MANIFESTS)} current manifests")
+            logger.info(f'Found {len(DEVICES["value"])} devices')
+
+
+
+
+            logger.info("-" * 90)
+
+        # Get serial numbers, AAD device IDs, and UPNs for all devices
+        SERIAL_NUMBERS = [val for d in DEVICES["value"] for key, val in d.items() if "serialNumber" in key if val is not None]
+
+        AAD_DEVICE_IDS = [
+            val for d in DEVICES["value"] for key, val in d.items() if "azureADDeviceId" in key if val is not None
         ]
 
+        UPNs = [val for d in DEVICES["value"] for key, val in d.items() if "userPrincipalName" in key if val is not None]
+
         # Get list of group manifests from json file or list
         if json_file:
             with open(json_file, "r") as f:
                 GROUPS = json.load(f)
         elif group_list:
             GROUPS = group_list
         else:
             raise Exception("No JSON file or list provided")
 
+        # Batch get group memberships for all devices and users
+        group_search = []
+        for group in GROUPS:
+            group_search.append('"displayName:%s"' % group["name"])
+
+        group_search_query = f'({" OR ".join(group_search)})'
+
+        if "device" in map(itemgetter("type"), GROUPS):
+            # Batch get ids for all devices and users
+            device_id_responses = batch_request(AAD_DEVICE_IDS, "devices", "", "deviceId", TOKEN)
+            device_group_responses = batch_request(
+                device_id_responses, "devices/", "/transitiveMemberOf?$search=%s" % group_search_query, "device", TOKEN
+            )
+
+        if "user" in map(itemgetter("type"), GROUPS):
+            device_upn_responses = batch_request(UPNs, "users", "", "upn", TOKEN)
+            user_group_responses = batch_request(
+                device_upn_responses,
+                "users/",
+                "/transitiveMemberOf?$select=id,displayName&$search=%s" % group_search_query,
+                "user",
+                TOKEN,
+            )
+
         # If not passing a serial number, delete manifest for device if it is not in Intune
         if not serial_number:
             delete_manifest_blob(
-                CONNECTION_STRING, CONTAINER_NAME, GROUPS, SERIAL_NUMBERS, SAFE_MANIFEST, TEST
+                CONNECTION_STRING,
+                CONTAINER_NAME,
+                GROUPS,
+                SERIAL_NUMBERS,
+                SAFE_MANIFEST,
+                TEST,
+                CURRENT_MANIFESTS,
             )
 
-        for device in DEVICES["value"]:
-
-            if not device["serialNumber"]:
-                continue
+        def process_device(device):
+            """Process each device"""
 
+            lock = threading.Lock()
             group_membership = []
             # If a manifest exists for the device, update it.
             if device["serialNumber"] in CURRENT_MANIFESTS:
-                
-                print("{0:-^{1}}".format(device["serialNumber"], 90))
-                print("Manifest found, checking for updates")
-
+                logger.debug("[%s] Manifest found, checking for updates..." % device["serialNumber"])
                 current_device_manifest = get_current_device_manifest(
                     CONNECTION_STRING, CONTAINER_NAME, device["serialNumber"]
                 )
 
                 device_manifest = Manifest(
                     catalogs=current_device_manifest["catalogs"],
                     included_manifests=current_device_manifest["included_manifests"],
                     display_name=current_device_manifest["display_name"],
                     serialnumber=current_device_manifest["serialnumber"],
                     user=current_device_manifest["user"],
                 )
 
+                if device_manifest.user != device["userPrincipalName"]:
+                    update_current_upn(
+                        CONNECTION_STRING,
+                        CONTAINER_NAME,
+                        device_manifest.serialnumber,
+                        device["userPrincipalName"],
+                        device_manifest.user,
+                        TEST,
+                    )
+                    device_manifest.user = device["userPrincipalName"]
+
                 # If device groups are in the JSON or list, get the groups the device is in
                 if "device" in map(itemgetter("type"), GROUPS):
                     device_groups = get_device_group_membership(
-                        TOKEN,
+                        device_group_responses,
                         device["azureADDeviceId"],
                         GROUPS,
                         CURRENT_MANIFESTS,
                         device_manifest,
                     )
                     if device_groups:
-                        group_membership += device_groups
+                        with lock:
+                            group_membership += device_groups
 
                 # If user groups are in the JSON or list, get the groups the device's user is in
                 if "user" in map(itemgetter("type"), GROUPS):
                     user_groups = get_user_group_membership(
-                        TOKEN,
-                        device["userPrincipalName"],
+                        user_group_responses,
                         GROUPS,
                         CURRENT_MANIFESTS,
                         device_manifest,
                     )
                     if user_groups:
-                        group_membership += user_groups
+                        with lock:
+                            group_membership += user_groups
 
                 update_manifest_blob(
                     CONNECTION_STRING,
                     CONTAINER_NAME,
                     device["serialNumber"],
                     device_manifest,
                     group_membership,
                     GROUPS,
                     TEST,
-                    DEFAULT_CATALOG
+                    DEFAULT_CATALOG,
+                    CURRENT_MANIFESTS,  # noqa: F821
                 )
 
             # If no manifest exists for the device, create one.
             else:
-                print("{0:-^{1}}".format(device["serialNumber"], 90))
-                print("Manifest not found, creating")
-
+                logger.info("[%s] No manifest found, creating..." % device["serialNumber"])
                 device_manifest = Manifest(
                     catalogs=[DEFAULT_CATALOG],
                     included_manifests=["site_default"],
                     display_name=device["serialNumber"],
                     serialnumber=device["serialNumber"],
                     user=device["userPrincipalName"],
                 )
 
                 # If device groups are in the JSON or list, get the groups the device is in
                 if "device" in map(itemgetter("type"), GROUPS):
                     device_groups = get_device_group_membership(
-                        TOKEN,
+                        device_group_responses,
                         device["azureADDeviceId"],
                         GROUPS,
                         CURRENT_MANIFESTS,
                         device_manifest,
                     )
                     if device_groups:
-                        group_membership += device_groups
+                        with lock:
+                            group_membership += device_groups
 
                 # If user groups are in the JSON or list, get the groups the device's user is in
                 if "user" in map(itemgetter("type"), GROUPS):
                     user_groups = get_user_group_membership(
-                        TOKEN,
-                        device["userPrincipalName"],
+                        user_group_responses,
                         GROUPS,
                         CURRENT_MANIFESTS,
                         device_manifest,
                     )
                     if user_groups:
-                        group_membership += user_groups
+                        with lock:
+                            group_membership += user_groups
 
-                device_manifest.catalogs = get_device_catalogs(
-                    GROUPS, device_manifest, DEFAULT_CATALOG, add_catalogs=True
-                )
+                device_manifest.catalogs = get_device_catalogs(GROUPS, device_manifest, DEFAULT_CATALOG, add_catalogs=True)
 
                 create_manifest_blob(
                     CONNECTION_STRING,
                     CONTAINER_NAME,
                     device["serialNumber"],
                     device_manifest,
-                    TEST
+                    TEST,
                 )
 
+        with ThreadPoolExecutor() as executor:
+            futures = [executor.submit(process_device, device) for device in DEVICES["value"] if device["serialNumber"]]
+            for future in as_completed(futures):
+                try:
+                    result = future.result()
+                except Exception as e:
+                    logger.error(f"Exception: {e}")
+
     if not kwargs:
-        run(args.json, args.group_list, args.serial_number, args.safe_manifest, args.test, args.default_catalog, args.certauth, args.interactiveauth)
+        run(
+            args.json,
+            args.group_list,
+            args.serial_number,
+            args.safe_manifest,
+            args.test,
+            args.default_catalog,
+            args.certauth,
+            args.interactiveauth,
+        )
     else:
-        run(j, l, s, sm, t, d, c, i)
+        run(j, g, s, sm, t, d, c, i)
+
+    logger.debug("Finished in {0} seconds.".format(time.time() - startTime))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `Munki-Manifest-Generator-1.1.2/setup.cfg` & `Munki-Manifest-Generator-1.2.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [metadata]
 name = Munki-Manifest-Generator
-version = 1.1.2
+version = 1.2.0
 author = Tobias Almén
 author_email = almenscorner@outlook.com
 description = Tool to create and update Munki manifests for devices managed in Intune
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/almenscorner/munki-manifest-generator
 project_urls = 
 	Bug Tracker = https://github.com/almenscorner/munki-manifest-generator/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
-python_requires = >=3.6
+python_requires = >=3.7
 install_requires = 
 	msal >= 1.20.0
-	msrest>=0.6.21
-	azure-storage-blob >= 12.13.1
+	msrest>=0.7.1
+	azure-storage-blob >= 12.15.0
+	retrying >= 1.3.4
 
 [options.entry_points]
 console_scripts = 
 	munki-manifest-generator = munki_manifest_generator.main:main
 
 [egg_info]
 tag_build =
```

