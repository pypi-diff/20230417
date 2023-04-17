# Comparing `tmp/cdktf-github-actions-0.0.88.tar.gz` & `tmp/cdktf-github-actions-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-github-actions-0.0.88.tar", last modified: Mon Apr 17 00:28:47 2023, max compression
+gzip compressed data, was "cdktf-github-actions-0.0.9.tar", last modified: Wed Jan 25 01:45:21 2023, max compression
```

## Comparing `cdktf-github-actions-0.0.88.tar` & `cdktf-github-actions-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:28:47.048966 cdktf-github-actions-0.0.88/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 00:28:35.000000 cdktf-github-actions-0.0.88/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 00:28:35.000000 cdktf-github-actions-0.0.88/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-17 00:28:47.048966 cdktf-github-actions-0.0.88/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-17 00:28:35.000000 cdktf-github-actions-0.0.88/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-17 00:28:35.000000 cdktf-github-actions-0.0.88/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 00:28:47.048966 cdktf-github-actions-0.0.88/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-17 00:28:35.000000 cdktf-github-actions-0.0.88/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:28:47.048966 cdktf-github-actions-0.0.88/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:28:47.048966 cdktf-github-actions-0.0.88/src/cdktf_github-actions/
--rw-r--r--   0 runner    (1001) docker     (123)   190483 2023-04-17 00:28:35.000000 cdktf-github-actions-0.0.88/src/cdktf_github-actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:28:47.048966 cdktf-github-actions-0.0.88/src/cdktf_github-actions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-17 00:28:35.000000 cdktf-github-actions-0.0.88/src/cdktf_github-actions/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   189086 2023-04-17 00:28:35.000000 cdktf-github-actions-0.0.88/src/cdktf_github-actions/_jsii/cdktf-github-actions@0.0.88.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 00:28:35.000000 cdktf-github-actions-0.0.88/src/cdktf_github-actions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:28:47.048966 cdktf-github-actions-0.0.88/src/cdktf_github_actions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-17 00:28:47.000000 cdktf-github-actions-0.0.88/src/cdktf_github_actions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-17 00:28:47.000000 cdktf-github-actions-0.0.88/src/cdktf_github_actions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 00:28:47.000000 cdktf-github-actions-0.0.88/src/cdktf_github_actions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-17 00:28:47.000000 cdktf-github-actions-0.0.88/src/cdktf_github_actions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 00:28:47.000000 cdktf-github-actions-0.0.88/src/cdktf_github_actions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:45:21.489591 cdktf-github-actions-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-25 01:45:09.000000 cdktf-github-actions-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-25 01:45:09.000000 cdktf-github-actions-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-01-25 01:45:21.489591 cdktf-github-actions-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-01-25 01:45:09.000000 cdktf-github-actions-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-25 01:45:09.000000 cdktf-github-actions-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 01:45:21.489591 cdktf-github-actions-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-01-25 01:45:09.000000 cdktf-github-actions-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:45:21.485591 cdktf-github-actions-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:45:21.485591 cdktf-github-actions-0.0.9/src/cdktf_github-actions/
+-rw-r--r--   0 runner    (1001) docker     (123)   190483 2023-01-25 01:45:09.000000 cdktf-github-actions-0.0.9/src/cdktf_github-actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:45:21.485591 cdktf-github-actions-0.0.9/src/cdktf_github-actions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-01-25 01:45:09.000000 cdktf-github-actions-0.0.9/src/cdktf_github-actions/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   177526 2023-01-25 01:45:09.000000 cdktf-github-actions-0.0.9/src/cdktf_github-actions/_jsii/cdktf-github-actions@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 01:45:09.000000 cdktf-github-actions-0.0.9/src/cdktf_github-actions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:45:21.485591 cdktf-github-actions-0.0.9/src/cdktf_github_actions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-01-25 01:45:20.000000 cdktf-github-actions-0.0.9/src/cdktf_github_actions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-01-25 01:45:21.000000 cdktf-github-actions-0.0.9/src/cdktf_github_actions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 01:45:21.000000 cdktf-github-actions-0.0.9/src/cdktf_github_actions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-01-25 01:45:21.000000 cdktf-github-actions-0.0.9/src/cdktf_github_actions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-25 01:45:21.000000 cdktf-github-actions-0.0.9/src/cdktf_github_actions.egg-info/top_level.txt
```

### Comparing `cdktf-github-actions-0.0.88/LICENSE` & `cdktf-github-actions-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-github-actions-0.0.88/PKG-INFO` & `cdktf-github-actions-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-github-actions
-Version: 0.0.88
+Version: 0.0.9
 Summary: @awlsring/cdktf-github-actions
 Home-page: https://github.com/awlsring/cdktf-github-actions.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-github-actions.git
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -108,7 +108,9 @@
 }
 
 const stack = new MyWorkflowStack(app, 'test');
 app.synth();
 ```
 
 The example above will create a secret with the name `MY_SECRET` and the value `123` in the repository. The secret will be referenced in the workflow using the name `token`.
+
+
```

### Comparing `cdktf-github-actions-0.0.88/README.md` & `cdktf-github-actions-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-github-actions-0.0.88/setup.py` & `cdktf-github-actions-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-github-actions",
-    "version": "0.0.88",
+    "version": "0.0.9",
     "description": "@awlsring/cdktf-github-actions",
     "license": "Apache-2.0",
     "url": "https://github.com/awlsring/cdktf-github-actions.git",
     "long_description_content_type": "text/markdown",
     "author": "awlsring<mattcanemail@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,39 +22,38 @@
     },
     "packages": [
         "cdktf_github-actions",
         "cdktf_github-actions._jsii"
     ],
     "package_data": {
         "cdktf_github-actions._jsii": [
-            "cdktf-github-actions@0.0.88.jsii.tgz"
+            "cdktf-github-actions@0.0.9.jsii.tgz"
         ],
         "cdktf_github-actions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdktf-cdktf-provider-github>=5.0.4, <6.0.0",
         "cdktf>=0.14.3, <0.15.0",
         "constructs>=10.1.52, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.73.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdktf-github-actions-0.0.88/src/cdktf_github-actions/__init__.py` & `cdktf-github-actions-0.0.9/src/cdktf_github-actions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-github-actions-0.0.88/src/cdktf_github_actions.egg-info/PKG-INFO` & `cdktf-github-actions-0.0.9/src/cdktf_github_actions.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-github-actions
-Version: 0.0.88
+Version: 0.0.9
 Summary: @awlsring/cdktf-github-actions
 Home-page: https://github.com/awlsring/cdktf-github-actions.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-github-actions.git
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -108,7 +108,9 @@
 }
 
 const stack = new MyWorkflowStack(app, 'test');
 app.synth();
 ```
 
 The example above will create a secret with the name `MY_SECRET` and the value `123` in the repository. The secret will be referenced in the workflow using the name `token`.
+
+
```

