# Comparing `tmp/mbonig.state-machine-0.0.22.tar.gz` & `tmp/mbonig.state-machine-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbonig.state-machine-0.0.22.tar", last modified: Mon Apr 17 13:34:00 2023, max compression
+gzip compressed data, was "mbonig.state-machine-0.0.23.tar", last modified: Mon Apr 17 13:48:10 2023, max compression
```

## Comparing `mbonig.state-machine-0.0.22.tar` & `mbonig.state-machine-0.0.23.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:34:00.468959 mbonig.state-machine-0.0.22/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-17 13:34:00.468959 mbonig.state-machine-0.0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:34:00.468959 mbonig.state-machine-0.0.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:34:00.464959 mbonig.state-machine-0.0.22/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:34:00.464959 mbonig.state-machine-0.0.22/src/mbonig/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:34:00.468959 mbonig.state-machine-0.0.22/src/mbonig/state_machine/
--rw-r--r--   0 runner    (1001) docker     (123)    21979 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/src/mbonig/state_machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:34:00.468959 mbonig.state-machine-0.0.22/src/mbonig/state_machine/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/src/mbonig/state_machine/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60486 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/src/mbonig/state_machine/_jsii/state-machine@0.0.22.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:33:47.000000 mbonig.state-machine-0.0.22/src/mbonig/state_machine/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:34:00.468959 mbonig.state-machine-0.0.22/src/mbonig.state_machine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-17 13:33:59.000000 mbonig.state-machine-0.0.22/src/mbonig.state_machine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-17 13:34:00.000000 mbonig.state-machine-0.0.22/src/mbonig.state_machine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:33:59.000000 mbonig.state-machine-0.0.22/src/mbonig.state_machine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-17 13:34:00.000000 mbonig.state-machine-0.0.22/src/mbonig.state_machine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 13:34:00.000000 mbonig.state-machine-0.0.22/src/mbonig.state_machine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:10.684103 mbonig.state-machine-0.0.23/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-04-17 13:48:10.680103 mbonig.state-machine-0.0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:48:10.684103 mbonig.state-machine-0.0.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:10.680103 mbonig.state-machine-0.0.23/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:10.680103 mbonig.state-machine-0.0.23/src/mbonig/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:10.680103 mbonig.state-machine-0.0.23/src/mbonig/state_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)    23458 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/src/mbonig/state_machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:10.680103 mbonig.state-machine-0.0.23/src/mbonig/state_machine/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/src/mbonig/state_machine/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   203418 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/src/mbonig/state_machine/_jsii/state-machine@0.0.23.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/src/mbonig/state_machine/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:10.680103 mbonig.state-machine-0.0.23/src/mbonig.state_machine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-04-17 13:48:10.000000 mbonig.state-machine-0.0.23/src/mbonig.state_machine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-17 13:48:10.000000 mbonig.state-machine-0.0.23/src/mbonig.state_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:48:10.000000 mbonig.state-machine-0.0.23/src/mbonig.state_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-17 13:48:10.000000 mbonig.state-machine-0.0.23/src/mbonig.state_machine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 13:48:10.000000 mbonig.state-machine-0.0.23/src/mbonig.state_machine.egg-info/top_level.txt
```

### Comparing `mbonig.state-machine-0.0.22/LICENSE` & `mbonig.state-machine-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `mbonig.state-machine-0.0.22/PKG-INFO` & `mbonig.state-machine-0.0.23/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbonig.state-machine
-Version: 0.0.22
+Version: 0.0.23
 Summary: A Step Function state machine construct focused on working well with the Workflow Studio
 Home-page: https://github.com/mbonig/state-machine.git
 Author: Matthew Bonig<matthew.bonig@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/mbonig/state-machine.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -116,14 +116,33 @@
     '@matthewbonig/state-machine',
   ]
 });
 
 new StepFunctionsAutoDiscover(project, { extension: AWS_RECOMMENDED_JSON_EXT });
 ```
 
