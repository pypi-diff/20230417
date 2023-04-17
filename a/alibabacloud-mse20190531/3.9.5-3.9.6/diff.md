# Comparing `tmp/alibabacloud_mse20190531-3.9.5.tar.gz` & `tmp/alibabacloud_mse20190531-3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_mse20190531-3.9.5.tar", last modified: Tue Sep 27 08:57:55 2022, max compression
+gzip compressed data, was "dist/alibabacloud_mse20190531-3.9.6.tar", last modified: Wed Sep 28 13:17:44 2022, max compression
```

## Comparing `alibabacloud_mse20190531-3.9.5.tar` & `alibabacloud_mse20190531-3.9.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/
--rw-r--r--   0 root         (0) root         (0)     1543 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2344 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/alibabacloud_mse20190531/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/alibabacloud_mse20190531/__init__.py
--rw-r--r--   0 root         (0) root         (0)   576282 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/alibabacloud_mse20190531/client.py
--rw-r--r--   0 root         (0) root         (0)  1321551 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/alibabacloud_mse20190531/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/alibabacloud_mse20190531.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2344 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/alibabacloud_mse20190531.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/alibabacloud_mse20190531.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/alibabacloud_mse20190531.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/alibabacloud_mse20190531.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/alibabacloud_mse20190531.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2626 2022-09-27 08:57:55.000000 alibabacloud_mse20190531-3.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/
+-rw-r--r--   0 root         (0) root         (0)     1606 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2344 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/alibabacloud_mse20190531/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/alibabacloud_mse20190531/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   577742 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/alibabacloud_mse20190531/client.py
+-rw-r--r--   0 root         (0) root         (0)  1329728 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/alibabacloud_mse20190531/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/alibabacloud_mse20190531.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2344 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/alibabacloud_mse20190531.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/alibabacloud_mse20190531.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/alibabacloud_mse20190531.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/alibabacloud_mse20190531.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/alibabacloud_mse20190531.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2626 2022-09-28 13:17:44.000000 alibabacloud_mse20190531-3.9.6/setup.py
```

### Comparing `alibabacloud_mse20190531-3.9.5/ChangeLog.md` & `alibabacloud_mse20190531-3.9.6/ChangeLog.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2022-09-27 Version: 3.9.5
+- Automatically generate sdk tasks.
+
 2022-09-27 Version: 3.9.4
 - Automatically generate sdk tasks.
 
 2022-09-22 Version: 3.9.3
 - Automatically generate sdk tasks.
 
 2022-09-21 Version: 3.9.2
```

### Comparing `alibabacloud_mse20190531-3.9.5/LICENSE` & `alibabacloud_mse20190531-3.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_mse20190531-3.9.5/PKG-INFO` & `alibabacloud_mse20190531-3.9.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_mse20190531
-Version: 3.9.5
+Version: 3.9.6
 Summary: Alibaba Cloud Microservice Engine (20190531) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mse20190531-3.9.5/README-CN.md` & `alibabacloud_mse20190531-3.9.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mse20190531-3.9.5/README.md` & `alibabacloud_mse20190531-3.9.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mse20190531-3.9.5/alibabacloud_mse20190531/client.py` & `alibabacloud_mse20190531-3.9.6/alibabacloud_mse20190531/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,20 @@
             query['Content'] = request.content
         if not UtilClient.is_unset(request.gateway_unique_id):
             query['GatewayUniqueId'] = request.gateway_unique_id
         if not UtilClient.is_unset(request.is_white):
             query['IsWhite'] = request.is_white
         if not UtilClient.is_unset(request.mse_session_id):
             query['MseSessionId'] = request.mse_session_id
