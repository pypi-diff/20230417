# Comparing `tmp/explainaboard_client-0.1.3.tar.gz` & `tmp/explainaboard_client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explainaboard_client-0.1.3.tar", last modified: Sat Apr  1 19:16:24 2023, max compression
+gzip compressed data, was "explainaboard_client-0.1.4.tar", last modified: Mon Apr 17 12:49:17 2023, max compression
```

## Comparing `explainaboard_client-0.1.3.tar` & `explainaboard_client-0.1.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 19:16:24.254059 explainaboard_client-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-01 19:16:24.254059 explainaboard_client-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 19:16:24.254059 explainaboard_client-0.1.3/explainaboard_client/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 19:16:24.254059 explainaboard_client-0.1.3/explainaboard_client/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/cli/delete_systems.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/cli/evaluate_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/cli/evaluate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/cli/find_systems.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/cli/upload_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/cli/upload_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/client_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 19:16:24.254059 explainaboard_client-0.1.3/explainaboard_client/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/tests/test_check_api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/tests/test_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/explainaboard_client/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 19:16:24.254059 explainaboard_client-0.1.3/explainaboard_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-01 19:16:24.000000 explainaboard_client-0.1.3/explainaboard_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-01 19:16:24.000000 explainaboard_client-0.1.3/explainaboard_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 19:16:24.000000 explainaboard_client-0.1.3/explainaboard_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-01 19:16:24.000000 explainaboard_client-0.1.3/explainaboard_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-01 19:16:24.000000 explainaboard_client-0.1.3/explainaboard_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-01 19:16:24.000000 explainaboard_client-0.1.3/explainaboard_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-01 19:16:24.254059 explainaboard_client-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-01 19:16:15.000000 explainaboard_client-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:49:17.938125 explainaboard_client-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-17 12:49:17.938125 explainaboard_client-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:49:17.934126 explainaboard_client-0.1.4/explainaboard_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:49:17.938125 explainaboard_client-0.1.4/explainaboard_client/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/cli/delete_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/cli/evaluate_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/cli/evaluate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/cli/find_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/cli/upload_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/cli/upload_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22528 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/client_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:49:17.938125 explainaboard_client-0.1.4/explainaboard_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/tests/test_check_api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/tests/test_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/explainaboard_client/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:49:17.934126 explainaboard_client-0.1.4/explainaboard_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-17 12:49:17.000000 explainaboard_client-0.1.4/explainaboard_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-17 12:49:17.000000 explainaboard_client-0.1.4/explainaboard_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 12:49:17.000000 explainaboard_client-0.1.4/explainaboard_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 12:49:17.000000 explainaboard_client-0.1.4/explainaboard_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-17 12:49:17.000000 explainaboard_client-0.1.4/explainaboard_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 12:49:17.000000 explainaboard_client-0.1.4/explainaboard_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-17 12:49:17.938125 explainaboard_client-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-17 12:49:12.000000 explainaboard_client-0.1.4/setup.py
```

### Comparing `explainaboard_client-0.1.3/PKG-INFO` & `explainaboard_client-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: explainaboard_client
-Version: 0.1.3
+Version: 0.1.4
 Summary: ExplainaBoard Client
 Home-page: https://github.com/neulab/explainaboard_client
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `explainaboard_client-0.1.3/README.md` & `explainaboard_client-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `explainaboard_client-0.1.3/explainaboard_client/cli/delete_systems.py` & `explainaboard_client-0.1.4/explainaboard_client/cli/delete_systems.py`

 * *Files identical despite different names*

### Comparing `explainaboard_client-0.1.3/explainaboard_client/cli/evaluate_benchmark.py` & `explainaboard_client-0.1.4/explainaboard_client/cli/evaluate_benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from explainaboard_api_client.model.system import System
 from explainaboard_api_client.model.system_create_props import SystemCreateProps
 from explainaboard_api_client.model.system_metadata import SystemMetadata
 from explainaboard_api_client.model.system_output_props import SystemOutputProps
 import explainaboard_client
 from explainaboard_client import ExplainaboardClient
 from explainaboard_client.client_utils import (
-    generate_dataset_id,
     prompt_for_auto_upgrade_and_exit,
 )
 from explainaboard_client.exceptions import APIVersionMismatchException
 
 
 def validate_outputs(system_outputs):
     for pth in system_outputs:
