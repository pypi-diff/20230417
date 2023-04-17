# Comparing `tmp/chaostoolkit-aws-0.8.0.tar.gz` & `tmp/chaostoolkit-aws-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chaostoolkit-aws-0.8.0.tar", last modified: Sat Oct  6 12:06:34 2018, max compression
+gzip compressed data, was "dist/chaostoolkit-aws-0.9.0.tar", last modified: Tue Nov 20 15:02:00 2018, max compression
```

## Comparing `chaostoolkit-aws-0.8.0.tar` & `chaostoolkit-aws-0.9.0.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:34.000000 chaostoolkit-aws-0.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11050 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     2563 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:34.000000 chaostoolkit-aws-0.8.0/chaostoolkit_aws.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2018-10-06 12:06:33.000000 chaostoolkit-aws-0.8.0/chaostoolkit_aws.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2018-10-06 12:06:33.000000 chaostoolkit-aws-0.8.0/chaostoolkit_aws.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    14826 2018-10-06 12:06:33.000000 chaostoolkit-aws-0.8.0/chaostoolkit_aws.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-10-06 12:06:33.000000 chaostoolkit-aws-0.8.0/chaostoolkit_aws.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      827 2018-10-06 12:06:34.000000 chaostoolkit-aws-0.8.0/chaostoolkit_aws.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3707 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      114 2018-10-06 12:06:34.000000 chaostoolkit-aws-0.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       57 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      127 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/requirements-dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    14826 2018-10-06 12:06:34.000000 chaostoolkit-aws-0.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      174 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/pytest.ini
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:34.000000 chaostoolkit-aws-0.8.0/chaosaws/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:34.000000 chaostoolkit-aws-0.8.0/chaosaws/elbv2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4716 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/elbv2/probes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/elbv2/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2943 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/elbv2/actions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7637 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:34.000000 chaostoolkit-aws-0.8.0/chaosaws/ecs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1401 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/ecs/probes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/ecs/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5917 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/ecs/actions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:34.000000 chaostoolkit-aws-0.8.0/chaosaws/asg/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8724 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/asg/probes.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:34.000000 chaostoolkit-aws-0.8.0/chaosaws/eks/
--rw-rw-r--   0 travis    (2000) travis    (2000)      974 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/eks/probes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/eks/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1092 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/eks/actions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:34.000000 chaostoolkit-aws-0.8.0/chaosaws/awslambda/
--rw-rw-r--   0 travis    (2000) travis    (2000)      591 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/awslambda/probes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/awslambda/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1505 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/awslambda/actions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:34.000000 chaostoolkit-aws-0.8.0/chaosaws/ec2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1326 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/ec2/probes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/ec2/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8543 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/ec2/actions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:34.000000 chaostoolkit-aws-0.8.0/chaosaws/iam/
--rw-rw-r--   0 travis    (2000) travis    (2000)      436 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/iam/probes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/iam/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2091 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/iam/actions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2018-10-06 12:06:04.000000 chaostoolkit-aws-0.8.0/chaosaws/types.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11050 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2635 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/chaostoolkit_aws.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/chaostoolkit_aws.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       58 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/chaostoolkit_aws.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14876 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/chaostoolkit_aws.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/chaostoolkit_aws.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      920 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/chaostoolkit_aws.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4048 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/CHANGELOG.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      114 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)       57 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      127 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/requirements-dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14876 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      174 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/pytest.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/chaosaws/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/chaosaws/elbv2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4716 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/elbv2/probes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/elbv2/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2943 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/elbv2/actions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/chaosaws/cloudwatch/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3862 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/cloudwatch/probes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/cloudwatch/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4863 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/cloudwatch/actions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7777 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/chaosaws/ecs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1401 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/ecs/probes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/ecs/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5917 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/ecs/actions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/chaosaws/asg/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8724 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/asg/probes.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/chaosaws/eks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      974 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/eks/probes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/eks/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1092 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/eks/actions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/chaosaws/awslambda/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2493 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/awslambda/probes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/awslambda/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5443 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/awslambda/actions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/chaosaws/ec2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1326 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/ec2/probes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/ec2/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8543 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/ec2/actions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-20 15:02:00.000000 chaostoolkit-aws-0.9.0/chaosaws/iam/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      436 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/iam/probes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/iam/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2091 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/iam/actions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2018-11-20 15:01:30.000000 chaostoolkit-aws-0.9.0/chaosaws/types.py
```

### Comparing `chaostoolkit-aws-0.8.0/README.md` & `chaostoolkit-aws-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `chaostoolkit-aws-0.8.0/setup.py` & `chaostoolkit-aws-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     'License :: Freely Distributable',
     'Operating System :: OS Independent',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: Implementation',
     'Programming Language :: Python :: Implementation :: CPython'
 ]
 author = 'chaostoolkit Team'
 author_email = 'contact@chaostoolkit.org'
 url = 'http://chaostoolkit.org'
 license = 'Apache License Version 2.0'
@@ -48,15 +49,16 @@
     'chaosaws',
     'chaosaws.ecs',
     'chaosaws.ec2',
     'chaosaws.eks',
     'chaosaws.iam',
     'chaosaws.elbv2',
     'chaosaws.asg',
-    'chaosaws.awslambda'
+    'chaosaws.awslambda',
+    'chaosaws.cloudwatch'
 ]
 
 needs_pytest = set(['pytest', 'test']).intersection(sys.argv)
 pytest_runner = ['pytest_runner'] if needs_pytest else []
 
 test_require = []
 with io.open('requirements-dev.txt') as f:
```

