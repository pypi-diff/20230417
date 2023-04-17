# Comparing `tmp/cdk-ecs-service-extensions-2.0.0a99.tar.gz` & `tmp/cdk-ecs-service-extensions-2.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-ecs-service-extensions-2.0.0a99.tar", last modified: Wed Jul 27 00:33:56 2022, max compression
+gzip compressed data, was "cdk-ecs-service-extensions-2.0.1a0.tar", last modified: Mon Apr 17 00:27:24 2023, max compression
```

## Comparing `cdk-ecs-service-extensions-2.0.0a99.tar` & `cdk-ecs-service-extensions-2.0.1a0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 00:33:56.124487 cdk-ecs-service-extensions-2.0.0a99/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-27 00:33:42.000000 cdk-ecs-service-extensions-2.0.0a99/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-27 00:33:42.000000 cdk-ecs-service-extensions-2.0.0a99/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-07-27 00:33:42.000000 cdk-ecs-service-extensions-2.0.0a99/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)    24826 2022-07-27 00:33:56.124487 cdk-ecs-service-extensions-2.0.0a99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    23876 2022-07-27 00:33:42.000000 cdk-ecs-service-extensions-2.0.0a99/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-07-27 00:33:42.000000 cdk-ecs-service-extensions-2.0.0a99/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-27 00:33:56.124487 cdk-ecs-service-extensions-2.0.0a99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-07-27 00:33:42.000000 cdk-ecs-service-extensions-2.0.0a99/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 00:33:56.124487 cdk-ecs-service-extensions-2.0.0a99/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 00:33:56.124487 cdk-ecs-service-extensions-2.0.0a99/src/cdk_ecs_service_extensions/
--rw-r--r--   0 runner    (1001) docker     (121)   230694 2022-07-27 00:33:42.000000 cdk-ecs-service-extensions-2.0.0a99/src/cdk_ecs_service_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 00:33:56.124487 cdk-ecs-service-extensions-2.0.0a99/src/cdk_ecs_service_extensions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-07-27 00:33:42.000000 cdk-ecs-service-extensions-2.0.0a99/src/cdk_ecs_service_extensions/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   163510 2022-07-27 00:33:42.000000 cdk-ecs-service-extensions-2.0.0a99/src/cdk_ecs_service_extensions/_jsii/ecs-service-extensions@2.0.0-alpha.99.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-27 00:33:42.000000 cdk-ecs-service-extensions-2.0.0a99/src/cdk_ecs_service_extensions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 00:33:56.124487 cdk-ecs-service-extensions-2.0.0a99/src/cdk_ecs_service_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    24826 2022-07-27 00:33:55.000000 cdk-ecs-service-extensions-2.0.0a99/src/cdk_ecs_service_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-07-27 00:33:56.000000 cdk-ecs-service-extensions-2.0.0a99/src/cdk_ecs_service_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-27 00:33:55.000000 cdk-ecs-service-extensions-2.0.0a99/src/cdk_ecs_service_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-07-27 00:33:55.000000 cdk-ecs-service-extensions-2.0.0a99/src/cdk_ecs_service_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-07-27 00:33:56.000000 cdk-ecs-service-extensions-2.0.0a99/src/cdk_ecs_service_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:27:24.034754 cdk-ecs-service-extensions-2.0.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 00:27:05.000000 cdk-ecs-service-extensions-2.0.1a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 00:27:05.000000 cdk-ecs-service-extensions-2.0.1a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-17 00:27:05.000000 cdk-ecs-service-extensions-2.0.1a0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    25294 2023-04-17 00:27:24.034754 cdk-ecs-service-extensions-2.0.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24273 2023-04-17 00:27:05.000000 cdk-ecs-service-extensions-2.0.1a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-17 00:27:05.000000 cdk-ecs-service-extensions-2.0.1a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 00:27:24.034754 cdk-ecs-service-extensions-2.0.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-17 00:27:05.000000 cdk-ecs-service-extensions-2.0.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:27:24.030753 cdk-ecs-service-extensions-2.0.1a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:27:24.034754 cdk-ecs-service-extensions-2.0.1a0/src/cdk_ecs_service_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)   295093 2023-04-17 00:27:05.000000 cdk-ecs-service-extensions-2.0.1a0/src/cdk_ecs_service_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:27:24.034754 cdk-ecs-service-extensions-2.0.1a0/src/cdk_ecs_service_extensions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-17 00:27:05.000000 cdk-ecs-service-extensions-2.0.1a0/src/cdk_ecs_service_extensions/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171898 2023-04-17 00:27:05.000000 cdk-ecs-service-extensions-2.0.1a0/src/cdk_ecs_service_extensions/_jsii/ecs-service-extensions@2.0.1-alpha.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 00:27:05.000000 cdk-ecs-service-extensions-2.0.1a0/src/cdk_ecs_service_extensions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:27:24.034754 cdk-ecs-service-extensions-2.0.1a0/src/cdk_ecs_service_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25294 2023-04-17 00:27:24.000000 cdk-ecs-service-extensions-2.0.1a0/src/cdk_ecs_service_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-17 00:27:24.000000 cdk-ecs-service-extensions-2.0.1a0/src/cdk_ecs_service_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 00:27:24.000000 cdk-ecs-service-extensions-2.0.1a0/src/cdk_ecs_service_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 00:27:24.000000 cdk-ecs-service-extensions-2.0.1a0/src/cdk_ecs_service_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 00:27:24.000000 cdk-ecs-service-extensions-2.0.1a0/src/cdk_ecs_service_extensions.egg-info/top_level.txt
```

### Comparing `cdk-ecs-service-extensions-2.0.0a99/LICENSE` & `cdk-ecs-service-extensions-2.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-ecs-service-extensions-2.0.0a99/PKG-INFO` & `cdk-ecs-service-extensions-2.0.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-ecs-service-extensions
-Version: 2.0.0a99
-Summary: @aws-cdk-containers/ecs-service-extensions
+Version: 2.0.1a0
+Summary: The CDK Construct Library that helps you build ECS services using simple extensions
 Home-page: https://github.com/cdklabs/cdk-ecs-service-extensions.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-ecs-service-extensions.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
@@ -241,14 +241,33 @@
 const nameService = new Service(this, 'name', {
   environment: environment,
   serviceDescription: nameDescription,
   taskRole,
 });
 ```
 
+## Configure Custom Health Check
+
+When you add an HTTPLoadBalancerExtension, you can customize the health checks by accessing the targetGroup field on the service.
+
+```python
+const service = new Service(stack, 'my-service', {
+  environment,
+  serviceDescription,
+  autoScaleTaskCount: {
+    maxTaskCount: 5,
+  },
+});
+
+service.targetGroup.configureHealthCheck({
+  path: '/',
+  port: '80',
+});
+```
+
 ## Task Auto-Scaling
 
 You can configure the task count of a service to match demand. The recommended way of achieving this is to configure target tracking policies for your service which scales in and out in order to keep metrics around target values.
 
 You need to configure an auto scaling target for the service by setting the `minTaskCount` (defaults to 1) and `maxTaskCount` in the `Service` construct. Then you can specify target values for "CPU Utilization" or "Memory Utilization" across all tasks in your service. Note that the `desiredCount` value will be set to `undefined` if the auto scaling target is configured.
 
 If you want to configure auto-scaling policies based on resources like Application Load Balancer or SQS Queues, you can set the corresponding resource-specific fields in the extension. For example, you can enable target tracking scaling based on Application Load Balancer request count as follows:
@@ -591,9 +610,7 @@
 We encourage the development of Community Service Extensions that support
 advanced features. Here are some useful extensions that we have reviewed:
 
 * [ListenerRulesExtension](https://www.npmjs.com/package/@wheatstalk/ecs-service-extension-listener-rules) for more precise control over Application Load Balancer rules
 
 > Please submit a pull request so that we can review your service extension and
 > list it here.
-
-
```

### Comparing `cdk-ecs-service-extensions-2.0.0a99/README.md` & `cdk-ecs-service-extensions-2.0.1a0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,33 @@
 const nameService = new Service(this, 'name', {
   environment: environment,
   serviceDescription: nameDescription,
   taskRole,
 });
 ```
 
+## Configure Custom Health Check
+
+When you add an HTTPLoadBalancerExtension, you can customize the health checks by accessing the targetGroup field on the service.
+
+```python
+const service = new Service(stack, 'my-service', {
+  environment,
+  serviceDescription,
+  autoScaleTaskCount: {
+    maxTaskCount: 5,
+  },
+});
+
+service.targetGroup.configureHealthCheck({
+  path: '/',
+  port: '80',
+});
+```
+
 ## Task Auto-Scaling
 
 You can configure the task count of a service to match demand. The recommended way of achieving this is to configure target tracking policies for your service which scales in and out in order to keep metrics around target values.
 
 You need to configure an auto scaling target for the service by setting the `minTaskCount` (defaults to 1) and `maxTaskCount` in the `Service` construct. Then you can specify target values for "CPU Utilization" or "Memory Utilization" across all tasks in your service. Note that the `desiredCount` value will be set to `undefined` if the auto scaling target is configured.
 
 If you want to configure auto-scaling policies based on resources like Application Load Balancer or SQS Queues, you can set the corresponding resource-specific fields in the extension. For example, you can enable target tracking scaling based on Application Load Balancer request count as follows:
```

### Comparing `cdk-ecs-service-extensions-2.0.0a99/setup.py` & `cdk-ecs-service-extensions-2.0.1a0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-ecs-service-extensions",
-    "version": "2.0.0.a99",
-    "description": "@aws-cdk-containers/ecs-service-extensions",
+    "version": "2.0.1.a0",
+    "description": "The CDK Construct Library that helps you build ECS services using simple extensions",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-ecs-service-extensions.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
     },
