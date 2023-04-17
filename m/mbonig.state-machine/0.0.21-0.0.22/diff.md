# Comparing `tmp/mbonig.state-machine-0.0.21.tar.gz` & `tmp/mbonig.state-machine-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbonig.state-machine-0.0.21.tar", last modified: Fri Dec 30 02:51:42 2022, max compression
+gzip compressed data, was "mbonig.state-machine-0.0.22.tar", last modified: Mon Apr 17 13:34:00 2023, max compression
```

## Comparing `mbonig.state-machine-0.0.21.tar` & `mbonig.state-machine-0.0.22.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 02:51:42.974061 mbonig.state-machine-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-12-30 02:51:29.000000 mbonig.state-machine-0.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-30 02:51:29.000000 mbonig.state-machine-0.0.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2022-12-30 02:51:42.974061 mbonig.state-machine-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2022-12-30 02:51:29.000000 mbonig.state-machine-0.0.21/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-30 02:51:29.000000 mbonig.state-machine-0.0.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-30 02:51:42.974061 mbonig.state-machine-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2022-12-30 02:51:29.000000 mbonig.state-machine-0.0.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 02:51:42.974061 mbonig.state-machine-0.0.21/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 02:51:42.974061 mbonig.state-machine-0.0.21/src/mbonig/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 02:51:42.974061 mbonig.state-machine-0.0.21/src/mbonig/state_machine/
--rw-r--r--   0 runner    (1001) docker     (123)    19685 2022-12-30 02:51:29.000000 mbonig.state-machine-0.0.21/src/mbonig/state_machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 02:51:42.974061 mbonig.state-machine-0.0.21/src/mbonig/state_machine/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2022-12-30 02:51:29.000000 mbonig.state-machine-0.0.21/src/mbonig/state_machine/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59239 2022-12-30 02:51:29.000000 mbonig.state-machine-0.0.21/src/mbonig/state_machine/_jsii/state-machine@0.0.21.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 02:51:29.000000 mbonig.state-machine-0.0.21/src/mbonig/state_machine/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 02:51:42.974061 mbonig.state-machine-0.0.21/src/mbonig.state_machine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2022-12-30 02:51:42.000000 mbonig.state-machine-0.0.21/src/mbonig.state_machine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2022-12-30 02:51:42.000000 mbonig.state-machine-0.0.21/src/mbonig.state_machine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 02:51:42.000000 mbonig.state-machine-0.0.21/src/mbonig.state_machine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2022-12-30 02:51:42.000000 mbonig.state-machine-0.0.21/src/mbonig.state_machine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-30 02:51:42.000000 mbonig.state-machine-0.0.21/src/mbonig.state_machine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:34:00.468959 mbonig.state-machine-0.0.22/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-17 13:34:00.468959 mbonig.state-machine-0.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:34:00.468959 mbonig.state-machine-0.0.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:34:00.464959 mbonig.state-machine-0.0.22/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:34:00.464959 mbonig.state-machine-0.0.22/src/mbonig/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:34:00.468959 mbonig.state-machine-0.0.22/src/mbonig/state_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)    21979 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/src/mbonig/state_machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:34:00.468959 mbonig.state-machine-0.0.22/src/mbonig/state_machine/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/src/mbonig/state_machine/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60486 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/src/mbonig/state_machine/_jsii/state-machine@0.0.22.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/src/mbonig/state_machine/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:34:00.468959 mbonig.state-machine-0.0.22/src/mbonig.state_machine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-17 13:33:59.000000 mbonig.state-machine-0.0.22/src/mbonig.state_machine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-17 13:34:00.000000 mbonig.state-machine-0.0.22/src/mbonig.state_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:33:59.000000 mbonig.state-machine-0.0.22/src/mbonig.state_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-17 13:34:00.000000 mbonig.state-machine-0.0.22/src/mbonig.state_machine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 13:34:00.000000 mbonig.state-machine-0.0.22/src/mbonig.state_machine.egg-info/top_level.txt
```

### Comparing `mbonig.state-machine-0.0.21/LICENSE` & `mbonig.state-machine-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `mbonig.state-machine-0.0.21/PKG-INFO` & `mbonig.state-machine-0.0.22/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: mbonig.state-machine
-Version: 0.0.21
-Summary: A Step Function state machine construct focused on working well with the Workflow Studio
-Home-page: https://github.com/mbonig/state-machine.git
-Author: Matthew Bonig<matthew.bonig@gmail.com>
-License: Apache-2.0
-Project-URL: Source, https://github.com/mbonig/state-machine.git
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Typing :: Typed
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Workflow Studio compatible State Machine
 
 [![View on Construct Hub](https://constructs.dev/badge?package=%40matthewbonig%2Fstate-machine)](https://constructs.dev/packages/@matthewbonig/state-machine)
 
 This is a Workflow Studio compatible AWS Step Function state machine construct.
 
 The goal of this construct is to make it easy to build and maintain your state machines using the Workflow Studio but still
@@ -93,14 +69,37 @@
   }
 }
 ```
 
 > :warning: **The interfaces and constructs generated here are NOT jsii compliant (they use Partials and Omits) and cannot be
 > compiled by jsii into other languages. If you plan to distribute any libraries you cannot use this.**
 