### Comparing `chaostoolkit-aws-0.8.0/LICENSE` & `chaostoolkit-aws-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chaostoolkit-aws-0.8.0/chaostoolkit_aws.egg-info/PKG-INFO` & `chaostoolkit-aws-0.9.0/chaostoolkit_aws.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: chaostoolkit-aws
-Version: 0.8.0
+Version: 0.9.0
 Summary: Chaos Toolkit Extension for AWS
 Home-page: http://chaostoolkit.org
 Author: chaostoolkit Team
 Author-email: contact@chaostoolkit.org
 License: Apache License Version 2.0
 Description: # Chaos Toolkit Extension for AWS
         
@@ -377,10 +377,11 @@
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.5.*
```

### Comparing `chaostoolkit-aws-0.8.0/chaostoolkit_aws.egg-info/SOURCES.txt` & `chaostoolkit-aws-0.9.0/chaostoolkit_aws.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 setup.py
 chaosaws/__init__.py
 chaosaws/types.py
 chaosaws/asg/probes.py
 chaosaws/awslambda/__init__.py
 chaosaws/awslambda/actions.py
 chaosaws/awslambda/probes.py
+chaosaws/cloudwatch/__init__.py
+chaosaws/cloudwatch/actions.py
+chaosaws/cloudwatch/probes.py
 chaosaws/ec2/__init__.py
 chaosaws/ec2/actions.py
 chaosaws/ec2/probes.py
 chaosaws/ecs/__init__.py
 chaosaws/ecs/actions.py
 chaosaws/ecs/probes.py
 chaosaws/eks/__init__.py
```

### Comparing `chaostoolkit-aws-0.8.0/CHANGELOG.md` & `chaostoolkit-aws-0.9.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 # Changelog
 
 ## [Unreleased][]
 
-[Unreleased]: https://github.com/chaostoolkit-incubator/chaostoolkit-aws/compare/0.8.0...HEAD
+[Unreleased]: https://github.com/chaostoolkit-incubator/chaostoolkit-aws/compare/0.9.0...HEAD
+
+## [0.9.0][]
+
+[0.9.0]: https://github.com/chaostoolkit-incubator/chaostoolkit-aws/compare/0.8.0...0.9.0
+
+### Added
+
+-   support for Python 3.7
+-   support for cloudwatch probes and actions
+-   support for invoking lambdas
+-   support for getting and updating lambda timeout and memory size limits
+-   probe for cloudwatch metric statistics
 
 ## [0.8.0][]
 
 [0.8.0]: https://github.com/chaostoolkit-incubator/chaostoolkit-aws/compare/0.7.1...0.8.0
 
 ### Changed