@@ -22,37 +22,38 @@
     },
     "packages": [
         "cdk_ecs_service_extensions",
         "cdk_ecs_service_extensions._jsii"
     ],
     "package_data": {
         "cdk_ecs_service_extensions._jsii": [
-            "ecs-service-extensions@2.0.0-alpha.99.jsii.tgz"
+            "ecs-service-extensions@2.0.1-alpha.0.jsii.tgz"
         ],
         "cdk_ecs_service_extensions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.8.0, <3.0.0",
+        "aws-cdk-lib>=2.52.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.63.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
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
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdk-ecs-service-extensions-2.0.0a99/src/cdk_ecs_service_extensions/__init__.py` & `cdk-ecs-service-extensions-2.0.1a0/src/cdk_ecs_service_extensions/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -217,14 +217,33 @@
 const nameService = new Service(this, 'name', {
   environment: environment,
   serviceDescription: nameDescription,
   taskRole,
 });
 ```
 
+## Configure Custom Health Check
+
+When you add an HTTPLoadBalancerExtension, you can customize the health checks by accessing the targetGroup field on the service.
+
+```python
+const service = new Service(stack, 'my-service', {
+  environment,
+  serviceDescription,
+  autoScaleTaskCount: {
+    maxTaskCount: 5,
+  },
+});
+
+service.targetGroup.configureHealthCheck({
+  path: '/',
+  port: '80',
+});
+```
+
 ## Task Auto-Scaling
 
 You can configure the task count of a service to match demand. The recommended way of achieving this is to configure target tracking policies for your service which scales in and out in order to keep metrics around target values.
 
 You need to configure an auto scaling target for the service by setting the `minTaskCount` (defaults to 1) and `maxTaskCount` in the `Service` construct. Then you can specify target values for "CPU Utilization" or "Memory Utilization" across all tasks in your service. Note that the `desiredCount` value will be set to `undefined` if the auto scaling target is configured.
 
 If you want to configure auto-scaling policies based on resources like Application Load Balancer or SQS Queues, you can set the corresponding resource-specific fields in the extension. For example, you can enable target tracking scaling based on Application Load Balancer request count as follows:
@@ -582,50 +601,216 @@
 import publication
 import typing_extensions
 
 from typeguard import check_type
 
 from ._jsii import *
 
-import aws_cdk
-import aws_cdk.aws_appmesh
-import aws_cdk.aws_ec2
-import aws_cdk.aws_ecs
-import aws_cdk.aws_iam
-import aws_cdk.aws_logs
-import aws_cdk.aws_route53
-import aws_cdk.aws_servicediscovery
-import aws_cdk.aws_sns
-import aws_cdk.aws_sqs
-import constructs
+import aws_cdk as _aws_cdk_ceddda9d
+import aws_cdk.aws_appmesh as _aws_cdk_aws_appmesh_ceddda9d
+import aws_cdk.aws_ec2 as _aws_cdk_aws_ec2_ceddda9d
+import aws_cdk.aws_ecs as _aws_cdk_aws_ecs_ceddda9d
+import aws_cdk.aws_elasticloadbalancingv2 as _aws_cdk_aws_elasticloadbalancingv2_ceddda9d
+import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
+import aws_cdk.aws_logs as _aws_cdk_aws_logs_ceddda9d
+import aws_cdk.aws_route53 as _aws_cdk_aws_route53_ceddda9d
+import aws_cdk.aws_servicediscovery as _aws_cdk_aws_servicediscovery_ceddda9d
+import aws_cdk.aws_sns as _aws_cdk_aws_sns_ceddda9d
+import aws_cdk.aws_sqs as _aws_cdk_aws_sqs_ceddda9d
+import constructs as _constructs_77d1e7e8
+
+
+@jsii.data_type(
+    jsii_type="@aws-cdk-containers/ecs-service-extensions.AliasedPortMutatingHookProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "alias_port": "aliasPort",
+        "port_mapping_name": "portMappingName",
+        "protocol": "protocol",
+    },
+)
+class AliasedPortMutatingHookProps:
+    def __init__(
+        self,
+        *,
+        alias_port: jsii.Number,
+        port_mapping_name: builtins.str,
+        protocol: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.AppProtocol] = None,
+    ) -> None:
+        '''
+        :param alias_port: (experimental) The port on the container which receives traffic. This is the same as the ``containerPort`` property of port mapping.
+        :param port_mapping_name: (experimental) The name by which to refer to this port mapping.
+        :param protocol: (experimental) The protocol which this port mapping expects to receive. Default: - none
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9eafc8bc30298b419ba1305209f1f31afbf65c9b3456fc2c643e9dc4c1bd501a)
+            check_type(argname="argument alias_port", value=alias_port, expected_type=type_hints["alias_port"])
+            check_type(argname="argument port_mapping_name", value=port_mapping_name, expected_type=type_hints["port_mapping_name"])
+            check_type(argname="argument protocol", value=protocol, expected_type=type_hints["protocol"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "alias_port": alias_port,
+            "port_mapping_name": port_mapping_name,
+        }
+        if protocol is not None:
+            self._values["protocol"] = protocol
+
+    @builtins.property
+    def alias_port(self) -> jsii.Number:
+        '''(experimental) The port on the container which receives traffic.
+
+        This is the same as the ``containerPort`` property of port mapping.
+
+        :stability: experimental
+        '''
+        result = self._values.get("alias_port")
+        assert result is not None, "Required property 'alias_port' is missing"
+        return typing.cast(jsii.Number, result)
+
+    @builtins.property
+    def port_mapping_name(self) -> builtins.str:
+        '''(experimental) The name by which to refer to this port mapping.
+
+        :stability: experimental
+        '''
+        result = self._values.get("port_mapping_name")
+        assert result is not None, "Required property 'port_mapping_name' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def protocol(self) -> typing.Optional[_aws_cdk_aws_ecs_ceddda9d.AppProtocol]:
+        '''(experimental) The protocol which this port mapping expects to receive.
+
+        :default: - none
+
+        :stability: experimental
+        '''
+        result = self._values.get("protocol")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ecs_ceddda9d.AppProtocol], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "AliasedPortMutatingHookProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="@aws-cdk-containers/ecs-service-extensions.AliasedPortProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "alias": "alias",
+        "alias_port": "aliasPort",
+        "app_protocol": "appProtocol",
+    },
+)
+class AliasedPortProps:
+    def __init__(
+        self,
+        *,
+        alias: builtins.str,
+        alias_port: typing.Optional[jsii.Number] = None,
+        app_protocol: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.AppProtocol] = None,
+    ) -> None:
+        '''(experimental) AliasedPortProps defines the properties of an aliased port extension.
+
+        :param alias: (experimental) The DNS alias to advertise for downstream clients.
+        :param alias_port: (experimental) The traffic port for clients to use to connect to the DNS alias. Default: - same as containerPort.
+        :param app_protocol: (experimental) The protocol to use over the specified port. May be one of HTTP, HTTP2, or GRPC. Default: - none
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__7d89a6c579317235d028edb793a72ba2e7d3ccda1e4b1f2602503eea428e930c)
+            check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
+            check_type(argname="argument alias_port", value=alias_port, expected_type=type_hints["alias_port"])
+            check_type(argname="argument app_protocol", value=app_protocol, expected_type=type_hints["app_protocol"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "alias": alias,
+        }
+        if alias_port is not None:
+            self._values["alias_port"] = alias_port
+        if app_protocol is not None:
+            self._values["app_protocol"] = app_protocol
+
+    @builtins.property
+    def alias(self) -> builtins.str:
+        '''(experimental) The DNS alias to advertise for downstream clients.
+
+        :stability: experimental
+        '''
+        result = self._values.get("alias")
+        assert result is not None, "Required property 'alias' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def alias_port(self) -> typing.Optional[jsii.Number]:
+        '''(experimental) The traffic port for clients to use to connect to the DNS alias.
+
+        :default: - same as containerPort.
+
+        :stability: experimental
+        '''
+        result = self._values.get("alias_port")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def app_protocol(self) -> typing.Optional[_aws_cdk_aws_ecs_ceddda9d.AppProtocol]:
+        '''(experimental) The protocol to use over the specified port.
+
+        May be one of HTTP, HTTP2, or GRPC.
+
+        :default: - none
+
+        :stability: experimental
+        '''
+        result = self._values.get("app_protocol")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ecs_ceddda9d.AppProtocol], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "AliasedPortProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk-containers/ecs-service-extensions.AssignPublicIpDnsOptions",
     jsii_struct_bases=[],
     name_mapping={"record_name": "recordName", "zone": "zone"},
 )
 class AssignPublicIpDnsOptions:
     def __init__(
         self,
         *,
         record_name: builtins.str,
-        zone: aws_cdk.aws_route53.IHostedZone,
+        zone: _aws_cdk_aws_route53_ceddda9d.IHostedZone,
     ) -> None:
         '''
         :param record_name: (experimental) Name of the record to add to the zone and in which to add the task IP addresses to.
         :param zone: (experimental) A DNS Zone to expose task IPs in.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(AssignPublicIpDnsOptions.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__fa7fb8b6574fcc7a10ce0f47113796062053fc86dbd682d2487f7cdfb34d46d0)
             check_type(argname="argument record_name", value=record_name, expected_type=type_hints["record_name"])
             check_type(argname="argument zone", value=zone, expected_type=type_hints["zone"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "record_name": record_name,
             "zone": zone,
         }
 
     @builtins.property
     def record_name(self) -> builtins.str:
         '''(experimental) Name of the record to add to the zone and in which to add the task IP addresses to.
@@ -637,22 +822,22 @@
             'myservice'
         '''
         result = self._values.get("record_name")
         assert result is not None, "Required property 'record_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def zone(self) -> aws_cdk.aws_route53.IHostedZone:
+    def zone(self) -> _aws_cdk_aws_route53_ceddda9d.IHostedZone:
         '''(experimental) A DNS Zone to expose task IPs in.
 
         :stability: experimental
         '''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
-        return typing.cast(aws_cdk.aws_route53.IHostedZone, result)
+        return typing.cast(_aws_cdk_aws_route53_ceddda9d.IHostedZone, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -667,27 +852,27 @@
     jsii_struct_bases=[],
     name_mapping={"dns": "dns"},
 )
 class AssignPublicIpExtensionOptions:
     def __init__(
         self,
         *,
-        dns: typing.Optional[AssignPublicIpDnsOptions] = None,
+        dns: typing.Optional[typing.Union[AssignPublicIpDnsOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param dns: (experimental) Enable publishing task public IPs to a recordset in a Route 53 hosted zone. Note: If you want to change the DNS zone or record name, you will need to remove this extension completely and then re-add it.
 
         :stability: experimental
         '''
         if isinstance(dns, dict):
             dns = AssignPublicIpDnsOptions(**dns)
         if __debug__:
-            type_hints = typing.get_type_hints(AssignPublicIpExtensionOptions.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__2deb6349e9cd894776e0a60628761c1ec58ee4da5eb9e508b90d05cf30b34874)
             check_type(argname="argument dns", value=dns, expected_type=type_hints["dns"])
-        self._values: typing.Dict[str, typing.Any] = {}
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
         if dns is not None:
             self._values["dns"] = dns
 
     @builtins.property
     def dns(self) -> typing.Optional[AssignPublicIpDnsOptions]:
         '''(experimental) Enable publishing task public IPs to a recordset in a Route 53 hosted zone.
 
@@ -735,20 +920,20 @@
         :param min_task_count: (experimental) The minimum number of tasks when scaling in. Default: - 1
         :param target_cpu_utilization: (experimental) The target value for CPU utilization across all tasks in the service.
         :param target_memory_utilization: (experimental) The target value for memory utilization across all tasks in the service.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(AutoScalingOptions.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__caf95230f9a127a46aef16659b3a944e6851420921875acc492c4a7722ded929)
             check_type(argname="argument max_task_count", value=max_task_count, expected_type=type_hints["max_task_count"])
             check_type(argname="argument min_task_count", value=min_task_count, expected_type=type_hints["min_task_count"])
             check_type(argname="argument target_cpu_utilization", value=target_cpu_utilization, expected_type=type_hints["target_cpu_utilization"])
             check_type(argname="argument target_memory_utilization", value=target_memory_utilization, expected_type=type_hints["target_memory_utilization"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "max_task_count": max_task_count,
         }
         if min_task_count is not None:
             self._values["min_task_count"] = min_task_count
         if target_cpu_utilization is not None:
             self._values["target_cpu_utilization"] = target_cpu_utilization
         if target_memory_utilization is not None:
@@ -815,17 +1000,17 @@
         '''(experimental) connectToProps will have all the extra parameters which are required for connecting services.
 
         :param local_bind_port: (experimental) localBindPort is the local port that this application should use when calling the upstream service in ECS Consul Mesh Extension Currently, this parameter will only be used in the ECSConsulMeshExtension https://github.com/aws-ia/ecs-consul-mesh-extension.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(ConnectToProps.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__20e37174ab201a5eb1d201637ac0c651f7361afe5cb95a69d57aeed17fde4cc3)
             check_type(argname="argument local_bind_port", value=local_bind_port, expected_type=type_hints["local_bind_port"])
-        self._values: typing.Dict[str, typing.Any] = {}
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
         if local_bind_port is not None:
             self._values["local_bind_port"] = local_bind_port
 
     @builtins.property
     def local_bind_port(self) -> typing.Optional[jsii.Number]:
         '''(experimental) localBindPort is the local port that this application should use when calling the upstream service in ECS Consul Mesh Extension Currently, this parameter will only be used in the ECSConsulMeshExtension https://github.com/aws-ia/ecs-consul-mesh-extension.
 
@@ -851,77 +1036,89 @@
     jsii_struct_bases=[],
     name_mapping={
         "cpu": "cpu",
         "image": "image",
         "memory_mib": "memoryMiB",
         "traffic_port": "trafficPort",
         "environment": "environment",
+        "environment_files": "environmentFiles",
         "log_group": "logGroup",
+        "secrets": "secrets",
     },
 )
 class ContainerExtensionProps:
     def __init__(
         self,
         *,
         cpu: jsii.Number,
-        image: aws_cdk.aws_ecs.ContainerImage,
+        image: _aws_cdk_aws_ecs_ceddda9d.ContainerImage,
         memory_mib: jsii.Number,
         traffic_port: jsii.Number,
         environment: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-        log_group: typing.Optional[aws_cdk.aws_logs.ILogGroup] = None,
+        environment_files: typing.Optional[typing.Sequence[_aws_cdk_aws_ecs_ceddda9d.EnvironmentFile]] = None,
+        log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
+        secrets: typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_ecs_ceddda9d.Secret]] = None,
     ) -> None:
         '''(experimental) Setting for the main application container of a service.
 
         :param cpu: (experimental) How much CPU the container requires.
         :param image: (experimental) The image to run.
         :param memory_mib: (experimental) How much memory in megabytes the container requires.
         :param traffic_port: (experimental) What port the image listen for traffic on.
         :param environment: (experimental) Environment variables to pass into the container. Default: - No environment variables.
+        :param environment_files: (experimental) The environment files to pass to the container. Default: - No environment files.
         :param log_group: (experimental) The log group into which application container logs should be routed. Default: - A log group is automatically created for you if the ``ECS_SERVICE_EXTENSIONS_ENABLE_DEFAULT_LOG_DRIVER`` feature flag is set.
+        :param secrets: (experimental) The secret environment variables to pass to the container. Default: - No secret environment variables.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(ContainerExtensionProps.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__592d522da39571a2b2a1780c28b1405f8f98b2f7ae4b9ff881cf256a8d3941d3)
             check_type(argname="argument cpu", value=cpu, expected_type=type_hints["cpu"])
             check_type(argname="argument image", value=image, expected_type=type_hints["image"])
             check_type(argname="argument memory_mib", value=memory_mib, expected_type=type_hints["memory_mib"])
             check_type(argname="argument traffic_port", value=traffic_port, expected_type=type_hints["traffic_port"])
             check_type(argname="argument environment", value=environment, expected_type=type_hints["environment"])
+            check_type(argname="argument environment_files", value=environment_files, expected_type=type_hints["environment_files"])
             check_type(argname="argument log_group", value=log_group, expected_type=type_hints["log_group"])
-        self._values: typing.Dict[str, typing.Any] = {
+            check_type(argname="argument secrets", value=secrets, expected_type=type_hints["secrets"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "cpu": cpu,
             "image": image,
             "memory_mib": memory_mib,
             "traffic_port": traffic_port,
         }
         if environment is not None:
             self._values["environment"] = environment
+        if environment_files is not None:
+            self._values["environment_files"] = environment_files
         if log_group is not None:
             self._values["log_group"] = log_group
+        if secrets is not None:
+            self._values["secrets"] = secrets
 
     @builtins.property
     def cpu(self) -> jsii.Number:
         '''(experimental) How much CPU the container requires.
 
         :stability: experimental
         '''
         result = self._values.get("cpu")
         assert result is not None, "Required property 'cpu' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
-    def image(self) -> aws_cdk.aws_ecs.ContainerImage:
+    def image(self) -> _aws_cdk_aws_ecs_ceddda9d.ContainerImage:
         '''(experimental) The image to run.
 
         :stability: experimental
         '''
         result = self._values.get("image")
         assert result is not None, "Required property 'image' is missing"
-        return typing.cast(aws_cdk.aws_ecs.ContainerImage, result)
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.ContainerImage, result)
 
     @builtins.property
     def memory_mib(self) -> jsii.Number:
         '''(experimental) How much memory in megabytes the container requires.
 
         :stability: experimental
         '''
@@ -949,23 +1146,50 @@
 
         :stability: experimental
         '''
         result = self._values.get("environment")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
-    def log_group(self) -> typing.Optional[aws_cdk.aws_logs.ILogGroup]:
+    def environment_files(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_ecs_ceddda9d.EnvironmentFile]]:
+        '''(experimental) The environment files to pass to the container.
+
+        :default: - No environment files.
+
+        :see: https://docs.aws.amazon.com/AmazonECS/latest/developerguide/taskdef-envfiles.html
+        :stability: experimental
+        '''
+        result = self._values.get("environment_files")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ecs_ceddda9d.EnvironmentFile]], result)
+
+    @builtins.property
+    def log_group(self) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
         '''(experimental) The log group into which application container logs should be routed.
 
         :default: - A log group is automatically created for you if the ``ECS_SERVICE_EXTENSIONS_ENABLE_DEFAULT_LOG_DRIVER`` feature flag is set.
 
         :stability: experimental
         '''
         result = self._values.get("log_group")
-        return typing.cast(typing.Optional[aws_cdk.aws_logs.ILogGroup], result)
+        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup], result)
+
+    @builtins.property
+    def secrets(
+        self,
+    ) -> typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_ecs_ceddda9d.Secret]]:
+        '''(experimental) The secret environment variables to pass to the container.
+
+        :default: - No secret environment variables.
+
+        :stability: experimental
+        '''
+        result = self._values.get("secrets")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_ecs_ceddda9d.Secret]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -993,46 +1217,46 @@
         '''
         jsii.create(self.__class__, self, [])
 
     @jsii.member(jsii_name="mutateContainerDefinition")
     def mutate_container_definition(
         self,
         *,
-        image: aws_cdk.aws_ecs.ContainerImage,
+        image: _aws_cdk_aws_ecs_ceddda9d.ContainerImage,
         command: typing.Optional[typing.Sequence[builtins.str]] = None,
         container_name: typing.Optional[builtins.str] = None,
         cpu: typing.Optional[jsii.Number] = None,
         disable_networking: typing.Optional[builtins.bool] = None,
         dns_search_domains: typing.Optional[typing.Sequence[builtins.str]] = None,
         dns_servers: typing.Optional[typing.Sequence[builtins.str]] = None,
         docker_labels: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         docker_security_options: typing.Optional[typing.Sequence[builtins.str]] = None,
         entry_point: typing.Optional[typing.Sequence[builtins.str]] = None,
         environment: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-        environment_files: typing.Optional[typing.Sequence[aws_cdk.aws_ecs.EnvironmentFile]] = None,
+        environment_files: typing.Optional[typing.Sequence[_aws_cdk_aws_ecs_ceddda9d.EnvironmentFile]] = None,
         essential: typing.Optional[builtins.bool] = None,
         extra_hosts: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         gpu_count: typing.Optional[jsii.Number] = None,
-        health_check: typing.Optional[aws_cdk.aws_ecs.HealthCheck] = None,
+        health_check: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.HealthCheck, typing.Dict[builtins.str, typing.Any]]] = None,
         hostname: typing.Optional[builtins.str] = None,
         inference_accelerator_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
-        linux_parameters: typing.Optional[aws_cdk.aws_ecs.LinuxParameters] = None,
-        logging: typing.Optional[aws_cdk.aws_ecs.LogDriver] = None,
+        linux_parameters: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.LinuxParameters] = None,
+        logging: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.LogDriver] = None,
         memory_limit_mib: typing.Optional[jsii.Number] = None,
         memory_reservation_mib: typing.Optional[jsii.Number] = None,
-        port_mappings: typing.Optional[typing.Sequence[aws_cdk.aws_ecs.PortMapping]] = None,
+        port_mappings: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecs_ceddda9d.PortMapping, typing.Dict[builtins.str, typing.Any]]]] = None,
         privileged: typing.Optional[builtins.bool] = None,
         readonly_root_filesystem: typing.Optional[builtins.bool] = None,
-        secrets: typing.Optional[typing.Mapping[builtins.str, aws_cdk.aws_ecs.Secret]] = None,
-        start_timeout: typing.Optional[aws_cdk.Duration] = None,
-        stop_timeout: typing.Optional[aws_cdk.Duration] = None,
-        system_controls: typing.Optional[typing.Sequence[aws_cdk.aws_ecs.SystemControl]] = None,
+        secrets: typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_ecs_ceddda9d.Secret]] = None,
+        start_timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        stop_timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        system_controls: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecs_ceddda9d.SystemControl, typing.Dict[builtins.str, typing.Any]]]] = None,
         user: typing.Optional[builtins.str] = None,
         working_directory: typing.Optional[builtins.str] = None,
-    ) -> aws_cdk.aws_ecs.ContainerDefinitionOptions:
+    ) -> _aws_cdk_aws_ecs_ceddda9d.ContainerDefinitionOptions:
         '''(experimental) This is a hook for modifying the container definition of any upstream containers.
 
         This is primarily used for the main application container.
         For example, the Firelens extension wants to be able to modify the logging
         settings of the application container.
 
         :param image: The image used to start a container. This string is passed directly to the Docker daemon. Images in the Docker Hub registry are available by default. Other repositories are specified with either repository-url/image:tag or repository-url/image@digest. TODO: Update these to specify using classes of IContainerImage
@@ -1065,15 +1289,15 @@
         :param stop_timeout: Time duration (in seconds) to wait before the container is forcefully killed if it doesn't exit normally on its own. Default: - none
         :param system_controls: A list of namespaced kernel parameters to set in the container. Default: - No system controls are set.
         :param user: The user name to use inside the container. Default: root
         :param working_directory: The working directory in which to run commands inside the container. Default: /
 
         :stability: experimental
         '''
-        props = aws_cdk.aws_ecs.ContainerDefinitionOptions(
+        props = _aws_cdk_aws_ecs_ceddda9d.ContainerDefinitionOptions(
             image=image,
             command=command,
             container_name=container_name,
             cpu=cpu,
             disable_networking=disable_networking,
             dns_search_domains=dns_search_domains,
             dns_servers=dns_servers,
@@ -1099,15 +1323,15 @@
             start_timeout=start_timeout,
             stop_timeout=stop_timeout,
             system_controls=system_controls,
             user=user,
             working_directory=working_directory,
         )
 
-        return typing.cast(aws_cdk.aws_ecs.ContainerDefinitionOptions, jsii.invoke(self, "mutateContainerDefinition", [props]))
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.ContainerDefinitionOptions, jsii.invoke(self, "mutateContainerDefinition", [props]))
 
 
 class _ContainerMutatingHookProxy(ContainerMutatingHook):
     pass
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the abstract class
 typing.cast(typing.Any, ContainerMutatingHook).__jsii_proxy_class__ = lambda : _ContainerMutatingHookProxy
@@ -1128,16 +1352,16 @@
 class CpuScalingProps:
     def __init__(
         self,
         *,
         initial_task_count: typing.Optional[jsii.Number] = None,
         max_task_count: typing.Optional[jsii.Number] = None,
         min_task_count: typing.Optional[jsii.Number] = None,
-        scale_in_cooldown: typing.Optional[aws_cdk.Duration] = None,
-        scale_out_cooldown: typing.Optional[aws_cdk.Duration] = None,
+        scale_in_cooldown: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        scale_out_cooldown: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         target_cpu_utilization: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''(deprecated) The autoscaling settings.
 
         :param initial_task_count: (deprecated) How many tasks to launch initially. Default: - 2
         :param max_task_count: (deprecated) The maximum number of tasks when scaling out. Default: - 8
         :param min_task_count: (deprecated) The minimum number of tasks when scaling in. Default: - 2
@@ -1150,22 +1374,22 @@
         use the ``minTaskCount`` and ``maxTaskCount`` properties of ``autoScaleTaskCount`` in the ``Service`` construct
         to configure the auto scaling target for the service. For more information, please refer
         https://github.com/aws/aws-cdk/blob/master/packages/%40aws-cdk-containers/ecs-service-extensions/README.md#task-auto-scaling .
 
         :stability: deprecated
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(CpuScalingProps.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__da64dd40c2eed49a661888472ad447cdd50d0d1de54b035c25e482f09c6e8d50)
             check_type(argname="argument initial_task_count", value=initial_task_count, expected_type=type_hints["initial_task_count"])
             check_type(argname="argument max_task_count", value=max_task_count, expected_type=type_hints["max_task_count"])
             check_type(argname="argument min_task_count", value=min_task_count, expected_type=type_hints["min_task_count"])
             check_type(argname="argument scale_in_cooldown", value=scale_in_cooldown, expected_type=type_hints["scale_in_cooldown"])
             check_type(argname="argument scale_out_cooldown", value=scale_out_cooldown, expected_type=type_hints["scale_out_cooldown"])
             check_type(argname="argument target_cpu_utilization", value=target_cpu_utilization, expected_type=type_hints["target_cpu_utilization"])
-        self._values: typing.Dict[str, typing.Any] = {}
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
         if initial_task_count is not None:
             self._values["initial_task_count"] = initial_task_count
         if max_task_count is not None:
             self._values["max_task_count"] = max_task_count
         if min_task_count is not None:
             self._values["min_task_count"] = min_task_count
         if scale_in_cooldown is not None:
@@ -1205,34 +1429,34 @@
 
         :stability: deprecated
         '''
         result = self._values.get("min_task_count")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    def scale_in_cooldown(self) -> typing.Optional[aws_cdk.Duration]:
+    def scale_in_cooldown(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
         '''(deprecated) How long to wait between scale in actions.
 
         :default: - 60 seconds
 
         :stability: deprecated
         '''
         result = self._values.get("scale_in_cooldown")
-        return typing.cast(typing.Optional[aws_cdk.Duration], result)
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
 
     @builtins.property
-    def scale_out_cooldown(self) -> typing.Optional[aws_cdk.Duration]:
+    def scale_out_cooldown(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
         '''(deprecated) How long to wait between scale out actions.
 
         :default: - 60 seconds
 
         :stability: deprecated
         '''
         result = self._values.get("scale_out_cooldown")
-        return typing.cast(typing.Optional[aws_cdk.Duration], result)
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
 
     @builtins.property
     def target_cpu_utilization(self) -> typing.Optional[jsii.Number]:
         '''(deprecated) The CPU utilization to try ot maintain.
 
         :default: - 50%
 
@@ -1259,27 +1483,27 @@
     name_mapping={"capacity_type": "capacityType", "cluster": "cluster"},
 )
 class EnvironmentAttributes:
     def __init__(
         self,
         *,
         capacity_type: "EnvironmentCapacityType",
-        cluster: aws_cdk.aws_ecs.ICluster,
+        cluster: _aws_cdk_aws_ecs_ceddda9d.ICluster,
     ) -> None:
         '''
         :param capacity_type: (experimental) The capacity type used by the service's cluster.
         :param cluster: (experimental) The cluster that is providing capacity for this service.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(EnvironmentAttributes.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__3972ae1eaa225a4a8fa626d5b9ec3fc0b64c420599bc3a5f3dd1d2aec30cfd77)
             check_type(argname="argument capacity_type", value=capacity_type, expected_type=type_hints["capacity_type"])
             check_type(argname="argument cluster", value=cluster, expected_type=type_hints["cluster"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "capacity_type": capacity_type,
             "cluster": cluster,
         }
 
     @builtins.property
     def capacity_type(self) -> "EnvironmentCapacityType":
         '''(experimental) The capacity type used by the service's cluster.
@@ -1287,22 +1511,22 @@
         :stability: experimental
         '''
         result = self._values.get("capacity_type")
         assert result is not None, "Required property 'capacity_type' is missing"
         return typing.cast("EnvironmentCapacityType", result)
 
     @builtins.property
-    def cluster(self) -> aws_cdk.aws_ecs.ICluster:
+    def cluster(self) -> _aws_cdk_aws_ecs_ceddda9d.ICluster:
         '''(experimental) The cluster that is providing capacity for this service.
 
         :stability: experimental
         '''
         result = self._values.get("cluster")
         assert result is not None, "Required property 'cluster' is missing"
-        return typing.cast(aws_cdk.aws_ecs.ICluster, result)
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.ICluster, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1342,31 +1566,31 @@
     name_mapping={"capacity_type": "capacityType", "cluster": "cluster", "vpc": "vpc"},
 )
 class EnvironmentProps:
     def __init__(
         self,
         *,
         capacity_type: typing.Optional[EnvironmentCapacityType] = None,
-        cluster: typing.Optional[aws_cdk.aws_ecs.Cluster] = None,
-        vpc: typing.Optional[aws_cdk.aws_ec2.IVpc] = None,
+        cluster: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.Cluster] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''(experimental) Settings for the environment where you want to deploy your services.
 
         :param capacity_type: (experimental) The type of capacity to use for this environment. Default: - EnvironmentCapacityType.FARGATE
         :param cluster: (experimental) The ECS cluster which provides compute capacity to this service. [disable-awslint:ref-via-interface] Default: - Create a new cluster
         :param vpc: (experimental) The VPC used by the service for networking. Default: - Create a new VPC
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(EnvironmentProps.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__4f994193a0844d1feecc18424b7d4cb07ff8d4ed7fb514183a12bd56930e922b)
             check_type(argname="argument capacity_type", value=capacity_type, expected_type=type_hints["capacity_type"])
             check_type(argname="argument cluster", value=cluster, expected_type=type_hints["cluster"])
             check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
-        self._values: typing.Dict[str, typing.Any] = {}
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
         if capacity_type is not None:
             self._values["capacity_type"] = capacity_type
         if cluster is not None:
             self._values["cluster"] = cluster
         if vpc is not None:
             self._values["vpc"] = vpc
 
@@ -1378,36 +1602,36 @@
 
         :stability: experimental
         '''
         result = self._values.get("capacity_type")
         return typing.cast(typing.Optional[EnvironmentCapacityType], result)
 
     @builtins.property
-    def cluster(self) -> typing.Optional[aws_cdk.aws_ecs.Cluster]:
+    def cluster(self) -> typing.Optional[_aws_cdk_aws_ecs_ceddda9d.Cluster]:
         '''(experimental) The ECS cluster which provides compute capacity to this service.
 
         [disable-awslint:ref-via-interface]
 
         :default: - Create a new cluster
 
         :stability: experimental
         '''
         result = self._values.get("cluster")
-        return typing.cast(typing.Optional[aws_cdk.aws_ecs.Cluster], result)
+        return typing.cast(typing.Optional[_aws_cdk_aws_ecs_ceddda9d.Cluster], result)
 
     @builtins.property
-    def vpc(self) -> typing.Optional[aws_cdk.aws_ec2.IVpc]:
+    def vpc(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc]:
         '''(experimental) The VPC used by the service for networking.
 
         :default: - Create a new VPC
 
         :stability: experimental
         '''
         result = self._values.get("vpc")
-        return typing.cast(typing.Optional[aws_cdk.aws_ec2.IVpc], result)
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -1426,15 +1650,15 @@
 
     :stability: experimental
     '''
 
     def __init__(
         self,
         *,
-        log_group: aws_cdk.aws_logs.LogGroup,
+        log_group: _aws_cdk_aws_logs_ceddda9d.LogGroup,
         parent_service: "Service",
     ) -> None:
         '''
         :param log_group: (experimental) The log group into which logs should be routed.
         :param parent_service: (experimental) The parent service that is being mutated.
 
         :stability: experimental
@@ -1443,46 +1667,46 @@
 
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="mutateContainerDefinition")
     def mutate_container_definition(
         self,
         *,
-        image: aws_cdk.aws_ecs.ContainerImage,
+        image: _aws_cdk_aws_ecs_ceddda9d.ContainerImage,
         command: typing.Optional[typing.Sequence[builtins.str]] = None,
         container_name: typing.Optional[builtins.str] = None,
         cpu: typing.Optional[jsii.Number] = None,
         disable_networking: typing.Optional[builtins.bool] = None,
         dns_search_domains: typing.Optional[typing.Sequence[builtins.str]] = None,
         dns_servers: typing.Optional[typing.Sequence[builtins.str]] = None,
         docker_labels: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         docker_security_options: typing.Optional[typing.Sequence[builtins.str]] = None,
         entry_point: typing.Optional[typing.Sequence[builtins.str]] = None,
         environment: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-        environment_files: typing.Optional[typing.Sequence[aws_cdk.aws_ecs.EnvironmentFile]] = None,
+        environment_files: typing.Optional[typing.Sequence[_aws_cdk_aws_ecs_ceddda9d.EnvironmentFile]] = None,
         essential: typing.Optional[builtins.bool] = None,
         extra_hosts: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         gpu_count: typing.Optional[jsii.Number] = None,
-        health_check: typing.Optional[aws_cdk.aws_ecs.HealthCheck] = None,
+        health_check: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.HealthCheck, typing.Dict[builtins.str, typing.Any]]] = None,
         hostname: typing.Optional[builtins.str] = None,
         inference_accelerator_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
-        linux_parameters: typing.Optional[aws_cdk.aws_ecs.LinuxParameters] = None,
-        logging: typing.Optional[aws_cdk.aws_ecs.LogDriver] = None,
+        linux_parameters: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.LinuxParameters] = None,
+        logging: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.LogDriver] = None,
         memory_limit_mib: typing.Optional[jsii.Number] = None,
         memory_reservation_mib: typing.Optional[jsii.Number] = None,
-        port_mappings: typing.Optional[typing.Sequence[aws_cdk.aws_ecs.PortMapping]] = None,
+        port_mappings: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecs_ceddda9d.PortMapping, typing.Dict[builtins.str, typing.Any]]]] = None,
         privileged: typing.Optional[builtins.bool] = None,
         readonly_root_filesystem: typing.Optional[builtins.bool] = None,
-        secrets: typing.Optional[typing.Mapping[builtins.str, aws_cdk.aws_ecs.Secret]] = None,
-        start_timeout: typing.Optional[aws_cdk.Duration] = None,
-        stop_timeout: typing.Optional[aws_cdk.Duration] = None,
-        system_controls: typing.Optional[typing.Sequence[aws_cdk.aws_ecs.SystemControl]] = None,
+        secrets: typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_ecs_ceddda9d.Secret]] = None,
+        start_timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        stop_timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        system_controls: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecs_ceddda9d.SystemControl, typing.Dict[builtins.str, typing.Any]]]] = None,
         user: typing.Optional[builtins.str] = None,
         working_directory: typing.Optional[builtins.str] = None,
-    ) -> aws_cdk.aws_ecs.ContainerDefinitionOptions:
+    ) -> _aws_cdk_aws_ecs_ceddda9d.ContainerDefinitionOptions:
         '''(experimental) This is a hook for modifying the container definition of any upstream containers.
 
         This is primarily used for the main application container.
         For example, the Firelens extension wants to be able to modify the logging
         settings of the application container.
 
         :param image: The image used to start a container. This string is passed directly to the Docker daemon. Images in the Docker Hub registry are available by default. Other repositories are specified with either repository-url/image:tag or repository-url/image@digest. TODO: Update these to specify using classes of IContainerImage
@@ -1515,15 +1739,15 @@
         :param stop_timeout: Time duration (in seconds) to wait before the container is forcefully killed if it doesn't exit normally on its own. Default: - none
         :param system_controls: A list of namespaced kernel parameters to set in the container. Default: - No system controls are set.
         :param user: The user name to use inside the container. Default: root
         :param working_directory: The working directory in which to run commands inside the container. Default: /
 
         :stability: experimental
         '''
-        props = aws_cdk.aws_ecs.ContainerDefinitionOptions(
+        props = _aws_cdk_aws_ecs_ceddda9d.ContainerDefinitionOptions(
             image=image,
             command=command,
             container_name=container_name,
             cpu=cpu,
             disable_networking=disable_networking,
             dns_search_domains=dns_search_domains,
             dns_servers=dns_servers,
@@ -1549,54 +1773,54 @@
             start_timeout=start_timeout,
             stop_timeout=stop_timeout,
             system_controls=system_controls,
             user=user,
             working_directory=working_directory,
         )
 
-        return typing.cast(aws_cdk.aws_ecs.ContainerDefinitionOptions, jsii.invoke(self, "mutateContainerDefinition", [props]))
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.ContainerDefinitionOptions, jsii.invoke(self, "mutateContainerDefinition", [props]))
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk-containers/ecs-service-extensions.FirelensProps",
     jsii_struct_bases=[],
     name_mapping={"log_group": "logGroup", "parent_service": "parentService"},
 )
 class FirelensProps:
     def __init__(
         self,
         *,
-        log_group: aws_cdk.aws_logs.LogGroup,
+        log_group: _aws_cdk_aws_logs_ceddda9d.LogGroup,
         parent_service: "Service",
     ) -> None:
         '''(experimental) Settings for the hook which mutates the application container to route logs through FireLens.
 
         :param log_group: (experimental) The log group into which logs should be routed.
         :param parent_service: (experimental) The parent service that is being mutated.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(FirelensProps.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__aceb6633b315022d8687596bd75918bf27f97bab07b5afe71b5de85deefef59c)
             check_type(argname="argument log_group", value=log_group, expected_type=type_hints["log_group"])
             check_type(argname="argument parent_service", value=parent_service, expected_type=type_hints["parent_service"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "log_group": log_group,
             "parent_service": parent_service,
         }
 
     @builtins.property
-    def log_group(self) -> aws_cdk.aws_logs.LogGroup:
+    def log_group(self) -> _aws_cdk_aws_logs_ceddda9d.LogGroup:
         '''(experimental) The log group into which logs should be routed.
 
         :stability: experimental
         '''
         result = self._values.get("log_group")
         assert result is not None, "Required property 'log_group' is missing"
-        return typing.cast(aws_cdk.aws_logs.LogGroup, result)
+        return typing.cast(_aws_cdk_aws_logs_ceddda9d.LogGroup, result)
 
     @builtins.property
     def parent_service(self) -> "Service":
         '''(experimental) The parent service that is being mutated.
 
         :stability: experimental
         '''
@@ -1629,17 +1853,17 @@
     ) -> None:
         '''
         :param requests_per_target: (experimental) The number of ALB requests per target.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(HttpLoadBalancerProps.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__82df5b77ad12b766d5e63af5b466f4e55ce579599801b70669df556201e35c2c)
             check_type(argname="argument requests_per_target", value=requests_per_target, expected_type=type_hints["requests_per_target"])
-        self._values: typing.Dict[str, typing.Any] = {}
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
         if requests_per_target is not None:
             self._values["requests_per_target"] = requests_per_target
 
     @builtins.property
     def requests_per_target(self) -> typing.Optional[jsii.Number]:
         '''(experimental) The number of ALB requests per target.
 
@@ -1663,62 +1887,64 @@
 @jsii.interface(jsii_type="@aws-cdk-containers/ecs-service-extensions.IEnvironment")
 class IEnvironment(typing_extensions.Protocol):
     '''(experimental) An environment into which to deploy a service.
 
     :stability: experimental
     '''
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="capacityType")
     def capacity_type(self) -> EnvironmentCapacityType:
         '''(experimental) The capacity type used by the service's cluster.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cluster")
-    def cluster(self) -> aws_cdk.aws_ecs.ICluster:
+    def cluster(self) -> _aws_cdk_aws_ecs_ceddda9d.ICluster:
         '''(experimental) The cluster that is providing capacity for this service.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="id")
     def id(self) -> builtins.str:
         '''(experimental) The name of this environment.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpc")
-    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
+    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
         '''(experimental) The VPC into which environment services should be placed.
 
         :stability: experimental
         '''
         ...
 
     @jsii.member(jsii_name="addDefaultCloudMapNamespace")
     def add_default_cloud_map_namespace(
         self,
         *,
         name: builtins.str,
-        type: typing.Optional[aws_cdk.aws_servicediscovery.NamespaceType] = None,
-        vpc: typing.Optional[aws_cdk.aws_ec2.IVpc] = None,
+        type: typing.Optional[_aws_cdk_aws_servicediscovery_ceddda9d.NamespaceType] = None,
+        use_for_service_connect: typing.Optional[builtins.bool] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''(experimental) Add a default cloudmap namespace to the environment's cluster.
 
         :param name: The name of the namespace, such as example.com.
         :param type: The type of CloudMap Namespace to create. Default: PrivateDns
+        :param use_for_service_connect: This property specifies whether to set the provided namespace as the service connect default in the cluster properties. Default: false
         :param vpc: The VPC to associate the namespace with. This property is required for private DNS namespaces. Default: VPC of the cluster for Private DNS Namespace, otherwise none
 
         :stability: experimental
         '''
         ...
 
 
@@ -1726,68 +1952,73 @@
     '''(experimental) An environment into which to deploy a service.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk-containers/ecs-service-extensions.IEnvironment"
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="capacityType")
     def capacity_type(self) -> EnvironmentCapacityType:
         '''(experimental) The capacity type used by the service's cluster.
 
         :stability: experimental
         '''
         return typing.cast(EnvironmentCapacityType, jsii.get(self, "capacityType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cluster")
-    def cluster(self) -> aws_cdk.aws_ecs.ICluster:
+    def cluster(self) -> _aws_cdk_aws_ecs_ceddda9d.ICluster:
         '''(experimental) The cluster that is providing capacity for this service.
 
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_ecs.ICluster, jsii.get(self, "cluster"))
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.ICluster, jsii.get(self, "cluster"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="id")
     def id(self) -> builtins.str:
         '''(experimental) The name of this environment.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "id"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpc")
-    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
+    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
         '''(experimental) The VPC into which environment services should be placed.
 
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_ec2.IVpc, jsii.get(self, "vpc"))
+        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, jsii.get(self, "vpc"))
 
     @jsii.member(jsii_name="addDefaultCloudMapNamespace")
     def add_default_cloud_map_namespace(
         self,
         *,
         name: builtins.str,
-        type: typing.Optional[aws_cdk.aws_servicediscovery.NamespaceType] = None,
-        vpc: typing.Optional[aws_cdk.aws_ec2.IVpc] = None,
+        type: typing.Optional[_aws_cdk_aws_servicediscovery_ceddda9d.NamespaceType] = None,
+        use_for_service_connect: typing.Optional[builtins.bool] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''(experimental) Add a default cloudmap namespace to the environment's cluster.
 
         :param name: The name of the namespace, such as example.com.
         :param type: The type of CloudMap Namespace to create. Default: PrivateDns
+        :param use_for_service_connect: This property specifies whether to set the provided namespace as the service connect default in the cluster properties. Default: false
         :param vpc: The VPC to associate the namespace with. This property is required for private DNS namespaces. Default: VPC of the cluster for Private DNS Namespace, otherwise none
 
         :stability: experimental
         '''
-        options = aws_cdk.aws_ecs.CloudMapNamespaceOptions(
-            name=name, type=type, vpc=vpc
+        options = _aws_cdk_aws_ecs_ceddda9d.CloudMapNamespaceOptions(
+            name=name,
+            type=type,
+            use_for_service_connect=use_for_service_connect,
+            vpc=vpc,
         )
 
         return typing.cast(None, jsii.invoke(self, "addDefaultCloudMapNamespace", [options]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IEnvironment).__jsii_proxy_class__ = lambda : _IEnvironmentProxy
 
@@ -1829,27 +2060,30 @@
 @jsii.interface(jsii_type="@aws-cdk-containers/ecs-service-extensions.ISubscribable")
 class ISubscribable(typing_extensions.Protocol):
     '''(experimental) An interface that will be implemented by all the resources that can be subscribed to.
 
     :stability: experimental
     '''
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="subscriptionQueue")
     def subscription_queue(self) -> typing.Optional["SubscriptionQueue"]:
         '''(experimental) The ``SubscriptionQueue`` object for the ``ISubscribable`` object.
 
         :default: none
 
         :stability: experimental
         '''
         ...
 
     @jsii.member(jsii_name="subscribe")
-    def subscribe(self, extension: "QueueExtension") -> aws_cdk.aws_sqs.IQueue:
+    def subscribe(
+        self,
+        extension: "QueueExtension",
+    ) -> _aws_cdk_aws_sqs_ceddda9d.IQueue:
         '''(experimental) All classes implementing this interface must also implement the ``subscribe()`` method.
 
         :param extension: -
 
         :stability: experimental
         '''
         ...
@@ -1859,164 +2093,172 @@
     '''(experimental) An interface that will be implemented by all the resources that can be subscribed to.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk-containers/ecs-service-extensions.ISubscribable"
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="subscriptionQueue")
     def subscription_queue(self) -> typing.Optional["SubscriptionQueue"]:
         '''(experimental) The ``SubscriptionQueue`` object for the ``ISubscribable`` object.
 
         :default: none
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional["SubscriptionQueue"], jsii.get(self, "subscriptionQueue"))
 
     @jsii.member(jsii_name="subscribe")
-    def subscribe(self, extension: "QueueExtension") -> aws_cdk.aws_sqs.IQueue:
+    def subscribe(
+        self,
+        extension: "QueueExtension",
+    ) -> _aws_cdk_aws_sqs_ceddda9d.IQueue:
         '''(experimental) All classes implementing this interface must also implement the ``subscribe()`` method.
 
         :param extension: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(ISubscribable.subscribe)
+            type_hints = typing.get_type_hints(_typecheckingstub__cd1578190a97094d760d76a2f5cebe69df504113964828b89844073359391cb5)
             check_type(argname="argument extension", value=extension, expected_type=type_hints["extension"])
-        return typing.cast(aws_cdk.aws_sqs.IQueue, jsii.invoke(self, "subscribe", [extension]))
+        return typing.cast(_aws_cdk_aws_sqs_ceddda9d.IQueue, jsii.invoke(self, "subscribe", [extension]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, ISubscribable).__jsii_proxy_class__ = lambda : _ISubscribableProxy
 
 
 @jsii.implements(IEnvironment)
 class ImportedEnvironment(
-    constructs.Construct,
+    _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk-containers/ecs-service-extensions.ImportedEnvironment",
 ):
     '''
     :stability: experimental
     '''
 
     def __init__(
         self,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         capacity_type: EnvironmentCapacityType,
-        cluster: aws_cdk.aws_ecs.ICluster,
+        cluster: _aws_cdk_aws_ecs_ceddda9d.ICluster,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param capacity_type: (experimental) The capacity type used by the service's cluster.
         :param cluster: (experimental) The cluster that is providing capacity for this service.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(ImportedEnvironment.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__91378335a3876039a3828c1245b7393e5a1292ba2a049277f1c28e0986b15b07)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = EnvironmentAttributes(capacity_type=capacity_type, cluster=cluster)
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.member(jsii_name="addDefaultCloudMapNamespace")
     def add_default_cloud_map_namespace(
         self,
         *,
         name: builtins.str,
-        type: typing.Optional[aws_cdk.aws_servicediscovery.NamespaceType] = None,
-        vpc: typing.Optional[aws_cdk.aws_ec2.IVpc] = None,
+        type: typing.Optional[_aws_cdk_aws_servicediscovery_ceddda9d.NamespaceType] = None,
+        use_for_service_connect: typing.Optional[builtins.bool] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''(experimental) Adding a default cloudmap namespace to the cluster will throw an error, as we don't own it.
 
         :param name: The name of the namespace, such as example.com.
         :param type: The type of CloudMap Namespace to create. Default: PrivateDns
+        :param use_for_service_connect: This property specifies whether to set the provided namespace as the service connect default in the cluster properties. Default: false
         :param vpc: The VPC to associate the namespace with. This property is required for private DNS namespaces. Default: VPC of the cluster for Private DNS Namespace, otherwise none
 
         :stability: experimental
         '''
-        _options = aws_cdk.aws_ecs.CloudMapNamespaceOptions(
-            name=name, type=type, vpc=vpc
+        _options = _aws_cdk_aws_ecs_ceddda9d.CloudMapNamespaceOptions(
+            name=name,
+            type=type,
+            use_for_service_connect=use_for_service_connect,
+            vpc=vpc,
         )
 
         return typing.cast(None, jsii.invoke(self, "addDefaultCloudMapNamespace", [_options]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="capacityType")
     def capacity_type(self) -> EnvironmentCapacityType:
         '''(experimental) The capacity type used by the service's cluster.
 
         :stability: experimental
         '''
         return typing.cast(EnvironmentCapacityType, jsii.get(self, "capacityType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cluster")
-    def cluster(self) -> aws_cdk.aws_ecs.ICluster:
+    def cluster(self) -> _aws_cdk_aws_ecs_ceddda9d.ICluster:
         '''(experimental) The cluster that is providing capacity for this service.
 
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_ecs.ICluster, jsii.get(self, "cluster"))
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.ICluster, jsii.get(self, "cluster"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="id")
     def id(self) -> builtins.str:
         '''(experimental) The name of this environment.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "id"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpc")
-    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
+    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
         '''(experimental) The VPC into which environment services should be placed.
 
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_ec2.IVpc, jsii.get(self, "vpc"))
+        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, jsii.get(self, "vpc"))
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk-containers/ecs-service-extensions.InjectableTopicProps",
     jsii_struct_bases=[],
     name_mapping={"topic": "topic"},
 )
 class InjectableTopicProps:
-    def __init__(self, *, topic: aws_cdk.aws_sns.ITopic) -> None:
+    def __init__(self, *, topic: _aws_cdk_aws_sns_ceddda9d.ITopic) -> None:
         '''(experimental) The settings for the ``InjectableTopic`` class.
 
         :param topic: (experimental) The SNS Topic to publish events to.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(InjectableTopicProps.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__5404fdd3e63bd485e4db5b2a113ebf7494d35cf4a96f038e9defb7d051989a59)
             check_type(argname="argument topic", value=topic, expected_type=type_hints["topic"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "topic": topic,
         }
 
     @builtins.property
-    def topic(self) -> aws_cdk.aws_sns.ITopic:
+    def topic(self) -> _aws_cdk_aws_sns_ceddda9d.ITopic:
         '''(experimental) The SNS Topic to publish events to.
 
         :stability: experimental
         '''
         result = self._values.get("topic")
         assert result is not None, "Required property 'topic' is missing"
-        return typing.cast(aws_cdk.aws_sns.ITopic, result)
+        return typing.cast(_aws_cdk_aws_sns_ceddda9d.ITopic, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -2036,17 +2278,17 @@
         '''(experimental) The settings for the Injecter extension.
 
         :param injectables: (experimental) The list of injectable resources for this service.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(InjecterExtensionProps.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__764a4ce423345733d9211ae0ec978efe2db85a96e72389375cfe172603235a12)
             check_type(argname="argument injectables", value=injectables, expected_type=type_hints["injectables"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "injectables": injectables,
         }
 
     @builtins.property
     def injectables(self) -> typing.List[IInjectable]:
         '''(experimental) The list of injectable resources for this service.
 
@@ -2073,43 +2315,43 @@
     jsii_struct_bases=[],
     name_mapping={"mesh": "mesh", "protocol": "protocol"},
 )
 class MeshProps:
     def __init__(
         self,
         *,
-        mesh: aws_cdk.aws_appmesh.Mesh,
+        mesh: _aws_cdk_aws_appmesh_ceddda9d.Mesh,
         protocol: typing.Optional["Protocol"] = None,
     ) -> None:
         '''(experimental) The settings for the App Mesh extension.
 
         :param mesh: (experimental) The service mesh into which to register the service.
         :param protocol: (experimental) The protocol of the service. Valid values are Protocol.HTTP, Protocol.HTTP2, Protocol.TCP, Protocol.GRPC Default: - Protocol.HTTP
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(MeshProps.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__142846b40345638745bc1a3ab27f3cab5f854bdaf8ca3b69b33a43f481fd5f56)
             check_type(argname="argument mesh", value=mesh, expected_type=type_hints["mesh"])
             check_type(argname="argument protocol", value=protocol, expected_type=type_hints["protocol"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "mesh": mesh,
         }
         if protocol is not None:
             self._values["protocol"] = protocol
 
     @builtins.property
-    def mesh(self) -> aws_cdk.aws_appmesh.Mesh:
+    def mesh(self) -> _aws_cdk_aws_appmesh_ceddda9d.Mesh:
         '''(experimental) The service mesh into which to register the service.
 
         :stability: experimental
         '''
         result = self._values.get("mesh")
         assert result is not None, "Required property 'mesh' is missing"
-        return typing.cast(aws_cdk.aws_appmesh.Mesh, result)
+        return typing.cast(_aws_cdk_aws_appmesh_ceddda9d.Mesh, result)
 
     @builtins.property
     def protocol(self) -> typing.Optional["Protocol"]:
         '''(experimental) The protocol of the service.
 
         Valid values are Protocol.HTTP, Protocol.HTTP2, Protocol.TCP, Protocol.GRPC
 
@@ -2165,52 +2407,52 @@
         "message_processing_time": "messageProcessingTime",
     },
 )
 class QueueAutoScalingOptions:
     def __init__(
         self,
         *,
-        acceptable_latency: aws_cdk.Duration,
-        message_processing_time: aws_cdk.Duration,
+        acceptable_latency: _aws_cdk_ceddda9d.Duration,
+        message_processing_time: _aws_cdk_ceddda9d.Duration,
     ) -> None:
         '''(experimental) Options for configuring SQS Queue auto scaling.
 
         :param acceptable_latency: (experimental) Acceptable amount of time a message can sit in the queue (including the time required to process it).
         :param message_processing_time: (experimental) Average amount of time for processing a single message in the queue.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(QueueAutoScalingOptions.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__a69b597f7f7ad40eda264d309c915a018cfc7e08a24d4fd3431b480aebba63ba)
             check_type(argname="argument acceptable_latency", value=acceptable_latency, expected_type=type_hints["acceptable_latency"])
             check_type(argname="argument message_processing_time", value=message_processing_time, expected_type=type_hints["message_processing_time"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "acceptable_latency": acceptable_latency,
             "message_processing_time": message_processing_time,
         }
 
     @builtins.property
-    def acceptable_latency(self) -> aws_cdk.Duration:
+    def acceptable_latency(self) -> _aws_cdk_ceddda9d.Duration:
         '''(experimental) Acceptable amount of time a message can sit in the queue (including the time required to process it).
 
         :stability: experimental
         '''
         result = self._values.get("acceptable_latency")
         assert result is not None, "Required property 'acceptable_latency' is missing"
-        return typing.cast(aws_cdk.Duration, result)
+        return typing.cast(_aws_cdk_ceddda9d.Duration, result)
 
     @builtins.property
-    def message_processing_time(self) -> aws_cdk.Duration:
+    def message_processing_time(self) -> _aws_cdk_ceddda9d.Duration:
         '''(experimental) Average amount of time for processing a single message in the queue.
 
         :stability: experimental
         '''
         result = self._values.get("message_processing_time")
         assert result is not None, "Required property 'message_processing_time' is missing"
-        return typing.cast(aws_cdk.Duration, result)
+        return typing.cast(_aws_cdk_ceddda9d.Duration, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -2229,53 +2471,53 @@
         "subscriptions": "subscriptions",
     },
 )
 class QueueExtensionProps:
     def __init__(
         self,
         *,
-        events_queue: typing.Optional[aws_cdk.aws_sqs.IQueue] = None,
-        scale_on_latency: typing.Optional[QueueAutoScalingOptions] = None,
+        events_queue: typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue] = None,
+        scale_on_latency: typing.Optional[typing.Union[QueueAutoScalingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         subscriptions: typing.Optional[typing.Sequence[ISubscribable]] = None,
     ) -> None:
         '''(experimental) The settings for the Queue extension.
 
         :param events_queue: (experimental) The user-provided default queue for this service. If the ``eventsQueue`` is not provided, a default SQS Queue is created for the service. Default: none
         :param scale_on_latency: (experimental) The user-provided queue delay fields to configure auto scaling for the default queue. Default: none
         :param subscriptions: (experimental) The list of subscriptions for this service. Default: none
 
         :stability: experimental
         '''
         if isinstance(scale_on_latency, dict):
             scale_on_latency = QueueAutoScalingOptions(**scale_on_latency)
         if __debug__:
-            type_hints = typing.get_type_hints(QueueExtensionProps.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__b4718a77605fed94d29789c1a434b9fcc1ae492a2a3de2712231624c092820cb)
             check_type(argname="argument events_queue", value=events_queue, expected_type=type_hints["events_queue"])
             check_type(argname="argument scale_on_latency", value=scale_on_latency, expected_type=type_hints["scale_on_latency"])
             check_type(argname="argument subscriptions", value=subscriptions, expected_type=type_hints["subscriptions"])
-        self._values: typing.Dict[str, typing.Any] = {}
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
         if events_queue is not None:
             self._values["events_queue"] = events_queue
         if scale_on_latency is not None:
             self._values["scale_on_latency"] = scale_on_latency
         if subscriptions is not None:
             self._values["subscriptions"] = subscriptions
 
     @builtins.property
-    def events_queue(self) -> typing.Optional[aws_cdk.aws_sqs.IQueue]:
+    def events_queue(self) -> typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue]:
         '''(experimental) The user-provided default queue for this service.
 
         If the ``eventsQueue`` is not provided, a default SQS Queue is created for the service.
 
         :default: none
 
         :stability: experimental
         '''
         result = self._values.get("events_queue")
-        return typing.cast(typing.Optional[aws_cdk.aws_sqs.IQueue], result)
+        return typing.cast(typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue], result)
 
     @builtins.property
     def scale_on_latency(self) -> typing.Optional[QueueAutoScalingOptions]:
         '''(experimental) The user-provided queue delay fields to configure auto scaling for the default queue.
 
         :default: none
 
@@ -2304,51 +2546,51 @@
     def __repr__(self) -> str:
         return "QueueExtensionProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class Service(
-    constructs.Construct,
+    _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk-containers/ecs-service-extensions.Service",
 ):
     '''(experimental) This Service construct serves as a Builder class for an ECS service.
 
     It
     supports various extensions and keeps track of any mutating state, allowing
     it to build up an ECS service progressively.
 
     :stability: experimental
     '''
 
     def __init__(
         self,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         environment: IEnvironment,
         service_description: "ServiceDescription",
-        auto_scale_task_count: typing.Optional[AutoScalingOptions] = None,
+        auto_scale_task_count: typing.Optional[typing.Union[AutoScalingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         desired_count: typing.Optional[jsii.Number] = None,
-        task_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
+        task_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param environment: (experimental) The environment to launch the service in.
         :param service_description: (experimental) The ServiceDescription used to build the service.
         :param auto_scale_task_count: (experimental) The options for configuring the auto scaling target. Default: none
         :param desired_count: (experimental) The desired number of instantiations of the task definition to keep running on the service. Default: - When creating the service, default is 1; when updating the service, default uses the current task number.
         :param task_role: (experimental) The name of the IAM role that grants containers in the task permission to call AWS APIs on your behalf. Default: - A task role is automatically created for you.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(Service.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__db3cb686a45270fdd7e768c5ae18b4f4f6f2162d2173f63f7c535361b5a43ee0)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = ServiceProps(
             environment=environment,
             service_description=service_description,
             auto_scale_task_count=auto_scale_task_count,
             desired_count=desired_count,
@@ -2367,15 +2609,15 @@
 
         :param url_name: - The identifier name for this URL.
         :param url: - The URL itself.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(Service.add_url)
+            type_hints = typing.get_type_hints(_typecheckingstub__502b75d7c9b239a450ef6b60bf75138f9e9ad1bf1db3c86bae3750bb5b2ddb85)
             check_type(argname="argument url_name", value=url_name, expected_type=type_hints["url_name"])
             check_type(argname="argument url", value=url, expected_type=type_hints["url"])
         return typing.cast(None, jsii.invoke(self, "addURL", [url_name, url]))
 
     @jsii.member(jsii_name="connectTo")
     def connect_to(
         self,
@@ -2387,15 +2629,15 @@
 
         :param service: -
         :param local_bind_port: (experimental) localBindPort is the local port that this application should use when calling the upstream service in ECS Consul Mesh Extension Currently, this parameter will only be used in the ECSConsulMeshExtension https://github.com/aws-ia/ecs-consul-mesh-extension.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(Service.connect_to)
+            type_hints = typing.get_type_hints(_typecheckingstub__74fb3efae7913ceb8ccea9c9b3493498efca8dbd55fc5e00f7140f8a17ed89a9)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
         connect_to_props = ConnectToProps(local_bind_port=local_bind_port)
 
         return typing.cast(None, jsii.invoke(self, "connectTo", [service, connect_to_props]))
 
     @jsii.member(jsii_name="enableAutoScalingPolicy")
     def enable_auto_scaling_policy(self) -> None:
@@ -2413,152 +2655,177 @@
         stored by one of the URL providing extensions.
 
         :param url_name: - The URL to look up.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(Service.get_url)
+            type_hints = typing.get_type_hints(_typecheckingstub__0f9661ad5046e27393ad9a87be136fc5dff0e8a0c90ab0d53f12343c56b38af2)
             check_type(argname="argument url_name", value=url_name, expected_type=type_hints["url_name"])
         return typing.cast(builtins.str, jsii.invoke(self, "getURL", [url_name]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="capacityType")
     def capacity_type(self) -> EnvironmentCapacityType:
         '''(experimental) The capacity type that this service will use.
 
         Valid values are EC2 or FARGATE.
 
         :stability: experimental
         '''
         return typing.cast(EnvironmentCapacityType, jsii.get(self, "capacityType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cluster")
-    def cluster(self) -> aws_cdk.aws_ecs.ICluster:
+    def cluster(self) -> _aws_cdk_aws_ecs_ceddda9d.ICluster:
         '''(experimental) The cluster that is providing capacity for this service.
 
         [disable-awslint:ref-via-interface]
 
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_ecs.ICluster, jsii.get(self, "cluster"))
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.ICluster, jsii.get(self, "cluster"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="environment")
     def environment(self) -> IEnvironment:
         '''(experimental) The environment where this service was launched.
 
         :stability: experimental
         '''
         return typing.cast(IEnvironment, jsii.get(self, "environment"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="id")
     def id(self) -> builtins.str:
         '''(experimental) The name of the service.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "id"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceDescription")
     def service_description(self) -> "ServiceDescription":
         '''(experimental) The ServiceDescription used to build this service.
 
         :stability: experimental
         '''
         return typing.cast("ServiceDescription", jsii.get(self, "serviceDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpc")
-    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
+    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
         '''(experimental) The VPC where this service should be placed.
 
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_ec2.IVpc, jsii.get(self, "vpc"))
+        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, jsii.get(self, "vpc"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scalableTaskCount")
-    def scalable_task_count(self) -> typing.Optional[aws_cdk.aws_ecs.ScalableTaskCount]:
+    def scalable_task_count(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_ecs_ceddda9d.ScalableTaskCount]:
         '''(experimental) The scalable attribute representing task count.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[aws_cdk.aws_ecs.ScalableTaskCount], jsii.get(self, "scalableTaskCount"))
+        return typing.cast(typing.Optional[_aws_cdk_aws_ecs_ceddda9d.ScalableTaskCount], jsii.get(self, "scalableTaskCount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ecsService")
     def ecs_service(
         self,
-    ) -> typing.Union[aws_cdk.aws_ecs.Ec2Service, aws_cdk.aws_ecs.FargateService]:
+    ) -> typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService]:
         '''(experimental) The underlying ECS service that was created.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Union[aws_cdk.aws_ecs.Ec2Service, aws_cdk.aws_ecs.FargateService], jsii.get(self, "ecsService"))
+        return typing.cast(typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService], jsii.get(self, "ecsService"))
 
     @ecs_service.setter
     def ecs_service(
         self,
-        value: typing.Union[aws_cdk.aws_ecs.Ec2Service, aws_cdk.aws_ecs.FargateService],
+        value: typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(getattr(Service, "ecs_service").fset)
+            type_hints = typing.get_type_hints(_typecheckingstub__48e0b209d664b802d972b8c57029dfafa732ddd80d7f15177ec1c19fa4ee27e4)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ecsService", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="taskDefinition")
-    def _task_definition(self) -> aws_cdk.aws_ecs.TaskDefinition:
+    def _task_definition(self) -> _aws_cdk_aws_ecs_ceddda9d.TaskDefinition:
         '''(experimental) The generated task definition for this service.
 
         It is only
         generated after .prepare() has been executed.
 
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_ecs.TaskDefinition, jsii.get(self, "taskDefinition"))
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.TaskDefinition, jsii.get(self, "taskDefinition"))
 
     @_task_definition.setter
-    def _task_definition(self, value: aws_cdk.aws_ecs.TaskDefinition) -> None:
+    def _task_definition(self, value: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(getattr(Service, "_task_definition").fset)
+            type_hints = typing.get_type_hints(_typecheckingstub__43501a7df8adf21fb5b2baed0861c8d54532787b41d74a178e59fb2f8d7cb4c7)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "taskDefinition", value)
 
+    @builtins.property
+    @jsii.member(jsii_name="targetGroup")
+    def target_group(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_elasticloadbalancingv2_ceddda9d.ApplicationTargetGroup]:
+        '''(experimental) The application target group if the service has an HTTPLoadBalancerExtension.
+
+        :stability: experimental
+        '''
+        return typing.cast(typing.Optional[_aws_cdk_aws_elasticloadbalancingv2_ceddda9d.ApplicationTargetGroup], jsii.get(self, "targetGroup"))
+
+    @target_group.setter
+    def target_group(
+        self,
+        value: typing.Optional[_aws_cdk_aws_elasticloadbalancingv2_ceddda9d.ApplicationTargetGroup],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ee366325f772dd64ac0fb090f415241df9c08abd4c10129d4accf09912d2ae3f)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "targetGroup", value)
+
 
 @jsii.data_type(
     jsii_type="@aws-cdk-containers/ecs-service-extensions.ServiceBuild",
     jsii_struct_bases=[],
     name_mapping={
         "cluster": "cluster",
         "task_definition": "taskDefinition",
         "assign_public_ip": "assignPublicIp",
         "cloud_map_options": "cloudMapOptions",
         "desired_count": "desiredCount",
         "health_check_grace_period": "healthCheckGracePeriod",
         "max_healthy_percent": "maxHealthyPercent",
         "min_healthy_percent": "minHealthyPercent",
+        "service_connect_configuration": "serviceConnectConfiguration",
     },
 )
 class ServiceBuild:
     def __init__(
         self,
         *,
-        cluster: aws_cdk.aws_ecs.ICluster,
-        task_definition: aws_cdk.aws_ecs.TaskDefinition,
+        cluster: _aws_cdk_aws_ecs_ceddda9d.ICluster,
+        task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
         assign_public_ip: typing.Optional[builtins.bool] = None,
-        cloud_map_options: typing.Optional[aws_cdk.aws_ecs.CloudMapOptions] = None,
+        cloud_map_options: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.CloudMapOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         desired_count: typing.Optional[jsii.Number] = None,
-        health_check_grace_period: typing.Optional[aws_cdk.Duration] = None,
+        health_check_grace_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         max_healthy_percent: typing.Optional[jsii.Number] = None,
         min_healthy_percent: typing.Optional[jsii.Number] = None,
+        service_connect_configuration: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.ServiceConnectProps, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''(experimental) A set of mutable service props in the process of being assembled using a builder pattern.
 
         They will eventually to be translated into an
         ecs.Ec2ServiceProps or ecs.FargateServiceProps interface, depending on the
         environment's capacity type.
 
@@ -2566,30 +2833,34 @@
         :param task_definition: (experimental) The task definition registered to this service.
         :param assign_public_ip: (experimental) Specifies whether the task's elastic network interface receives a public IP address. If true, each task will receive a public IP address. Default: - false
         :param cloud_map_options: (experimental) Configuration for how to register the service in service discovery. Default: - No Cloud Map configured
         :param desired_count: (experimental) How many tasks to run. Default: - 1
         :param health_check_grace_period: (experimental) How long the healthcheck can fail during initial task startup before the task is considered unhealthy. This is used to give the task more time to start passing healthchecks. Default: - No grace period
         :param max_healthy_percent: (experimental) Maximum percentage of tasks that can be launched. Default: - 200
         :param min_healthy_percent: (experimental) Minimum healthy task percentage. Default: - 100
+        :param service_connect_configuration: (experimental) Configuration for service connect for this service. Default: - No Service Connect configured.
 
         :stability: experimental
         '''
         if isinstance(cloud_map_options, dict):
-            cloud_map_options = aws_cdk.aws_ecs.CloudMapOptions(**cloud_map_options)
+            cloud_map_options = _aws_cdk_aws_ecs_ceddda9d.CloudMapOptions(**cloud_map_options)
+        if isinstance(service_connect_configuration, dict):
+            service_connect_configuration = _aws_cdk_aws_ecs_ceddda9d.ServiceConnectProps(**service_connect_configuration)
         if __debug__:
-            type_hints = typing.get_type_hints(ServiceBuild.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__bbc157cc76350e79845bf03bad3f7df149e831066f26c4ce897b5f0aa26318c9)
             check_type(argname="argument cluster", value=cluster, expected_type=type_hints["cluster"])
             check_type(argname="argument task_definition", value=task_definition, expected_type=type_hints["task_definition"])
             check_type(argname="argument assign_public_ip", value=assign_public_ip, expected_type=type_hints["assign_public_ip"])
             check_type(argname="argument cloud_map_options", value=cloud_map_options, expected_type=type_hints["cloud_map_options"])
             check_type(argname="argument desired_count", value=desired_count, expected_type=type_hints["desired_count"])
             check_type(argname="argument health_check_grace_period", value=health_check_grace_period, expected_type=type_hints["health_check_grace_period"])
             check_type(argname="argument max_healthy_percent", value=max_healthy_percent, expected_type=type_hints["max_healthy_percent"])
             check_type(argname="argument min_healthy_percent", value=min_healthy_percent, expected_type=type_hints["min_healthy_percent"])
-        self._values: typing.Dict[str, typing.Any] = {
+            check_type(argname="argument service_connect_configuration", value=service_connect_configuration, expected_type=type_hints["service_connect_configuration"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "cluster": cluster,
             "task_definition": task_definition,
         }
         if assign_public_ip is not None:
             self._values["assign_public_ip"] = assign_public_ip
         if cloud_map_options is not None:
             self._values["cloud_map_options"] = cloud_map_options
@@ -2597,34 +2868,36 @@
             self._values["desired_count"] = desired_count
         if health_check_grace_period is not None:
             self._values["health_check_grace_period"] = health_check_grace_period
         if max_healthy_percent is not None:
             self._values["max_healthy_percent"] = max_healthy_percent
         if min_healthy_percent is not None:
             self._values["min_healthy_percent"] = min_healthy_percent
+        if service_connect_configuration is not None:
+            self._values["service_connect_configuration"] = service_connect_configuration
 
     @builtins.property
-    def cluster(self) -> aws_cdk.aws_ecs.ICluster:
+    def cluster(self) -> _aws_cdk_aws_ecs_ceddda9d.ICluster:
         '''(experimental) The cluster in which to launch the service.
 
         :stability: experimental
         '''
         result = self._values.get("cluster")
         assert result is not None, "Required property 'cluster' is missing"
-        return typing.cast(aws_cdk.aws_ecs.ICluster, result)
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.ICluster, result)
 
     @builtins.property
-    def task_definition(self) -> aws_cdk.aws_ecs.TaskDefinition:
+    def task_definition(self) -> _aws_cdk_aws_ecs_ceddda9d.TaskDefinition:
         '''(experimental) The task definition registered to this service.
 
         :stability: experimental
         '''
         result = self._values.get("task_definition")
         assert result is not None, "Required property 'task_definition' is missing"
-        return typing.cast(aws_cdk.aws_ecs.TaskDefinition, result)
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.TaskDefinition, result)
 
     @builtins.property
     def assign_public_ip(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Specifies whether the task's elastic network interface receives a public IP address.
 
         If true, each task will receive a public IP address.
 
@@ -2632,48 +2905,50 @@
 
         :stability: experimental
         '''
         result = self._values.get("assign_public_ip")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def cloud_map_options(self) -> typing.Optional[aws_cdk.aws_ecs.CloudMapOptions]:
+    def cloud_map_options(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_ecs_ceddda9d.CloudMapOptions]:
         '''(experimental) Configuration for how to register the service in service discovery.
 
         :default: - No Cloud Map configured
 
         :stability: experimental
         '''
         result = self._values.get("cloud_map_options")
-        return typing.cast(typing.Optional[aws_cdk.aws_ecs.CloudMapOptions], result)
+        return typing.cast(typing.Optional[_aws_cdk_aws_ecs_ceddda9d.CloudMapOptions], result)
 
     @builtins.property
     def desired_count(self) -> typing.Optional[jsii.Number]:
         '''(experimental) How many tasks to run.
 
         :default: - 1
 
         :stability: experimental
         '''
         result = self._values.get("desired_count")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    def health_check_grace_period(self) -> typing.Optional[aws_cdk.Duration]:
+    def health_check_grace_period(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
         '''(experimental) How long the healthcheck can fail during initial task startup before the task is considered unhealthy.
 
         This is used to give the task more
         time to start passing healthchecks.
 
         :default: - No grace period
 
         :stability: experimental
         '''
         result = self._values.get("health_check_grace_period")
-        return typing.cast(typing.Optional[aws_cdk.Duration], result)
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
 
     @builtins.property
     def max_healthy_percent(self) -> typing.Optional[jsii.Number]:
         '''(experimental) Maximum percentage of tasks that can be launched.
 
         :default: - 200
 
@@ -2689,14 +2964,27 @@
         :default: - 100
 
         :stability: experimental
         '''
         result = self._values.get("min_healthy_percent")
         return typing.cast(typing.Optional[jsii.Number], result)
 
+    @builtins.property
+    def service_connect_configuration(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_ecs_ceddda9d.ServiceConnectProps]:
+        '''(experimental) Configuration for service connect for this service.
+
+        :default: - No Service Connect configured.
+
+        :stability: experimental
+        '''
+        result = self._values.get("service_connect_configuration")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ecs_ceddda9d.ServiceConnectProps], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -2732,15 +3020,15 @@
         to add resources to or configure properties for the service.
 
         :param extension: - The extension that you wish to add.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(ServiceDescription.add)
+            type_hints = typing.get_type_hints(_typecheckingstub__c093f5c31129726d3d125fea26e2c3fd91a85698eb1ba8473769eac664ab595a)
             check_type(argname="argument extension", value=extension, expected_type=type_hints["extension"])
         return typing.cast("ServiceDescription", jsii.invoke(self, "add", [extension]))
 
     @jsii.member(jsii_name="get")
     def get(self, name: builtins.str) -> "ServiceExtension":
         '''(experimental) Get the extension with a specific name.
 
@@ -2748,34 +3036,34 @@
         extensions in order to discover each other.
 
         :param name: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(ServiceDescription.get)
+            type_hints = typing.get_type_hints(_typecheckingstub__8352914d442a0691483353eb819f6ab07a7c3906ffcb4a5f205881cab8855693)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         return typing.cast("ServiceExtension", jsii.invoke(self, "get", [name]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="extensions")
     def extensions(self) -> typing.Mapping[builtins.str, "ServiceExtension"]:
         '''(experimental) The list of extensions that have been registered to run when preparing this service.
 
         :stability: experimental
         '''
         return typing.cast(typing.Mapping[builtins.str, "ServiceExtension"], jsii.get(self, "extensions"))
 
     @extensions.setter
     def extensions(
         self,
         value: typing.Mapping[builtins.str, "ServiceExtension"],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(getattr(ServiceDescription, "extensions").fset)
+            type_hints = typing.get_type_hints(_typecheckingstub__f3cc49fbfe806b68e28897ef0a6adb82ef13ea662595a6dc16cfbd1c8f3d80ff)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "extensions", value)
 
 
 class ServiceExtension(
     metaclass=jsii.JSIIAbstractClass,
     jsii_type="@aws-cdk-containers/ecs-service-extensions.ServiceExtension",
@@ -2792,15 +3080,15 @@
     def __init__(self, name: builtins.str) -> None:
         '''
         :param name: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(ServiceExtension.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__1942fe00f761e2c51266b2c817c5520489ca4dfc5fb00a8121bfc670fbf52e3f)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         jsii.create(self.__class__, self, [name])
 
     @jsii.member(jsii_name="addContainerMutatingHook")
     def add_container_mutating_hook(self, hook: ContainerMutatingHook) -> None:
         '''(experimental) This hook allows another service extension to register a mutating hook for changing the primary container of this extension.
 
@@ -2810,15 +3098,15 @@
         route logs through Firelens.
 
         :param hook: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(ServiceExtension.add_container_mutating_hook)
+            type_hints = typing.get_type_hints(_typecheckingstub__67016c4360f564fd4fe54d7d2b5edd75e564f902aee57e11136af32477ecb5c5)
             check_type(argname="argument hook", value=hook, expected_type=type_hints["hook"])
         return typing.cast(None, jsii.invoke(self, "addContainerMutatingHook", [hook]))
 
     @jsii.member(jsii_name="addHooks")
     def add_hooks(self) -> None:
         '''(experimental) A hook that allows the extension to add hooks to other extensions that are registered.
 
@@ -2841,105 +3129,108 @@
 
         :param service: - The other service to connect to.
         :param local_bind_port: (experimental) localBindPort is the local port that this application should use when calling the upstream service in ECS Consul Mesh Extension Currently, this parameter will only be used in the ECSConsulMeshExtension https://github.com/aws-ia/ecs-consul-mesh-extension.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(ServiceExtension.connect_to_service)
+            type_hints = typing.get_type_hints(_typecheckingstub__8e2d8de0dbe555c1e1b7b50b5b988162b03bc53d683e2a98a1659e95e6b1180c)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
         connect_to_props = ConnectToProps(local_bind_port=local_bind_port)
 
         return typing.cast(None, jsii.invoke(self, "connectToService", [service, connect_to_props]))
 
     @jsii.member(jsii_name="modifyServiceProps")
     def modify_service_props(
         self,
         *,
-        cluster: aws_cdk.aws_ecs.ICluster,
-        task_definition: aws_cdk.aws_ecs.TaskDefinition,
+        cluster: _aws_cdk_aws_ecs_ceddda9d.ICluster,
+        task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
         assign_public_ip: typing.Optional[builtins.bool] = None,
-        cloud_map_options: typing.Optional[aws_cdk.aws_ecs.CloudMapOptions] = None,
+        cloud_map_options: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.CloudMapOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         desired_count: typing.Optional[jsii.Number] = None,
-        health_check_grace_period: typing.Optional[aws_cdk.Duration] = None,
+        health_check_grace_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         max_healthy_percent: typing.Optional[jsii.Number] = None,
         min_healthy_percent: typing.Optional[jsii.Number] = None,
+        service_connect_configuration: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.ServiceConnectProps, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> ServiceBuild:
         '''(experimental) Prior to launching the task definition as a service, this hook is called on each extension to give it a chance to mutate the properties of the service to be created.
 
         :param cluster: (experimental) The cluster in which to launch the service.
         :param task_definition: (experimental) The task definition registered to this service.
         :param assign_public_ip: (experimental) Specifies whether the task's elastic network interface receives a public IP address. If true, each task will receive a public IP address. Default: - false
         :param cloud_map_options: (experimental) Configuration for how to register the service in service discovery. Default: - No Cloud Map configured
         :param desired_count: (experimental) How many tasks to run. Default: - 1
         :param health_check_grace_period: (experimental) How long the healthcheck can fail during initial task startup before the task is considered unhealthy. This is used to give the task more time to start passing healthchecks. Default: - No grace period
         :param max_healthy_percent: (experimental) Maximum percentage of tasks that can be launched. Default: - 200
         :param min_healthy_percent: (experimental) Minimum healthy task percentage. Default: - 100
+        :param service_connect_configuration: (experimental) Configuration for service connect for this service. Default: - No Service Connect configured.
 
         :stability: experimental
         '''
         props = ServiceBuild(
             cluster=cluster,
             task_definition=task_definition,
             assign_public_ip=assign_public_ip,
             cloud_map_options=cloud_map_options,
             desired_count=desired_count,
             health_check_grace_period=health_check_grace_period,
             max_healthy_percent=max_healthy_percent,
             min_healthy_percent=min_healthy_percent,
+            service_connect_configuration=service_connect_configuration,
         )
 
         return typing.cast(ServiceBuild, jsii.invoke(self, "modifyServiceProps", [props]))
 
     @jsii.member(jsii_name="modifyTaskDefinitionProps")
     def modify_task_definition_props(
         self,
         *,
-        compatibility: aws_cdk.aws_ecs.Compatibility,
+        compatibility: _aws_cdk_aws_ecs_ceddda9d.Compatibility,
         cpu: typing.Optional[builtins.str] = None,
         ephemeral_storage_gib: typing.Optional[jsii.Number] = None,
-        inference_accelerators: typing.Optional[typing.Sequence[aws_cdk.aws_ecs.InferenceAccelerator]] = None,
-        ipc_mode: typing.Optional[aws_cdk.aws_ecs.IpcMode] = None,
+        inference_accelerators: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecs_ceddda9d.InferenceAccelerator, typing.Dict[builtins.str, typing.Any]]]] = None,
+        ipc_mode: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.IpcMode] = None,
         memory_mib: typing.Optional[builtins.str] = None,
-        network_mode: typing.Optional[aws_cdk.aws_ecs.NetworkMode] = None,
-        pid_mode: typing.Optional[aws_cdk.aws_ecs.PidMode] = None,
-        placement_constraints: typing.Optional[typing.Sequence[aws_cdk.aws_ecs.PlacementConstraint]] = None,
-        runtime_platform: typing.Optional[aws_cdk.aws_ecs.RuntimePlatform] = None,
-        execution_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
+        network_mode: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.NetworkMode] = None,
+        pid_mode: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.PidMode] = None,
+        placement_constraints: typing.Optional[typing.Sequence[_aws_cdk_aws_ecs_ceddda9d.PlacementConstraint]] = None,
+        runtime_platform: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.RuntimePlatform, typing.Dict[builtins.str, typing.Any]]] = None,
+        execution_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         family: typing.Optional[builtins.str] = None,
-        proxy_configuration: typing.Optional[aws_cdk.aws_ecs.ProxyConfiguration] = None,
-        task_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
-        volumes: typing.Optional[typing.Sequence[aws_cdk.aws_ecs.Volume]] = None,
-    ) -> aws_cdk.aws_ecs.TaskDefinitionProps:
+        proxy_configuration: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.ProxyConfiguration] = None,
+        task_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        volumes: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecs_ceddda9d.Volume, typing.Dict[builtins.str, typing.Any]]]] = None,
+    ) -> _aws_cdk_aws_ecs_ceddda9d.TaskDefinitionProps:
         '''(experimental) This is a hook which allows extensions to modify the settings of the task definition prior to it being created.
 
         For example, the App Mesh
         extension needs to configure an Envoy proxy in the task definition,
         or the Application extension wants to set the overall resource for
         the task.
 
         :param compatibility: The task launch type compatiblity requirement.
-        :param cpu: The number of cpu units used by the task. If you are using the EC2 launch type, this field is optional and any value can be used. If you are using the Fargate launch type, this field is required and you must use one of the following values, which determines your range of valid values for the memory parameter: 256 (.25 vCPU) - Available memory values: 512 (0.5 GB), 1024 (1 GB), 2048 (2 GB) 512 (.5 vCPU) - Available memory values: 1024 (1 GB), 2048 (2 GB), 3072 (3 GB), 4096 (4 GB) 1024 (1 vCPU) - Available memory values: 2048 (2 GB), 3072 (3 GB), 4096 (4 GB), 5120 (5 GB), 6144 (6 GB), 7168 (7 GB), 8192 (8 GB) 2048 (2 vCPU) - Available memory values: Between 4096 (4 GB) and 16384 (16 GB) in increments of 1024 (1 GB) 4096 (4 vCPU) - Available memory values: Between 8192 (8 GB) and 30720 (30 GB) in increments of 1024 (1 GB) Default: - CPU units are not specified.
+        :param cpu: The number of cpu units used by the task. If you are using the EC2 launch type, this field is optional and any value can be used. If you are using the Fargate launch type, this field is required and you must use one of the following values, which determines your range of valid values for the memory parameter: 256 (.25 vCPU) - Available memory values: 512 (0.5 GB), 1024 (1 GB), 2048 (2 GB) 512 (.5 vCPU) - Available memory values: 1024 (1 GB), 2048 (2 GB), 3072 (3 GB), 4096 (4 GB) 1024 (1 vCPU) - Available memory values: 2048 (2 GB), 3072 (3 GB), 4096 (4 GB), 5120 (5 GB), 6144 (6 GB), 7168 (7 GB), 8192 (8 GB) 2048 (2 vCPU) - Available memory values: Between 4096 (4 GB) and 16384 (16 GB) in increments of 1024 (1 GB) 4096 (4 vCPU) - Available memory values: Between 8192 (8 GB) and 30720 (30 GB) in increments of 1024 (1 GB) 8192 (8 vCPU) - Available memory values: Between 16384 (16 GB) and 61440 (60 GB) in increments of 4096 (4 GB) 16384 (16 vCPU) - Available memory values: Between 32768 (32 GB) and 122880 (120 GB) in increments of 8192 (8 GB) Default: - CPU units are not specified.
         :param ephemeral_storage_gib: The amount (in GiB) of ephemeral storage to be allocated to the task. Only supported in Fargate platform version 1.4.0 or later. Default: - Undefined, in which case, the task will receive 20GiB ephemeral storage.
         :param inference_accelerators: The inference accelerators to use for the containers in the task. Not supported in Fargate. Default: - No inference accelerators.
         :param ipc_mode: The IPC resource namespace to use for the containers in the task. Not supported in Fargate and Windows containers. Default: - IpcMode used by the task is not specified
-        :param memory_mib: The amount (in MiB) of memory used by the task. If using the EC2 launch type, this field is optional and any value can be used. If using the Fargate launch type, this field is required and you must use one of the following values, which determines your range of valid values for the cpu parameter: 512 (0.5 GB), 1024 (1 GB), 2048 (2 GB) - Available cpu values: 256 (.25 vCPU) 1024 (1 GB), 2048 (2 GB), 3072 (3 GB), 4096 (4 GB) - Available cpu values: 512 (.5 vCPU) 2048 (2 GB), 3072 (3 GB), 4096 (4 GB), 5120 (5 GB), 6144 (6 GB), 7168 (7 GB), 8192 (8 GB) - Available cpu values: 1024 (1 vCPU) Between 4096 (4 GB) and 16384 (16 GB) in increments of 1024 (1 GB) - Available cpu values: 2048 (2 vCPU) Between 8192 (8 GB) and 30720 (30 GB) in increments of 1024 (1 GB) - Available cpu values: 4096 (4 vCPU) Default: - Memory used by task is not specified.
+        :param memory_mib: The amount (in MiB) of memory used by the task. If using the EC2 launch type, this field is optional and any value can be used. If using the Fargate launch type, this field is required and you must use one of the following values, which determines your range of valid values for the cpu parameter: 512 (0.5 GB), 1024 (1 GB), 2048 (2 GB) - Available cpu values: 256 (.25 vCPU) 1024 (1 GB), 2048 (2 GB), 3072 (3 GB), 4096 (4 GB) - Available cpu values: 512 (.5 vCPU) 2048 (2 GB), 3072 (3 GB), 4096 (4 GB), 5120 (5 GB), 6144 (6 GB), 7168 (7 GB), 8192 (8 GB) - Available cpu values: 1024 (1 vCPU) Between 4096 (4 GB) and 16384 (16 GB) in increments of 1024 (1 GB) - Available cpu values: 2048 (2 vCPU) Between 8192 (8 GB) and 30720 (30 GB) in increments of 1024 (1 GB) - Available cpu values: 4096 (4 vCPU) Between 16384 (16 GB) and 61440 (60 GB) in increments of 4096 (4 GB) - Available cpu values: 8192 (8 vCPU) Between 32768 (32 GB) and 122880 (120 GB) in increments of 8192 (8 GB) - Available cpu values: 16384 (16 vCPU) Default: - Memory used by task is not specified.
         :param network_mode: The networking mode to use for the containers in the task. On Fargate, the only supported networking mode is AwsVpc. Default: - NetworkMode.Bridge for EC2 & External tasks, AwsVpc for Fargate tasks.
         :param pid_mode: The process namespace to use for the containers in the task. Not supported in Fargate and Windows containers. Default: - PidMode used by the task is not specified
         :param placement_constraints: The placement constraints to use for tasks in the service. You can specify a maximum of 10 constraints per task (this limit includes constraints in the task definition and those specified at run time). Not supported in Fargate. Default: - No placement constraints.
         :param runtime_platform: The operating system that your task definitions are running on. A runtimePlatform is supported only for tasks using the Fargate launch type. Default: - Undefined.
         :param execution_role: The name of the IAM task execution role that grants the ECS agent permission to call AWS APIs on your behalf. The role will be used to retrieve container images from ECR and create CloudWatch log groups. Default: - An execution role will be automatically created if you use ECR images in your task definition.
         :param family: The name of a family that this task definition is registered to. A family groups multiple versions of a task definition. Default: - Automatically generated name.
         :param proxy_configuration: The configuration details for the App Mesh proxy. Default: - No proxy configuration.
         :param task_role: The name of the IAM role that grants containers in the task permission to call AWS APIs on your behalf. Default: - A task role is automatically created for you.
         :param volumes: The list of volume definitions for the task. For more information, see `Task Definition Parameter Volumes <https://docs.aws.amazon.com/AmazonECS/latest/developerguide//task_definition_parameters.html#volumes>`_. Default: - No volumes are passed to the Docker daemon on a container instance.
 
         :stability: experimental
         '''
-        props = aws_cdk.aws_ecs.TaskDefinitionProps(
+        props = _aws_cdk_aws_ecs_ceddda9d.TaskDefinitionProps(
             compatibility=compatibility,
             cpu=cpu,
             ephemeral_storage_gib=ephemeral_storage_gib,
             inference_accelerators=inference_accelerators,
             ipc_mode=ipc_mode,
             memory_mib=memory_mib,
             network_mode=network_mode,
@@ -2949,27 +3240,27 @@
             execution_role=execution_role,
             family=family,
             proxy_configuration=proxy_configuration,
             task_role=task_role,
             volumes=volumes,
         )
 
-        return typing.cast(aws_cdk.aws_ecs.TaskDefinitionProps, jsii.invoke(self, "modifyTaskDefinitionProps", [props]))
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.TaskDefinitionProps, jsii.invoke(self, "modifyTaskDefinitionProps", [props]))
 
     @jsii.member(jsii_name="prehook")
-    def prehook(self, parent: Service, scope: constructs.Construct) -> None:
+    def prehook(self, parent: Service, scope: _constructs_77d1e7e8.Construct) -> None:
         '''(experimental) A hook that is called for each extension ahead of time to allow for any initial setup, such as creating resources in advance.
 
         :param parent: - The parent service which this extension has been added to.
         :param scope: - The scope that this extension should create resources in.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(ServiceExtension.prehook)
+            type_hints = typing.get_type_hints(_typecheckingstub__eefdf655cd0e7f30d0fcf6f77a6d8729245c20be4605fa83182a750656dd59de)
             check_type(argname="argument parent", value=parent, expected_type=type_hints["parent"])
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
         return typing.cast(None, jsii.invoke(self, "prehook", [parent, scope]))
 
     @jsii.member(jsii_name="resolveContainerDependencies")
     def resolve_container_dependencies(self) -> None:
         '''(experimental) Once all containers are added to the task definition, this hook is called for each extension to give it a chance to resolve its dependency graph so that its container starts in the right order based on the other extensions that were enabled.
@@ -2977,81 +3268,81 @@
         :stability: experimental
         '''
         return typing.cast(None, jsii.invoke(self, "resolveContainerDependencies", []))
 
     @jsii.member(jsii_name="useService")
     def use_service(
         self,
-        service: typing.Union[aws_cdk.aws_ecs.Ec2Service, aws_cdk.aws_ecs.FargateService],
+        service: typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService],
     ) -> None:
         '''(experimental) When this hook is implemented by extension, it allows the extension to use the service which has been created.
 
         It is generally used to
         create any final resources which might depend on the service itself.
 
         :param service: - The generated service.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(ServiceExtension.use_service)
+            type_hints = typing.get_type_hints(_typecheckingstub__38e3e0860e30eb48b790e6fc0840c9d9d36bff02f4ab4e976e145f4f85ef048d)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
         return typing.cast(None, jsii.invoke(self, "useService", [service]))
 
     @jsii.member(jsii_name="useTaskDefinition")
     def use_task_definition(
         self,
-        task_definition: aws_cdk.aws_ecs.TaskDefinition,
+        task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
     ) -> None:
         '''(experimental) Once the task definition is created, this hook is called for each extension to give it a chance to add containers to the task definition, change the task definition's role to add permissions, etc.
 
         :param task_definition: - The created task definition to add containers to.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(ServiceExtension.use_task_definition)