+        if not UtilClient.is_unset(request.name):
+            query['Name'] = request.name
+        if not UtilClient.is_unset(request.note):
+            query['Note'] = request.note
+        if not UtilClient.is_unset(request.resource_id_json_list):
+            query['ResourceIdJsonList'] = request.resource_id_json_list
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.status):
             query['Status'] = request.status
         if not UtilClient.is_unset(request.type):
             query['Type'] = request.type
         req = open_api_models.OpenApiRequest(
@@ -191,14 +197,20 @@
             query['Content'] = request.content
         if not UtilClient.is_unset(request.gateway_unique_id):
             query['GatewayUniqueId'] = request.gateway_unique_id
         if not UtilClient.is_unset(request.is_white):
             query['IsWhite'] = request.is_white
         if not UtilClient.is_unset(request.mse_session_id):
             query['MseSessionId'] = request.mse_session_id
+        if not UtilClient.is_unset(request.name):
+            query['Name'] = request.name
+        if not UtilClient.is_unset(request.note):
+            query['Note'] = request.note
+        if not UtilClient.is_unset(request.resource_id_json_list):
+            query['ResourceIdJsonList'] = request.resource_id_json_list
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.status):
             query['Status'] = request.status
         if not UtilClient.is_unset(request.type):
             query['Type'] = request.type
         req = open_api_models.OpenApiRequest(
@@ -261,14 +273,16 @@
             query['Region'] = request.region
         if not UtilClient.is_unset(request.replica):
             query['Replica'] = request.replica
         if not UtilClient.is_unset(request.slb_spec):
             query['SlbSpec'] = request.slb_spec
         if not UtilClient.is_unset(request.spec):
             query['Spec'] = request.spec
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         if not UtilClient.is_unset(request.v_switch_id):
             query['VSwitchId'] = request.v_switch_id
         if not UtilClient.is_unset(request.v_switch_id_2):
             query['VSwitchId2'] = request.v_switch_id_2
         if not UtilClient.is_unset(request.vpc):
             query['Vpc'] = request.vpc
         if not UtilClient.is_unset(request.xtrace_ratio):
@@ -319,14 +333,16 @@
             query['Region'] = request.region
         if not UtilClient.is_unset(request.replica):
             query['Replica'] = request.replica
         if not UtilClient.is_unset(request.slb_spec):
             query['SlbSpec'] = request.slb_spec
         if not UtilClient.is_unset(request.spec):
             query['Spec'] = request.spec
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         if not UtilClient.is_unset(request.v_switch_id):
             query['VSwitchId'] = request.v_switch_id
         if not UtilClient.is_unset(request.v_switch_id_2):
             query['VSwitchId2'] = request.v_switch_id_2
         if not UtilClient.is_unset(request.vpc):
             query['Vpc'] = request.vpc
         if not UtilClient.is_unset(request.xtrace_ratio):
@@ -10855,14 +10871,20 @@
             query['GatewayUniqueId'] = request.gateway_unique_id
         if not UtilClient.is_unset(request.id):
             query['Id'] = request.id
         if not UtilClient.is_unset(request.is_white):
             query['IsWhite'] = request.is_white
         if not UtilClient.is_unset(request.mse_session_id):
             query['MseSessionId'] = request.mse_session_id
+        if not UtilClient.is_unset(request.name):
+            query['Name'] = request.name
+        if not UtilClient.is_unset(request.note):
+            query['Note'] = request.note
+        if not UtilClient.is_unset(request.resource_id_json_list):
+            query['ResourceIdJsonList'] = request.resource_id_json_list
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.status):
             query['Status'] = request.status
         if not UtilClient.is_unset(request.type):
             query['Type'] = request.type
         req = open_api_models.OpenApiRequest(
@@ -10899,14 +10921,20 @@
             query['GatewayUniqueId'] = request.gateway_unique_id
         if not UtilClient.is_unset(request.id):
             query['Id'] = request.id
         if not UtilClient.is_unset(request.is_white):
             query['IsWhite'] = request.is_white
         if not UtilClient.is_unset(request.mse_session_id):
             query['MseSessionId'] = request.mse_session_id
+        if not UtilClient.is_unset(request.name):
+            query['Name'] = request.name
+        if not UtilClient.is_unset(request.note):
+            query['Note'] = request.note
+        if not UtilClient.is_unset(request.resource_id_json_list):
+            query['ResourceIdJsonList'] = request.resource_id_json_list
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.status):
             query['Status'] = request.status
         if not UtilClient.is_unset(request.type):
             query['Type'] = request.type
         req = open_api_models.OpenApiRequest(
```

### Comparing `alibabacloud_mse20190531-3.9.5/alibabacloud_mse20190531/models.py` & `alibabacloud_mse20190531-3.9.6/alibabacloud_mse20190531/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -656,23 +656,29 @@
     def __init__(
         self,
         accept_language: str = None,
         content: str = None,
         gateway_unique_id: str = None,
         is_white: bool = None,
         mse_session_id: str = None,
+        name: str = None,
+        note: str = None,
+        resource_id_json_list: str = None,
         resource_type: str = None,
         status: str = None,
         type: str = None,
     ):
         self.accept_language = accept_language
         self.content = content
         self.gateway_unique_id = gateway_unique_id
         self.is_white = is_white
         self.mse_session_id = mse_session_id
+        self.name = name
+        self.note = note
+        self.resource_id_json_list = resource_id_json_list
         self.resource_type = resource_type
         self.status = status
         self.type = type
 
     def validate(self):
         pass
 
@@ -688,14 +694,20 @@
             result['Content'] = self.content
         if self.gateway_unique_id is not None:
             result['GatewayUniqueId'] = self.gateway_unique_id
         if self.is_white is not None:
             result['IsWhite'] = self.is_white
         if self.mse_session_id is not None:
             result['MseSessionId'] = self.mse_session_id
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.note is not None:
+            result['Note'] = self.note
+        if self.resource_id_json_list is not None:
+            result['ResourceIdJsonList'] = self.resource_id_json_list
         if self.resource_type is not None:
             result['ResourceType'] = self.resource_type
         if self.status is not None:
             result['Status'] = self.status
         if self.type is not None:
             result['Type'] = self.type
         return result
@@ -708,14 +720,20 @@
             self.content = m.get('Content')
         if m.get('GatewayUniqueId') is not None:
             self.gateway_unique_id = m.get('GatewayUniqueId')
         if m.get('IsWhite') is not None:
             self.is_white = m.get('IsWhite')
         if m.get('MseSessionId') is not None:
             self.mse_session_id = m.get('MseSessionId')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Note') is not None:
+            self.note = m.get('Note')
+        if m.get('ResourceIdJsonList') is not None:
+            self.resource_id_json_list = m.get('ResourceIdJsonList')
         if m.get('ResourceType') is not None:
             self.resource_type = m.get('ResourceType')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
@@ -818,14 +836,47 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AddBlackWhiteListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class AddGatewayRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class AddGatewayRequest(TeaModel):
     def __init__(
         self,
         accept_language: str = None,
         enable_hardware_acceleration: bool = None,
         enable_sls: bool = None,
         enable_xtrace: bool = None,
@@ -833,14 +884,15 @@
         internet_slb_spec: str = None,
         mse_session_id: str = None,
         name: str = None,
         region: str = None,
         replica: int = None,
         slb_spec: str = None,
         spec: str = None,
+        tag: List[AddGatewayRequestTag] = None,
         v_switch_id: str = None,
         v_switch_id_2: str = None,
         vpc: str = None,
         xtrace_ratio: str = None,
     ):
         self.accept_language = accept_language
         self.enable_hardware_acceleration = enable_hardware_acceleration
@@ -850,21 +902,25 @@
         self.internet_slb_spec = internet_slb_spec
         self.mse_session_id = mse_session_id
         self.name = name
         self.region = region
         self.replica = replica
         self.slb_spec = slb_spec
         self.spec = spec
+        self.tag = tag
         self.v_switch_id = v_switch_id
         self.v_switch_id_2 = v_switch_id_2
         self.vpc = vpc
         self.xtrace_ratio = xtrace_ratio
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -888,14 +944,18 @@
             result['Region'] = self.region
         if self.replica is not None:
             result['Replica'] = self.replica
         if self.slb_spec is not None:
             result['SlbSpec'] = self.slb_spec
         if self.spec is not None:
             result['Spec'] = self.spec
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
         if self.v_switch_id is not None:
             result['VSwitchId'] = self.v_switch_id
         if self.v_switch_id_2 is not None:
             result['VSwitchId2'] = self.v_switch_id_2
         if self.vpc is not None:
             result['Vpc'] = self.vpc
         if self.xtrace_ratio is not None:
@@ -924,14 +984,19 @@
             self.region = m.get('Region')
         if m.get('Replica') is not None:
             self.replica = m.get('Replica')
         if m.get('SlbSpec') is not None:
             self.slb_spec = m.get('SlbSpec')
         if m.get('Spec') is not None:
             self.spec = m.get('Spec')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = AddGatewayRequestTag()
+                self.tag.append(temp_model.from_map(k))
         if m.get('VSwitchId') is not None:
             self.v_switch_id = m.get('VSwitchId')
         if m.get('VSwitchId2') is not None:
             self.v_switch_id_2 = m.get('VSwitchId2')
         if m.get('Vpc') is not None:
             self.vpc = m.get('Vpc')
         if m.get('XtraceRatio') is not None:
@@ -11164,14 +11229,15 @@
         end_date: str = None,
         gateway_unique_id: str = None,
         gmt_create: str = None,
         gmt_modified: str = None,
         id: int = None,
         instance_id: str = None,
         log_config_details: GetGatewayResponseBodyDataLogConfigDetails = None,
+        mse_tag: str = None,
         name: str = None,
         primary_user: str = None,
         region: str = None,
         replica: int = None,
         security_group: str = None,
         spec: str = None,
         status: int = None,
@@ -11185,14 +11251,15 @@
         self.end_date = end_date
         self.gateway_unique_id = gateway_unique_id
         self.gmt_create = gmt_create
         self.gmt_modified = gmt_modified
         self.id = id
         self.instance_id = instance_id
         self.log_config_details = log_config_details
+        self.mse_tag = mse_tag
         self.name = name
         self.primary_user = primary_user
         self.region = region
         self.replica = replica
         self.security_group = security_group
         self.spec = spec
         self.status = status
@@ -11226,14 +11293,16 @@
             result['GmtModified'] = self.gmt_modified
         if self.id is not None:
             result['Id'] = self.id
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.log_config_details is not None:
             result['LogConfigDetails'] = self.log_config_details.to_map()
+        if self.mse_tag is not None:
+            result['MseTag'] = self.mse_tag
         if self.name is not None:
             result['Name'] = self.name
         if self.primary_user is not None:
             result['PrimaryUser'] = self.primary_user
         if self.region is not None:
             result['Region'] = self.region
         if self.replica is not None:
@@ -11271,14 +11340,16 @@
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('LogConfigDetails') is not None:
             temp_model = GetGatewayResponseBodyDataLogConfigDetails()
             self.log_config_details = temp_model.from_map(m['LogConfigDetails'])
+        if m.get('MseTag') is not None:
+            self.mse_tag = m.get('MseTag')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('PrimaryUser') is not None:
             self.primary_user = m.get('PrimaryUser')
         if m.get('Region') is not None:
             self.region = m.get('Region')
         if m.get('Replica') is not None:
@@ -12002,24 +12073,26 @@
         agreement_type: str = None,
         group_name: str = None,
         name: str = None,
         namespace: str = None,
         percent: int = None,
         service_id: int = None,
         service_name: str = None,
+        service_port: int = None,
         source_type: str = None,
         version: str = None,
     ):
         self.agreement_type = agreement_type
         self.group_name = group_name
         self.name = name
         self.namespace = namespace
         self.percent = percent
         self.service_id = service_id
         self.service_name = service_name