+### Alternative Extensions
+
+There is an optional parameter, `extension` that you can pass to have it search for alternative extensions.
+AWS recommends that ASL definition files have a `.asl.json` extension, which will be picked up by some IDE
+tools. This extension was recommended after initial development of this component. Therefore, the default is
+to use the original extension. But, you can override this by passing a different extension to the
+AutoDiscover's constructor options. There are two constants defined, `JSON_STEPFUNCTION_EXT` and `AWS_RECOMMENDED_JSON_EXT` that you can use.
+
+```js
+// ...
+const { StepFunctionsAutoDiscover, AWS_RECOMMENDED_EXT } = require('@matthewbonig/state-machine');
+
+const project = new awscdk.AwsCdkTypeScriptApp({
+  // ...,
+  deps: [
+    // ...,
+    '@matthewbonig/state-machine',
+  ]
+});
+
+new StepFunctionsAutoDiscover(project, { extension: AWS_RECOMMENDED_JSON_EXT });
+```
+
 ### Examples
 
 ```python
 const secret = new Secret(stack, 'Secret', {});
 new StateMachine(stack, 'Test', {
   stateMachineName: 'A nice state machine',
   definition: JSON.parse(fs.readFileSync(path.join(__dirname, 'sample.json'), 'utf8').toString()),
@@ -213,9 +212,7 @@
 ## Issues
 
 Please open any issues you have on [Github](https://github.com/mbonig/state-machine/issues).
 
 ## Contributing
 
 Please submit PRs from forked repositories if you'd like to contribute.
-
-
```

### Comparing `mbonig.state-machine-0.0.21/setup.py` & `mbonig.state-machine-0.0.22/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "mbonig.state-machine",
-    "version": "0.0.21",
+    "version": "0.0.22",
     "description": "A Step Function state machine construct focused on working well with the Workflow Studio",
     "license": "Apache-2.0",
     "url": "https://github.com/mbonig/state-machine.git",
     "long_description_content_type": "text/markdown",
     "author": "Matthew Bonig<matthew.bonig@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "mbonig.state_machine",
         "mbonig.state_machine._jsii"
     ],
     "package_data": {
         "mbonig.state_machine._jsii": [
-            "state-machine@0.0.21.jsii.tgz"
+            "state-machine@0.0.22.jsii.tgz"
         ],
         "mbonig.state_machine": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `mbonig.state-machine-0.0.21/src/mbonig/state_machine/__init__.py` & `mbonig.state-machine-0.0.22/src/mbonig/state_machine/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,37 @@
   }
 }
 ```
 
 > :warning: **The interfaces and constructs generated here are NOT jsii compliant (they use Partials and Omits) and cannot be
 > compiled by jsii into other languages. If you plan to distribute any libraries you cannot use this.**
 
+### Alternative Extensions
+
+There is an optional parameter, `extension` that you can pass to have it search for alternative extensions.
+AWS recommends that ASL definition files have a `.asl.json` extension, which will be picked up by some IDE
+tools. This extension was recommended after initial development of this component. Therefore, the default is
+to use the original extension. But, you can override this by passing a different extension to the
+AutoDiscover's constructor options. There are two constants defined, `JSON_STEPFUNCTION_EXT` and `AWS_RECOMMENDED_JSON_EXT` that you can use.
+
+```js
+// ...
+const { StepFunctionsAutoDiscover, AWS_RECOMMENDED_EXT } = require('@matthewbonig/state-machine');
+
+const project = new awscdk.AwsCdkTypeScriptApp({
+  // ...,
+  deps: [
+    // ...,
+    '@matthewbonig/state-machine',
+  ]
+});
+
+new StepFunctionsAutoDiscover(project, { extension: AWS_RECOMMENDED_JSON_EXT });
+```
+
 ### Examples
 
 ```python
 const secret = new Secret(stack, 'Secret', {});
 new StateMachine(stack, 'Test', {
   stateMachineName: 'A nice state machine',
   definition: JSON.parse(fs.readFileSync(path.join(__dirname, 'sample.json'), 'utf8').toString()),
@@ -432,38 +455,57 @@
        new StepFunctionsAutoDiscover(project);
 
     And any *.workflow.json file will cause the generation of a new strongly-typed StateMachine-derived class you can use.
     Note that these constructs are NOT jsii-compatible. If you need that,
     please open an `issue <https://github.com/mbonig/state-machine/issues/new>`_
     '''
 
-    def __init__(self, project: _projen_awscdk_04054675.AwsCdkTypeScriptApp) -> None:
+    def __init__(
+        self,
+        project: _projen_awscdk_04054675.AwsCdkTypeScriptApp,
+        *,
+        extension: typing.Optional[builtins.str] = None,
+    ) -> None:
         '''
         :param project: -
+        :param extension: An optional extension to use for discovering state machine files. Default: '.workflow.json' (JSON_STEPFUNCTION_EXT)
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c649450e91e3d86f8bc8dcd15b8fc411dc8026258b00a2237b8e6584ba5a685f)
             check_type(argname="argument project", value=project, expected_type=type_hints["project"])