+            type_hints = typing.get_type_hints(_typecheckingstub__e93694c5c40f28677d9914773fe2949cbdf32f19f86771a0f343852c4a456833)
             check_type(argname="argument task_definition", value=task_definition, expected_type=type_hints["task_definition"])
         return typing.cast(None, jsii.invoke(self, "useTaskDefinition", [task_definition]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="containerMutatingHooks")
     def _container_mutating_hooks(self) -> typing.List[ContainerMutatingHook]:
         '''
         :stability: experimental
         '''
         return typing.cast(typing.List[ContainerMutatingHook], jsii.get(self, "containerMutatingHooks"))
 
     @_container_mutating_hooks.setter
     def _container_mutating_hooks(
         self,
         value: typing.List[ContainerMutatingHook],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(getattr(ServiceExtension, "_container_mutating_hooks").fset)
+            type_hints = typing.get_type_hints(_typecheckingstub__299f56627660a08293011eb309421e4c9ecab06a492c5135e001bb57465be12a)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "containerMutatingHooks", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         '''(experimental) The name of the extension.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(getattr(ServiceExtension, "name").fset)
+            type_hints = typing.get_type_hints(_typecheckingstub__ffd5c720e9e1800e56e330f06b53101d51e941eae8399ed18a6ce3469d004a45)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="parentService")
     def _parent_service(self) -> Service:
         '''(experimental) The service which this extension is being added to.
 
         Initially, extensions are collected into a ServiceDescription, but no service
         exists yet. Later, when the ServiceDescription is used to create a service,
         the extension is told what Service it is now working on.
@@ -3059,54 +3350,56 @@
         :stability: experimental
         '''
         return typing.cast(Service, jsii.get(self, "parentService"))
 
     @_parent_service.setter
     def _parent_service(self, value: Service) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(getattr(ServiceExtension, "_parent_service").fset)
+            type_hints = typing.get_type_hints(_typecheckingstub__888537d4e44499688ac07459949d868e9b29b5f5b71d885c9f28d9f42d26a293)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "parentService", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scope")
-    def _scope(self) -> constructs.Construct:
+    def _scope(self) -> _constructs_77d1e7e8.Construct:
         '''
         :stability: experimental
         '''
-        return typing.cast(constructs.Construct, jsii.get(self, "scope"))
+        return typing.cast(_constructs_77d1e7e8.Construct, jsii.get(self, "scope"))
 
     @_scope.setter
-    def _scope(self, value: constructs.Construct) -> None:
+    def _scope(self, value: _constructs_77d1e7e8.Construct) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(getattr(ServiceExtension, "_scope").fset)
+            type_hints = typing.get_type_hints(_typecheckingstub__22b87c7ca09e39c9e04f952a479384b276834e484577d808867f6e8cd36eae87)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scope", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="container")
-    def container(self) -> typing.Optional[aws_cdk.aws_ecs.ContainerDefinition]:
+    def container(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_ecs_ceddda9d.ContainerDefinition]:
         '''(experimental) The container for this extension.
 
         Most extensions have a container, but not
         every extension is required to have a container. Some extensions may just
         modify the properties of the service, or create external resources
         connected to the service.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[aws_cdk.aws_ecs.ContainerDefinition], jsii.get(self, "container"))
+        return typing.cast(typing.Optional[_aws_cdk_aws_ecs_ceddda9d.ContainerDefinition], jsii.get(self, "container"))
 
     @container.setter
     def container(
         self,
-        value: typing.Optional[aws_cdk.aws_ecs.ContainerDefinition],
+        value: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.ContainerDefinition],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(getattr(ServiceExtension, "container").fset)
+            type_hints = typing.get_type_hints(_typecheckingstub__54f71fbef259bce4d04ac1599a7734f8470b603b265ce3c405992e7d9403cc63)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "container", value)
 
 
 class _ServiceExtensionProxy(ServiceExtension):
     pass
 