+        self.service_port = service_port
         self.source_type = source_type
         self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -12038,14 +12111,16 @@
             result['Namespace'] = self.namespace
         if self.percent is not None:
             result['Percent'] = self.percent
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
         if self.service_name is not None:
             result['ServiceName'] = self.service_name
+        if self.service_port is not None:
+            result['ServicePort'] = self.service_port
         if self.source_type is not None:
             result['SourceType'] = self.source_type
         if self.version is not None:
             result['Version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
@@ -12060,14 +12135,16 @@
             self.namespace = m.get('Namespace')
         if m.get('Percent') is not None:
             self.percent = m.get('Percent')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
         if m.get('ServiceName') is not None:
             self.service_name = m.get('ServiceName')
+        if m.get('ServicePort') is not None:
+            self.service_port = m.get('ServicePort')
         if m.get('SourceType') is not None:
             self.source_type = m.get('SourceType')
         if m.get('Version') is not None:
             self.version = m.get('Version')
         return self
 
 
@@ -12486,24 +12563,26 @@
         agreement_type: str = None,
         group_name: str = None,
         name: str = None,
         namespace: str = None,
         percent: int = None,
         service_id: int = None,
         service_name: str = None,
+        service_port: int = None,
         source_type: str = None,
         version: str = None,
     ):
         self.agreement_type = agreement_type
         self.group_name = group_name
         self.name = name
         self.namespace = namespace
         self.percent = percent
         self.service_id = service_id
         self.service_name = service_name