-        _options = StepFunctionsAutoDiscoverOptions()
+        _options = StepFunctionsAutoDiscoverOptions(extension=extension)
 
         jsii.create(self.__class__, self, [project, _options])
 
 
 @jsii.data_type(
     jsii_type="@matthewbonig/state-machine.StepFunctionsAutoDiscoverOptions",
     jsii_struct_bases=[],
-    name_mapping={},
+    name_mapping={"extension": "extension"},
 )
 class StepFunctionsAutoDiscoverOptions:
-    def __init__(self) -> None:
-        '''For future use.
-
-        No properties, yet.
+    def __init__(self, *, extension: typing.Optional[builtins.str] = None) -> None:
+        '''
+        :param extension: An optional extension to use for discovering state machine files. Default: '.workflow.json' (JSON_STEPFUNCTION_EXT)
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b4f1d2b9a4db46b698e396f194da56d74c782e43b0713389383441bd9dcf9ce3)
+            check_type(argname="argument extension", value=extension, expected_type=type_hints["extension"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if extension is not None:
+            self._values["extension"] = extension
+
+    @builtins.property
+    def extension(self) -> typing.Optional[builtins.str]:
+        '''An optional extension to use for discovering state machine files.
+
+        :default: '.workflow.json' (JSON_STEPFUNCTION_EXT)
+        '''
+        result = self._values.get("extension")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -510,10 +552,19 @@
     tracing_enabled: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__c649450e91e3d86f8bc8dcd15b8fc411dc8026258b00a2237b8e6584ba5a685f(
     project: _projen_awscdk_04054675.AwsCdkTypeScriptApp,
+    *,
+    extension: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b4f1d2b9a4db46b698e396f194da56d74c782e43b0713389383441bd9dcf9ce3(
+    *,
+    extension: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `mbonig.state-machine-0.0.21/src/mbonig.state_machine.egg-info/PKG-INFO` & `mbonig.state-machine-0.0.22/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbonig.state-machine
-Version: 0.0.21
+Version: 0.0.22
 Summary: A Step Function state machine construct focused on working well with the Workflow Studio
 Home-page: https://github.com/mbonig/state-machine.git
 Author: Matthew Bonig<matthew.bonig@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/mbonig/state-machine.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -93,14 +93,37 @@
   }
 }
 ```
 
 > :warning: **The interfaces and constructs generated here are NOT jsii compliant (they use Partials and Omits) and cannot be
 > compiled by jsii into other languages. If you plan to distribute any libraries you cannot use this.**
 
+### Alternative Extensions
+
+There is an optional parameter, `extension` that you can pass to have it search for alternative extensions.
+AWS recommends that ASL definition files have a `.asl.json` extension, which will be picked up by some IDE
+tools. This extension was recommended after initial development of this component. Therefore, the default is
+to use the original extension. But, you can override this by passing a different extension to the
+AutoDiscover's constructor options. There are two constants defined, `JSON_STEPFUNCTION_EXT` and `AWS_RECOMMENDED_JSON_EXT` that you can use.
+
+```js
+// ...
+const { StepFunctionsAutoDiscover, AWS_RECOMMENDED_EXT } = require('@matthewbonig/state-machine');
+
+const project = new awscdk.AwsCdkTypeScriptApp({
+  // ...,
+  deps: [
+    // ...,
+    '@matthewbonig/state-machine',
+  ]
+});
+
+new StepFunctionsAutoDiscover(project, { extension: AWS_RECOMMENDED_JSON_EXT });
+```
+
 ### Examples
 
 ```python
 const secret = new Secret(stack, 'Secret', {});
 new StateMachine(stack, 'Test', {
   stateMachineName: 'A nice state machine',
   definition: JSON.parse(fs.readFileSync(path.join(__dirname, 'sample.json'), 'utf8').toString()),
```