@@ -3127,38 +3420,38 @@
 )
 class ServiceProps:
     def __init__(
         self,
         *,
         environment: IEnvironment,
         service_description: ServiceDescription,
-        auto_scale_task_count: typing.Optional[AutoScalingOptions] = None,
+        auto_scale_task_count: typing.Optional[typing.Union[AutoScalingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         desired_count: typing.Optional[jsii.Number] = None,
-        task_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
+        task_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     ) -> None:
         '''(experimental) The settings for an ECS Service.
 
         :param environment: (experimental) The environment to launch the service in.
         :param service_description: (experimental) The ServiceDescription used to build the service.
         :param auto_scale_task_count: (experimental) The options for configuring the auto scaling target. Default: none
         :param desired_count: (experimental) The desired number of instantiations of the task definition to keep running on the service. Default: - When creating the service, default is 1; when updating the service, default uses the current task number.
         :param task_role: (experimental) The name of the IAM role that grants containers in the task permission to call AWS APIs on your behalf. Default: - A task role is automatically created for you.
 
         :stability: experimental
         '''
         if isinstance(auto_scale_task_count, dict):
             auto_scale_task_count = AutoScalingOptions(**auto_scale_task_count)
         if __debug__:
-            type_hints = typing.get_type_hints(ServiceProps.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__8324f912a77ba2380fbec2194e091c70e44826a63d04c9b3b3178db416008d54)
             check_type(argname="argument environment", value=environment, expected_type=type_hints["environment"])
             check_type(argname="argument service_description", value=service_description, expected_type=type_hints["service_description"])
             check_type(argname="argument auto_scale_task_count", value=auto_scale_task_count, expected_type=type_hints["auto_scale_task_count"])
             check_type(argname="argument desired_count", value=desired_count, expected_type=type_hints["desired_count"])
             check_type(argname="argument task_role", value=task_role, expected_type=type_hints["task_role"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "environment": environment,
             "service_description": service_description,
         }
         if auto_scale_task_count is not None:
             self._values["auto_scale_task_count"] = auto_scale_task_count
         if desired_count is not None:
             self._values["desired_count"] = desired_count
@@ -3207,23 +3500,23 @@
 
         :stability: experimental
         '''
         result = self._values.get("desired_count")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    def task_role(self) -> typing.Optional[aws_cdk.aws_iam.IRole]:
+    def task_role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
         '''(experimental) The name of the IAM role that grants containers in the task permission to call AWS APIs on your behalf.
 
         :default: - A task role is automatically created for you.
 
         :stability: experimental
         '''
         result = self._values.get("task_role")
-        return typing.cast(typing.Optional[aws_cdk.aws_iam.IRole], result)
+        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -3238,45 +3531,45 @@
     jsii_struct_bases=[],
     name_mapping={"queue": "queue", "scale_on_latency": "scaleOnLatency"},
 )
 class SubscriptionQueue:
     def __init__(
         self,
         *,
-        queue: aws_cdk.aws_sqs.IQueue,
-        scale_on_latency: typing.Optional[QueueAutoScalingOptions] = None,
+        queue: _aws_cdk_aws_sqs_ceddda9d.IQueue,
+        scale_on_latency: typing.Optional[typing.Union[QueueAutoScalingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''(experimental) ``SubscriptionQueue`` represents the subscription queue object which includes the topic-specific queue and its corresponding auto scaling fields.
 
         :param queue: (experimental) The user-provided queue to subscribe to the given topic.
         :param scale_on_latency: (experimental) The user-provided queue delay fields to configure auto scaling for the topic-specific queue. Default: none
 
         :stability: experimental
         '''
         if isinstance(scale_on_latency, dict):
             scale_on_latency = QueueAutoScalingOptions(**scale_on_latency)
         if __debug__:
-            type_hints = typing.get_type_hints(SubscriptionQueue.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__2ab599485b374c44897ab0ae8820090231221b727f0f9968276a4071085689df)
             check_type(argname="argument queue", value=queue, expected_type=type_hints["queue"])
             check_type(argname="argument scale_on_latency", value=scale_on_latency, expected_type=type_hints["scale_on_latency"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "queue": queue,
         }
         if scale_on_latency is not None:
             self._values["scale_on_latency"] = scale_on_latency
 
     @builtins.property
-    def queue(self) -> aws_cdk.aws_sqs.IQueue:
+    def queue(self) -> _aws_cdk_aws_sqs_ceddda9d.IQueue:
         '''(experimental) The user-provided queue to subscribe to the given topic.
 
         :stability: experimental
         '''
         result = self._values.get("queue")
         assert result is not None, "Required property 'queue' is missing"
-        return typing.cast(aws_cdk.aws_sqs.IQueue, result)
+        return typing.cast(_aws_cdk_aws_sqs_ceddda9d.IQueue, result)
 
     @builtins.property
     def scale_on_latency(self) -> typing.Optional[QueueAutoScalingOptions]:
         '''(experimental) The user-provided queue delay fields to configure auto scaling for the topic-specific queue.
 
         :default: none
 
@@ -3306,17 +3599,17 @@
 
     :stability: experimental
     '''
 
     def __init__(
         self,
         *,
-        topic: aws_cdk.aws_sns.ITopic,
-        queue: typing.Optional[aws_cdk.aws_sqs.IQueue] = None,
-        topic_subscription_queue: typing.Optional[SubscriptionQueue] = None,
+        topic: _aws_cdk_aws_sns_ceddda9d.ITopic,
+        queue: typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue] = None,
+        topic_subscription_queue: typing.Optional[typing.Union[SubscriptionQueue, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param topic: (experimental) The SNS Topic to subscribe to.
         :param queue: (deprecated) The user-provided queue to subscribe to the given topic. Default: none
         :param topic_subscription_queue: (experimental) The object representing topic-specific queue and corresponding queue delay fields to configure auto scaling. If not provided, the default ``eventsQueue`` will subscribe to the given topic. Default: none
 
         :stability: experimental
@@ -3324,53 +3617,56 @@
         props = TopicSubscriptionProps(
             topic=topic, queue=queue, topic_subscription_queue=topic_subscription_queue
         )
 
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="subscribe")
-    def subscribe(self, extension: "QueueExtension") -> aws_cdk.aws_sqs.IQueue:
+    def subscribe(
+        self,
+        extension: "QueueExtension",
+    ) -> _aws_cdk_aws_sqs_ceddda9d.IQueue:
         '''(experimental) This method sets up SNS Topic subscriptions for the SQS queue provided by the user.
 
         If a ``queue`` is not provided,
         the default ``eventsQueue`` subscribes to the given topic.
 
         :param extension: ``QueueExtension`` added to the service.
 
         :return: the queue subscribed to the given topic
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(TopicSubscription.subscribe)
+            type_hints = typing.get_type_hints(_typecheckingstub__542dd993b9b30463def0028989d7fe8b3f0f9e422cb20bea69ab3b83367fbdb4)
             check_type(argname="argument extension", value=extension, expected_type=type_hints["extension"])
-        return typing.cast(aws_cdk.aws_sqs.IQueue, jsii.invoke(self, "subscribe", [extension]))
+        return typing.cast(_aws_cdk_aws_sqs_ceddda9d.IQueue, jsii.invoke(self, "subscribe", [extension]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="topic")
-    def topic(self) -> aws_cdk.aws_sns.ITopic:
+    def topic(self) -> _aws_cdk_aws_sns_ceddda9d.ITopic:
         '''
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_sns.ITopic, jsii.get(self, "topic"))
+        return typing.cast(_aws_cdk_aws_sns_ceddda9d.ITopic, jsii.get(self, "topic"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="queue")
-    def queue(self) -> typing.Optional[aws_cdk.aws_sqs.IQueue]:
+    def queue(self) -> typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue]:
         '''(deprecated) The queue that subscribes to the given topic.
 
         :default: none
 
         :deprecated: use ``subscriptionQueue``
 
         :stability: deprecated
         '''
-        return typing.cast(typing.Optional[aws_cdk.aws_sqs.IQueue], jsii.get(self, "queue"))
+        return typing.cast(typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue], jsii.get(self, "queue"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="subscriptionQueue")
     def subscription_queue(self) -> typing.Optional[SubscriptionQueue]:
         '''(experimental) The subscription queue object for this subscription.
 
         :default: none
 
         :stability: experimental
@@ -3387,63 +3683,63 @@
         "topic_subscription_queue": "topicSubscriptionQueue",
     },
 )
 class TopicSubscriptionProps:
     def __init__(
         self,
         *,
-        topic: aws_cdk.aws_sns.ITopic,
-        queue: typing.Optional[aws_cdk.aws_sqs.IQueue] = None,
-        topic_subscription_queue: typing.Optional[SubscriptionQueue] = None,
+        topic: _aws_cdk_aws_sns_ceddda9d.ITopic,
+        queue: typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue] = None,
+        topic_subscription_queue: typing.Optional[typing.Union[SubscriptionQueue, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''(experimental) The topic-specific settings for creating the queue subscriptions.
 
         :param topic: (experimental) The SNS Topic to subscribe to.
         :param queue: (deprecated) The user-provided queue to subscribe to the given topic. Default: none
         :param topic_subscription_queue: (experimental) The object representing topic-specific queue and corresponding queue delay fields to configure auto scaling. If not provided, the default ``eventsQueue`` will subscribe to the given topic. Default: none
 
         :stability: experimental
         '''
         if isinstance(topic_subscription_queue, dict):
             topic_subscription_queue = SubscriptionQueue(**topic_subscription_queue)
         if __debug__:
-            type_hints = typing.get_type_hints(TopicSubscriptionProps.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__6ce31ca30734748c8286306049838377fd0ae5237a93f44655e549a682baaf92)
             check_type(argname="argument topic", value=topic, expected_type=type_hints["topic"])
             check_type(argname="argument queue", value=queue, expected_type=type_hints["queue"])
             check_type(argname="argument topic_subscription_queue", value=topic_subscription_queue, expected_type=type_hints["topic_subscription_queue"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "topic": topic,
         }
         if queue is not None:
             self._values["queue"] = queue
         if topic_subscription_queue is not None:
             self._values["topic_subscription_queue"] = topic_subscription_queue
 
     @builtins.property
-    def topic(self) -> aws_cdk.aws_sns.ITopic:
+    def topic(self) -> _aws_cdk_aws_sns_ceddda9d.ITopic:
         '''(experimental) The SNS Topic to subscribe to.
 
         :stability: experimental
         '''
         result = self._values.get("topic")
         assert result is not None, "Required property 'topic' is missing"
-        return typing.cast(aws_cdk.aws_sns.ITopic, result)
+        return typing.cast(_aws_cdk_aws_sns_ceddda9d.ITopic, result)
 
     @builtins.property
-    def queue(self) -> typing.Optional[aws_cdk.aws_sqs.IQueue]:
+    def queue(self) -> typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue]:
         '''(deprecated) The user-provided queue to subscribe to the given topic.
 
         :default: none
 
         :deprecated: use ``topicSubscriptionQueue``
 
         :stability: deprecated
         '''
         result = self._values.get("queue")
-        return typing.cast(typing.Optional[aws_cdk.aws_sqs.IQueue], result)
+        return typing.cast(typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue], result)
 
     @builtins.property
     def topic_subscription_queue(self) -> typing.Optional[SubscriptionQueue]:
         '''(experimental) The object representing topic-specific queue and corresponding queue delay fields to configure auto scaling.
 
         If not provided, the default ``eventsQueue`` will subscribe to the given topic.
 
@@ -3479,24 +3775,24 @@
     def __init__(self) -> None:
         '''
         :stability: experimental
         '''
         jsii.create(self.__class__, self, [])
 
     @jsii.member(jsii_name="prehook")
-    def prehook(self, service: Service, scope: constructs.Construct) -> None:
+    def prehook(self, service: Service, scope: _constructs_77d1e7e8.Construct) -> None:
         '''(experimental) A hook that is called for each extension ahead of time to allow for any initial setup, such as creating resources in advance.
 
         :param service: -
         :param scope: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(XRayExtension.prehook)
+            type_hints = typing.get_type_hints(_typecheckingstub__a25c259153e7aabb24a4f343378b533b165fcb42b53180b3fdd7f72da6371ad2)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
         return typing.cast(None, jsii.invoke(self, "prehook", [service, scope]))
 
     @jsii.member(jsii_name="resolveContainerDependencies")
     def resolve_container_dependencies(self) -> None:
         '''(experimental) Once all containers are added to the task definition, this hook is called for each extension to give it a chance to resolve its dependency graph so that its container starts in the right order based on the other extensions that were enabled.
@@ -3504,28 +3800,331 @@
         :stability: experimental
         '''
         return typing.cast(None, jsii.invoke(self, "resolveContainerDependencies", []))
 
     @jsii.member(jsii_name="useTaskDefinition")
     def use_task_definition(
         self,
-        task_definition: aws_cdk.aws_ecs.TaskDefinition,
+        task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
     ) -> None:
         '''(experimental) Once the task definition is created, this hook is called for each extension to give it a chance to add containers to the task definition, change the task definition's role to add permissions, etc.
 
         :param task_definition: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(XRayExtension.use_task_definition)
+            type_hints = typing.get_type_hints(_typecheckingstub__02d9f8aa0fd942e4f491eeddab502c60a5a201811637d732a37f9d950cb67311)
             check_type(argname="argument task_definition", value=task_definition, expected_type=type_hints["task_definition"])
         return typing.cast(None, jsii.invoke(self, "useTaskDefinition", [task_definition]))
 
 
+class AliasedPortExtension(
+    ServiceExtension,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@aws-cdk-containers/ecs-service-extensions.AliasedPortExtension",
+):
+    '''
+    :stability: experimental
+    '''
+
+    def __init__(
+        self,
+        *,
+        alias: builtins.str,
+        alias_port: typing.Optional[jsii.Number] = None,
+        app_protocol: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.AppProtocol] = None,
+    ) -> None:
+        '''
+        :param alias: (experimental) The DNS alias to advertise for downstream clients.
+        :param alias_port: (experimental) The traffic port for clients to use to connect to the DNS alias. Default: - same as containerPort.
+        :param app_protocol: (experimental) The protocol to use over the specified port. May be one of HTTP, HTTP2, or GRPC. Default: - none
+
+        :stability: experimental
+        '''
+        props = AliasedPortProps(
+            alias=alias, alias_port=alias_port, app_protocol=app_protocol
+        )
+
+        jsii.create(self.__class__, self, [props])
+
+    @jsii.member(jsii_name="addHooks")
+    def add_hooks(self) -> None:
+        '''(experimental) A hook that allows the extension to add hooks to other extensions that are registered.
+
+        :stability: experimental
+        '''
+        return typing.cast(None, jsii.invoke(self, "addHooks", []))
+
+    @jsii.member(jsii_name="modifyServiceProps")
+    def modify_service_props(
+        self,
+        *,
+        cluster: _aws_cdk_aws_ecs_ceddda9d.ICluster,
+        task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
+        assign_public_ip: typing.Optional[builtins.bool] = None,
+        cloud_map_options: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.CloudMapOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        desired_count: typing.Optional[jsii.Number] = None,
+        health_check_grace_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        max_healthy_percent: typing.Optional[jsii.Number] = None,
+        min_healthy_percent: typing.Optional[jsii.Number] = None,
+        service_connect_configuration: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.ServiceConnectProps, typing.Dict[builtins.str, typing.Any]]] = None,
+    ) -> ServiceBuild:
+        '''(experimental) Prior to launching the task definition as a service, this hook is called on each extension to give it a chance to mutate the properties of the service to be created.
+
+        :param cluster: (experimental) The cluster in which to launch the service.
+        :param task_definition: (experimental) The task definition registered to this service.
+        :param assign_public_ip: (experimental) Specifies whether the task's elastic network interface receives a public IP address. If true, each task will receive a public IP address. Default: - false
+        :param cloud_map_options: (experimental) Configuration for how to register the service in service discovery. Default: - No Cloud Map configured
+        :param desired_count: (experimental) How many tasks to run. Default: - 1
+        :param health_check_grace_period: (experimental) How long the healthcheck can fail during initial task startup before the task is considered unhealthy. This is used to give the task more time to start passing healthchecks. Default: - No grace period
+        :param max_healthy_percent: (experimental) Maximum percentage of tasks that can be launched. Default: - 200
+        :param min_healthy_percent: (experimental) Minimum healthy task percentage. Default: - 100
+        :param service_connect_configuration: (experimental) Configuration for service connect for this service. Default: - No Service Connect configured.
+
+        :stability: experimental
+        '''
+        props = ServiceBuild(
+            cluster=cluster,
+            task_definition=task_definition,
+            assign_public_ip=assign_public_ip,
+            cloud_map_options=cloud_map_options,
+            desired_count=desired_count,
+            health_check_grace_period=health_check_grace_period,
+            max_healthy_percent=max_healthy_percent,
+            min_healthy_percent=min_healthy_percent,
+            service_connect_configuration=service_connect_configuration,
+        )
+
+        return typing.cast(ServiceBuild, jsii.invoke(self, "modifyServiceProps", [props]))
+
+    @jsii.member(jsii_name="prehook")
+    def prehook(self, service: Service, scope: _constructs_77d1e7e8.Construct) -> None:
+        '''(experimental) A hook that is called for each extension ahead of time to allow for any initial setup, such as creating resources in advance.
+
+        :param service: -
+        :param scope: -
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__1043b521b7d8a62b95b2d33c980009a15390b055b8b23fb3fa89a4601d987fbe)
+            check_type(argname="argument service", value=service, expected_type=type_hints["service"])
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+        return typing.cast(None, jsii.invoke(self, "prehook", [service, scope]))
+
+    @builtins.property
+    @jsii.member(jsii_name="alias")
+    def _alias(self) -> builtins.str:
+        '''
+        :stability: experimental
+        '''
+        return typing.cast(builtins.str, jsii.get(self, "alias"))
+
+    @_alias.setter
+    def _alias(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__0d404dfff99916347cd236463a68228c5807d4e62df7247b71f3de0207b4ecdb)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "alias", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="aliasPort")
+    def _alias_port(self) -> typing.Optional[jsii.Number]:
+        '''
+        :stability: experimental
+        '''
+        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "aliasPort"))
+
+    @_alias_port.setter
+    def _alias_port(self, value: typing.Optional[jsii.Number]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__69dab24a138f3970d3fecdca97edefcacb2ca2b0f643129d3cda322bcb9be285)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "aliasPort", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="appProtocol")
+    def _app_protocol(self) -> typing.Optional[_aws_cdk_aws_ecs_ceddda9d.AppProtocol]:
+        '''
+        :stability: experimental
+        '''
+        return typing.cast(typing.Optional[_aws_cdk_aws_ecs_ceddda9d.AppProtocol], jsii.get(self, "appProtocol"))
+
+    @_app_protocol.setter
+    def _app_protocol(
+        self,
+        value: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.AppProtocol],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__e54f461371069afdb909684795279f736b187cc7fb5b7ef682d1fb827a6b0846)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "appProtocol", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="namespace")
+    def _namespace(self) -> typing.Optional[builtins.str]:
+        '''
+        :stability: experimental
+        '''
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "namespace"))
+
+    @_namespace.setter
+    def _namespace(self, value: typing.Optional[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__0681b9db0238b5ddb0fd915e2a2f44cec1c3d21ec400322498e8bfe207d0f483)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "namespace", value)
+
+
+class AliasedPortMutatingHook(
+    ContainerMutatingHook,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@aws-cdk-containers/ecs-service-extensions.AliasedPortMutatingHook",
+):
+    '''(experimental) This hook modifies the application container's settings so that its primary port mapping has a name.
+
+    :stability: experimental
+    '''
+
+    def __init__(
+        self,
+        *,
+        alias_port: jsii.Number,
+        port_mapping_name: builtins.str,
+        protocol: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.AppProtocol] = None,
+    ) -> None:
+        '''
+        :param alias_port: (experimental) The port on the container which receives traffic. This is the same as the ``containerPort`` property of port mapping.
+        :param port_mapping_name: (experimental) The name by which to refer to this port mapping.
+        :param protocol: (experimental) The protocol which this port mapping expects to receive. Default: - none
+
+        :stability: experimental
+        '''
+        props = AliasedPortMutatingHookProps(
+            alias_port=alias_port,
+            port_mapping_name=port_mapping_name,
+            protocol=protocol,
+        )
+
+        jsii.create(self.__class__, self, [props])
+
+    @jsii.member(jsii_name="mutateContainerDefinition")
+    def mutate_container_definition(
+        self,
+        *,
+        image: _aws_cdk_aws_ecs_ceddda9d.ContainerImage,
+        command: typing.Optional[typing.Sequence[builtins.str]] = None,
+        container_name: typing.Optional[builtins.str] = None,
+        cpu: typing.Optional[jsii.Number] = None,
+        disable_networking: typing.Optional[builtins.bool] = None,
+        dns_search_domains: typing.Optional[typing.Sequence[builtins.str]] = None,
+        dns_servers: typing.Optional[typing.Sequence[builtins.str]] = None,
+        docker_labels: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        docker_security_options: typing.Optional[typing.Sequence[builtins.str]] = None,
+        entry_point: typing.Optional[typing.Sequence[builtins.str]] = None,
+        environment: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        environment_files: typing.Optional[typing.Sequence[_aws_cdk_aws_ecs_ceddda9d.EnvironmentFile]] = None,
+        essential: typing.Optional[builtins.bool] = None,
+        extra_hosts: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        gpu_count: typing.Optional[jsii.Number] = None,
+        health_check: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.HealthCheck, typing.Dict[builtins.str, typing.Any]]] = None,
+        hostname: typing.Optional[builtins.str] = None,
+        inference_accelerator_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
+        linux_parameters: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.LinuxParameters] = None,
+        logging: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.LogDriver] = None,
+        memory_limit_mib: typing.Optional[jsii.Number] = None,
+        memory_reservation_mib: typing.Optional[jsii.Number] = None,
+        port_mappings: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecs_ceddda9d.PortMapping, typing.Dict[builtins.str, typing.Any]]]] = None,
+        privileged: typing.Optional[builtins.bool] = None,
+        readonly_root_filesystem: typing.Optional[builtins.bool] = None,
+        secrets: typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_ecs_ceddda9d.Secret]] = None,
+        start_timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        stop_timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        system_controls: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecs_ceddda9d.SystemControl, typing.Dict[builtins.str, typing.Any]]]] = None,
+        user: typing.Optional[builtins.str] = None,
+        working_directory: typing.Optional[builtins.str] = None,
+    ) -> _aws_cdk_aws_ecs_ceddda9d.ContainerDefinitionOptions:
+        '''(experimental) This is a hook for modifying the container definition of any upstream containers.
+
+        This is primarily used for the main application container.
+        For example, the Firelens extension wants to be able to modify the logging
+        settings of the application container.
+
+        :param image: The image used to start a container. This string is passed directly to the Docker daemon. Images in the Docker Hub registry are available by default. Other repositories are specified with either repository-url/image:tag or repository-url/image@digest. TODO: Update these to specify using classes of IContainerImage
+        :param command: The command that is passed to the container. If you provide a shell command as a single string, you have to quote command-line arguments. Default: - CMD value built into container image.
+        :param container_name: The name of the container. Default: - id of node associated with ContainerDefinition.
+        :param cpu: The minimum number of CPU units to reserve for the container. Default: - No minimum CPU units reserved.
+        :param disable_networking: Specifies whether networking is disabled within the container. When this parameter is true, networking is disabled within the container. Default: false
+        :param dns_search_domains: A list of DNS search domains that are presented to the container. Default: - No search domains.
+        :param dns_servers: A list of DNS servers that are presented to the container. Default: - Default DNS servers.
+        :param docker_labels: A key/value map of labels to add to the container. Default: - No labels.
+        :param docker_security_options: A list of strings to provide custom labels for SELinux and AppArmor multi-level security systems. Default: - No security labels.
+        :param entry_point: The ENTRYPOINT value to pass to the container. Default: - Entry point configured in container.
+        :param environment: The environment variables to pass to the container. Default: - No environment variables.
+        :param environment_files: The environment files to pass to the container. Default: - No environment files.
+        :param essential: Specifies whether the container is marked essential. If the essential parameter of a container is marked as true, and that container fails or stops for any reason, all other containers that are part of the task are stopped. If the essential parameter of a container is marked as false, then its failure does not affect the rest of the containers in a task. All tasks must have at least one essential container. If this parameter is omitted, a container is assumed to be essential. Default: true
+        :param extra_hosts: A list of hostnames and IP address mappings to append to the /etc/hosts file on the container. Default: - No extra hosts.
+        :param gpu_count: The number of GPUs assigned to the container. Default: - No GPUs assigned.
+        :param health_check: The health check command and associated configuration parameters for the container. Default: - Health check configuration from container.
+        :param hostname: The hostname to use for your container. Default: - Automatic hostname.
+        :param inference_accelerator_resources: The inference accelerators referenced by the container. Default: - No inference accelerators assigned.
+        :param linux_parameters: Linux-specific modifications that are applied to the container, such as Linux kernel capabilities. For more information see `KernelCapabilities <https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_KernelCapabilities.html>`_. Default: - No Linux parameters.
+        :param logging: The log configuration specification for the container. Default: - Containers use the same logging driver that the Docker daemon uses.
+        :param memory_limit_mib: The amount (in MiB) of memory to present to the container. If your container attempts to exceed the allocated memory, the container is terminated. At least one of memoryLimitMiB and memoryReservationMiB is required for non-Fargate services. Default: - No memory limit.
+        :param memory_reservation_mib: The soft limit (in MiB) of memory to reserve for the container. When system memory is under heavy contention, Docker attempts to keep the container memory to this soft limit. However, your container can consume more memory when it needs to, up to either the hard limit specified with the memory parameter (if applicable), or all of the available memory on the container instance, whichever comes first. At least one of memoryLimitMiB and memoryReservationMiB is required for non-Fargate services. Default: - No memory reserved.
+        :param port_mappings: The port mappings to add to the container definition. Default: - No ports are mapped.
+        :param privileged: Specifies whether the container is marked as privileged. When this parameter is true, the container is given elevated privileges on the host container instance (similar to the root user). Default: false
+        :param readonly_root_filesystem: When this parameter is true, the container is given read-only access to its root file system. Default: false
+        :param secrets: The secret environment variables to pass to the container. Default: - No secret environment variables.
+        :param start_timeout: Time duration (in seconds) to wait before giving up on resolving dependencies for a container. Default: - none
+        :param stop_timeout: Time duration (in seconds) to wait before the container is forcefully killed if it doesn't exit normally on its own. Default: - none
+        :param system_controls: A list of namespaced kernel parameters to set in the container. Default: - No system controls are set.
+        :param user: The user name to use inside the container. Default: root
+        :param working_directory: The working directory in which to run commands inside the container. Default: /
+
+        :stability: experimental
+        '''
+        props = _aws_cdk_aws_ecs_ceddda9d.ContainerDefinitionOptions(
+            image=image,
+            command=command,
+            container_name=container_name,
+            cpu=cpu,
+            disable_networking=disable_networking,
+            dns_search_domains=dns_search_domains,
+            dns_servers=dns_servers,
+            docker_labels=docker_labels,
+            docker_security_options=docker_security_options,
+            entry_point=entry_point,
+            environment=environment,
+            environment_files=environment_files,
+            essential=essential,
+            extra_hosts=extra_hosts,
+            gpu_count=gpu_count,
+            health_check=health_check,
+            hostname=hostname,
+            inference_accelerator_resources=inference_accelerator_resources,
+            linux_parameters=linux_parameters,
+            logging=logging,
+            memory_limit_mib=memory_limit_mib,
+            memory_reservation_mib=memory_reservation_mib,
+            port_mappings=port_mappings,
+            privileged=privileged,
+            readonly_root_filesystem=readonly_root_filesystem,
+            secrets=secrets,
+            start_timeout=start_timeout,
+            stop_timeout=stop_timeout,
+            system_controls=system_controls,
+            user=user,
+            working_directory=working_directory,
+        )
+
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.ContainerDefinitionOptions, jsii.invoke(self, "mutateContainerDefinition", [props]))
+
+
 class AppMeshExtension(
     ServiceExtension,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk-containers/ecs-service-extensions.AppMeshExtension",
 ):
     '''(experimental) This extension adds an Envoy sidecar to the task definition and creates the App Mesh resources required to route network traffic to the container in a service mesh.
 
@@ -3536,15 +4135,15 @@
 
     :stability: experimental
     '''
 
     def __init__(
         self,
         *,
-        mesh: aws_cdk.aws_appmesh.Mesh,
+        mesh: _aws_cdk_aws_appmesh_ceddda9d.Mesh,
         protocol: typing.Optional[Protocol] = None,
     ) -> None:
         '''
         :param mesh: (experimental) The service mesh into which to register the service.
         :param protocol: (experimental) The protocol of the service. Valid values are Protocol.HTTP, Protocol.HTTP2, Protocol.TCP, Protocol.GRPC Default: - Protocol.HTTP
 
         :stability: experimental
@@ -3568,105 +4167,108 @@
 
         :param other_service: -
         :param local_bind_port: (experimental) localBindPort is the local port that this application should use when calling the upstream service in ECS Consul Mesh Extension Currently, this parameter will only be used in the ECSConsulMeshExtension https://github.com/aws-ia/ecs-consul-mesh-extension.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(AppMeshExtension.connect_to_service)
+            type_hints = typing.get_type_hints(_typecheckingstub__46aa6bb7020052c416acf790220f414bc6b66910844ccb7115c05c2109ffc6bf)
             check_type(argname="argument other_service", value=other_service, expected_type=type_hints["other_service"])
         _connect_to_props = ConnectToProps(local_bind_port=local_bind_port)
 
         return typing.cast(None, jsii.invoke(self, "connectToService", [other_service, _connect_to_props]))
 
     @jsii.member(jsii_name="modifyServiceProps")
     def modify_service_props(
         self,
         *,
-        cluster: aws_cdk.aws_ecs.ICluster,
-        task_definition: aws_cdk.aws_ecs.TaskDefinition,
+        cluster: _aws_cdk_aws_ecs_ceddda9d.ICluster,
+        task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
         assign_public_ip: typing.Optional[builtins.bool] = None,
-        cloud_map_options: typing.Optional[aws_cdk.aws_ecs.CloudMapOptions] = None,
+        cloud_map_options: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.CloudMapOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         desired_count: typing.Optional[jsii.Number] = None,
-        health_check_grace_period: typing.Optional[aws_cdk.Duration] = None,
+        health_check_grace_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         max_healthy_percent: typing.Optional[jsii.Number] = None,
         min_healthy_percent: typing.Optional[jsii.Number] = None,
+        service_connect_configuration: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.ServiceConnectProps, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> ServiceBuild:
         '''(experimental) Prior to launching the task definition as a service, this hook is called on each extension to give it a chance to mutate the properties of the service to be created.
 
         :param cluster: (experimental) The cluster in which to launch the service.
         :param task_definition: (experimental) The task definition registered to this service.
         :param assign_public_ip: (experimental) Specifies whether the task's elastic network interface receives a public IP address. If true, each task will receive a public IP address. Default: - false
         :param cloud_map_options: (experimental) Configuration for how to register the service in service discovery. Default: - No Cloud Map configured
         :param desired_count: (experimental) How many tasks to run. Default: - 1
         :param health_check_grace_period: (experimental) How long the healthcheck can fail during initial task startup before the task is considered unhealthy. This is used to give the task more time to start passing healthchecks. Default: - No grace period
         :param max_healthy_percent: (experimental) Maximum percentage of tasks that can be launched. Default: - 200
         :param min_healthy_percent: (experimental) Minimum healthy task percentage. Default: - 100