+        self.service_port = service_port
         self.source_type = source_type
         self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -12522,14 +12601,16 @@
             result['Namespace'] = self.namespace
         if self.percent is not None:
             result['Percent'] = self.percent
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
         if self.service_name is not None:
             result['ServiceName'] = self.service_name
+        if self.service_port is not None:
+            result['ServicePort'] = self.service_port
         if self.source_type is not None:
             result['SourceType'] = self.source_type
         if self.version is not None:
             result['Version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
@@ -12544,14 +12625,16 @@
             self.namespace = m.get('Namespace')
         if m.get('Percent') is not None:
             self.percent = m.get('Percent')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
         if m.get('ServiceName') is not None:
             self.service_name = m.get('ServiceName')
+        if m.get('ServicePort') is not None:
+            self.service_port = m.get('ServicePort')
         if m.get('SourceType') is not None:
             self.source_type = m.get('SourceType')
         if m.get('Version') is not None:
             self.version = m.get('Version')
         return self
 
 
@@ -13013,14 +13096,79 @@
         if m.get('Key') is not None:
             self.key = m.get('Key')
         if m.get('Values') is not None:
             self.values = m.get('Values')
         return self
 
 
+class GetGatewayServiceDetailResponseBodyDataPortTrafficPolicyList(TeaModel):
+    def __init__(
+        self,
+        gateway_unique_id: str = None,
+        gmt_create: str = None,
+        gmt_modified: str = None,
+        id: int = None,
+        service_id: int = None,
+        service_port: int = None,
+        traffic_policy: TrafficPolicy = None,
+    ):
+        self.gateway_unique_id = gateway_unique_id
+        self.gmt_create = gmt_create
+        self.gmt_modified = gmt_modified
+        self.id = id
+        self.service_id = service_id
+        self.service_port = service_port
+        self.traffic_policy = traffic_policy
+
+    def validate(self):
+        if self.traffic_policy:
+            self.traffic_policy.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.gateway_unique_id is not None:
+            result['GatewayUniqueId'] = self.gateway_unique_id
+        if self.gmt_create is not None:
+            result['GmtCreate'] = self.gmt_create
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.service_id is not None:
+            result['ServiceId'] = self.service_id
+        if self.service_port is not None:
+            result['ServicePort'] = self.service_port
+        if self.traffic_policy is not None:
+            result['TrafficPolicy'] = self.traffic_policy.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('GatewayUniqueId') is not None:
+            self.gateway_unique_id = m.get('GatewayUniqueId')
+        if m.get('GmtCreate') is not None:
+            self.gmt_create = m.get('GmtCreate')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('ServiceId') is not None:
+            self.service_id = m.get('ServiceId')
+        if m.get('ServicePort') is not None:
+            self.service_port = m.get('ServicePort')
+        if m.get('TrafficPolicy') is not None:
+            temp_model = TrafficPolicy()
+            self.traffic_policy = temp_model.from_map(m['TrafficPolicy'])
+        return self
+
+
 class GetGatewayServiceDetailResponseBodyDataVersionDetailsServiceVersionLabels(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
         self.key = key
@@ -13184,14 +13332,16 @@
         health_status: str = None,
         id: int = None,
         ips: List[str] = None,
         label_details: List[GetGatewayServiceDetailResponseBodyDataLabelDetails] = None,
         meta_info: str = None,
         name: str = None,
         namespace: str = None,
+        port_traffic_policy_list: List[GetGatewayServiceDetailResponseBodyDataPortTrafficPolicyList] = None,
+        ports: List[int] = None,
         service_name_in_registry: str = None,
         service_protocol: str = None,
         source_id: int = None,
         source_type: str = None,
         version_details: List[GetGatewayServiceDetailResponseBodyDataVersionDetails] = None,
         versions: List[GetGatewayServiceDetailResponseBodyDataVersions] = None,
     ):
@@ -13205,28 +13355,34 @@
         self.health_status = health_status
         self.id = id
         self.ips = ips
         self.label_details = label_details
         self.meta_info = meta_info
         self.name = name
         self.namespace = namespace
+        self.port_traffic_policy_list = port_traffic_policy_list
+        self.ports = ports
         self.service_name_in_registry = service_name_in_registry
         self.service_protocol = service_protocol
         self.source_id = source_id
         self.source_type = source_type
         self.version_details = version_details
         self.versions = versions
 
     def validate(self):
         if self.gateway_traffic_policy:
             self.gateway_traffic_policy.validate()
         if self.label_details:
             for k in self.label_details:
                 if k:
                     k.validate()
+        if self.port_traffic_policy_list:
+            for k in self.port_traffic_policy_list:
+                if k:
+                    k.validate()
         if self.version_details:
             for k in self.version_details:
                 if k:
                     k.validate()
         if self.versions:
             for k in self.versions:
                 if k:
@@ -13264,14 +13420,20 @@
                 result['LabelDetails'].append(k.to_map() if k else None)
         if self.meta_info is not None:
             result['MetaInfo'] = self.meta_info
         if self.name is not None:
             result['Name'] = self.name
         if self.namespace is not None:
             result['Namespace'] = self.namespace
+        result['PortTrafficPolicyList'] = []
+        if self.port_traffic_policy_list is not None:
+            for k in self.port_traffic_policy_list:
+                result['PortTrafficPolicyList'].append(k.to_map() if k else None)
+        if self.ports is not None:
+            result['Ports'] = self.ports
         if self.service_name_in_registry is not None:
             result['ServiceNameInRegistry'] = self.service_name_in_registry
         if self.service_protocol is not None:
             result['ServiceProtocol'] = self.service_protocol
         if self.source_id is not None:
             result['SourceId'] = self.source_id
         if self.source_type is not None:
@@ -13316,14 +13478,21 @@
                 self.label_details.append(temp_model.from_map(k))
         if m.get('MetaInfo') is not None:
             self.meta_info = m.get('MetaInfo')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Namespace') is not None:
             self.namespace = m.get('Namespace')
+        self.port_traffic_policy_list = []
+        if m.get('PortTrafficPolicyList') is not None:
+            for k in m.get('PortTrafficPolicyList'):
+                temp_model = GetGatewayServiceDetailResponseBodyDataPortTrafficPolicyList()
+                self.port_traffic_policy_list.append(temp_model.from_map(k))
+        if m.get('Ports') is not None:
+            self.ports = m.get('Ports')
         if m.get('ServiceNameInRegistry') is not None:
             self.service_name_in_registry = m.get('ServiceNameInRegistry')
         if m.get('ServiceProtocol') is not None:
             self.service_protocol = m.get('ServiceProtocol')
         if m.get('SourceId') is not None:
             self.source_id = m.get('SourceId')
         if m.get('SourceType') is not None:
@@ -20391,20 +20560,22 @@
 
 class ListGatewayRequestFilterParams(TeaModel):
     def __init__(
         self,
         gateway_type: str = None,
         gateway_unique_id: str = None,
         instance_id: str = None,
+        mse_tag: str = None,
         name: str = None,
         vpc: str = None,
     ):
         self.gateway_type = gateway_type
         self.gateway_unique_id = gateway_unique_id
         self.instance_id = instance_id
+        self.mse_tag = mse_tag
         self.name = name
         self.vpc = vpc
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -20415,28 +20586,32 @@
         result = dict()
         if self.gateway_type is not None:
             result['GatewayType'] = self.gateway_type
         if self.gateway_unique_id is not None:
             result['GatewayUniqueId'] = self.gateway_unique_id
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
+        if self.mse_tag is not None:
+            result['MseTag'] = self.mse_tag
         if self.name is not None:
             result['Name'] = self.name
         if self.vpc is not None:
             result['Vpc'] = self.vpc
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('GatewayType') is not None:
             self.gateway_type = m.get('GatewayType')
         if m.get('GatewayUniqueId') is not None:
             self.gateway_unique_id = m.get('GatewayUniqueId')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
+        if m.get('MseTag') is not None:
+            self.mse_tag = m.get('MseTag')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Vpc') is not None:
             self.vpc = m.get('Vpc')
         return self
 
 
@@ -20760,14 +20935,15 @@
         gmt_create: str = None,
         gmt_modified: str = None,
         id: int = None,
         init_config: ListGatewayResponseBodyDataResultInitConfig = None,
         instance_id: str = None,
         internet_slb: List[ListGatewayResponseBodyDataResultInternetSlb] = None,
         latest_version: str = None,
+        mse_tag: str = None,
         must_upgrade: bool = None,
         name: str = None,
         primary_user: str = None,
         region: str = None,
         replica: int = None,
         roll_back: bool = None,
         slb: List[ListGatewayResponseBodyDataResultSlb] = None,
@@ -20791,14 +20967,15 @@
         self.gmt_create = gmt_create
         self.gmt_modified = gmt_modified
         self.id = id
         self.init_config = init_config
         self.instance_id = instance_id
         self.internet_slb = internet_slb
         self.latest_version = latest_version
+        self.mse_tag = mse_tag
         self.must_upgrade = must_upgrade
         self.name = name
         self.primary_user = primary_user
         self.region = region
         self.replica = replica
         self.roll_back = roll_back
         self.slb = slb
@@ -20858,14 +21035,16 @@
             result['InstanceId'] = self.instance_id
         result['InternetSlb'] = []
         if self.internet_slb is not None:
             for k in self.internet_slb:
                 result['InternetSlb'].append(k.to_map() if k else None)
         if self.latest_version is not None:
             result['LatestVersion'] = self.latest_version
+        if self.mse_tag is not None:
+            result['MseTag'] = self.mse_tag
         if self.must_upgrade is not None:
             result['MustUpgrade'] = self.must_upgrade
         if self.name is not None:
             result['Name'] = self.name
         if self.primary_user is not None:
             result['PrimaryUser'] = self.primary_user
         if self.region is not None:
@@ -20928,14 +21107,16 @@
         self.internet_slb = []
         if m.get('InternetSlb') is not None:
             for k in m.get('InternetSlb'):
                 temp_model = ListGatewayResponseBodyDataResultInternetSlb()
                 self.internet_slb.append(temp_model.from_map(k))
         if m.get('LatestVersion') is not None:
             self.latest_version = m.get('LatestVersion')
+        if m.get('MseTag') is not None:
+            self.mse_tag = m.get('MseTag')
         if m.get('MustUpgrade') is not None:
             self.must_upgrade = m.get('MustUpgrade')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('PrimaryUser') is not None:
             self.primary_user = m.get('PrimaryUser')
         if m.get('Region') is not None:
@@ -21679,24 +21860,26 @@
         agreement_type: str = None,
         group_name: str = None,
         name: str = None,
         namespace: str = None,
         percent: int = None,
         service_id: int = None,
         service_name: str = None,
+        service_port: int = None,
         source_type: str = None,
         version: str = None,
     ):
         self.agreement_type = agreement_type
         self.group_name = group_name
         self.name = name
         self.namespace = namespace
         self.percent = percent
         self.service_id = service_id
         self.service_name = service_name