@@ -131,15 +130,16 @@
         metadata = SystemMetadata(
             task=task,
             is_private=not args.public,
             system_name=args.system_name,
             metric_names=metric_names,
             source_language=source_language,
             target_language=target_language,
-            dataset_metadata_id=generate_dataset_id(dataset_name, sub_dataset),
+            dataset_name=dataset_name,
+            sub_dataset=sub_dataset,
             dataset_split=dataset_split,
             shared_users=shared_users,
             system_details=system_details,
             system_tags=system_tags,
         )
 
         create_props = SystemCreateProps(
```

### Comparing `explainaboard_client-0.1.3/explainaboard_client/cli/evaluate_system.py` & `explainaboard_client-0.1.4/explainaboard_client/cli/evaluate_system.py`

 * *Files identical despite different names*

### Comparing `explainaboard_client-0.1.3/explainaboard_client/cli/find_systems.py` & `explainaboard_client-0.1.4/explainaboard_client/cli/find_systems.py`

 * *Files identical despite different names*

### Comparing `explainaboard_client-0.1.3/explainaboard_client/client.py` & `explainaboard_client-0.1.4/explainaboard_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     SystemCreateProps,
     SystemOutputProps,
 )
 import explainaboard_client
 from explainaboard_client.client_utils import (
     encode_file_to_base64,
     encode_string_to_base64,
-    generate_dataset_id,
 )
 from explainaboard_client.config import get_host
 from explainaboard_client.exceptions import APIVersionMismatchException
 from explainaboard_client.tasks import DEFAULT_METRICS, infer_file_type, TaskType
 
 
 class ExplainaboardClient:
@@ -180,26 +179,24 @@
         system_tags = system_tags or []
 
         # Do the actual upload
         metadata = SystemMetadata(
             task=task,
             is_private=not public,
             system_name=system_name,
+            dataset_name=dataset,
+            sub_dataset=sub_dataset,
             metric_names=metric_names,
             source_language=source_language,
             target_language=target_language,
             dataset_split=split,
             shared_users=shared_users,
             system_tags=system_tags,
             system_details=system_details,
         )
-        if dataset is not None:
-            metadata.dataset_metadata_id = generate_dataset_id(dataset, sub_dataset)
-        elif not custom_dataset:
-            raise ValueError("Must specify dataset or custom_dataset")
 
         loaded_system_output = SystemOutputProps(
             data=encode_string_to_base64(
                 json.dumps(self._convert_to_json(system_output))
             ),
             file_type="json",
         )
@@ -291,26 +288,24 @@
                 system_details = json.load(fin)
 
         # Do the actual upload
         metadata = SystemMetadata(
             task=task,
             is_private=not public,
             system_name=system_name,
+            dataset_name=dataset,
+            sub_dataset=sub_dataset,
             metric_names=metric_names,
             source_language=source_language,
             target_language=target_language,
             dataset_split=split,
             shared_users=shared_users,
             system_details=system_details,
             system_tags=system_tags,
         )