+        :param service_connect_configuration: (experimental) Configuration for service connect for this service. Default: - No Service Connect configured.
 
         :stability: experimental
         '''
         props = ServiceBuild(
             cluster=cluster,
             task_definition=task_definition,
             assign_public_ip=assign_public_ip,
             cloud_map_options=cloud_map_options,
             desired_count=desired_count,
             health_check_grace_period=health_check_grace_period,
             max_healthy_percent=max_healthy_percent,
             min_healthy_percent=min_healthy_percent,
+            service_connect_configuration=service_connect_configuration,
         )
 
         return typing.cast(ServiceBuild, jsii.invoke(self, "modifyServiceProps", [props]))
 
     @jsii.member(jsii_name="modifyTaskDefinitionProps")
     def modify_task_definition_props(
         self,
         *,
-        compatibility: aws_cdk.aws_ecs.Compatibility,
+        compatibility: _aws_cdk_aws_ecs_ceddda9d.Compatibility,
         cpu: typing.Optional[builtins.str] = None,
         ephemeral_storage_gib: typing.Optional[jsii.Number] = None,
-        inference_accelerators: typing.Optional[typing.Sequence[aws_cdk.aws_ecs.InferenceAccelerator]] = None,
-        ipc_mode: typing.Optional[aws_cdk.aws_ecs.IpcMode] = None,
+        inference_accelerators: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecs_ceddda9d.InferenceAccelerator, typing.Dict[builtins.str, typing.Any]]]] = None,
+        ipc_mode: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.IpcMode] = None,
         memory_mib: typing.Optional[builtins.str] = None,
-        network_mode: typing.Optional[aws_cdk.aws_ecs.NetworkMode] = None,
-        pid_mode: typing.Optional[aws_cdk.aws_ecs.PidMode] = None,
-        placement_constraints: typing.Optional[typing.Sequence[aws_cdk.aws_ecs.PlacementConstraint]] = None,
-        runtime_platform: typing.Optional[aws_cdk.aws_ecs.RuntimePlatform] = None,
-        execution_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
+        network_mode: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.NetworkMode] = None,
+        pid_mode: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.PidMode] = None,
+        placement_constraints: typing.Optional[typing.Sequence[_aws_cdk_aws_ecs_ceddda9d.PlacementConstraint]] = None,
+        runtime_platform: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.RuntimePlatform, typing.Dict[builtins.str, typing.Any]]] = None,
+        execution_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         family: typing.Optional[builtins.str] = None,
-        proxy_configuration: typing.Optional[aws_cdk.aws_ecs.ProxyConfiguration] = None,
-        task_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
-        volumes: typing.Optional[typing.Sequence[aws_cdk.aws_ecs.Volume]] = None,
-    ) -> aws_cdk.aws_ecs.TaskDefinitionProps:
+        proxy_configuration: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.ProxyConfiguration] = None,
+        task_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        volumes: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecs_ceddda9d.Volume, typing.Dict[builtins.str, typing.Any]]]] = None,
+    ) -> _aws_cdk_aws_ecs_ceddda9d.TaskDefinitionProps:
         '''(experimental) This is a hook which allows extensions to modify the settings of the task definition prior to it being created.
 
         For example, the App Mesh
         extension needs to configure an Envoy proxy in the task definition,
         or the Application extension wants to set the overall resource for
         the task.
 
         :param compatibility: The task launch type compatiblity requirement.