+        self.service_port = service_port
         self.source_type = source_type
         self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -21715,14 +21898,16 @@
             result['Namespace'] = self.namespace
         if self.percent is not None:
             result['Percent'] = self.percent
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
         if self.service_name is not None:
             result['ServiceName'] = self.service_name
+        if self.service_port is not None:
+            result['ServicePort'] = self.service_port
         if self.source_type is not None:
             result['SourceType'] = self.source_type
         if self.version is not None:
             result['Version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
@@ -21737,14 +21922,16 @@
             self.namespace = m.get('Namespace')
         if m.get('Percent') is not None:
             self.percent = m.get('Percent')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
         if m.get('ServiceName') is not None:
             self.service_name = m.get('ServiceName')
+        if m.get('ServicePort') is not None:
+            self.service_port = m.get('ServicePort')
         if m.get('SourceType') is not None:
             self.source_type = m.get('SourceType')
         if m.get('Version') is not None:
             self.version = m.get('Version')
         return self
 
 
@@ -22133,25 +22320,27 @@
         group_name: str = None,
         http_dubbo_transcoder: ListGatewayRouteResponseBodyDataResultRouteServicesHttpDubboTranscoder = None,
         name: str = None,
         namespace: str = None,
         percent: int = None,
         service_id: int = None,
         service_name: str = None,
+        service_port: int = None,
         source_type: str = None,
         version: str = None,
     ):
         self.agreement_type = agreement_type
         self.group_name = group_name
         self.http_dubbo_transcoder = http_dubbo_transcoder
         self.name = name
         self.namespace = namespace
         self.percent = percent
         self.service_id = service_id
         self.service_name = service_name