-        if dataset is not None:
-            metadata.dataset_metadata_id = generate_dataset_id(dataset, sub_dataset)
-        elif not custom_dataset_file:
-            raise ValueError("Must specify dataset or custom_dataset_file")
 
         loaded_system_output = SystemOutputProps(
             data=encode_file_to_base64(system_output_file),
             file_type=system_output_file_type,
         )
         if custom_dataset_file:
             loaded_custom_dataset = SystemOutputProps(
```

### Comparing `explainaboard_client-0.1.3/explainaboard_client/client_utils.py` & `explainaboard_client-0.1.4/explainaboard_client/client_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,25 +13,14 @@
         return base64.b64encode(f.read()).decode("utf-8")
 
 
 def encode_string_to_base64(text: str) -> str:
     return base64.b64encode(text.encode("utf-8")).decode("utf-8")
 
 
-def generate_dataset_id(dataset_name: str, sub_dataset: Optional[str]) -> str:
-    """HACK probably shouldn't expose this logic to the users"""
-    if not dataset_name:
-        raise ValueError(
-            "dataset_name cannot be None or empty. If you are "
-            "using a custom dataset, please remove the dataset argument."
-        )
-    sub_dataset = sub_dataset if sub_dataset else "None"
-    return f"{dataset_name}---{sub_dataset}"
-
-
 def sanitize_for_json(input_obj: Any) -> Any:
     if hasattr(input_obj, "to_dict"):
         return sanitize_for_json(getattr(input_obj, "to_dict")())
     elif isinstance(input_obj, dict):
         return {k: sanitize_for_json(v) for k, v in input_obj.items()}
     elif isinstance(input_obj, list):
         return [sanitize_for_json(v) for v in input_obj]
```

### Comparing `explainaboard_client-0.1.3/explainaboard_client/config.py` & `explainaboard_client-0.1.4/explainaboard_client/config.py`

 * *Files identical despite different names*

### Comparing `explainaboard_client-0.1.3/explainaboard_client/data_utils.py` & `explainaboard_client-0.1.4/explainaboard_client/data_utils.py`

 * *Files identical despite different names*

### Comparing `explainaboard_client-0.1.3/explainaboard_client/tasks.py` & `explainaboard_client-0.1.4/explainaboard_client/tasks.py`

 * *Files identical despite different names*

### Comparing `explainaboard_client-0.1.3/explainaboard_client/tests/test_benchmark.py` & `explainaboard_client-0.1.4/explainaboard_client/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `explainaboard_client-0.1.3/explainaboard_client/tests/test_check_api_version.py` & `explainaboard_client-0.1.4/explainaboard_client/tests/test_check_api_version.py`

 * *Files identical despite different names*

### Comparing `explainaboard_client-0.1.3/explainaboard_client/tests/test_cli.py` & `explainaboard_client-0.1.4/explainaboard_client/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `explainaboard_client-0.1.3/explainaboard_client/tests/test_system.py` & `explainaboard_client-0.1.4/explainaboard_client/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `explainaboard_client-0.1.3/explainaboard_client/tests/test_tabular.py` & `explainaboard_client-0.1.4/explainaboard_client/tests/test_tabular.py`

 * *Files identical despite different names*

### Comparing `explainaboard_client-0.1.3/explainaboard_client/tests/test_user.py` & `explainaboard_client-0.1.4/explainaboard_client/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `explainaboard_client-0.1.3/explainaboard_client/tests/test_utils.py` & `explainaboard_client-0.1.4/explainaboard_client/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `explainaboard_client-0.1.3/explainaboard_client.egg-info/PKG-INFO` & `explainaboard_client-0.1.4/explainaboard_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: explainaboard-client
-Version: 0.1.3
+Version: 0.1.4
 Summary: ExplainaBoard Client
 Home-page: https://github.com/neulab/explainaboard_client
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `explainaboard_client-0.1.3/explainaboard_client.egg-info/SOURCES.txt` & `explainaboard_client-0.1.4/explainaboard_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `explainaboard_client-0.1.3/setup.py` & `explainaboard_client-0.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
     packages=find_packages(),
     entry_points={
         "console_scripts": [],
     },
-    install_requires=["explainaboard_api_client>=0.4.1"],
+    install_requires=["explainaboard_api_client>=0.4.3"],
     extras_require={
         "dev": [
             "pre-commit",
         ],
     },
     include_package_data=True,
 )
```