-        :param cpu: The number of cpu units used by the task. If you are using the EC2 launch type, this field is optional and any value can be used. If you are using the Fargate launch type, this field is required and you must use one of the following values, which determines your range of valid values for the memory parameter: 256 (.25 vCPU) - Available memory values: 512 (0.5 GB), 1024 (1 GB), 2048 (2 GB) 512 (.5 vCPU) - Available memory values: 1024 (1 GB), 2048 (2 GB), 3072 (3 GB), 4096 (4 GB) 1024 (1 vCPU) - Available memory values: 2048 (2 GB), 3072 (3 GB), 4096 (4 GB), 5120 (5 GB), 6144 (6 GB), 7168 (7 GB), 8192 (8 GB) 2048 (2 vCPU) - Available memory values: Between 4096 (4 GB) and 16384 (16 GB) in increments of 1024 (1 GB) 4096 (4 vCPU) - Available memory values: Between 8192 (8 GB) and 30720 (30 GB) in increments of 1024 (1 GB) Default: - CPU units are not specified.
+        :param cpu: The number of cpu units used by the task. If you are using the EC2 launch type, this field is optional and any value can be used. If you are using the Fargate launch type, this field is required and you must use one of the following values, which determines your range of valid values for the memory parameter: 256 (.25 vCPU) - Available memory values: 512 (0.5 GB), 1024 (1 GB), 2048 (2 GB) 512 (.5 vCPU) - Available memory values: 1024 (1 GB), 2048 (2 GB), 3072 (3 GB), 4096 (4 GB) 1024 (1 vCPU) - Available memory values: 2048 (2 GB), 3072 (3 GB), 4096 (4 GB), 5120 (5 GB), 6144 (6 GB), 7168 (7 GB), 8192 (8 GB) 2048 (2 vCPU) - Available memory values: Between 4096 (4 GB) and 16384 (16 GB) in increments of 1024 (1 GB) 4096 (4 vCPU) - Available memory values: Between 8192 (8 GB) and 30720 (30 GB) in increments of 1024 (1 GB) 8192 (8 vCPU) - Available memory values: Between 16384 (16 GB) and 61440 (60 GB) in increments of 4096 (4 GB) 16384 (16 vCPU) - Available memory values: Between 32768 (32 GB) and 122880 (120 GB) in increments of 8192 (8 GB) Default: - CPU units are not specified.
         :param ephemeral_storage_gib: The amount (in GiB) of ephemeral storage to be allocated to the task. Only supported in Fargate platform version 1.4.0 or later. Default: - Undefined, in which case, the task will receive 20GiB ephemeral storage.
         :param inference_accelerators: The inference accelerators to use for the containers in the task. Not supported in Fargate. Default: - No inference accelerators.
         :param ipc_mode: The IPC resource namespace to use for the containers in the task. Not supported in Fargate and Windows containers. Default: - IpcMode used by the task is not specified
-        :param memory_mib: The amount (in MiB) of memory used by the task. If using the EC2 launch type, this field is optional and any value can be used. If using the Fargate launch type, this field is required and you must use one of the following values, which determines your range of valid values for the cpu parameter: 512 (0.5 GB), 1024 (1 GB), 2048 (2 GB) - Available cpu values: 256 (.25 vCPU) 1024 (1 GB), 2048 (2 GB), 3072 (3 GB), 4096 (4 GB) - Available cpu values: 512 (.5 vCPU) 2048 (2 GB), 3072 (3 GB), 4096 (4 GB), 5120 (5 GB), 6144 (6 GB), 7168 (7 GB), 8192 (8 GB) - Available cpu values: 1024 (1 vCPU) Between 4096 (4 GB) and 16384 (16 GB) in increments of 1024 (1 GB) - Available cpu values: 2048 (2 vCPU) Between 8192 (8 GB) and 30720 (30 GB) in increments of 1024 (1 GB) - Available cpu values: 4096 (4 vCPU) Default: - Memory used by task is not specified.
+        :param memory_mib: The amount (in MiB) of memory used by the task. If using the EC2 launch type, this field is optional and any value can be used. If using the Fargate launch type, this field is required and you must use one of the following values, which determines your range of valid values for the cpu parameter: 512 (0.5 GB), 1024 (1 GB), 2048 (2 GB) - Available cpu values: 256 (.25 vCPU) 1024 (1 GB), 2048 (2 GB), 3072 (3 GB), 4096 (4 GB) - Available cpu values: 512 (.5 vCPU) 2048 (2 GB), 3072 (3 GB), 4096 (4 GB), 5120 (5 GB), 6144 (6 GB), 7168 (7 GB), 8192 (8 GB) - Available cpu values: 1024 (1 vCPU) Between 4096 (4 GB) and 16384 (16 GB) in increments of 1024 (1 GB) - Available cpu values: 2048 (2 vCPU) Between 8192 (8 GB) and 30720 (30 GB) in increments of 1024 (1 GB) - Available cpu values: 4096 (4 vCPU) Between 16384 (16 GB) and 61440 (60 GB) in increments of 4096 (4 GB) - Available cpu values: 8192 (8 vCPU) Between 32768 (32 GB) and 122880 (120 GB) in increments of 8192 (8 GB) - Available cpu values: 16384 (16 vCPU) Default: - Memory used by task is not specified.
         :param network_mode: The networking mode to use for the containers in the task. On Fargate, the only supported networking mode is AwsVpc. Default: - NetworkMode.Bridge for EC2 & External tasks, AwsVpc for Fargate tasks.
         :param pid_mode: The process namespace to use for the containers in the task. Not supported in Fargate and Windows containers. Default: - PidMode used by the task is not specified
         :param placement_constraints: The placement constraints to use for tasks in the service. You can specify a maximum of 10 constraints per task (this limit includes constraints in the task definition and those specified at run time). Not supported in Fargate. Default: - No placement constraints.
         :param runtime_platform: The operating system that your task definitions are running on. A runtimePlatform is supported only for tasks using the Fargate launch type. Default: - Undefined.
         :param execution_role: The name of the IAM task execution role that grants the ECS agent permission to call AWS APIs on your behalf. The role will be used to retrieve container images from ECR and create CloudWatch log groups. Default: - An execution role will be automatically created if you use ECR images in your task definition.
         :param family: The name of a family that this task definition is registered to. A family groups multiple versions of a task definition. Default: - Automatically generated name.
         :param proxy_configuration: The configuration details for the App Mesh proxy. Default: - No proxy configuration.
         :param task_role: The name of the IAM role that grants containers in the task permission to call AWS APIs on your behalf. Default: - A task role is automatically created for you.
         :param volumes: The list of volume definitions for the task. For more information, see `Task Definition Parameter Volumes <https://docs.aws.amazon.com/AmazonECS/latest/developerguide//task_definition_parameters.html#volumes>`_. Default: - No volumes are passed to the Docker daemon on a container instance.
 
         :stability: experimental
         '''
-        props = aws_cdk.aws_ecs.TaskDefinitionProps(
+        props = _aws_cdk_aws_ecs_ceddda9d.TaskDefinitionProps(
             compatibility=compatibility,
             cpu=cpu,
             ephemeral_storage_gib=ephemeral_storage_gib,
             inference_accelerators=inference_accelerators,
             ipc_mode=ipc_mode,
             memory_mib=memory_mib,
             network_mode=network_mode,
@@ -3676,134 +4278,140 @@
             execution_role=execution_role,
             family=family,
             proxy_configuration=proxy_configuration,
             task_role=task_role,
             volumes=volumes,
         )
 
-        return typing.cast(aws_cdk.aws_ecs.TaskDefinitionProps, jsii.invoke(self, "modifyTaskDefinitionProps", [props]))
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.TaskDefinitionProps, jsii.invoke(self, "modifyTaskDefinitionProps", [props]))
 
     @jsii.member(jsii_name="prehook")
-    def prehook(self, service: Service, scope: constructs.Construct) -> None:
+    def prehook(self, service: Service, scope: _constructs_77d1e7e8.Construct) -> None:
         '''(experimental) A hook that is called for each extension ahead of time to allow for any initial setup, such as creating resources in advance.
 
         :param service: -
         :param scope: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(AppMeshExtension.prehook)
+            type_hints = typing.get_type_hints(_typecheckingstub__b1b6f62b521bb2433821c150319d469dc1de71f54acbc0eeed2b5d8899969492)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
         return typing.cast(None, jsii.invoke(self, "prehook", [service, scope]))
 
     @jsii.member(jsii_name="useService")
     def use_service(
         self,
-        service: typing.Union[aws_cdk.aws_ecs.Ec2Service, aws_cdk.aws_ecs.FargateService],
+        service: typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService],
     ) -> None:
         '''(experimental) When this hook is implemented by extension, it allows the extension to use the service which has been created.
 
         It is generally used to
         create any final resources which might depend on the service itself.
 
         :param service: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(AppMeshExtension.use_service)
+            type_hints = typing.get_type_hints(_typecheckingstub__24ba92fd0ac0c816d12da606204e42c52685b9a00b8a9281497f2571d1e2e592)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
         return typing.cast(None, jsii.invoke(self, "useService", [service]))
 
     @jsii.member(jsii_name="useTaskDefinition")
     def use_task_definition(
         self,
-        task_definition: aws_cdk.aws_ecs.TaskDefinition,
+        task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
     ) -> None:
         '''(experimental) Once the task definition is created, this hook is called for each extension to give it a chance to add containers to the task definition, change the task definition's role to add permissions, etc.
 
         :param task_definition: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(AppMeshExtension.use_task_definition)
+            type_hints = typing.get_type_hints(_typecheckingstub__cf33dc4c9eb7ff891208bb61924a68ed4b4b593f76966a06f425ad88130bd43a)
             check_type(argname="argument task_definition", value=task_definition, expected_type=type_hints["task_definition"])
         return typing.cast(None, jsii.invoke(self, "useTaskDefinition", [task_definition]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="protocol")
     def protocol(self) -> Protocol:
         '''(experimental) The protocol used for AppMesh routing.
 
         default - Protocol.HTTP
 
         :stability: experimental
         '''
         return typing.cast(Protocol, jsii.get(self, "protocol"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="route")
-    def _route(self) -> aws_cdk.aws_appmesh.Route:
+    def _route(self) -> _aws_cdk_aws_appmesh_ceddda9d.Route:
         '''
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_appmesh.Route, jsii.get(self, "route"))
+        return typing.cast(_aws_cdk_aws_appmesh_ceddda9d.Route, jsii.get(self, "route"))
 
     @_route.setter
-    def _route(self, value: aws_cdk.aws_appmesh.Route) -> None:
+    def _route(self, value: _aws_cdk_aws_appmesh_ceddda9d.Route) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(getattr(AppMeshExtension, "_route").fset)
+            type_hints = typing.get_type_hints(_typecheckingstub__45282d066b0851dbef347c4ad1b08a63c9a6a9fd89bb9bab0d0344a37d51d7e0)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "route", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="virtualNode")
-    def _virtual_node(self) -> aws_cdk.aws_appmesh.VirtualNode:
+    def _virtual_node(self) -> _aws_cdk_aws_appmesh_ceddda9d.VirtualNode:
         '''
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_appmesh.VirtualNode, jsii.get(self, "virtualNode"))
+        return typing.cast(_aws_cdk_aws_appmesh_ceddda9d.VirtualNode, jsii.get(self, "virtualNode"))
 
     @_virtual_node.setter
-    def _virtual_node(self, value: aws_cdk.aws_appmesh.VirtualNode) -> None:
+    def _virtual_node(self, value: _aws_cdk_aws_appmesh_ceddda9d.VirtualNode) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(getattr(AppMeshExtension, "_virtual_node").fset)
+            type_hints = typing.get_type_hints(_typecheckingstub__5a5ea5a7d7c3e24afe0e0135e50a5e8582a8802d26297326e82b08535ed8db7d)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "virtualNode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="virtualRouter")
-    def _virtual_router(self) -> aws_cdk.aws_appmesh.VirtualRouter:
+    def _virtual_router(self) -> _aws_cdk_aws_appmesh_ceddda9d.VirtualRouter:
         '''
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_appmesh.VirtualRouter, jsii.get(self, "virtualRouter"))
+        return typing.cast(_aws_cdk_aws_appmesh_ceddda9d.VirtualRouter, jsii.get(self, "virtualRouter"))
 
     @_virtual_router.setter
-    def _virtual_router(self, value: aws_cdk.aws_appmesh.VirtualRouter) -> None:
+    def _virtual_router(
+        self,
+        value: _aws_cdk_aws_appmesh_ceddda9d.VirtualRouter,
+    ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(getattr(AppMeshExtension, "_virtual_router").fset)
+            type_hints = typing.get_type_hints(_typecheckingstub__2568f8d0e5d292fdf59d27fa103da5a8e7dcf882c1d57cdb4fb9bc163dd53968)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "virtualRouter", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="virtualService")
-    def _virtual_service(self) -> aws_cdk.aws_appmesh.VirtualService:
+    def _virtual_service(self) -> _aws_cdk_aws_appmesh_ceddda9d.VirtualService:
         '''
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_appmesh.VirtualService, jsii.get(self, "virtualService"))
+        return typing.cast(_aws_cdk_aws_appmesh_ceddda9d.VirtualService, jsii.get(self, "virtualService"))
 
     @_virtual_service.setter
