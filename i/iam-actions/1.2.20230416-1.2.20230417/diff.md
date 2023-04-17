# Comparing `tmp/iam_actions-1.2.20230416.tar.gz` & `tmp/iam_actions-1.2.20230417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230416.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230417.tar", max compression
```

## Comparing `iam_actions-1.2.20230416.tar` & `iam_actions-1.2.20230417.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-04-16 02:30:06.363304 iam_actions-1.2.20230416/LICENSE
--rw-r--r--   0        0        0     2302 2023-04-16 02:30:06.363304 iam_actions-1.2.20230416/README.md
--rw-r--r--   0        0        0      228 2023-04-16 02:30:06.363304 iam_actions-1.2.20230416/iam_actions/__init__.py
--rw-r--r--   0        0        0  4212929 2023-04-16 02:32:02.413449 iam_actions-1.2.20230416/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-04-16 02:30:06.363304 iam_actions-1.2.20230416/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-04-16 02:30:06.363304 iam_actions-1.2.20230416/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-04-16 02:30:06.363304 iam_actions-1.2.20230416/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-04-16 02:30:06.363304 iam_actions-1.2.20230416/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-04-16 02:30:06.363304 iam_actions-1.2.20230416/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-04-16 02:30:06.363304 iam_actions-1.2.20230416/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-04-16 02:30:06.363304 iam_actions-1.2.20230416/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-04-16 02:30:06.363304 iam_actions-1.2.20230416/iam_actions/generate/services.py
--rw-r--r--   0        0        0   540625 2023-04-16 02:32:02.413449 iam_actions-1.2.20230416/iam_actions/policies.json
--rw-r--r--   0        0        0   190432 2023-04-16 02:32:02.413449 iam_actions-1.2.20230416/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   524216 2023-04-16 02:32:02.413449 iam_actions-1.2.20230416/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-04-16 02:32:03.341546 iam_actions-1.2.20230416/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230416/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230416/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-17 02:26:35.841894 iam_actions-1.2.20230417/LICENSE
+-rw-r--r--   0        0        0     2302 2023-04-17 02:26:35.841894 iam_actions-1.2.20230417/README.md
+-rw-r--r--   0        0        0      228 2023-04-17 02:26:35.841894 iam_actions-1.2.20230417/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4213887 2023-04-17 02:28:15.521736 iam_actions-1.2.20230417/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-04-17 02:26:35.841894 iam_actions-1.2.20230417/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-04-17 02:26:35.841894 iam_actions-1.2.20230417/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-04-17 02:26:35.841894 iam_actions-1.2.20230417/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-04-17 02:26:35.841894 iam_actions-1.2.20230417/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-04-17 02:26:35.841894 iam_actions-1.2.20230417/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-04-17 02:26:35.841894 iam_actions-1.2.20230417/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-04-17 02:26:35.841894 iam_actions-1.2.20230417/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-04-17 02:26:35.841894 iam_actions-1.2.20230417/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   540792 2023-04-17 02:28:15.521736 iam_actions-1.2.20230417/iam_actions/policies.json
+-rw-r--r--   0        0        0   190432 2023-04-17 02:28:15.521736 iam_actions-1.2.20230417/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   524379 2023-04-17 02:28:15.521736 iam_actions-1.2.20230417/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-04-17 02:28:16.297736 iam_actions-1.2.20230417/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230417/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230417/PKG-INFO
```

### Comparing `iam_actions-1.2.20230416/LICENSE` & `iam_actions-1.2.20230417/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230416/README.md` & `iam_actions-1.2.20230417/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230416/iam_actions/actions.json` & `iam_actions-1.2.20230417/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999282819951949%*

 * *Differences: {"'drs'": "{'DeleteLaunchConfigurationTemplate': OrderedDict([('access_level', 'Undocumented'), "*

 * *          "('action', 'DeleteLaunchConfigurationTemplate'), ('condition_keys', []), "*

 * *          "('description', 'Not Documented by AWS'), ('orphan', False), ('resources', [])]), "*

 * *          "'UpdateLaunchConfigurationTemplate': OrderedDict([('access_level', 'Undocumented'), "*

 * *          "('action', 'UpdateLaunchConfigurationTemplate'), ('condition_keys', []), "*

 * *          "('description', 'Not Documented by AWS' […]*

```diff
@@ -39003,14 +39003,22 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to extend a source server",
             "orphan": false,
             "resources": []
         },
+        "CreateLaunchConfigurationTemplate": {
+            "access_level": "Undocumented",
+            "action": "CreateLaunchConfigurationTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateRecoveryInstanceForDrs": {
             "access_level": "Write",
             "action": "CreateRecoveryInstanceForDrs",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -39048,14 +39056,22 @@
             "condition_keys": [],
             "description": "Grants permission to delete a job",
             "orphan": false,
             "resources": [
                 "JobResource"
             ]
         },
+        "DeleteLaunchConfigurationTemplate": {
+            "access_level": "Undocumented",
+            "action": "DeleteLaunchConfigurationTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteRecoveryInstance": {
             "access_level": "Write",
             "action": "DeleteRecoveryInstance",
             "condition_keys": [],
             "description": "Grants permission to delete recovery instance",
             "orphan": false,
             "resources": [
@@ -39096,14 +39112,22 @@
             "access_level": "Read",
             "action": "DescribeJobs",
             "condition_keys": [],
             "description": "Grants permission to describe jobs",
             "orphan": false,
             "resources": []
         },
+        "DescribeLaunchConfigurationTemplates": {
+            "access_level": "Undocumented",
+            "action": "DescribeLaunchConfigurationTemplates",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeRecoveryInstances": {
             "access_level": "Read",
             "action": "DescribeRecoveryInstances",
             "condition_keys": [],
             "description": "Grants permission to describe recovery instances",
             "orphan": false,
             "resources": []
@@ -39689,14 +39713,22 @@
             "condition_keys": [],
             "description": "Grants permission to update launch configuration",
             "orphan": false,
             "resources": [
                 "SourceServerResource"
             ]
         },
+        "UpdateLaunchConfigurationTemplate": {
+            "access_level": "Undocumented",
+            "action": "UpdateLaunchConfigurationTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateReplicationCertificateForDrs": {
             "access_level": "Write",
             "action": "UpdateReplicationCertificateForDrs",
             "condition_keys": [],
             "description": "Grants permission to update a replication certificate",
             "orphan": false,
             "resources": [
```

### Comparing `iam_actions-1.2.20230416/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230417/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230416/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230417/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230416/iam_actions/generate/generate.py` & `iam_actions-1.2.20230417/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230416/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230417/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230416/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230417/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230416/iam_actions/generate/services.py` & `iam_actions-1.2.20230417/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230416/iam_actions/policies.json` & `iam_actions-1.2.20230417/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999994298095564%*

 * *Differences: {"'serviceMap'": "{'AWS Elastic Disaster Recovery': {'Actions': {insert: [(5, "*

 * *                 "'CreateLaunchConfigurationTemplate'), (10, 'DeleteLaunchConfigurationTemplate'), "*

 * *                 "(16, 'DescribeLaunchConfigurationTemplates'), (75, "*

 * *                 "'UpdateLaunchConfigurationTemplate')]}}}"}*

```diff
@@ -3158,23 +3158,26 @@
             "ARNRegex": "^arn:aws:drs:.+",
             "Actions": [
                 "AssociateFailbackClientToRecoveryInstanceForDrs",
                 "BatchCreateVolumeSnapshotGroupForDrs",
                 "BatchDeleteSnapshotRequestForDrs",
                 "CreateConvertedSnapshotForDrs",
                 "CreateExtendedSourceServer",
+                "CreateLaunchConfigurationTemplate",
                 "CreateRecoveryInstanceForDrs",
                 "CreateReplicationConfigurationTemplate",
                 "CreateSourceServerForDrs",
                 "DeleteJob",
+                "DeleteLaunchConfigurationTemplate",
                 "DeleteRecoveryInstance",
                 "DeleteReplicationConfigurationTemplate",
                 "DeleteSourceServer",
                 "DescribeJobLogItems",
                 "DescribeJobs",
+                "DescribeLaunchConfigurationTemplates",
                 "DescribeRecoveryInstances",
                 "DescribeRecoverySnapshots",
                 "DescribeReplicationConfigurationTemplates",
                 "DescribeReplicationServerAssociationsForDrs",
                 "DescribeSnapshotRequestsForDrs",
                 "DescribeSourceServers",
                 "DisconnectRecoveryInstance",
@@ -3225,14 +3228,15 @@
                 "UpdateAgentReplicationInfoForDrs",
                 "UpdateAgentReplicationProcessStateForDrs",
                 "UpdateAgentSourcePropertiesForDrs",
                 "UpdateFailbackClientDeviceMappingForDrs",
                 "UpdateFailbackClientLastSeenForDrs",
                 "UpdateFailbackReplicationConfiguration",
                 "UpdateLaunchConfiguration",
+                "UpdateLaunchConfigurationTemplate",
                 "UpdateReplicationCertificateForDrs",
                 "UpdateReplicationConfiguration",
                 "UpdateReplicationConfigurationTemplate"
             ],
             "HasResource": true,
             "StringPrefix": "drs",
             "conditionKeys": [
```

### Comparing `iam_actions-1.2.20230416/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230417/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230416/iam_actions/services.json` & `iam_actions-1.2.20230417/iam_actions/services.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999940234995996%*

 * *Differences: {"'drs'": "{'Actions': {insert: [(5, 'CreateLaunchConfigurationTemplate'), (10, "*

 * *          "'DeleteLaunchConfigurationTemplate'), (16, 'DescribeLaunchConfigurationTemplates'), "*

 * *          "(75, 'UpdateLaunchConfigurationTemplate')]}}"}*

```diff
@@ -5854,23 +5854,26 @@
         ],
         "Actions": [
             "AssociateFailbackClientToRecoveryInstanceForDrs",
             "BatchCreateVolumeSnapshotGroupForDrs",
             "BatchDeleteSnapshotRequestForDrs",
             "CreateConvertedSnapshotForDrs",
             "CreateExtendedSourceServer",
+            "CreateLaunchConfigurationTemplate",
             "CreateRecoveryInstanceForDrs",
             "CreateReplicationConfigurationTemplate",
             "CreateSourceServerForDrs",
             "DeleteJob",
+            "DeleteLaunchConfigurationTemplate",
             "DeleteRecoveryInstance",
             "DeleteReplicationConfigurationTemplate",
             "DeleteSourceServer",
             "DescribeJobLogItems",
             "DescribeJobs",
+            "DescribeLaunchConfigurationTemplates",
             "DescribeRecoveryInstances",
             "DescribeRecoverySnapshots",
             "DescribeReplicationConfigurationTemplates",
             "DescribeReplicationServerAssociationsForDrs",
             "DescribeSnapshotRequestsForDrs",
             "DescribeSourceServers",
             "DisconnectRecoveryInstance",
@@ -5921,14 +5924,15 @@
             "UpdateAgentReplicationInfoForDrs",
             "UpdateAgentReplicationProcessStateForDrs",
             "UpdateAgentSourcePropertiesForDrs",
             "UpdateFailbackClientDeviceMappingForDrs",
             "UpdateFailbackClientLastSeenForDrs",
             "UpdateFailbackReplicationConfiguration",
             "UpdateLaunchConfiguration",
+            "UpdateLaunchConfigurationTemplate",
             "UpdateReplicationCertificateForDrs",
             "UpdateReplicationConfiguration",
             "UpdateReplicationConfigurationTemplate"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
```

### Comparing `iam_actions-1.2.20230416/pyproject.toml` & `iam_actions-1.2.20230417/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230416"
+version = "1.2.20230417"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230416/setup.py` & `iam_actions-1.2.20230417/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230416',
+    'version': '1.2.20230417',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230416/PKG-INFO` & `iam_actions-1.2.20230417/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230416
+Version: 1.2.20230417
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