+### Yaml files
+
+Yaml files are supported as well. You can provide an extension to the AutoDiscover component to have it search for yaml files. If the file has 'yaml' or 'yml' anywhere in the name it will be parsed as yaml. If not, it will be parsed as json.
+
+```js
+// ...
+const { StepFunctionsAutoDiscover } = require('@matthewbonig/state-machine');
+
+const project = new awscdk.AwsCdkTypeScriptApp({
+  // ...,
+  deps: [
+    // ...,
+    '@matthewbonig/state-machine',
+  ]
+});
+
+new StepFunctionsAutoDiscover(project, { extension: '.yaml.asl' });
+```
+
 ### Examples
 
 ```python
 const secret = new Secret(stack, 'Secret', {});
 new StateMachine(stack, 'Test', {
   stateMachineName: 'A nice state machine',
   definition: JSON.parse(fs.readFileSync(path.join(__dirname, 'sample.json'), 'utf8').toString()),
```

### Comparing `mbonig.state-machine-0.0.22/README.md` & `mbonig.state-machine-0.0.23/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -92,14 +92,33 @@
     '@matthewbonig/state-machine',
   ]
 });
 
 new StepFunctionsAutoDiscover(project, { extension: AWS_RECOMMENDED_JSON_EXT });
 ```
 
+### Yaml files
+
+Yaml files are supported as well. You can provide an extension to the AutoDiscover component to have it search for yaml files. If the file has 'yaml' or 'yml' anywhere in the name it will be parsed as yaml. If not, it will be parsed as json.
+
+```js
+// ...
+const { StepFunctionsAutoDiscover } = require('@matthewbonig/state-machine');
+
+const project = new awscdk.AwsCdkTypeScriptApp({
+  // ...,
+  deps: [
+    // ...,
+    '@matthewbonig/state-machine',
+  ]
+});
+
+new StepFunctionsAutoDiscover(project, { extension: '.yaml.asl' });
+```
+
 ### Examples
 
 ```python
 const secret = new Secret(stack, 'Secret', {});
 new StateMachine(stack, 'Test', {
   stateMachineName: 'A nice state machine',
   definition: JSON.parse(fs.readFileSync(path.join(__dirname, 'sample.json'), 'utf8').toString()),
```

### Comparing `mbonig.state-machine-0.0.22/setup.py` & `mbonig.state-machine-0.0.23/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "mbonig.state-machine",
-    "version": "0.0.22",
+    "version": "0.0.23",
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
-            "state-machine@0.0.22.jsii.tgz"
+            "state-machine@0.0.23.jsii.tgz"
         ],
         "mbonig.state_machine": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `mbonig.state-machine-0.0.22/src/mbonig/state_machine/__init__.py` & `mbonig.state-machine-0.0.23/src/mbonig/state_machine/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,33 @@
     '@matthewbonig/state-machine',
   ]
 });
 
 new StepFunctionsAutoDiscover(project, { extension: AWS_RECOMMENDED_JSON_EXT });
 ```
 
+### Yaml files
+
+Yaml files are supported as well. You can provide an extension to the AutoDiscover component to have it search for yaml files. If the file has 'yaml' or 'yml' anywhere in the name it will be parsed as yaml. If not, it will be parsed as json.
+
+```js
+// ...
+const { StepFunctionsAutoDiscover } = require('@matthewbonig/state-machine');
+
+const project = new awscdk.AwsCdkTypeScriptApp({
+  // ...,
+  deps: [
+    // ...,
+    '@matthewbonig/state-machine',
+  ]
+});
+
+new StepFunctionsAutoDiscover(project, { extension: '.yaml.asl' });
+```
+
 ### Examples
 
 ```python
 const secret = new Secret(stack, 'Secret', {});
 new StateMachine(stack, 'Test', {
   stateMachineName: 'A nice state machine',
   definition: JSON.parse(fs.readFileSync(path.join(__dirname, 'sample.json'), 'utf8').toString()),
@@ -247,40 +266,43 @@
 ):
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         definition: typing.Any,
+        asl_yaml: typing.Optional[builtins.bool] = None,
         logs: typing.Optional[typing.Union[_aws_cdk_aws_stepfunctions_ceddda9d.LogOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         overrides: typing.Any = None,
         role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         state_machine_type: typing.Optional[_aws_cdk_aws_stepfunctions_ceddda9d.StateMachineType] = None,
         timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         tracing_enabled: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param definition: An object that can be serialized into an ASL.
+        :param asl_yaml: Should the ASL definition be written as YAML. Default: false
         :param logs: Defines what execution history events are logged and where they are logged. Default: No logging
         :param overrides: An object that matches the schema/shape of the ASL .States map with overridden values.
         :param role: The execution role for the state machine service. Default: A role is automatically created
         :param state_machine_name: A name for the state machine. Default: A name is automatically generated
         :param state_machine_type: Type of the state machine. Default: StateMachineType.STANDARD
         :param timeout: Maximum run time for this state machine. Default: No timeout
         :param tracing_enabled: Specifies whether Amazon X-Ray tracing is enabled for this state machine. Default: false
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__470c1f9840bf90327b7a15067476a056d8e6c623b9641c0bbdfcefd7ad0958e3)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = StateMachineProps(
             definition=definition,
+            asl_yaml=asl_yaml,
             logs=logs,
             overrides=overrides,
             role=role,
             state_machine_name=state_machine_name,
             state_machine_type=state_machine_type,
             timeout=timeout,
             tracing_enabled=tracing_enabled,
@@ -290,61 +312,67 @@
 
 
 @jsii.data_type(
     jsii_type="@matthewbonig/state-machine.StateMachineProps",
     jsii_struct_bases=[],
     name_mapping={
         "definition": "definition",
+        "asl_yaml": "aslYaml",
         "logs": "logs",
         "overrides": "overrides",
         "role": "role",
         "state_machine_name": "stateMachineName",
         "state_machine_type": "stateMachineType",
         "timeout": "timeout",
         "tracing_enabled": "tracingEnabled",
     },
 )
 class StateMachineProps:
     def __init__(
         self,
         *,
         definition: typing.Any,
+        asl_yaml: typing.Optional[builtins.bool] = None,
         logs: typing.Optional[typing.Union[_aws_cdk_aws_stepfunctions_ceddda9d.LogOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         overrides: typing.Any = None,
         role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         state_machine_type: typing.Optional[_aws_cdk_aws_stepfunctions_ceddda9d.StateMachineType] = None,
         timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         tracing_enabled: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param definition: An object that can be serialized into an ASL.
+        :param asl_yaml: Should the ASL definition be written as YAML. Default: false
         :param logs: Defines what execution history events are logged and where they are logged. Default: No logging
         :param overrides: An object that matches the schema/shape of the ASL .States map with overridden values.
         :param role: The execution role for the state machine service. Default: A role is automatically created
         :param state_machine_name: A name for the state machine. Default: A name is automatically generated
         :param state_machine_type: Type of the state machine. Default: StateMachineType.STANDARD
         :param timeout: Maximum run time for this state machine. Default: No timeout
         :param tracing_enabled: Specifies whether Amazon X-Ray tracing is enabled for this state machine. Default: false
         '''
         if isinstance(logs, dict):
             logs = _aws_cdk_aws_stepfunctions_ceddda9d.LogOptions(**logs)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__83faeefbcd93a9a43e3a73870180709f3f441ca4082b11c441a11477932acce8)
             check_type(argname="argument definition", value=definition, expected_type=type_hints["definition"])
+            check_type(argname="argument asl_yaml", value=asl_yaml, expected_type=type_hints["asl_yaml"])
             check_type(argname="argument logs", value=logs, expected_type=type_hints["logs"])
             check_type(argname="argument overrides", value=overrides, expected_type=type_hints["overrides"])
             check_type(argname="argument role", value=role, expected_type=type_hints["role"])
             check_type(argname="argument state_machine_name", value=state_machine_name, expected_type=type_hints["state_machine_name"])
             check_type(argname="argument state_machine_type", value=state_machine_type, expected_type=type_hints["state_machine_type"])
             check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
             check_type(argname="argument tracing_enabled", value=tracing_enabled, expected_type=type_hints["tracing_enabled"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "definition": definition,
         }
+        if asl_yaml is not None:
+            self._values["asl_yaml"] = asl_yaml
         if logs is not None:
             self._values["logs"] = logs
         if overrides is not None:
             self._values["overrides"] = overrides
         if role is not None:
             self._values["role"] = role
         if state_machine_name is not None:
@@ -360,14 +388,23 @@
     def definition(self) -> typing.Any:
         '''An object that can be serialized into an ASL.'''
         result = self._values.get("definition")
         assert result is not None, "Required property 'definition' is missing"
         return typing.cast(typing.Any, result)
 
     @builtins.property
+    def asl_yaml(self) -> typing.Optional[builtins.bool]:
+        '''Should the ASL definition be written as YAML.
+
+        :default: false
+        '''
+        result = self._values.get("asl_yaml")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def logs(self) -> typing.Optional[_aws_cdk_aws_stepfunctions_ceddda9d.LogOptions]:
         '''Defines what execution history events are logged and where they are logged.
 
         :default: No logging
         '''
         result = self._values.get("logs")
         return typing.cast(typing.Optional[_aws_cdk_aws_stepfunctions_ceddda9d.LogOptions], result)
@@ -525,28 +562,30 @@
 publication.publish()
 
 def _typecheckingstub__470c1f9840bf90327b7a15067476a056d8e6c623b9641c0bbdfcefd7ad0958e3(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     definition: typing.Any,
+    asl_yaml: typing.Optional[builtins.bool] = None,
     logs: typing.Optional[typing.Union[_aws_cdk_aws_stepfunctions_ceddda9d.LogOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     overrides: typing.Any = None,
     role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     state_machine_type: typing.Optional[_aws_cdk_aws_stepfunctions_ceddda9d.StateMachineType] = None,
     timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     tracing_enabled: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__83faeefbcd93a9a43e3a73870180709f3f441ca4082b11c441a11477932acce8(
     *,
     definition: typing.Any,
+    asl_yaml: typing.Optional[builtins.bool] = None,
     logs: typing.Optional[typing.Union[_aws_cdk_aws_stepfunctions_ceddda9d.LogOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     overrides: typing.Any = None,
     role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     state_machine_type: typing.Optional[_aws_cdk_aws_stepfunctions_ceddda9d.StateMachineType] = None,
     timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     tracing_enabled: typing.Optional[builtins.bool] = None,
```

### Comparing `mbonig.state-machine-0.0.22/src/mbonig.state_machine.egg-info/PKG-INFO` & `mbonig.state-machine-0.0.23/src/mbonig.state_machine.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbonig.state-machine
-Version: 0.0.22
+Version: 0.0.23
 Summary: A Step Function state machine construct focused on working well with the Workflow Studio
 Home-page: https://github.com/mbonig/state-machine.git
 Author: Matthew Bonig<matthew.bonig@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/mbonig/state-machine.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -116,14 +116,33 @@
     '@matthewbonig/state-machine',
   ]
 });
 
 new StepFunctionsAutoDiscover(project, { extension: AWS_RECOMMENDED_JSON_EXT });
 ```
 
+### Yaml files
+
+Yaml files are supported as well. You can provide an extension to the AutoDiscover component to have it search for yaml files. If the file has 'yaml' or 'yml' anywhere in the name it will be parsed as yaml. If not, it will be parsed as json.
+
+```js
+// ...
+const { StepFunctionsAutoDiscover } = require('@matthewbonig/state-machine');
+
+const project = new awscdk.AwsCdkTypeScriptApp({
+  // ...,
+  deps: [
+    // ...,
+    '@matthewbonig/state-machine',
+  ]
+});
+
+new StepFunctionsAutoDiscover(project, { extension: '.yaml.asl' });
+```
+
 ### Examples
 
 ```python
 const secret = new Secret(stack, 'Secret', {});
 new StateMachine(stack, 'Test', {
   stateMachineName: 'A nice state machine',
   definition: JSON.parse(fs.readFileSync(path.join(__dirname, 'sample.json'), 'utf8').toString()),
```