+        self.service_port = service_port
         self.source_type = source_type
         self.version = version
 
     def validate(self):
         if self.http_dubbo_transcoder:
             self.http_dubbo_transcoder.validate()
 
@@ -22173,14 +22362,16 @@
             result['Namespace'] = self.namespace
         if self.percent is not None:
             result['Percent'] = self.percent
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
         if self.service_name is not None:
             result['ServiceName'] = self.service_name
+        if self.service_port is not None:
+            result['ServicePort'] = self.service_port
         if self.source_type is not None:
             result['SourceType'] = self.source_type
         if self.version is not None:
             result['Version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
@@ -22198,14 +22389,16 @@
             self.namespace = m.get('Namespace')
         if m.get('Percent') is not None:
             self.percent = m.get('Percent')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
         if m.get('ServiceName') is not None:
             self.service_name = m.get('ServiceName')
+        if m.get('ServicePort') is not None:
+            self.service_port = m.get('ServicePort')
         if m.get('SourceType') is not None:
             self.source_type = m.get('SourceType')
         if m.get('Version') is not None:
             self.version = m.get('Version')
         return self
 
 
@@ -23094,14 +23287,15 @@
         health_check_info: ListGatewayServiceResponseBodyDataResultHealthCheckInfo = None,
         health_status: str = None,
         id: int = None,
         ips: List[str] = None,
         meta_info: str = None,
         name: str = None,
         namespace: str = None,
+        ports: List[int] = None,
         service_name_in_registry: str = None,
         service_port: int = None,
         service_protocol: str = None,
         source_id: int = None,
         source_type: str = None,
         unhealthy_endpoints: List[str] = None,
         versions: List[ListGatewayServiceResponseBodyDataResultVersions] = None,
@@ -23117,14 +23311,15 @@
         self.health_check_info = health_check_info
         self.health_status = health_status
         self.id = id
         self.ips = ips
         self.meta_info = meta_info
         self.name = name
         self.namespace = namespace
+        self.ports = ports
         self.service_name_in_registry = service_name_in_registry
         self.service_port = service_port
         self.service_protocol = service_protocol
         self.source_id = source_id
         self.source_type = source_type
         self.unhealthy_endpoints = unhealthy_endpoints
         self.versions = versions
@@ -23171,14 +23366,16 @@
             result['Ips'] = self.ips
         if self.meta_info is not None:
             result['MetaInfo'] = self.meta_info
         if self.name is not None:
             result['Name'] = self.name
         if self.namespace is not None:
             result['Namespace'] = self.namespace
+        if self.ports is not None:
+            result['Ports'] = self.ports
         if self.service_name_in_registry is not None:
             result['ServiceNameInRegistry'] = self.service_name_in_registry
         if self.service_port is not None:
             result['ServicePort'] = self.service_port
         if self.service_protocol is not None:
             result['ServiceProtocol'] = self.service_protocol
         if self.source_id is not None:
@@ -23223,14 +23420,16 @@
             self.ips = m.get('Ips')
         if m.get('MetaInfo') is not None:
             self.meta_info = m.get('MetaInfo')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Namespace') is not None:
             self.namespace = m.get('Namespace')
+        if m.get('Ports') is not None:
+            self.ports = m.get('Ports')
         if m.get('ServiceNameInRegistry') is not None:
             self.service_name_in_registry = m.get('ServiceNameInRegistry')
         if m.get('ServicePort') is not None:
             self.service_port = m.get('ServicePort')
         if m.get('ServiceProtocol') is not None:
             self.service_protocol = m.get('ServiceProtocol')
         if m.get('SourceId') is not None:
@@ -31944,24 +32143,30 @@
         self,
         accept_language: str = None,
         content: str = None,
         gateway_unique_id: str = None,
         id: int = None,
         is_white: bool = None,
         mse_session_id: str = None,
+        name: str = None,
+        note: str = None,
+        resource_id_json_list: str = None,
         resource_type: str = None,
         status: str = None,
         type: str = None,
     ):
         self.accept_language = accept_language
         self.content = content
         self.gateway_unique_id = gateway_unique_id
         self.id = id
         self.is_white = is_white
         self.mse_session_id = mse_session_id