-    def _virtual_service(self, value: aws_cdk.aws_appmesh.VirtualService) -> None:
+    def _virtual_service(
+        self,
+        value: _aws_cdk_aws_appmesh_ceddda9d.VirtualService,
+    ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(getattr(AppMeshExtension, "_virtual_service").fset)
+            type_hints = typing.get_type_hints(_typecheckingstub__557e91721e7f9fa56fe8c0aaed4a95b39f55db769264f9dfe1a37478a24c0cb5)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "virtualService", value)
 
 
 class AssignPublicIpExtension(
     ServiceExtension,
     metaclass=jsii.JSIIMeta,
@@ -3816,110 +4424,113 @@
 
     :stability: experimental
     '''
 
     def __init__(
         self,
         *,
-        dns: typing.Optional[AssignPublicIpDnsOptions] = None,
+        dns: typing.Optional[typing.Union[AssignPublicIpDnsOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param dns: (experimental) Enable publishing task public IPs to a recordset in a Route 53 hosted zone. Note: If you want to change the DNS zone or record name, you will need to remove this extension completely and then re-add it.
 
         :stability: experimental
         '''
         options = AssignPublicIpExtensionOptions(dns=dns)
 
         jsii.create(self.__class__, self, [options])
 
     @jsii.member(jsii_name="modifyServiceProps")
     def modify_service_props(
         self,
         *,
-        cluster: aws_cdk.aws_ecs.ICluster,
-        task_definition: aws_cdk.aws_ecs.TaskDefinition,
+        cluster: _aws_cdk_aws_ecs_ceddda9d.ICluster,
+        task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
         assign_public_ip: typing.Optional[builtins.bool] = None,
-        cloud_map_options: typing.Optional[aws_cdk.aws_ecs.CloudMapOptions] = None,
+        cloud_map_options: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.CloudMapOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         desired_count: typing.Optional[jsii.Number] = None,
-        health_check_grace_period: typing.Optional[aws_cdk.Duration] = None,
+        health_check_grace_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         max_healthy_percent: typing.Optional[jsii.Number] = None,
         min_healthy_percent: typing.Optional[jsii.Number] = None,
+        service_connect_configuration: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.ServiceConnectProps, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> ServiceBuild:
         '''(experimental) Prior to launching the task definition as a service, this hook is called on each extension to give it a chance to mutate the properties of the service to be created.
 
         :param cluster: (experimental) The cluster in which to launch the service.
         :param task_definition: (experimental) The task definition registered to this service.
         :param assign_public_ip: (experimental) Specifies whether the task's elastic network interface receives a public IP address. If true, each task will receive a public IP address. Default: - false
         :param cloud_map_options: (experimental) Configuration for how to register the service in service discovery. Default: - No Cloud Map configured
         :param desired_count: (experimental) How many tasks to run. Default: - 1
         :param health_check_grace_period: (experimental) How long the healthcheck can fail during initial task startup before the task is considered unhealthy. This is used to give the task more time to start passing healthchecks. Default: - No grace period
         :param max_healthy_percent: (experimental) Maximum percentage of tasks that can be launched. Default: - 200
         :param min_healthy_percent: (experimental) Minimum healthy task percentage. Default: - 100
+        :param service_connect_configuration: (experimental) Configuration for service connect for this service. Default: - No Service Connect configured.
 
         :stability: experimental
         '''
         props = ServiceBuild(
             cluster=cluster,
             task_definition=task_definition,
             assign_public_ip=assign_public_ip,
             cloud_map_options=cloud_map_options,
             desired_count=desired_count,
             health_check_grace_period=health_check_grace_period,
             max_healthy_percent=max_healthy_percent,
             min_healthy_percent=min_healthy_percent,
+            service_connect_configuration=service_connect_configuration,
         )
 
         return typing.cast(ServiceBuild, jsii.invoke(self, "modifyServiceProps", [props]))
 
     @jsii.member(jsii_name="prehook")
-    def prehook(self, service: Service, _scope: constructs.Construct) -> None:
+    def prehook(self, service: Service, _scope: _constructs_77d1e7e8.Construct) -> None:
         '''(experimental) A hook that is called for each extension ahead of time to allow for any initial setup, such as creating resources in advance.
 
         :param service: -
         :param _scope: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(AssignPublicIpExtension.prehook)
+            type_hints = typing.get_type_hints(_typecheckingstub__38ed1898de13597e3b7d93ee40ce523a890f585a491f671852960714fca854b9)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
             check_type(argname="argument _scope", value=_scope, expected_type=type_hints["_scope"])
         return typing.cast(None, jsii.invoke(self, "prehook", [service, _scope]))
 
     @jsii.member(jsii_name="useService")
     def use_service(
         self,
-        service: typing.Union[aws_cdk.aws_ecs.Ec2Service, aws_cdk.aws_ecs.FargateService],
+        service: typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService],
     ) -> None:
         '''(experimental) When this hook is implemented by extension, it allows the extension to use the service which has been created.
 
         It is generally used to
         create any final resources which might depend on the service itself.
 
         :param service: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(AssignPublicIpExtension.use_service)
+            type_hints = typing.get_type_hints(_typecheckingstub__0f2291ce04b362972e55218aa333ff0f9a122a5ea15c56cbb478a163c766c66d)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
         return typing.cast(None, jsii.invoke(self, "useService", [service]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dns")
     def dns(self) -> typing.Optional[AssignPublicIpDnsOptions]:
         '''
         :stability: experimental
         '''
         return typing.cast(typing.Optional[AssignPublicIpDnsOptions], jsii.get(self, "dns"))
 
     @dns.setter
     def dns(self, value: typing.Optional[AssignPublicIpDnsOptions]) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(getattr(AssignPublicIpExtension, "dns").fset)
+            type_hints = typing.get_type_hints(_typecheckingstub__2f90c2896c6abdd26969b3d38d54e26dc6e666b6c62b45540f048bb96e0d86c9)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dns", value)
 
 
 class CloudwatchAgentExtension(
     ServiceExtension,
     metaclass=jsii.JSIIMeta,
@@ -3933,24 +4544,24 @@
     def __init__(self) -> None:
         '''
         :stability: experimental
         '''
         jsii.create(self.__class__, self, [])
 
     @jsii.member(jsii_name="prehook")
-    def prehook(self, service: Service, scope: constructs.Construct) -> None:
+    def prehook(self, service: Service, scope: _constructs_77d1e7e8.Construct) -> None:
         '''(experimental) A hook that is called for each extension ahead of time to allow for any initial setup, such as creating resources in advance.
 
         :param service: -
         :param scope: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(CloudwatchAgentExtension.prehook)
+            type_hints = typing.get_type_hints(_typecheckingstub__077bc8d3188083769fa35aaf406ea73e7e9b53de59360a4febecb76aca3e8e02)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
         return typing.cast(None, jsii.invoke(self, "prehook", [service, scope]))
 
     @jsii.member(jsii_name="resolveContainerDependencies")
     def resolve_container_dependencies(self) -> None:
         '''(experimental) Once all containers are added to the task definition, this hook is called for each extension to give it a chance to resolve its dependency graph so that its container starts in the right order based on the other extensions that were enabled.
@@ -3958,24 +4569,24 @@
         :stability: experimental
         '''
         return typing.cast(None, jsii.invoke(self, "resolveContainerDependencies", []))
 
     @jsii.member(jsii_name="useTaskDefinition")
     def use_task_definition(
         self,
-        task_definition: aws_cdk.aws_ecs.TaskDefinition,
+        task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
     ) -> None:
         '''(experimental) Once the task definition is created, this hook is called for each extension to give it a chance to add containers to the task definition, change the task definition's role to add permissions, etc.
 
         :param task_definition: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(CloudwatchAgentExtension.use_task_definition)
+            type_hints = typing.get_type_hints(_typecheckingstub__cbde7e49a59cd7cc4d0cae1ae170cfed00a9cd120d6514ef8d2e21e07d37c2c8)
             check_type(argname="argument task_definition", value=task_definition, expected_type=type_hints["task_definition"])
         return typing.cast(None, jsii.invoke(self, "useTaskDefinition", [task_definition]))
 
 
 class Container(
     ServiceExtension,
     metaclass=jsii.JSIIMeta,
@@ -3990,87 +4601,93 @@
     :stability: experimental
     '''
 
     def __init__(
         self,
         *,
         cpu: jsii.Number,
-        image: aws_cdk.aws_ecs.ContainerImage,
+        image: _aws_cdk_aws_ecs_ceddda9d.ContainerImage,
         memory_mib: jsii.Number,
         traffic_port: jsii.Number,
         environment: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-        log_group: typing.Optional[aws_cdk.aws_logs.ILogGroup] = None,
+        environment_files: typing.Optional[typing.Sequence[_aws_cdk_aws_ecs_ceddda9d.EnvironmentFile]] = None,
+        log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
+        secrets: typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_ecs_ceddda9d.Secret]] = None,
     ) -> None:
         '''
         :param cpu: (experimental) How much CPU the container requires.
         :param image: (experimental) The image to run.
         :param memory_mib: (experimental) How much memory in megabytes the container requires.
         :param traffic_port: (experimental) What port the image listen for traffic on.
         :param environment: (experimental) Environment variables to pass into the container. Default: - No environment variables.
+        :param environment_files: (experimental) The environment files to pass to the container. Default: - No environment files.
         :param log_group: (experimental) The log group into which application container logs should be routed. Default: - A log group is automatically created for you if the ``ECS_SERVICE_EXTENSIONS_ENABLE_DEFAULT_LOG_DRIVER`` feature flag is set.
+        :param secrets: (experimental) The secret environment variables to pass to the container. Default: - No secret environment variables.
 
         :stability: experimental
         '''
         props = ContainerExtensionProps(
             cpu=cpu,
             image=image,
             memory_mib=memory_mib,
             traffic_port=traffic_port,
             environment=environment,
+            environment_files=environment_files,
             log_group=log_group,
+            secrets=secrets,
         )
 
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="modifyTaskDefinitionProps")
     def modify_task_definition_props(
         self,
         *,
-        compatibility: aws_cdk.aws_ecs.Compatibility,
+        compatibility: _aws_cdk_aws_ecs_ceddda9d.Compatibility,
         cpu: typing.Optional[builtins.str] = None,
         ephemeral_storage_gib: typing.Optional[jsii.Number] = None,
-        inference_accelerators: typing.Optional[typing.Sequence[aws_cdk.aws_ecs.InferenceAccelerator]] = None,
-        ipc_mode: typing.Optional[aws_cdk.aws_ecs.IpcMode] = None,
+        inference_accelerators: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecs_ceddda9d.InferenceAccelerator, typing.Dict[builtins.str, typing.Any]]]] = None,
+        ipc_mode: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.IpcMode] = None,
         memory_mib: typing.Optional[builtins.str] = None,
-        network_mode: typing.Optional[aws_cdk.aws_ecs.NetworkMode] = None,
-        pid_mode: typing.Optional[aws_cdk.aws_ecs.PidMode] = None,
-        placement_constraints: typing.Optional[typing.Sequence[aws_cdk.aws_ecs.PlacementConstraint]] = None,
-        runtime_platform: typing.Optional[aws_cdk.aws_ecs.RuntimePlatform] = None,
-        execution_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
+        network_mode: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.NetworkMode] = None,
+        pid_mode: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.PidMode] = None,
+        placement_constraints: typing.Optional[typing.Sequence[_aws_cdk_aws_ecs_ceddda9d.PlacementConstraint]] = None,
+        runtime_platform: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.RuntimePlatform, typing.Dict[builtins.str, typing.Any]]] = None,
+        execution_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         family: typing.Optional[builtins.str] = None,
-        proxy_configuration: typing.Optional[aws_cdk.aws_ecs.ProxyConfiguration] = None,
-        task_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
-        volumes: typing.Optional[typing.Sequence[aws_cdk.aws_ecs.Volume]] = None,
-    ) -> aws_cdk.aws_ecs.TaskDefinitionProps:
+        proxy_configuration: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.ProxyConfiguration] = None,
+        task_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        volumes: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecs_ceddda9d.Volume, typing.Dict[builtins.str, typing.Any]]]] = None,
+    ) -> _aws_cdk_aws_ecs_ceddda9d.TaskDefinitionProps:
         '''(experimental) This is a hook which allows extensions to modify the settings of the task definition prior to it being created.
 
         For example, the App Mesh
         extension needs to configure an Envoy proxy in the task definition,
         or the Application extension wants to set the overall resource for
         the task.
 
         :param compatibility: The task launch type compatiblity requirement.
-        :param cpu: The number of cpu units used by the task. If you are using the EC2 launch type, this field is optional and any value can be used. If you are using the Fargate launch type, this field is required and you must use one of the following values, which determines your range of valid values for the memory parameter: 256 (.25 vCPU) - Available memory values: 512 (0.5 GB), 1024 (1 GB), 2048 (2 GB) 512 (.5 vCPU) - Available memory values: 1024 (1 GB), 2048 (2 GB), 3072 (3 GB), 4096 (4 GB) 1024 (1 vCPU) - Available memory values: 2048 (2 GB), 3072 (3 GB), 4096 (4 GB), 5120 (5 GB), 6144 (6 GB), 7168 (7 GB), 8192 (8 GB) 2048 (2 vCPU) - Available memory values: Between 4096 (4 GB) and 16384 (16 GB) in increments of 1024 (1 GB) 4096 (4 vCPU) - Available memory values: Between 8192 (8 GB) and 30720 (30 GB) in increments of 1024 (1 GB) Default: - CPU units are not specified.
+        :param cpu: The number of cpu units used by the task. If you are using the EC2 launch type, this field is optional and any value can be used. If you are using the Fargate launch type, this field is required and you must use one of the following values, which determines your range of valid values for the memory parameter: 256 (.25 vCPU) - Available memory values: 512 (0.5 GB), 1024 (1 GB), 2048 (2 GB) 512 (.5 vCPU) - Available memory values: 1024 (1 GB), 2048 (2 GB), 3072 (3 GB), 4096 (4 GB) 1024 (1 vCPU) - Available memory values: 2048 (2 GB), 3072 (3 GB), 4096 (4 GB), 5120 (5 GB), 6144 (6 GB), 7168 (7 GB), 8192 (8 GB) 2048 (2 vCPU) - Available memory values: Between 4096 (4 GB) and 16384 (16 GB) in increments of 1024 (1 GB) 4096 (4 vCPU) - Available memory values: Between 8192 (8 GB) and 30720 (30 GB) in increments of 1024 (1 GB) 8192 (8 vCPU) - Available memory values: Between 16384 (16 GB) and 61440 (60 GB) in increments of 4096 (4 GB) 16384 (16 vCPU) - Available memory values: Between 32768 (32 GB) and 122880 (120 GB) in increments of 8192 (8 GB) Default: - CPU units are not specified.
         :param ephemeral_storage_gib: The amount (in GiB) of ephemeral storage to be allocated to the task. Only supported in Fargate platform version 1.4.0 or later. Default: - Undefined, in which case, the task will receive 20GiB ephemeral storage.
         :param inference_accelerators: The inference accelerators to use for the containers in the task. Not supported in Fargate. Default: - No inference accelerators.
         :param ipc_mode: The IPC resource namespace to use for the containers in the task. Not supported in Fargate and Windows containers. Default: - IpcMode used by the task is not specified
-        :param memory_mib: The amount (in MiB) of memory used by the task. If using the EC2 launch type, this field is optional and any value can be used. If using the Fargate launch type, this field is required and you must use one of the following values, which determines your range of valid values for the cpu parameter: 512 (0.5 GB), 1024 (1 GB), 2048 (2 GB) - Available cpu values: 256 (.25 vCPU) 1024 (1 GB), 2048 (2 GB), 3072 (3 GB), 4096 (4 GB) - Available cpu values: 512 (.5 vCPU) 2048 (2 GB), 3072 (3 GB), 4096 (4 GB), 5120 (5 GB), 6144 (6 GB), 7168 (7 GB), 8192 (8 GB) - Available cpu values: 1024 (1 vCPU) Between 4096 (4 GB) and 16384 (16 GB) in increments of 1024 (1 GB) - Available cpu values: 2048 (2 vCPU) Between 8192 (8 GB) and 30720 (30 GB) in increments of 1024 (1 GB) - Available cpu values: 4096 (4 vCPU) Default: - Memory used by task is not specified.
+        :param memory_mib: The amount (in MiB) of memory used by the task. If using the EC2 launch type, this field is optional and any value can be used. If using the Fargate launch type, this field is required and you must use one of the following values, which determines your range of valid values for the cpu parameter: 512 (0.5 GB), 1024 (1 GB), 2048 (2 GB) - Available cpu values: 256 (.25 vCPU) 1024 (1 GB), 2048 (2 GB), 3072 (3 GB), 4096 (4 GB) - Available cpu values: 512 (.5 vCPU) 2048 (2 GB), 3072 (3 GB), 4096 (4 GB), 5120 (5 GB), 6144 (6 GB), 7168 (7 GB), 8192 (8 GB) - Available cpu values: 1024 (1 vCPU) Between 4096 (4 GB) and 16384 (16 GB) in increments of 1024 (1 GB) - Available cpu values: 2048 (2 vCPU) Between 8192 (8 GB) and 30720 (30 GB) in increments of 1024 (1 GB) - Available cpu values: 4096 (4 vCPU) Between 16384 (16 GB) and 61440 (60 GB) in increments of 4096 (4 GB) - Available cpu values: 8192 (8 vCPU) Between 32768 (32 GB) and 122880 (120 GB) in increments of 8192 (8 GB) - Available cpu values: 16384 (16 vCPU) Default: - Memory used by task is not specified.
         :param network_mode: The networking mode to use for the containers in the task. On Fargate, the only supported networking mode is AwsVpc. Default: - NetworkMode.Bridge for EC2 & External tasks, AwsVpc for Fargate tasks.
         :param pid_mode: The process namespace to use for the containers in the task. Not supported in Fargate and Windows containers. Default: - PidMode used by the task is not specified
         :param placement_constraints: The placement constraints to use for tasks in the service. You can specify a maximum of 10 constraints per task (this limit includes constraints in the task definition and those specified at run time). Not supported in Fargate. Default: - No placement constraints.
         :param runtime_platform: The operating system that your task definitions are running on. A runtimePlatform is supported only for tasks using the Fargate launch type. Default: - Undefined.
         :param execution_role: The name of the IAM task execution role that grants the ECS agent permission to call AWS APIs on your behalf. The role will be used to retrieve container images from ECR and create CloudWatch log groups. Default: - An execution role will be automatically created if you use ECR images in your task definition.
         :param family: The name of a family that this task definition is registered to. A family groups multiple versions of a task definition. Default: - Automatically generated name.
         :param proxy_configuration: The configuration details for the App Mesh proxy. Default: - No proxy configuration.
         :param task_role: The name of the IAM role that grants containers in the task permission to call AWS APIs on your behalf. Default: - A task role is automatically created for you.
         :param volumes: The list of volume definitions for the task. For more information, see `Task Definition Parameter Volumes <https://docs.aws.amazon.com/AmazonECS/latest/developerguide//task_definition_parameters.html#volumes>`_. Default: - No volumes are passed to the Docker daemon on a container instance.
 
         :stability: experimental
         '''
-        props = aws_cdk.aws_ecs.TaskDefinitionProps(
+        props = _aws_cdk_aws_ecs_ceddda9d.TaskDefinitionProps(
             compatibility=compatibility,
             cpu=cpu,
             ephemeral_storage_gib=ephemeral_storage_gib,
             inference_accelerators=inference_accelerators,
             ipc_mode=ipc_mode,
             memory_mib=memory_mib,
             network_mode=network_mode,
@@ -4080,27 +4697,27 @@
             execution_role=execution_role,
             family=family,
             proxy_configuration=proxy_configuration,
             task_role=task_role,
             volumes=volumes,
         )
 
-        return typing.cast(aws_cdk.aws_ecs.TaskDefinitionProps, jsii.invoke(self, "modifyTaskDefinitionProps", [props]))
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.TaskDefinitionProps, jsii.invoke(self, "modifyTaskDefinitionProps", [props]))
 
     @jsii.member(jsii_name="prehook")
-    def prehook(self, service: Service, scope: constructs.Construct) -> None:
+    def prehook(self, service: Service, scope: _constructs_77d1e7e8.Construct) -> None:
         '''(experimental) A hook that is called for each extension ahead of time to allow for any initial setup, such as creating resources in advance.
 
         :param service: -
         :param scope: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(Container.prehook)
+            type_hints = typing.get_type_hints(_typecheckingstub__bf3fc5c42aa1818482bd8743e8f10ba77aaf61317153f1d97445a58428f36bfd)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
         return typing.cast(None, jsii.invoke(self, "prehook", [service, scope]))
 
     @jsii.member(jsii_name="resolveContainerDependencies")
     def resolve_container_dependencies(self) -> None:
         '''(experimental) Once all containers are added to the task definition, this hook is called for each extension to give it a chance to resolve its dependency graph so that its container starts in the right order based on the other extensions that were enabled.
@@ -4108,56 +4725,59 @@
         :stability: experimental
         '''
         return typing.cast(None, jsii.invoke(self, "resolveContainerDependencies", []))
 
     @jsii.member(jsii_name="useTaskDefinition")
     def use_task_definition(
         self,
-        task_definition: aws_cdk.aws_ecs.TaskDefinition,
+        task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
     ) -> None:
         '''(experimental) Once the task definition is created, this hook is called for each extension to give it a chance to add containers to the task definition, change the task definition's role to add permissions, etc.
 
         :param task_definition: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(Container.use_task_definition)
+            type_hints = typing.get_type_hints(_typecheckingstub__fbba7cbbc3927c630f737fd180e52eb90546a0dea499f24f8979548d012cdb6a)
             check_type(argname="argument task_definition", value=task_definition, expected_type=type_hints["task_definition"])
         return typing.cast(None, jsii.invoke(self, "useTaskDefinition", [task_definition]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="trafficPort")
     def traffic_port(self) -> jsii.Number:
         '''(experimental) The port on which the container expects to receive network traffic.
 
         :stability: experimental
         '''
         return typing.cast(jsii.Number, jsii.get(self, "trafficPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logGroup")
-    def log_group(self) -> typing.Optional[aws_cdk.aws_logs.ILogGroup]:
+    def log_group(self) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
         '''(experimental) The log group into which application container logs should be routed.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[aws_cdk.aws_logs.ILogGroup], jsii.get(self, "logGroup"))
+        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup], jsii.get(self, "logGroup"))
 
     @log_group.setter
-    def log_group(self, value: typing.Optional[aws_cdk.aws_logs.ILogGroup]) -> None:
+    def log_group(
+        self,
+        value: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup],
+    ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(getattr(Container, "log_group").fset)
+            type_hints = typing.get_type_hints(_typecheckingstub__5b56773bc13f3475e7efec07360704534718edfb3b9af5f22103e481189bef3f)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logGroup", value)
 
 
 @jsii.implements(IEnvironment)
 class Environment(
-    constructs.Construct,
+    _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk-containers/ecs-service-extensions.Environment",
 ):
     '''(experimental) An environment into which to deploy a service.
 
     This environment
     can either be instantiated with a pre-existing AWS VPC and ECS cluster,
@@ -4165,124 +4785,129 @@
     a cluster with Fargate capacity.
 
     :stability: experimental
     '''
 
     def __init__(
         self,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         capacity_type: typing.Optional[EnvironmentCapacityType] = None,
-        cluster: typing.Optional[aws_cdk.aws_ecs.Cluster] = None,
-        vpc: typing.Optional[aws_cdk.aws_ec2.IVpc] = None,
+        cluster: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.Cluster] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param capacity_type: (experimental) The type of capacity to use for this environment. Default: - EnvironmentCapacityType.FARGATE
         :param cluster: (experimental) The ECS cluster which provides compute capacity to this service. [disable-awslint:ref-via-interface] Default: - Create a new cluster
         :param vpc: (experimental) The VPC used by the service for networking. Default: - Create a new VPC
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(Environment.__init__)
+            type_hints = typing.get_type_hints(_typecheckingstub__79df512c816cd130c68fb458db12eca79849784c45022a670ceeb7656c517376)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = EnvironmentProps(capacity_type=capacity_type, cluster=cluster, vpc=vpc)
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromEnvironmentAttributes") # type: ignore[misc]
+    @jsii.member(jsii_name="fromEnvironmentAttributes")
     @builtins.classmethod
     def from_environment_attributes(
         cls,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         capacity_type: EnvironmentCapacityType,
-        cluster: aws_cdk.aws_ecs.ICluster,
+        cluster: _aws_cdk_aws_ecs_ceddda9d.ICluster,
     ) -> IEnvironment:
         '''(experimental) Import an existing environment from its attributes.
 
         :param scope: -
         :param id: -
         :param capacity_type: (experimental) The capacity type used by the service's cluster.
         :param cluster: (experimental) The cluster that is providing capacity for this service.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(Environment.from_environment_attributes)
+            type_hints = typing.get_type_hints(_typecheckingstub__032296542d572c6b398d9bf3c547056ab67cd1b9afdb7c038ad699976d18e3db)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         attrs = EnvironmentAttributes(capacity_type=capacity_type, cluster=cluster)
 
         return typing.cast(IEnvironment, jsii.sinvoke(cls, "fromEnvironmentAttributes", [scope, id, attrs]))
 
     @jsii.member(jsii_name="addDefaultCloudMapNamespace")
     def add_default_cloud_map_namespace(
         self,
         *,
         name: builtins.str,
-        type: typing.Optional[aws_cdk.aws_servicediscovery.NamespaceType] = None,
-        vpc: typing.Optional[aws_cdk.aws_ec2.IVpc] = None,
+        type: typing.Optional[_aws_cdk_aws_servicediscovery_ceddda9d.NamespaceType] = None,
+        use_for_service_connect: typing.Optional[builtins.bool] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''(experimental) Add a default cloudmap namespace to the environment's cluster.
 
         The environment's cluster must not be imported.
 
         :param name: The name of the namespace, such as example.com.
         :param type: The type of CloudMap Namespace to create. Default: PrivateDns
+        :param use_for_service_connect: This property specifies whether to set the provided namespace as the service connect default in the cluster properties. Default: false
         :param vpc: The VPC to associate the namespace with. This property is required for private DNS namespaces. Default: VPC of the cluster for Private DNS Namespace, otherwise none
 
         :stability: experimental
         '''
-        options = aws_cdk.aws_ecs.CloudMapNamespaceOptions(
-            name=name, type=type, vpc=vpc
+        options = _aws_cdk_aws_ecs_ceddda9d.CloudMapNamespaceOptions(
+            name=name,
+            type=type,
+            use_for_service_connect=use_for_service_connect,
+            vpc=vpc,
         )
 
         return typing.cast(None, jsii.invoke(self, "addDefaultCloudMapNamespace", [options]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="capacityType")
     def capacity_type(self) -> EnvironmentCapacityType:
         '''(experimental) The capacity type used by the service's cluster.
 
         :stability: experimental
         '''
         return typing.cast(EnvironmentCapacityType, jsii.get(self, "capacityType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cluster")
-    def cluster(self) -> aws_cdk.aws_ecs.ICluster:
+    def cluster(self) -> _aws_cdk_aws_ecs_ceddda9d.ICluster:
         '''(experimental) The cluster that is providing capacity for this service.
 
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_ecs.ICluster, jsii.get(self, "cluster"))
+        return typing.cast(_aws_cdk_aws_ecs_ceddda9d.ICluster, jsii.get(self, "cluster"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="id")
     def id(self) -> builtins.str:
         '''(experimental) The name of this environment.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "id"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpc")
-    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
+    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
         '''(experimental) The VPC where environment services should be placed.
 
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_ec2.IVpc, jsii.get(self, "vpc"))
+        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, jsii.get(self, "vpc"))
 
 
 class FireLensExtension(
     ServiceExtension,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk-containers/ecs-service-extensions.FireLensExtension",
 ):
@@ -4302,24 +4927,24 @@
         '''(experimental) A hook that allows the extension to add hooks to other extensions that are registered.
 
         :stability: experimental
         '''
         return typing.cast(None, jsii.invoke(self, "addHooks", []))
 
     @jsii.member(jsii_name="prehook")
-    def prehook(self, service: Service, scope: constructs.Construct) -> None:
+    def prehook(self, service: Service, scope: _constructs_77d1e7e8.Construct) -> None:
         '''(experimental) A hook that is called for each extension ahead of time to allow for any initial setup, such as creating resources in advance.
 
         :param service: -
         :param scope: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(FireLensExtension.prehook)
+            type_hints = typing.get_type_hints(_typecheckingstub__fc44db22afa05d01048722e48f64c16657acd6619ff44e75cd439cc75e743eb1)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
         return typing.cast(None, jsii.invoke(self, "prehook", [service, scope]))
 
     @jsii.member(jsii_name="resolveContainerDependencies")
     def resolve_container_dependencies(self) -> None:
         '''(experimental) Once all containers are added to the task definition, this hook is called for each extension to give it a chance to resolve its dependency graph so that its container starts in the right order based on the other extensions that were enabled.
@@ -4327,24 +4952,24 @@
         :stability: experimental
         '''
         return typing.cast(None, jsii.invoke(self, "resolveContainerDependencies", []))
 
     @jsii.member(jsii_name="useTaskDefinition")
     def use_task_definition(
         self,
-        task_definition: aws_cdk.aws_ecs.TaskDefinition,
+        task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
     ) -> None:
         '''(experimental) Once the task definition is created, this hook is called for each extension to give it a chance to add containers to the task definition, change the task definition's role to add permissions, etc.
 
         :param task_definition: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(FireLensExtension.use_task_definition)
+            type_hints = typing.get_type_hints(_typecheckingstub__26302b705de590e08625ea7201dd37b89ed5101384565fd0faf5199984ed9c46)
             check_type(argname="argument task_definition", value=task_definition, expected_type=type_hints["task_definition"])
         return typing.cast(None, jsii.invoke(self, "useTaskDefinition", [task_definition]))
 
 
 class HttpLoadBalancerExtension(
     ServiceExtension,
     metaclass=jsii.JSIIMeta,
@@ -4369,122 +4994,125 @@
 
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="modifyServiceProps")
     def modify_service_props(
         self,
         *,
-        cluster: aws_cdk.aws_ecs.ICluster,
-        task_definition: aws_cdk.aws_ecs.TaskDefinition,
+        cluster: _aws_cdk_aws_ecs_ceddda9d.ICluster,
+        task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
         assign_public_ip: typing.Optional[builtins.bool] = None,
-        cloud_map_options: typing.Optional[aws_cdk.aws_ecs.CloudMapOptions] = None,
+        cloud_map_options: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.CloudMapOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         desired_count: typing.Optional[jsii.Number] = None,
-        health_check_grace_period: typing.Optional[aws_cdk.Duration] = None,
+        health_check_grace_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         max_healthy_percent: typing.Optional[jsii.Number] = None,
         min_healthy_percent: typing.Optional[jsii.Number] = None,
+        service_connect_configuration: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.ServiceConnectProps, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> ServiceBuild:
         '''(experimental) Prior to launching the task definition as a service, this hook is called on each extension to give it a chance to mutate the properties of the service to be created.
 
         :param cluster: (experimental) The cluster in which to launch the service.
         :param task_definition: (experimental) The task definition registered to this service.
         :param assign_public_ip: (experimental) Specifies whether the task's elastic network interface receives a public IP address. If true, each task will receive a public IP address. Default: - false
         :param cloud_map_options: (experimental) Configuration for how to register the service in service discovery. Default: - No Cloud Map configured
         :param desired_count: (experimental) How many tasks to run. Default: - 1
         :param health_check_grace_period: (experimental) How long the healthcheck can fail during initial task startup before the task is considered unhealthy. This is used to give the task more time to start passing healthchecks. Default: - No grace period
         :param max_healthy_percent: (experimental) Maximum percentage of tasks that can be launched. Default: - 200
         :param min_healthy_percent: (experimental) Minimum healthy task percentage. Default: - 100
+        :param service_connect_configuration: (experimental) Configuration for service connect for this service. Default: - No Service Connect configured.
 
         :stability: experimental
         '''
         props = ServiceBuild(
             cluster=cluster,
             task_definition=task_definition,
             assign_public_ip=assign_public_ip,
             cloud_map_options=cloud_map_options,
             desired_count=desired_count,
             health_check_grace_period=health_check_grace_period,
             max_healthy_percent=max_healthy_percent,
             min_healthy_percent=min_healthy_percent,
+            service_connect_configuration=service_connect_configuration,
         )
 
         return typing.cast(ServiceBuild, jsii.invoke(self, "modifyServiceProps", [props]))
 
     @jsii.member(jsii_name="prehook")
-    def prehook(self, service: Service, scope: constructs.Construct) -> None:
+    def prehook(self, service: Service, scope: _constructs_77d1e7e8.Construct) -> None:
         '''(experimental) A hook that is called for each extension ahead of time to allow for any initial setup, such as creating resources in advance.
 
         :param service: -
         :param scope: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(HttpLoadBalancerExtension.prehook)
+            type_hints = typing.get_type_hints(_typecheckingstub__ed8391caad963614ec93d1a0d7e9d9747d62bf0d502b9ad5c4c57f654c5f7315)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
         return typing.cast(None, jsii.invoke(self, "prehook", [service, scope]))
 
     @jsii.member(jsii_name="useService")
     def use_service(
         self,
-        service: typing.Union[aws_cdk.aws_ecs.Ec2Service, aws_cdk.aws_ecs.FargateService],
+        service: typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService],
     ) -> None:
         '''(experimental) When this hook is implemented by extension, it allows the extension to use the service which has been created.
 
         It is generally used to
         create any final resources which might depend on the service itself.
 
         :param service: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(HttpLoadBalancerExtension.use_service)
+            type_hints = typing.get_type_hints(_typecheckingstub__5d2291e3a7f3e7948ea69040817ea11f3b4c2e634bcdd8ac8fb0199f4fe839bb)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
         return typing.cast(None, jsii.invoke(self, "useService", [service]))
 
 
 @jsii.interface(
     jsii_type="@aws-cdk-containers/ecs-service-extensions.IGrantInjectable"
 )
 class IGrantInjectable(IInjectable, typing_extensions.Protocol):
     '''(experimental) An interface that will be implemented by all the injectable resources that need to grant permissions to the task role.
 
     :stability: experimental
     '''
 
     @jsii.member(jsii_name="grant")
-    def grant(self, task_definition: aws_cdk.aws_ecs.TaskDefinition) -> None:
+    def grant(self, task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition) -> None:
         '''
         :param task_definition: -
 
         :stability: experimental
         '''
         ...
 
 
 class _IGrantInjectableProxy(
-    jsii.proxy_for(IInjectable) # type: ignore[misc]
+    jsii.proxy_for(IInjectable), # type: ignore[misc]
 ):
     '''(experimental) An interface that will be implemented by all the injectable resources that need to grant permissions to the task role.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk-containers/ecs-service-extensions.IGrantInjectable"
 
     @jsii.member(jsii_name="grant")
-    def grant(self, task_definition: aws_cdk.aws_ecs.TaskDefinition) -> None:
+    def grant(self, task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition) -> None:
         '''
         :param task_definition: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(IGrantInjectable.grant)
+            type_hints = typing.get_type_hints(_typecheckingstub__d5c9b77d6baabb5e5cb335d3b7b76d564d05a0a40856291a10a44c767bc2520b)
             check_type(argname="argument task_definition", value=task_definition, expected_type=type_hints["task_definition"])
         return typing.cast(None, jsii.invoke(self, "grant", [task_definition]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IGrantInjectable).__jsii_proxy_class__ = lambda : _IGrantInjectableProxy
 
 
@@ -4494,15 +5122,15 @@
     jsii_type="@aws-cdk-containers/ecs-service-extensions.InjectableTopic",
 ):
     '''(experimental) The ``InjectableTopic`` class represents SNS Topic resource that can be published events to by the parent service.
 
     :stability: experimental
     '''
 
-    def __init__(self, *, topic: aws_cdk.aws_sns.ITopic) -> None:
+    def __init__(self, *, topic: _aws_cdk_aws_sns_ceddda9d.ITopic) -> None:
         '''
         :param topic: (experimental) The SNS Topic to publish events to.
 
         :stability: experimental
         '''
         props = InjectableTopicProps(topic=topic)
 
@@ -4512,32 +5140,32 @@
     def environment_variables(self) -> typing.Mapping[builtins.str, builtins.str]:
         '''
         :stability: experimental
         '''
         return typing.cast(typing.Mapping[builtins.str, builtins.str], jsii.invoke(self, "environmentVariables", []))
 
     @jsii.member(jsii_name="grant")
-    def grant(self, task_definition: aws_cdk.aws_ecs.TaskDefinition) -> None:
+    def grant(self, task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition) -> None:
         '''
         :param task_definition: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(InjectableTopic.grant)
+            type_hints = typing.get_type_hints(_typecheckingstub__48c7f195f42f8e59cbbfa1cbbb92b61da9881c8a02edf111a97cd4db56e0e94a)
             check_type(argname="argument task_definition", value=task_definition, expected_type=type_hints["task_definition"])
         return typing.cast(None, jsii.invoke(self, "grant", [task_definition]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="topic")
-    def topic(self) -> aws_cdk.aws_sns.ITopic:
+    def topic(self) -> _aws_cdk_aws_sns_ceddda9d.ITopic:
         '''
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_sns.ITopic, jsii.get(self, "topic"))
+        return typing.cast(_aws_cdk_aws_sns_ceddda9d.ITopic, jsii.get(self, "topic"))
 
 
 class InjecterExtension(
     ServiceExtension,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk-containers/ecs-service-extensions.InjecterExtension",
 ):
@@ -4563,41 +5191,41 @@
         '''(experimental) Add hooks to the main application extension so that it is modified to add the injectable resource environment variables to the container environment.
 
         :stability: experimental
         '''
         return typing.cast(None, jsii.invoke(self, "addHooks", []))
 
     @jsii.member(jsii_name="prehook")
-    def prehook(self, service: Service, scope: constructs.Construct) -> None:
+    def prehook(self, service: Service, scope: _constructs_77d1e7e8.Construct) -> None:
         '''(experimental) A hook that is called for each extension ahead of time to allow for any initial setup, such as creating resources in advance.
 
         :param service: -
         :param scope: -
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(InjecterExtension.prehook)
+            type_hints = typing.get_type_hints(_typecheckingstub__ba812a9535025f034270daebc1bb1dcb1c0aa3ad083d9911e25dd4ed1bdd49dd)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
         return typing.cast(None, jsii.invoke(self, "prehook", [service, scope]))
 
     @jsii.member(jsii_name="useTaskDefinition")
     def use_task_definition(
         self,
-        task_definition: aws_cdk.aws_ecs.TaskDefinition,
+        task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
     ) -> None:
         '''(experimental) After the task definition has been created, this hook grants the required permissions to the task role for the parent service.
 
         :param task_definition: The created task definition.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(InjecterExtension.use_task_definition)
+            type_hints = typing.get_type_hints(_typecheckingstub__965f371f47a5e35e297c690ad4fd62e38130d0f53ddfa246cbd67b7e5a78ebd3)
             check_type(argname="argument task_definition", value=task_definition, expected_type=type_hints["task_definition"])
         return typing.cast(None, jsii.invoke(self, "useTaskDefinition", [task_definition]))
 
 
 class QueueExtension(
     ServiceExtension,
     metaclass=jsii.JSIIMeta,
@@ -4615,16 +5243,16 @@
 
     :stability: experimental
     '''
 
     def __init__(
         self,
         *,
-        events_queue: typing.Optional[aws_cdk.aws_sqs.IQueue] = None,
-        scale_on_latency: typing.Optional[QueueAutoScalingOptions] = None,
+        events_queue: typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue] = None,
+        scale_on_latency: typing.Optional[typing.Union[QueueAutoScalingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         subscriptions: typing.Optional[typing.Sequence[ISubscribable]] = None,
     ) -> None:
         '''
         :param events_queue: (experimental) The user-provided default queue for this service. If the ``eventsQueue`` is not provided, a default SQS Queue is created for the service. Default: none
         :param scale_on_latency: (experimental) The user-provided queue delay fields to configure auto scaling for the default queue. Default: none
         :param subscriptions: (experimental) The list of subscriptions for this service. Default: none
 
@@ -4643,96 +5271,99 @@
         '''(experimental) Add hooks to the main application extension so that it is modified to add the events queue URL to the container environment.
 
         :stability: experimental
         '''
         return typing.cast(None, jsii.invoke(self, "addHooks", []))
 
     @jsii.member(jsii_name="prehook")
-    def prehook(self, service: Service, scope: constructs.Construct) -> None:
+    def prehook(self, service: Service, scope: _constructs_77d1e7e8.Construct) -> None:
         '''(experimental) This hook creates (if required) and sets the default queue ``eventsQueue``.
 
         It also sets up the subscriptions for
         the provided ``ISubscribable`` objects.
 
         :param service: The parent service which this extension has been added to.
         :param scope: The scope that this extension should create resources in.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(QueueExtension.prehook)
+            type_hints = typing.get_type_hints(_typecheckingstub__9c2f5ee1195fd16f7e0ef20ecbd77d67b9fbafa0ecd9617a5e91a28ef3de4ced)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
         return typing.cast(None, jsii.invoke(self, "prehook", [service, scope]))
 
     @jsii.member(jsii_name="useService")
     def use_service(
         self,
-        service: typing.Union[aws_cdk.aws_ecs.Ec2Service, aws_cdk.aws_ecs.FargateService],
+        service: typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService],
     ) -> None:
         '''(experimental) When this hook is implemented by extension, it allows the extension to use the service which has been created.
 
         It is used to add target tracking
         scaling policies for the SQS Queues of the service. It also creates an AWS Lambda
         Function for calculating the backlog per task metric.
 
         :param service: - The generated service.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(QueueExtension.use_service)
+            type_hints = typing.get_type_hints(_typecheckingstub__1c33c510d93072d2b4ea0fcf0ba7fbae74143e371e7996c0e2805f9cf1a9af7c)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
         return typing.cast(None, jsii.invoke(self, "useService", [service]))
 
     @jsii.member(jsii_name="useTaskDefinition")
     def use_task_definition(
         self,
-        task_definition: aws_cdk.aws_ecs.TaskDefinition,
+        task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
     ) -> None:
         '''(experimental) After the task definition has been created, this hook grants SQS permissions to the task role.
 
         :param task_definition: The created task definition.
 
         :stability: experimental
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(QueueExtension.use_task_definition)
+            type_hints = typing.get_type_hints(_typecheckingstub__994a45034920765ebf187cd6c2f9dd5d5d81863eb6a995f3f6c09b1d1ef8cce1)
             check_type(argname="argument task_definition", value=task_definition, expected_type=type_hints["task_definition"])
         return typing.cast(None, jsii.invoke(self, "useTaskDefinition", [task_definition]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="eventsQueue")
-    def events_queue(self) -> aws_cdk.aws_sqs.IQueue:
+    def events_queue(self) -> _aws_cdk_aws_sqs_ceddda9d.IQueue:
         '''
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_sqs.IQueue, jsii.get(self, "eventsQueue"))
+        return typing.cast(_aws_cdk_aws_sqs_ceddda9d.IQueue, jsii.get(self, "eventsQueue"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoscalingOptions")
     def autoscaling_options(self) -> typing.Optional[QueueAutoScalingOptions]:
         '''
         :stability: experimental
         '''
         return typing.cast(typing.Optional[QueueAutoScalingOptions], jsii.get(self, "autoscalingOptions"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logGroup")
-    def log_group(self) -> typing.Optional[aws_cdk.aws_logs.ILogGroup]:
+    def log_group(self) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
         '''(experimental) The log group created by the extension where the AWS Lambda function logs are stored.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[aws_cdk.aws_logs.ILogGroup], jsii.get(self, "logGroup"))
+        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup], jsii.get(self, "logGroup"))
 
     @log_group.setter
-    def log_group(self, value: typing.Optional[aws_cdk.aws_logs.ILogGroup]) -> None:
+    def log_group(
+        self,
+        value: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup],
+    ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(getattr(QueueExtension, "log_group").fset)
+            type_hints = typing.get_type_hints(_typecheckingstub__6e381a94b8fd01616977d82ea065a59158d8c683625e4200204ab6cae2823a5e)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logGroup", value)
 
 
 class ScaleOnCpuUtilization(
     ServiceExtension,
     metaclass=jsii.JSIIMeta,
@@ -4750,16 +5381,16 @@
 
     def __init__(
         self,
         *,
         initial_task_count: typing.Optional[jsii.Number] = None,
         max_task_count: typing.Optional[jsii.Number] = None,
         min_task_count: typing.Optional[jsii.Number] = None,
-        scale_in_cooldown: typing.Optional[aws_cdk.Duration] = None,
-        scale_out_cooldown: typing.Optional[aws_cdk.Duration] = None,
+        scale_in_cooldown: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        scale_out_cooldown: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         target_cpu_utilization: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
         :param initial_task_count: (deprecated) How many tasks to launch initially. Default: - 2
         :param max_task_count: (deprecated) The maximum number of tasks when scaling out. Default: - 8
         :param min_task_count: (deprecated) The minimum number of tasks when scaling in. Default: - 2
         :param scale_in_cooldown: (deprecated) How long to wait between scale in actions. Default: - 60 seconds
@@ -4779,124 +5410,131 @@
 
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="modifyServiceProps")
     def modify_service_props(
         self,
         *,
-        cluster: aws_cdk.aws_ecs.ICluster,
-        task_definition: aws_cdk.aws_ecs.TaskDefinition,
+        cluster: _aws_cdk_aws_ecs_ceddda9d.ICluster,
+        task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
         assign_public_ip: typing.Optional[builtins.bool] = None,
-        cloud_map_options: typing.Optional[aws_cdk.aws_ecs.CloudMapOptions] = None,
+        cloud_map_options: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.CloudMapOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         desired_count: typing.Optional[jsii.Number] = None,
-        health_check_grace_period: typing.Optional[aws_cdk.Duration] = None,
+        health_check_grace_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         max_healthy_percent: typing.Optional[jsii.Number] = None,
         min_healthy_percent: typing.Optional[jsii.Number] = None,
+        service_connect_configuration: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.ServiceConnectProps, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> ServiceBuild:
         '''(deprecated) Prior to launching the task definition as a service, this hook is called on each extension to give it a chance to mutate the properties of the service to be created.
 
         :param cluster: (experimental) The cluster in which to launch the service.
         :param task_definition: (experimental) The task definition registered to this service.
         :param assign_public_ip: (experimental) Specifies whether the task's elastic network interface receives a public IP address. If true, each task will receive a public IP address. Default: - false
         :param cloud_map_options: (experimental) Configuration for how to register the service in service discovery. Default: - No Cloud Map configured
         :param desired_count: (experimental) How many tasks to run. Default: - 1
         :param health_check_grace_period: (experimental) How long the healthcheck can fail during initial task startup before the task is considered unhealthy. This is used to give the task more time to start passing healthchecks. Default: - No grace period
         :param max_healthy_percent: (experimental) Maximum percentage of tasks that can be launched. Default: - 200
         :param min_healthy_percent: (experimental) Minimum healthy task percentage. Default: - 100
+        :param service_connect_configuration: (experimental) Configuration for service connect for this service. Default: - No Service Connect configured.
 
         :stability: deprecated
         '''
         props = ServiceBuild(
             cluster=cluster,
             task_definition=task_definition,
             assign_public_ip=assign_public_ip,
             cloud_map_options=cloud_map_options,
             desired_count=desired_count,
             health_check_grace_period=health_check_grace_period,
             max_healthy_percent=max_healthy_percent,
             min_healthy_percent=min_healthy_percent,
+            service_connect_configuration=service_connect_configuration,
         )
 
         return typing.cast(ServiceBuild, jsii.invoke(self, "modifyServiceProps", [props]))
 
     @jsii.member(jsii_name="useService")
     def use_service(
         self,
-        service: typing.Union[aws_cdk.aws_ecs.Ec2Service, aws_cdk.aws_ecs.FargateService],
+        service: typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService],
     ) -> None:
         '''(deprecated) When this hook is implemented by extension, it allows the extension to use the service which has been created.
 
         It is generally used to
         create any final resources which might depend on the service itself.
 
         :param service: -
 
         :stability: deprecated
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(ScaleOnCpuUtilization.use_service)
+            type_hints = typing.get_type_hints(_typecheckingstub__3cee1d52046f25f6baf6e7092422c633ee0e1b80c82bc9313467d3eea1800a1f)
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
         return typing.cast(None, jsii.invoke(self, "useService", [service]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="initialTaskCount")
     def initial_task_count(self) -> jsii.Number:
         '''(deprecated) How many tasks to launch initially.
 
         :stability: deprecated
         '''
         return typing.cast(jsii.Number, jsii.get(self, "initialTaskCount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maxTaskCount")
     def max_task_count(self) -> jsii.Number:
         '''(deprecated) The maximum number of tasks when scaling out.
 
         :stability: deprecated
         '''
         return typing.cast(jsii.Number, jsii.get(self, "maxTaskCount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="minTaskCount")
     def min_task_count(self) -> jsii.Number:
         '''(deprecated) The minimum number of tasks when scaling in.
 
         :stability: deprecated
         '''
         return typing.cast(jsii.Number, jsii.get(self, "minTaskCount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scaleInCooldown")
-    def scale_in_cooldown(self) -> aws_cdk.Duration:
+    def scale_in_cooldown(self) -> _aws_cdk_ceddda9d.Duration:
         '''(deprecated) How long to wait between scale in actions.
 
         :stability: deprecated
         '''
-        return typing.cast(aws_cdk.Duration, jsii.get(self, "scaleInCooldown"))
+        return typing.cast(_aws_cdk_ceddda9d.Duration, jsii.get(self, "scaleInCooldown"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scaleOutCooldown")
-    def scale_out_cooldown(self) -> aws_cdk.Duration:
+    def scale_out_cooldown(self) -> _aws_cdk_ceddda9d.Duration:
         '''(deprecated) How long to wait between scale out actions.
 
         :stability: deprecated
         '''
-        return typing.cast(aws_cdk.Duration, jsii.get(self, "scaleOutCooldown"))
+        return typing.cast(_aws_cdk_ceddda9d.Duration, jsii.get(self, "scaleOutCooldown"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="targetCpuUtilization")
     def target_cpu_utilization(self) -> jsii.Number:
         '''(deprecated) The CPU utilization to try ot maintain.
 
         :stability: deprecated
         '''
         return typing.cast(jsii.Number, jsii.get(self, "targetCpuUtilization"))
 
 
 __all__ = [
+    "AliasedPortExtension",
+    "AliasedPortMutatingHook",
+    "AliasedPortMutatingHookProps",
+    "AliasedPortProps",
     "AppMeshExtension",
     "AssignPublicIpDnsOptions",
     "AssignPublicIpExtension",
     "AssignPublicIpExtensionOptions",
     "AutoScalingOptions",
     "CloudwatchAgentExtension",
     "ConnectToProps",
@@ -4936,7 +5574,607 @@
     "SubscriptionQueue",
     "TopicSubscription",
     "TopicSubscriptionProps",
     "XRayExtension",
 ]
 
 publication.publish()
+
+def _typecheckingstub__9eafc8bc30298b419ba1305209f1f31afbf65c9b3456fc2c643e9dc4c1bd501a(
+    *,
+    alias_port: jsii.Number,
+    port_mapping_name: builtins.str,
+    protocol: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.AppProtocol] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7d89a6c579317235d028edb793a72ba2e7d3ccda1e4b1f2602503eea428e930c(
+    *,
+    alias: builtins.str,
+    alias_port: typing.Optional[jsii.Number] = None,
+    app_protocol: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.AppProtocol] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__fa7fb8b6574fcc7a10ce0f47113796062053fc86dbd682d2487f7cdfb34d46d0(
+    *,
+    record_name: builtins.str,
+    zone: _aws_cdk_aws_route53_ceddda9d.IHostedZone,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__2deb6349e9cd894776e0a60628761c1ec58ee4da5eb9e508b90d05cf30b34874(
+    *,
+    dns: typing.Optional[typing.Union[AssignPublicIpDnsOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__caf95230f9a127a46aef16659b3a944e6851420921875acc492c4a7722ded929(
+    *,
+    max_task_count: jsii.Number,
+    min_task_count: typing.Optional[jsii.Number] = None,
+    target_cpu_utilization: typing.Optional[jsii.Number] = None,
+    target_memory_utilization: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__20e37174ab201a5eb1d201637ac0c651f7361afe5cb95a69d57aeed17fde4cc3(
+    *,
+    local_bind_port: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__592d522da39571a2b2a1780c28b1405f8f98b2f7ae4b9ff881cf256a8d3941d3(
+    *,
+    cpu: jsii.Number,
+    image: _aws_cdk_aws_ecs_ceddda9d.ContainerImage,
+    memory_mib: jsii.Number,
+    traffic_port: jsii.Number,
+    environment: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    environment_files: typing.Optional[typing.Sequence[_aws_cdk_aws_ecs_ceddda9d.EnvironmentFile]] = None,
+    log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
+    secrets: typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_ecs_ceddda9d.Secret]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__da64dd40c2eed49a661888472ad447cdd50d0d1de54b035c25e482f09c6e8d50(
+    *,
+    initial_task_count: typing.Optional[jsii.Number] = None,
+    max_task_count: typing.Optional[jsii.Number] = None,
+    min_task_count: typing.Optional[jsii.Number] = None,
+    scale_in_cooldown: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+    scale_out_cooldown: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+    target_cpu_utilization: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3972ae1eaa225a4a8fa626d5b9ec3fc0b64c420599bc3a5f3dd1d2aec30cfd77(
+    *,
+    capacity_type: EnvironmentCapacityType,
+    cluster: _aws_cdk_aws_ecs_ceddda9d.ICluster,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4f994193a0844d1feecc18424b7d4cb07ff8d4ed7fb514183a12bd56930e922b(
+    *,
+    capacity_type: typing.Optional[EnvironmentCapacityType] = None,
+    cluster: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.Cluster] = None,
+    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__aceb6633b315022d8687596bd75918bf27f97bab07b5afe71b5de85deefef59c(
+    *,
+    log_group: _aws_cdk_aws_logs_ceddda9d.LogGroup,
+    parent_service: Service,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__82df5b77ad12b766d5e63af5b466f4e55ce579599801b70669df556201e35c2c(
+    *,
+    requests_per_target: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__cd1578190a97094d760d76a2f5cebe69df504113964828b89844073359391cb5(
+    extension: QueueExtension,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__91378335a3876039a3828c1245b7393e5a1292ba2a049277f1c28e0986b15b07(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    capacity_type: EnvironmentCapacityType,
+    cluster: _aws_cdk_aws_ecs_ceddda9d.ICluster,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__5404fdd3e63bd485e4db5b2a113ebf7494d35cf4a96f038e9defb7d051989a59(
+    *,
+    topic: _aws_cdk_aws_sns_ceddda9d.ITopic,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__764a4ce423345733d9211ae0ec978efe2db85a96e72389375cfe172603235a12(
+    *,
+    injectables: typing.Sequence[IInjectable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__142846b40345638745bc1a3ab27f3cab5f854bdaf8ca3b69b33a43f481fd5f56(
+    *,
+    mesh: _aws_cdk_aws_appmesh_ceddda9d.Mesh,
+    protocol: typing.Optional[Protocol] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a69b597f7f7ad40eda264d309c915a018cfc7e08a24d4fd3431b480aebba63ba(
+    *,
+    acceptable_latency: _aws_cdk_ceddda9d.Duration,
+    message_processing_time: _aws_cdk_ceddda9d.Duration,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b4718a77605fed94d29789c1a434b9fcc1ae492a2a3de2712231624c092820cb(
+    *,
+    events_queue: typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue] = None,
+    scale_on_latency: typing.Optional[typing.Union[QueueAutoScalingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    subscriptions: typing.Optional[typing.Sequence[ISubscribable]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__db3cb686a45270fdd7e768c5ae18b4f4f6f2162d2173f63f7c535361b5a43ee0(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    environment: IEnvironment,
+    service_description: ServiceDescription,
+    auto_scale_task_count: typing.Optional[typing.Union[AutoScalingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    desired_count: typing.Optional[jsii.Number] = None,
+    task_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__502b75d7c9b239a450ef6b60bf75138f9e9ad1bf1db3c86bae3750bb5b2ddb85(
+    url_name: builtins.str,
+    url: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__74fb3efae7913ceb8ccea9c9b3493498efca8dbd55fc5e00f7140f8a17ed89a9(
+    service: Service,
+    *,
+    local_bind_port: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0f9661ad5046e27393ad9a87be136fc5dff0e8a0c90ab0d53f12343c56b38af2(
+    url_name: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__48e0b209d664b802d972b8c57029dfafa732ddd80d7f15177ec1c19fa4ee27e4(
+    value: typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__43501a7df8adf21fb5b2baed0861c8d54532787b41d74a178e59fb2f8d7cb4c7(
+    value: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ee366325f772dd64ac0fb090f415241df9c08abd4c10129d4accf09912d2ae3f(
+    value: typing.Optional[_aws_cdk_aws_elasticloadbalancingv2_ceddda9d.ApplicationTargetGroup],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__bbc157cc76350e79845bf03bad3f7df149e831066f26c4ce897b5f0aa26318c9(
+    *,
+    cluster: _aws_cdk_aws_ecs_ceddda9d.ICluster,
+    task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
+    assign_public_ip: typing.Optional[builtins.bool] = None,
+    cloud_map_options: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.CloudMapOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    desired_count: typing.Optional[jsii.Number] = None,
+    health_check_grace_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+    max_healthy_percent: typing.Optional[jsii.Number] = None,
+    min_healthy_percent: typing.Optional[jsii.Number] = None,
+    service_connect_configuration: typing.Optional[typing.Union[_aws_cdk_aws_ecs_ceddda9d.ServiceConnectProps, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__c093f5c31129726d3d125fea26e2c3fd91a85698eb1ba8473769eac664ab595a(
+    extension: ServiceExtension,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8352914d442a0691483353eb819f6ab07a7c3906ffcb4a5f205881cab8855693(
+    name: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__f3cc49fbfe806b68e28897ef0a6adb82ef13ea662595a6dc16cfbd1c8f3d80ff(
+    value: typing.Mapping[builtins.str, ServiceExtension],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__1942fe00f761e2c51266b2c817c5520489ca4dfc5fb00a8121bfc670fbf52e3f(
+    name: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__67016c4360f564fd4fe54d7d2b5edd75e564f902aee57e11136af32477ecb5c5(
+    hook: ContainerMutatingHook,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8e2d8de0dbe555c1e1b7b50b5b988162b03bc53d683e2a98a1659e95e6b1180c(
+    service: Service,
+    *,
+    local_bind_port: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__eefdf655cd0e7f30d0fcf6f77a6d8729245c20be4605fa83182a750656dd59de(
+    parent: Service,
+    scope: _constructs_77d1e7e8.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__38e3e0860e30eb48b790e6fc0840c9d9d36bff02f4ab4e976e145f4f85ef048d(
+    service: typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e93694c5c40f28677d9914773fe2949cbdf32f19f86771a0f343852c4a456833(
+    task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__299f56627660a08293011eb309421e4c9ecab06a492c5135e001bb57465be12a(
+    value: typing.List[ContainerMutatingHook],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ffd5c720e9e1800e56e330f06b53101d51e941eae8399ed18a6ce3469d004a45(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__888537d4e44499688ac07459949d868e9b29b5f5b71d885c9f28d9f42d26a293(
+    value: Service,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__22b87c7ca09e39c9e04f952a479384b276834e484577d808867f6e8cd36eae87(
+    value: _constructs_77d1e7e8.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__54f71fbef259bce4d04ac1599a7734f8470b603b265ce3c405992e7d9403cc63(
+    value: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.ContainerDefinition],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8324f912a77ba2380fbec2194e091c70e44826a63d04c9b3b3178db416008d54(
+    *,
+    environment: IEnvironment,
+    service_description: ServiceDescription,
+    auto_scale_task_count: typing.Optional[typing.Union[AutoScalingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    desired_count: typing.Optional[jsii.Number] = None,
+    task_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__2ab599485b374c44897ab0ae8820090231221b727f0f9968276a4071085689df(
+    *,
+    queue: _aws_cdk_aws_sqs_ceddda9d.IQueue,
+    scale_on_latency: typing.Optional[typing.Union[QueueAutoScalingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__542dd993b9b30463def0028989d7fe8b3f0f9e422cb20bea69ab3b83367fbdb4(
+    extension: QueueExtension,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__6ce31ca30734748c8286306049838377fd0ae5237a93f44655e549a682baaf92(
+    *,
+    topic: _aws_cdk_aws_sns_ceddda9d.ITopic,
+    queue: typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue] = None,
+    topic_subscription_queue: typing.Optional[typing.Union[SubscriptionQueue, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a25c259153e7aabb24a4f343378b533b165fcb42b53180b3fdd7f72da6371ad2(
+    service: Service,
+    scope: _constructs_77d1e7e8.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__02d9f8aa0fd942e4f491eeddab502c60a5a201811637d732a37f9d950cb67311(
+    task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__1043b521b7d8a62b95b2d33c980009a15390b055b8b23fb3fa89a4601d987fbe(
+    service: Service,
+    scope: _constructs_77d1e7e8.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0d404dfff99916347cd236463a68228c5807d4e62df7247b71f3de0207b4ecdb(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__69dab24a138f3970d3fecdca97edefcacb2ca2b0f643129d3cda322bcb9be285(
+    value: typing.Optional[jsii.Number],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e54f461371069afdb909684795279f736b187cc7fb5b7ef682d1fb827a6b0846(
+    value: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.AppProtocol],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0681b9db0238b5ddb0fd915e2a2f44cec1c3d21ec400322498e8bfe207d0f483(
+    value: typing.Optional[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__46aa6bb7020052c416acf790220f414bc6b66910844ccb7115c05c2109ffc6bf(
+    other_service: Service,
+    *,
+    local_bind_port: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b1b6f62b521bb2433821c150319d469dc1de71f54acbc0eeed2b5d8899969492(
+    service: Service,
+    scope: _constructs_77d1e7e8.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__24ba92fd0ac0c816d12da606204e42c52685b9a00b8a9281497f2571d1e2e592(
+    service: typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__cf33dc4c9eb7ff891208bb61924a68ed4b4b593f76966a06f425ad88130bd43a(
+    task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__45282d066b0851dbef347c4ad1b08a63c9a6a9fd89bb9bab0d0344a37d51d7e0(
+    value: _aws_cdk_aws_appmesh_ceddda9d.Route,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__5a5ea5a7d7c3e24afe0e0135e50a5e8582a8802d26297326e82b08535ed8db7d(
+    value: _aws_cdk_aws_appmesh_ceddda9d.VirtualNode,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__2568f8d0e5d292fdf59d27fa103da5a8e7dcf882c1d57cdb4fb9bc163dd53968(
+    value: _aws_cdk_aws_appmesh_ceddda9d.VirtualRouter,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__557e91721e7f9fa56fe8c0aaed4a95b39f55db769264f9dfe1a37478a24c0cb5(
+    value: _aws_cdk_aws_appmesh_ceddda9d.VirtualService,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__38ed1898de13597e3b7d93ee40ce523a890f585a491f671852960714fca854b9(
+    service: Service,
+    _scope: _constructs_77d1e7e8.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0f2291ce04b362972e55218aa333ff0f9a122a5ea15c56cbb478a163c766c66d(
+    service: typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__2f90c2896c6abdd26969b3d38d54e26dc6e666b6c62b45540f048bb96e0d86c9(
+    value: typing.Optional[AssignPublicIpDnsOptions],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__077bc8d3188083769fa35aaf406ea73e7e9b53de59360a4febecb76aca3e8e02(
+    service: Service,
+    scope: _constructs_77d1e7e8.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__cbde7e49a59cd7cc4d0cae1ae170cfed00a9cd120d6514ef8d2e21e07d37c2c8(
+    task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__bf3fc5c42aa1818482bd8743e8f10ba77aaf61317153f1d97445a58428f36bfd(
+    service: Service,
+    scope: _constructs_77d1e7e8.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__fbba7cbbc3927c630f737fd180e52eb90546a0dea499f24f8979548d012cdb6a(
+    task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__5b56773bc13f3475e7efec07360704534718edfb3b9af5f22103e481189bef3f(
+    value: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__79df512c816cd130c68fb458db12eca79849784c45022a670ceeb7656c517376(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    capacity_type: typing.Optional[EnvironmentCapacityType] = None,
+    cluster: typing.Optional[_aws_cdk_aws_ecs_ceddda9d.Cluster] = None,
+    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__032296542d572c6b398d9bf3c547056ab67cd1b9afdb7c038ad699976d18e3db(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    capacity_type: EnvironmentCapacityType,
+    cluster: _aws_cdk_aws_ecs_ceddda9d.ICluster,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__fc44db22afa05d01048722e48f64c16657acd6619ff44e75cd439cc75e743eb1(
+    service: Service,
+    scope: _constructs_77d1e7e8.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__26302b705de590e08625ea7201dd37b89ed5101384565fd0faf5199984ed9c46(
+    task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ed8391caad963614ec93d1a0d7e9d9747d62bf0d502b9ad5c4c57f654c5f7315(
+    service: Service,
+    scope: _constructs_77d1e7e8.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__5d2291e3a7f3e7948ea69040817ea11f3b4c2e634bcdd8ac8fb0199f4fe839bb(
+    service: typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__d5c9b77d6baabb5e5cb335d3b7b76d564d05a0a40856291a10a44c767bc2520b(
+    task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__48c7f195f42f8e59cbbfa1cbbb92b61da9881c8a02edf111a97cd4db56e0e94a(
+    task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ba812a9535025f034270daebc1bb1dcb1c0aa3ad083d9911e25dd4ed1bdd49dd(
+    service: Service,
+    scope: _constructs_77d1e7e8.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__965f371f47a5e35e297c690ad4fd62e38130d0f53ddfa246cbd67b7e5a78ebd3(
+    task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9c2f5ee1195fd16f7e0ef20ecbd77d67b9fbafa0ecd9617a5e91a28ef3de4ced(
+    service: Service,
+    scope: _constructs_77d1e7e8.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__1c33c510d93072d2b4ea0fcf0ba7fbae74143e371e7996c0e2805f9cf1a9af7c(
+    service: typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__994a45034920765ebf187cd6c2f9dd5d5d81863eb6a995f3f6c09b1d1ef8cce1(
+    task_definition: _aws_cdk_aws_ecs_ceddda9d.TaskDefinition,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__6e381a94b8fd01616977d82ea065a59158d8c683625e4200204ab6cae2823a5e(
+    value: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3cee1d52046f25f6baf6e7092422c633ee0e1b80c82bc9313467d3eea1800a1f(
+    service: typing.Union[_aws_cdk_aws_ecs_ceddda9d.Ec2Service, _aws_cdk_aws_ecs_ceddda9d.FargateService],
+) -> None:
+    """Type checking stubs"""
+    pass
```

### Comparing `cdk-ecs-service-extensions-2.0.0a99/src/cdk_ecs_service_extensions.egg-info/PKG-INFO` & `cdk-ecs-service-extensions-2.0.1a0/src/cdk_ecs_service_extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-ecs-service-extensions
-Version: 2.0.0a99
-Summary: @aws-cdk-containers/ecs-service-extensions
+Version: 2.0.1a0
+Summary: The CDK Construct Library that helps you build ECS services using simple extensions
 Home-page: https://github.com/cdklabs/cdk-ecs-service-extensions.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-ecs-service-extensions.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
@@ -241,14 +241,33 @@
 const nameService = new Service(this, 'name', {
   environment: environment,
   serviceDescription: nameDescription,
   taskRole,
 });
 ```
 
+## Configure Custom Health Check
+
+When you add an HTTPLoadBalancerExtension, you can customize the health checks by accessing the targetGroup field on the service.
+
+```python
+const service = new Service(stack, 'my-service', {
+  environment,
+  serviceDescription,
+  autoScaleTaskCount: {
+    maxTaskCount: 5,
+  },
+});
+
+service.targetGroup.configureHealthCheck({
+  path: '/',
+  port: '80',
+});
+```
+
 ## Task Auto-Scaling
 
 You can configure the task count of a service to match demand. The recommended way of achieving this is to configure target tracking policies for your service which scales in and out in order to keep metrics around target values.
 
 You need to configure an auto scaling target for the service by setting the `minTaskCount` (defaults to 1) and `maxTaskCount` in the `Service` construct. Then you can specify target values for "CPU Utilization" or "Memory Utilization" across all tasks in your service. Note that the `desiredCount` value will be set to `undefined` if the auto scaling target is configured.
 
 If you want to configure auto-scaling policies based on resources like Application Load Balancer or SQS Queues, you can set the corresponding resource-specific fields in the extension. For example, you can enable target tracking scaling based on Application Load Balancer request count as follows:
@@ -591,9 +610,7 @@
 We encourage the development of Community Service Extensions that support
 advanced features. Here are some useful extensions that we have reviewed:
 
 * [ListenerRulesExtension](https://www.npmjs.com/package/@wheatstalk/ecs-service-extension-listener-rules) for more precise control over Application Load Balancer rules
 
 > Please submit a pull request so that we can review your service extension and
 > list it here.
-
-
```

### Comparing `cdk-ecs-service-extensions-2.0.0a99/src/cdk_ecs_service_extensions.egg-info/SOURCES.txt` & `cdk-ecs-service-extensions-2.0.1a0/src/cdk_ecs_service_extensions.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdk_ecs_service_extensions/py.typed
 src/cdk_ecs_service_extensions.egg-info/PKG-INFO
 src/cdk_ecs_service_extensions.egg-info/SOURCES.txt
 src/cdk_ecs_service_extensions.egg-info/dependency_links.txt
 src/cdk_ecs_service_extensions.egg-info/requires.txt
 src/cdk_ecs_service_extensions.egg-info/top_level.txt
 src/cdk_ecs_service_extensions/_jsii/__init__.py
-src/cdk_ecs_service_extensions/_jsii/ecs-service-extensions@2.0.0-alpha.99.jsii.tgz
+src/cdk_ecs_service_extensions/_jsii/ecs-service-extensions@2.0.1-alpha.0.jsii.tgz
```