```

### Comparing `chaostoolkit-aws-0.8.0/PKG-INFO` & `chaostoolkit-aws-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: chaostoolkit-aws
-Version: 0.8.0
+Version: 0.9.0
 Summary: Chaos Toolkit Extension for AWS
 Home-page: http://chaostoolkit.org
 Author: chaostoolkit Team
 Author-email: contact@chaostoolkit.org
 License: Apache License Version 2.0
 Description: # Chaos Toolkit Extension for AWS
         
@@ -377,10 +377,11 @@
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.5.*
```

### Comparing `chaostoolkit-aws-0.8.0/chaosaws/elbv2/probes.py` & `chaostoolkit-aws-0.9.0/chaosaws/elbv2/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-aws-0.8.0/chaosaws/elbv2/actions.py` & `chaostoolkit-aws-0.9.0/chaosaws/elbv2/actions.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-aws-0.8.0/chaosaws/__init__.py` & `chaostoolkit-aws-0.9.0/chaosaws/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from chaoslib.discovery.discover import (discover_actions, discover_probes,
                                          initialize_discovery_result)
 from chaoslib.exceptions import DiscoveryFailed
 from chaoslib.types import (Configuration, DiscoveredActivities,
                             DiscoveredSystemInfo, Discovery, Secrets)
 from logzero import logger
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 __all__ = ["__version__", "discover", "aws_client", "signed_api_call"]
 
 
 def get_credentials(secrets: Secrets = None) -> Dict[str, str]:
     """
     Credentialss may be provided via the secrets object. When they aren't,
     they will be loaded from the process environment (for instance, read from
@@ -179,9 +179,11 @@
     activities.extend(discover_actions("chaosaws.eks.actions"))
     activities.extend(discover_probes("chaosaws.eks.probes"))
     activities.extend(discover_actions("chaosaws.elbv2.actions"))
     activities.extend(discover_probes("chaosaws.elbv2.probes"))
     activities.extend(discover_probes("chaosaws.asg.probes"))
     activities.extend(discover_actions("chaosaws.awslambda.actions"))
     activities.extend(discover_probes("chaosaws.awslambda.probes"))
+    activities.extend(discover_actions("chaosaws.cloudwatch.actions"))
+    activities.extend(discover_probes("chaosaws.cloudwatch.probes"))
 
     return activities
```

### Comparing `chaostoolkit-aws-0.8.0/chaosaws/ecs/probes.py` & `chaostoolkit-aws-0.9.0/chaosaws/ecs/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-aws-0.8.0/chaosaws/ecs/actions.py` & `chaostoolkit-aws-0.9.0/chaosaws/ecs/actions.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-aws-0.8.0/chaosaws/asg/probes.py` & `chaostoolkit-aws-0.9.0/chaosaws/asg/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-aws-0.8.0/chaosaws/eks/probes.py` & `chaostoolkit-aws-0.9.0/chaosaws/eks/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-aws-0.8.0/chaosaws/eks/actions.py` & `chaostoolkit-aws-0.9.0/chaosaws/eks/actions.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-aws-0.8.0/chaosaws/ec2/probes.py` & `chaostoolkit-aws-0.9.0/chaosaws/ec2/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-aws-0.8.0/chaosaws/ec2/actions.py` & `chaostoolkit-aws-0.9.0/chaosaws/ec2/actions.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-aws-0.8.0/chaosaws/iam/actions.py` & `chaostoolkit-aws-0.9.0/chaosaws/iam/actions.py`

 * *Files identical despite different names*