+        self.name = name
+        self.note = note
+        self.resource_id_json_list = resource_id_json_list
         self.resource_type = resource_type
         self.status = status
         self.type = type
 
     def validate(self):
         pass
 
@@ -31979,14 +32184,20 @@
             result['GatewayUniqueId'] = self.gateway_unique_id
         if self.id is not None:
             result['Id'] = self.id
         if self.is_white is not None:
             result['IsWhite'] = self.is_white
         if self.mse_session_id is not None:
             result['MseSessionId'] = self.mse_session_id
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.note is not None:
+            result['Note'] = self.note
+        if self.resource_id_json_list is not None:
+            result['ResourceIdJsonList'] = self.resource_id_json_list
         if self.resource_type is not None:
             result['ResourceType'] = self.resource_type
         if self.status is not None:
             result['Status'] = self.status
         if self.type is not None:
             result['Type'] = self.type
         return result
@@ -32001,14 +32212,20 @@
             self.gateway_unique_id = m.get('GatewayUniqueId')
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('IsWhite') is not None:
             self.is_white = m.get('IsWhite')
         if m.get('MseSessionId') is not None:
             self.mse_session_id = m.get('MseSessionId')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Note') is not None:
+            self.note = m.get('Note')
+        if m.get('ResourceIdJsonList') is not None:
+            self.resource_id_json_list = m.get('ResourceIdJsonList')
         if m.get('ResourceType') is not None:
             self.resource_type = m.get('ResourceType')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
```

### Comparing `alibabacloud_mse20190531-3.9.5/alibabacloud_mse20190531.egg-info/PKG-INFO` & `alibabacloud_mse20190531-3.9.6/alibabacloud_mse20190531.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-mse20190531
-Version: 3.9.5
+Version: 3.9.6
 Summary: Alibaba Cloud Microservice Engine (20190531) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mse20190531-3.9.5/setup.py` & `alibabacloud_mse20190531-3.9.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_mse20190531.
 
-Created on 27/09/2022
+Created on 28/09/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_mse20190531"
 NAME = "alibabacloud_mse20190531" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Microservice Engine (20190531) SDK Library for Python"
```

