# Comparing `tmp/alibabacloud_servicecatalog20210901-1.1.3.tar.gz` & `tmp/alibabacloud_servicecatalog20210901-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_servicecatalog20210901-1.1.3.tar", last modified: Mon Mar 20 05:36:38 2023, max compression
+gzip compressed data, was "dist/alibabacloud_servicecatalog20210901-1.1.4.tar", last modified: Mon Apr 17 09:18:33 2023, max compression
```

## Comparing `alibabacloud_servicecatalog20210901-1.1.3.tar` & `alibabacloud_servicecatalog20210901-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/
--rw-r--r--   0 root         (0) root         (0)      304 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1055 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/alibabacloud_servicecatalog20210901/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/alibabacloud_servicecatalog20210901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   153644 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/alibabacloud_servicecatalog20210901/client.py
--rw-r--r--   0 root         (0) root         (0)   327987 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/alibabacloud_servicecatalog20210901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/alibabacloud_servicecatalog20210901.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/alibabacloud_servicecatalog20210901.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/alibabacloud_servicecatalog20210901.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/alibabacloud_servicecatalog20210901.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/alibabacloud_servicecatalog20210901.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/alibabacloud_servicecatalog20210901.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2665 2023-03-20 05:36:38.000000 alibabacloud_servicecatalog20210901-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:18:33.000000 alibabacloud_servicecatalog20210901-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-04-17 09:18:32.000000 alibabacloud_servicecatalog20210901-1.1.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-17 09:18:32.000000 alibabacloud_servicecatalog20210901-1.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-17 09:18:32.000000 alibabacloud_servicecatalog20210901-1.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-04-17 09:18:33.000000 alibabacloud_servicecatalog20210901-1.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-04-17 09:18:32.000000 alibabacloud_servicecatalog20210901-1.1.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-04-17 09:18:32.000000 alibabacloud_servicecatalog20210901-1.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:18:33.000000 alibabacloud_servicecatalog20210901-1.1.4/alibabacloud_servicecatalog20210901/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-17 09:18:32.000000 alibabacloud_servicecatalog20210901-1.1.4/alibabacloud_servicecatalog20210901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179538 2023-04-17 09:18:32.000000 alibabacloud_servicecatalog20210901-1.1.4/alibabacloud_servicecatalog20210901/client.py
+-rw-r--r--   0 root         (0) root         (0)   374656 2023-04-17 09:18:32.000000 alibabacloud_servicecatalog20210901-1.1.4/alibabacloud_servicecatalog20210901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:18:33.000000 alibabacloud_servicecatalog20210901-1.1.4/alibabacloud_servicecatalog20210901.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-04-17 09:18:32.000000 alibabacloud_servicecatalog20210901-1.1.4/alibabacloud_servicecatalog20210901.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2023-04-17 09:18:33.000000 alibabacloud_servicecatalog20210901-1.1.4/alibabacloud_servicecatalog20210901.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 09:18:32.000000 alibabacloud_servicecatalog20210901-1.1.4/alibabacloud_servicecatalog20210901.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-17 09:18:32.000000 alibabacloud_servicecatalog20210901-1.1.4/alibabacloud_servicecatalog20210901.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-17 09:18:32.000000 alibabacloud_servicecatalog20210901-1.1.4/alibabacloud_servicecatalog20210901.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-17 09:18:33.000000 alibabacloud_servicecatalog20210901-1.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-04-17 09:18:32.000000 alibabacloud_servicecatalog20210901-1.1.4/setup.py
```

### Comparing `alibabacloud_servicecatalog20210901-1.1.3/LICENSE` & `alibabacloud_servicecatalog20210901-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_servicecatalog20210901-1.1.3/PKG-INFO` & `alibabacloud_servicecatalog20210901-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_servicecatalog20210901
-Version: 1.1.3
+Version: 1.1.4
 Summary: Alibaba Cloud servicecatalog (20210901) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_servicecatalog20210901-1.1.3/README-CN.md` & `alibabacloud_servicecatalog20210901-1.1.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_servicecatalog20210901-1.1.3/README.md` & `alibabacloud_servicecatalog20210901-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_servicecatalog20210901-1.1.3/alibabacloud_servicecatalog20210901/client.py` & `alibabacloud_servicecatalog20210901-1.1.4/alibabacloud_servicecatalog20210901/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -267,14 +267,88 @@
     async def associate_product_with_portfolio_async(
         self,
         request: servicecatalog_20210901_models.AssociateProductWithPortfolioRequest,
     ) -> servicecatalog_20210901_models.AssociateProductWithPortfolioResponse:
         runtime = util_models.RuntimeOptions()
         return await self.associate_product_with_portfolio_with_options_async(request, runtime)
 
+    def associate_tag_option_with_resource_with_options(
+        self,
+        request: servicecatalog_20210901_models.AssociateTagOptionWithResourceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.AssociateTagOptionWithResourceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.resource_id):
+            body['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.tag_option_id):
+            body['TagOptionId'] = request.tag_option_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AssociateTagOptionWithResource',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.AssociateTagOptionWithResourceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def associate_tag_option_with_resource_with_options_async(
+        self,
+        request: servicecatalog_20210901_models.AssociateTagOptionWithResourceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.AssociateTagOptionWithResourceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.resource_id):
+            body['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.tag_option_id):
+            body['TagOptionId'] = request.tag_option_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AssociateTagOptionWithResource',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.AssociateTagOptionWithResourceResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def associate_tag_option_with_resource(
+        self,
+        request: servicecatalog_20210901_models.AssociateTagOptionWithResourceRequest,
+    ) -> servicecatalog_20210901_models.AssociateTagOptionWithResourceResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.associate_tag_option_with_resource_with_options(request, runtime)
+
+    async def associate_tag_option_with_resource_async(
+        self,
+        request: servicecatalog_20210901_models.AssociateTagOptionWithResourceRequest,
+    ) -> servicecatalog_20210901_models.AssociateTagOptionWithResourceResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.associate_tag_option_with_resource_with_options_async(request, runtime)
+
     def cancel_provisioned_product_plan_with_options(
         self,
         request: servicecatalog_20210901_models.CancelProvisionedProductPlanRequest,
         runtime: util_models.RuntimeOptions,
     ) -> servicecatalog_20210901_models.CancelProvisionedProductPlanResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -337,14 +411,88 @@
     async def cancel_provisioned_product_plan_async(
         self,
         request: servicecatalog_20210901_models.CancelProvisionedProductPlanRequest,
     ) -> servicecatalog_20210901_models.CancelProvisionedProductPlanResponse:
         runtime = util_models.RuntimeOptions()
         return await self.cancel_provisioned_product_plan_with_options_async(request, runtime)
 
+    def copy_product_with_options(
+        self,
+        request: servicecatalog_20210901_models.CopyProductRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.CopyProductResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.source_product_arn):
+            body['SourceProductArn'] = request.source_product_arn
+        if not UtilClient.is_unset(request.target_product_name):
+            body['TargetProductName'] = request.target_product_name
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CopyProduct',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.CopyProductResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def copy_product_with_options_async(
+        self,
+        request: servicecatalog_20210901_models.CopyProductRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.CopyProductResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.source_product_arn):
+            body['SourceProductArn'] = request.source_product_arn
+        if not UtilClient.is_unset(request.target_product_name):
+            body['TargetProductName'] = request.target_product_name
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CopyProduct',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.CopyProductResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def copy_product(
+        self,
+        request: servicecatalog_20210901_models.CopyProductRequest,
+    ) -> servicecatalog_20210901_models.CopyProductResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.copy_product_with_options(request, runtime)
+
+    async def copy_product_async(
+        self,
+        request: servicecatalog_20210901_models.CopyProductRequest,
+    ) -> servicecatalog_20210901_models.CopyProductResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.copy_product_with_options_async(request, runtime)
+
     def create_constraint_with_options(
         self,
         request: servicecatalog_20210901_models.CreateConstraintRequest,
         runtime: util_models.RuntimeOptions,
     ) -> servicecatalog_20210901_models.CreateConstraintResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -851,14 +999,88 @@
     async def create_provisioned_product_plan_async(
         self,
         request: servicecatalog_20210901_models.CreateProvisionedProductPlanRequest,
     ) -> servicecatalog_20210901_models.CreateProvisionedProductPlanResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_provisioned_product_plan_with_options_async(request, runtime)
 
+    def create_tag_option_with_options(
+        self,
+        request: servicecatalog_20210901_models.CreateTagOptionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.CreateTagOptionResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.key):
+            body['Key'] = request.key
+        if not UtilClient.is_unset(request.value):
+            body['Value'] = request.value
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateTagOption',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.CreateTagOptionResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_tag_option_with_options_async(
+        self,
+        request: servicecatalog_20210901_models.CreateTagOptionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.CreateTagOptionResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.key):
+            body['Key'] = request.key
+        if not UtilClient.is_unset(request.value):
+            body['Value'] = request.value
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateTagOption',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.CreateTagOptionResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_tag_option(
+        self,
+        request: servicecatalog_20210901_models.CreateTagOptionRequest,
+    ) -> servicecatalog_20210901_models.CreateTagOptionResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_tag_option_with_options(request, runtime)
+
+    async def create_tag_option_async(
+        self,
+        request: servicecatalog_20210901_models.CreateTagOptionRequest,
+    ) -> servicecatalog_20210901_models.CreateTagOptionResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_tag_option_with_options_async(request, runtime)
+
     def create_template_with_options(
         self,
         request: servicecatalog_20210901_models.CreateTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> servicecatalog_20210901_models.CreateTemplateResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -1279,14 +1501,158 @@
     async def delete_provisioned_product_plan_async(
         self,
         request: servicecatalog_20210901_models.DeleteProvisionedProductPlanRequest,
     ) -> servicecatalog_20210901_models.DeleteProvisionedProductPlanResponse:
         runtime = util_models.RuntimeOptions()
         return await self.delete_provisioned_product_plan_with_options_async(request, runtime)
 
+    def delete_tag_option_with_options(
+        self,
+        request: servicecatalog_20210901_models.DeleteTagOptionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.DeleteTagOptionResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.tag_option_id):
+            body['TagOptionId'] = request.tag_option_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DeleteTagOption',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.DeleteTagOptionResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_tag_option_with_options_async(
+        self,
+        request: servicecatalog_20210901_models.DeleteTagOptionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.DeleteTagOptionResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.tag_option_id):
+            body['TagOptionId'] = request.tag_option_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DeleteTagOption',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.DeleteTagOptionResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_tag_option(
+        self,
+        request: servicecatalog_20210901_models.DeleteTagOptionRequest,
+    ) -> servicecatalog_20210901_models.DeleteTagOptionResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_tag_option_with_options(request, runtime)
+
+    async def delete_tag_option_async(
+        self,
+        request: servicecatalog_20210901_models.DeleteTagOptionRequest,
+    ) -> servicecatalog_20210901_models.DeleteTagOptionResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_tag_option_with_options_async(request, runtime)
+
+    def dis_associate_tag_option_from_resource_with_options(
+        self,
+        request: servicecatalog_20210901_models.DisAssociateTagOptionFromResourceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.DisAssociateTagOptionFromResourceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.resource_id):
+            body['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.tag_option_id):
+            body['TagOptionId'] = request.tag_option_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DisAssociateTagOptionFromResource',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.DisAssociateTagOptionFromResourceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def dis_associate_tag_option_from_resource_with_options_async(
+        self,
+        request: servicecatalog_20210901_models.DisAssociateTagOptionFromResourceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.DisAssociateTagOptionFromResourceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.resource_id):
+            body['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.tag_option_id):
+            body['TagOptionId'] = request.tag_option_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DisAssociateTagOptionFromResource',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.DisAssociateTagOptionFromResourceResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def dis_associate_tag_option_from_resource(
+        self,
+        request: servicecatalog_20210901_models.DisAssociateTagOptionFromResourceRequest,
+    ) -> servicecatalog_20210901_models.DisAssociateTagOptionFromResourceResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.dis_associate_tag_option_from_resource_with_options(request, runtime)
+
+    async def dis_associate_tag_option_from_resource_async(
+        self,
+        request: servicecatalog_20210901_models.DisAssociateTagOptionFromResourceRequest,
+    ) -> servicecatalog_20210901_models.DisAssociateTagOptionFromResourceResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.dis_associate_tag_option_from_resource_with_options_async(request, runtime)
+
     def disassociate_principal_from_portfolio_with_options(
         self,
         request: servicecatalog_20210901_models.DisassociatePrincipalFromPortfolioRequest,
         runtime: util_models.RuntimeOptions,
     ) -> servicecatalog_20210901_models.DisassociatePrincipalFromPortfolioResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -1717,15 +2083,15 @@
 
     def get_product_as_end_user_with_options(
         self,
         request: servicecatalog_20210901_models.GetProductAsEndUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> servicecatalog_20210901_models.GetProductAsEndUserResponse:
         """
-        Make sure that the administrator grants the end user the permissions to manage the product. For more information, see [Grant the end user the permissions to access the product](~~405233~~).
+        Make sure that you are granted the permissions to manage relevant products as a user by an administrator. For more information, see [Manage access permissions](~~405233~~).
         
         @param request: GetProductAsEndUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetProductAsEndUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1752,15 +2118,15 @@
 
     async def get_product_as_end_user_with_options_async(
         self,
         request: servicecatalog_20210901_models.GetProductAsEndUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> servicecatalog_20210901_models.GetProductAsEndUserResponse:
         """
-        Make sure that the administrator grants the end user the permissions to manage the product. For more information, see [Grant the end user the permissions to access the product](~~405233~~).
+        Make sure that you are granted the permissions to manage relevant products as a user by an administrator. For more information, see [Manage access permissions](~~405233~~).
         
         @param request: GetProductAsEndUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetProductAsEndUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1786,28 +2152,28 @@
         )
 
     def get_product_as_end_user(
         self,
         request: servicecatalog_20210901_models.GetProductAsEndUserRequest,
     ) -> servicecatalog_20210901_models.GetProductAsEndUserResponse:
         """
-        Make sure that the administrator grants the end user the permissions to manage the product. For more information, see [Grant the end user the permissions to access the product](~~405233~~).
+        Make sure that you are granted the permissions to manage relevant products as a user by an administrator. For more information, see [Manage access permissions](~~405233~~).
         
         @param request: GetProductAsEndUserRequest
         @return: GetProductAsEndUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_product_as_end_user_with_options(request, runtime)
 
     async def get_product_as_end_user_async(
         self,
         request: servicecatalog_20210901_models.GetProductAsEndUserRequest,
     ) -> servicecatalog_20210901_models.GetProductAsEndUserResponse:
         """
-        Make sure that the administrator grants the end user the permissions to manage the product. For more information, see [Grant the end user the permissions to access the product](~~405233~~).
+        Make sure that you are granted the permissions to manage relevant products as a user by an administrator. For more information, see [Manage access permissions](~~405233~~).
         
         @param request: GetProductAsEndUserRequest
         @return: GetProductAsEndUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_product_as_end_user_with_options_async(request, runtime)
 
@@ -2017,14 +2383,80 @@
     async def get_provisioned_product_plan_async(
         self,
         request: servicecatalog_20210901_models.GetProvisionedProductPlanRequest,
     ) -> servicecatalog_20210901_models.GetProvisionedProductPlanResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_provisioned_product_plan_with_options_async(request, runtime)
 
+    def get_tag_option_with_options(
+        self,
+        request: servicecatalog_20210901_models.GetTagOptionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.GetTagOptionResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetTagOption',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.GetTagOptionResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_tag_option_with_options_async(
+        self,
+        request: servicecatalog_20210901_models.GetTagOptionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.GetTagOptionResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetTagOption',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.GetTagOptionResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_tag_option(
+        self,
+        request: servicecatalog_20210901_models.GetTagOptionRequest,
+    ) -> servicecatalog_20210901_models.GetTagOptionResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_tag_option_with_options(request, runtime)
+
+    async def get_tag_option_async(
+        self,
+        request: servicecatalog_20210901_models.GetTagOptionRequest,
+    ) -> servicecatalog_20210901_models.GetTagOptionResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_tag_option_with_options_async(request, runtime)
+
     def get_task_with_options(
         self,
         request: servicecatalog_20210901_models.GetTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> servicecatalog_20210901_models.GetTaskResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -2589,15 +3021,15 @@
 
     def list_products_as_end_user_with_options(
         self,
         request: servicecatalog_20210901_models.ListProductsAsEndUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> servicecatalog_20210901_models.ListProductsAsEndUserResponse:
         """
-        Make sure that the administrator grants the end user the permissions to manage the product. For more information, see [Grant the end user the permissions to access the product](~~405233~~).
+        Make sure that you are granted the permissions to manage relevant products as a user by an administrator. For more information, see [Manage access permissions](~~405233~~).
         
         @param request: ListProductsAsEndUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListProductsAsEndUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2632,15 +3064,15 @@
 
     async def list_products_as_end_user_with_options_async(
         self,
         request: servicecatalog_20210901_models.ListProductsAsEndUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> servicecatalog_20210901_models.ListProductsAsEndUserResponse:
         """
-        Make sure that the administrator grants the end user the permissions to manage the product. For more information, see [Grant the end user the permissions to access the product](~~405233~~).
+        Make sure that you are granted the permissions to manage relevant products as a user by an administrator. For more information, see [Manage access permissions](~~405233~~).
         
         @param request: ListProductsAsEndUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListProductsAsEndUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2674,28 +3106,28 @@
         )
 
     def list_products_as_end_user(
         self,
         request: servicecatalog_20210901_models.ListProductsAsEndUserRequest,
     ) -> servicecatalog_20210901_models.ListProductsAsEndUserResponse:
         """
-        Make sure that the administrator grants the end user the permissions to manage the product. For more information, see [Grant the end user the permissions to access the product](~~405233~~).
+        Make sure that you are granted the permissions to manage relevant products as a user by an administrator. For more information, see [Manage access permissions](~~405233~~).
         
         @param request: ListProductsAsEndUserRequest
         @return: ListProductsAsEndUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_products_as_end_user_with_options(request, runtime)
 
     async def list_products_as_end_user_async(
         self,
         request: servicecatalog_20210901_models.ListProductsAsEndUserRequest,
     ) -> servicecatalog_20210901_models.ListProductsAsEndUserResponse:
         """
-        Make sure that the administrator grants the end user the permissions to manage the product. For more information, see [Grant the end user the permissions to access the product](~~405233~~).
+        Make sure that you are granted the permissions to manage relevant products as a user by an administrator. For more information, see [Manage access permissions](~~405233~~).
         
         @param request: ListProductsAsEndUserRequest
         @return: ListProductsAsEndUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_products_as_end_user_with_options_async(request, runtime)
 
@@ -2999,14 +3431,154 @@
         runtime = util_models.RuntimeOptions()
         return self.list_regions_with_options(runtime)
 
     async def list_regions_async(self) -> servicecatalog_20210901_models.ListRegionsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_regions_with_options_async(runtime)
 
+    def list_resources_for_tag_option_with_options(
+        self,
+        request: servicecatalog_20210901_models.ListResourcesForTagOptionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.ListResourcesForTagOptionResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListResourcesForTagOption',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.ListResourcesForTagOptionResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_resources_for_tag_option_with_options_async(
+        self,
+        request: servicecatalog_20210901_models.ListResourcesForTagOptionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.ListResourcesForTagOptionResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListResourcesForTagOption',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.ListResourcesForTagOptionResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_resources_for_tag_option(
+        self,
+        request: servicecatalog_20210901_models.ListResourcesForTagOptionRequest,
+    ) -> servicecatalog_20210901_models.ListResourcesForTagOptionResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_resources_for_tag_option_with_options(request, runtime)
+
+    async def list_resources_for_tag_option_async(
+        self,
+        request: servicecatalog_20210901_models.ListResourcesForTagOptionRequest,
+    ) -> servicecatalog_20210901_models.ListResourcesForTagOptionResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_resources_for_tag_option_with_options_async(request, runtime)
+
+    def list_tag_options_with_options(
+        self,
+        tmp_req: servicecatalog_20210901_models.ListTagOptionsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.ListTagOptionsResponse:
+        UtilClient.validate_model(tmp_req)
+        request = servicecatalog_20210901_models.ListTagOptionsShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.filters):
+            request.filters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.filters, 'Filters', 'json')
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTagOptions',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.ListTagOptionsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_tag_options_with_options_async(
+        self,
+        tmp_req: servicecatalog_20210901_models.ListTagOptionsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.ListTagOptionsResponse:
+        UtilClient.validate_model(tmp_req)
+        request = servicecatalog_20210901_models.ListTagOptionsShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.filters):
+            request.filters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.filters, 'Filters', 'json')
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTagOptions',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.ListTagOptionsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_tag_options(
+        self,
+        request: servicecatalog_20210901_models.ListTagOptionsRequest,
+    ) -> servicecatalog_20210901_models.ListTagOptionsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_tag_options_with_options(request, runtime)
+
+    async def list_tag_options_async(
+        self,
+        request: servicecatalog_20210901_models.ListTagOptionsRequest,
+    ) -> servicecatalog_20210901_models.ListTagOptionsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_tag_options_with_options_async(request, runtime)
+
     def list_tasks_with_options(
         self,
         request: servicecatalog_20210901_models.ListTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> servicecatalog_20210901_models.ListTasksResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -3692,7 +4264,85 @@
 
     async def update_provisioned_product_plan_async(
         self,
         request: servicecatalog_20210901_models.UpdateProvisionedProductPlanRequest,
     ) -> servicecatalog_20210901_models.UpdateProvisionedProductPlanResponse:
         runtime = util_models.RuntimeOptions()
         return await self.update_provisioned_product_plan_with_options_async(request, runtime)
+
+    def update_tag_option_with_options(
+        self,
+        request: servicecatalog_20210901_models.UpdateTagOptionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.UpdateTagOptionResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.active):
+            body['Active'] = request.active
+        if not UtilClient.is_unset(request.tag_option_id):
+            body['TagOptionId'] = request.tag_option_id
+        if not UtilClient.is_unset(request.value):
+            body['Value'] = request.value
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateTagOption',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.UpdateTagOptionResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def update_tag_option_with_options_async(
+        self,
+        request: servicecatalog_20210901_models.UpdateTagOptionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> servicecatalog_20210901_models.UpdateTagOptionResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.active):
+            body['Active'] = request.active
+        if not UtilClient.is_unset(request.tag_option_id):
+            body['TagOptionId'] = request.tag_option_id
+        if not UtilClient.is_unset(request.value):
+            body['Value'] = request.value
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateTagOption',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            servicecatalog_20210901_models.UpdateTagOptionResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_tag_option(
+        self,
+        request: servicecatalog_20210901_models.UpdateTagOptionRequest,
+    ) -> servicecatalog_20210901_models.UpdateTagOptionResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.update_tag_option_with_options(request, runtime)
+
+    async def update_tag_option_async(
+        self,
+        request: servicecatalog_20210901_models.UpdateTagOptionRequest,
+    ) -> servicecatalog_20210901_models.UpdateTagOptionResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.update_tag_option_with_options_async(request, runtime)
```

### Comparing `alibabacloud_servicecatalog20210901-1.1.3/alibabacloud_servicecatalog20210901/models.py` & `alibabacloud_servicecatalog20210901-1.1.4/alibabacloud_servicecatalog20210901/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -338,14 +338,118 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AssociateProductWithPortfolioResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class AssociateTagOptionWithResourceRequest(TeaModel):
+    def __init__(
+        self,
+        resource_id: str = None,
+        tag_option_id: str = None,
+    ):
+        self.resource_id = resource_id
+        self.tag_option_id = tag_option_id
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
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.tag_option_id is not None:
+            result['TagOptionId'] = self.tag_option_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('TagOptionId') is not None:
+            self.tag_option_id = m.get('TagOptionId')
+        return self
+
+
+class AssociateTagOptionWithResourceResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class AssociateTagOptionWithResourceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AssociateTagOptionWithResourceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AssociateTagOptionWithResourceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CancelProvisionedProductPlanRequest(TeaModel):
     def __init__(
         self,
         plan_id: str = None,
     ):
         self.plan_id = plan_id
 
@@ -436,14 +540,118 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CancelProvisionedProductPlanResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CopyProductRequest(TeaModel):
+    def __init__(
+        self,
+        source_product_arn: str = None,
+        target_product_name: str = None,
+    ):
+        self.source_product_arn = source_product_arn
+        self.target_product_name = target_product_name
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
+        if self.source_product_arn is not None:
+            result['SourceProductArn'] = self.source_product_arn
+        if self.target_product_name is not None:
+            result['TargetProductName'] = self.target_product_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('SourceProductArn') is not None:
+            self.source_product_arn = m.get('SourceProductArn')
+        if m.get('TargetProductName') is not None:
+            self.target_product_name = m.get('TargetProductName')
+        return self
+
+
+class CopyProductResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CopyProductResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CopyProductResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CopyProductResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateConstraintRequest(TeaModel):
     def __init__(
         self,
         config: str = None,
         constraint_type: str = None,
         description: str = None,
         portfolio_id: str = None,
@@ -714,37 +922,37 @@
         active: bool = None,
         description: str = None,
         guidance: str = None,
         product_version_name: str = None,
         template_type: str = None,
         template_url: str = None,
     ):
-        # Specifies whether the product version is visible to end users. Valid values:
+        # Specifies whether to enable the product version. Valid values:
         # 
-        # *   true: The product version is visible to end users. This is the default value.
-        # *   false: The product version is invisible to end users.
+        # *   true: enables the product version. This is the default value.
+        # *   false: disables the product version.
         self.active = active
         # The description of the product version.
         # 
         # The value must be 1 to 128 characters in length.
         self.description = description
         # The recommendation information. Valid values:
         # 
         # *   Default: No recommendation information is provided. This is the default value.
-        # *   Recommended: the recommendation version.
+        # *   Recommended: the recommended version.
         # *   Latest: the latest version.
-        # *   Deprecated: the version that is about to be deprecated.
+        # *   Deprecated: the version that is about to be discontinued.
         self.guidance = guidance
         # The name of the product version.
         # 
         # The value must be 1 to 128 characters in length.
         self.product_version_name = product_version_name
         # The type of the template.
         # 
-        # The value is fixed as RosTerraformTemplate, which specifies that the Terraform template is supported by ROS.
+        # Set the value to RosTerraformTemplate, which specifies the Terraform template that is supported by ROS.
         self.template_type = template_type
         # The URL of the template.
         # 
         # For more information about how to obtain the URL of a template, see [CreateTemplate](~~CreateTemplate~~).
         self.template_url = template_url
 
     def validate(self):
@@ -802,15 +1010,15 @@
         self.description = description
         # The name of the product.
         # 
         # The value must be 1 to 128 characters in length.
         self.product_name = product_name
         # The type of the product.
         # 
-        # The value is fixed as Ros, which specifies Resource Orchestration Service (ROS).
+        # Set the value to Ros, which specifies Resource Orchestration Service (ROS).
         self.product_type = product_type
         # The information about the product version.
         self.product_version_parameters = product_version_parameters
         # The provider of the product.
         # 
         # The value must be 1 to 128 characters in length.
         self.provider_name = provider_name
@@ -868,15 +1076,15 @@
         self.description = description
         # The name of the product.
         # 
         # The value must be 1 to 128 characters in length.
         self.product_name = product_name
         # The type of the product.
         # 
-        # The value is fixed as Ros, which specifies Resource Orchestration Service (ROS).
+        # Set the value to Ros, which specifies Resource Orchestration Service (ROS).
         self.product_type = product_type
         # The information about the product version.
         self.product_version_parameters_shrink = product_version_parameters_shrink
         # The provider of the product.
         # 
         # The value must be 1 to 128 characters in length.
         self.provider_name = provider_name
@@ -1010,39 +1218,39 @@
         description: str = None,
         guidance: str = None,
         product_id: str = None,
         product_version_name: str = None,
         template_type: str = None,
         template_url: str = None,
     ):
-        # Specifies whether the product version is visible to end users. Valid values:
+        # Specifies whether the product version is active. Valid values:
         # 
-        # *   true: The product version is visible to end users. This is the default value.
-        # *   false: The product version is invisible to end users.
+        # *   true: The product version is active. This is the default value.
+        # *   false: The product version is inactive.
         self.active = active
         # The description of the product version.
         # 
         # The value must be 1 to 128 characters in length.
         self.description = description
         # The recommendation information. Valid values:
         # 
         # *   Default: No recommendation information is provided. This is the default value.
         # *   Recommended: the recommendation version.
         # *   Latest: the latest version.
-        # *   Deprecated: the version that is about to be deprecated.
+        # *   Deprecated: the version that is about to be discontinued.
         self.guidance = guidance
         # The ID of the product to which the product version belongs.
         self.product_id = product_id
         # The name of the product version.
         # 
         # The value must be 1 to 128 characters in length.
         self.product_version_name = product_version_name
         # The type of the template.
         # 
-        # The value is fixed as RosTerraformTemplate, which specifies that the Terraform template is supported by Resource Orchestration Service (ROS).
+        # The value is fixed as RosTerraformTemplate, which specifies the Terraform template that is supported by Resource Orchestration Service (ROS).
         self.template_type = template_type
         # The URL of the template.
         # 
         # For more information about how to obtain the URL of a template, see [CreateTemplate](~~CreateTemplate~~).
         self.template_url = template_url
 
     def validate(self):
@@ -1444,21 +1652,188 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateProvisionedProductPlanResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateTagOptionRequest(TeaModel):
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
+class CreateTagOptionResponseBodyTagOptionDetail(TeaModel):
+    def __init__(
+        self,
+        active: bool = None,
+        key: str = None,
+        owner: str = None,
+        tag_option_id: str = None,
+        value: str = None,
+    ):
+        self.active = active
+        self.key = key
+        self.owner = owner
+        self.tag_option_id = tag_option_id
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
+        if self.active is not None:
+            result['Active'] = self.active
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.owner is not None:
+            result['Owner'] = self.owner
+        if self.tag_option_id is not None:
+            result['TagOptionId'] = self.tag_option_id
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Active') is not None:
+            self.active = m.get('Active')
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Owner') is not None:
+            self.owner = m.get('Owner')
+        if m.get('TagOptionId') is not None:
+            self.tag_option_id = m.get('TagOptionId')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class CreateTagOptionResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        tag_option_detail: CreateTagOptionResponseBodyTagOptionDetail = None,
+    ):
+        self.request_id = request_id
+        self.tag_option_detail = tag_option_detail
+
+    def validate(self):
+        if self.tag_option_detail:
+            self.tag_option_detail.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.tag_option_detail is not None:
+            result['TagOptionDetail'] = self.tag_option_detail.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TagOptionDetail') is not None:
+            temp_model = CreateTagOptionResponseBodyTagOptionDetail()
+            self.tag_option_detail = temp_model.from_map(m['TagOptionDetail'])
+        return self
+
+
+class CreateTagOptionResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateTagOptionResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateTagOptionResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateTemplateRequestTerraformVariables(TeaModel):
     def __init__(
         self,
         description: str = None,
         variable_name: str = None,
     ):
+        # The description of the variable.
+        # 
+        # For more information about the format of variable descriptions, see [Methods and suggestions for Terraform code development](~~322216~~).
         self.description = description
+        # The name of the variable.
         self.variable_name = variable_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1490,16 +1865,19 @@
     ):
         # The content of the template.
         # 
         # For more information about the template syntax, see [Structure of Terraform templates](~~184397~~).
         self.template_body = template_body
         # The type of the template.
         # 
-        # The value is fixed as RosTerraformTemplate, which specifies that the Terraform template is supported by Resource Orchestration Service (ROS).
+        # Set the value to RosTerraformTemplate, which specifies the Terraform template that is supported by Resource Orchestration Service (ROS).
         self.template_type = template_type
+        # The variable settings of the Terraform template. You can configure the variables in a structured manner. Service Catalog applies the variable settings to the template.
+        # 
+        # > The variables must be defined in the Terraform template.
         self.terraform_variables = terraform_variables
 
     def validate(self):
         if self.terraform_variables:
             for k in self.terraform_variables:
                 if k:
                     k.validate()
@@ -2109,14 +2487,216 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteProvisionedProductPlanResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteTagOptionRequest(TeaModel):
+    def __init__(
+        self,
+        tag_option_id: str = None,
+    ):
+        self.tag_option_id = tag_option_id
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
+        if self.tag_option_id is not None:
+            result['TagOptionId'] = self.tag_option_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TagOptionId') is not None:
+            self.tag_option_id = m.get('TagOptionId')
+        return self
+
+
+class DeleteTagOptionResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteTagOptionResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteTagOptionResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteTagOptionResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DisAssociateTagOptionFromResourceRequest(TeaModel):
+    def __init__(
+        self,
+        resource_id: str = None,
+        tag_option_id: str = None,
+    ):
+        self.resource_id = resource_id
+        self.tag_option_id = tag_option_id
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
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.tag_option_id is not None:
+            result['TagOptionId'] = self.tag_option_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('TagOptionId') is not None:
+            self.tag_option_id = m.get('TagOptionId')
+        return self
+
+
+class DisAssociateTagOptionFromResourceResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DisAssociateTagOptionFromResourceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DisAssociateTagOptionFromResourceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DisAssociateTagOptionFromResourceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DisassociatePrincipalFromPortfolioRequest(TeaModel):
     def __init__(
         self,
         portfolio_id: str = None,
         principal_id: str = None,
         principal_type: str = None,
     ):
@@ -2729,48 +3309,114 @@
         if m.get('PortfolioName') is not None:
             self.portfolio_name = m.get('PortfolioName')
         if m.get('ProviderName') is not None:
             self.provider_name = m.get('ProviderName')
         return self
 
 
+class GetPortfolioResponseBodyTagOptions(TeaModel):
+    def __init__(
+        self,
+        active: bool = None,
+        key: str = None,
+        owner: str = None,
+        tag_option_id: str = None,
+        value: str = None,
+    ):
+        self.active = active
+        self.key = key
+        self.owner = owner
+        self.tag_option_id = tag_option_id
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
+        if self.active is not None:
+            result['Active'] = self.active
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.owner is not None:
+            result['Owner'] = self.owner
+        if self.tag_option_id is not None:
+            result['TagOptionId'] = self.tag_option_id
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Active') is not None:
+            self.active = m.get('Active')
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Owner') is not None:
+            self.owner = m.get('Owner')
+        if m.get('TagOptionId') is not None:
+            self.tag_option_id = m.get('TagOptionId')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class GetPortfolioResponseBody(TeaModel):
     def __init__(
         self,
         portfolio_detail: GetPortfolioResponseBodyPortfolioDetail = None,
         request_id: str = None,
+        tag_options: List[GetPortfolioResponseBodyTagOptions] = None,
     ):
         # The details of the product portfolio.
         self.portfolio_detail = portfolio_detail
         # The ID of the request.
         self.request_id = request_id
+        self.tag_options = tag_options
 
     def validate(self):
         if self.portfolio_detail:
             self.portfolio_detail.validate()
+        if self.tag_options:
+            for k in self.tag_options:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.portfolio_detail is not None:
             result['PortfolioDetail'] = self.portfolio_detail.to_map()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
+        result['TagOptions'] = []
+        if self.tag_options is not None:
+            for k in self.tag_options:
+                result['TagOptions'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('PortfolioDetail') is not None:
             temp_model = GetPortfolioResponseBodyPortfolioDetail()
             self.portfolio_detail = temp_model.from_map(m['PortfolioDetail'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        self.tag_options = []
+        if m.get('TagOptions') is not None:
+            for k in m.get('TagOptions'):
+                temp_model = GetPortfolioResponseBodyTagOptions()
+                self.tag_options.append(temp_model.from_map(k))
         return self
 
 
 class GetPortfolioResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -2912,48 +3558,114 @@
         if m.get('ProductType') is not None:
             self.product_type = m.get('ProductType')
         if m.get('ProviderName') is not None:
             self.provider_name = m.get('ProviderName')
         return self
 
 
+class GetProductAsAdminResponseBodyTagOptions(TeaModel):
+    def __init__(
+        self,
+        active: bool = None,
+        key: str = None,
+        owner: str = None,
+        tag_option_id: str = None,
+        value: str = None,
+    ):
+        self.active = active
+        self.key = key
+        self.owner = owner
+        self.tag_option_id = tag_option_id
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
+        if self.active is not None:
+            result['Active'] = self.active
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.owner is not None:
+            result['Owner'] = self.owner
+        if self.tag_option_id is not None:
+            result['TagOptionId'] = self.tag_option_id
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Active') is not None:
+            self.active = m.get('Active')
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Owner') is not None:
+            self.owner = m.get('Owner')
+        if m.get('TagOptionId') is not None:
+            self.tag_option_id = m.get('TagOptionId')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class GetProductAsAdminResponseBody(TeaModel):
     def __init__(
         self,
         product_detail: GetProductAsAdminResponseBodyProductDetail = None,
         request_id: str = None,
+        tag_options: List[GetProductAsAdminResponseBodyTagOptions] = None,
     ):
         # The information about the product.
         self.product_detail = product_detail
         # The ID of the request.
         self.request_id = request_id
+        self.tag_options = tag_options
 
     def validate(self):
         if self.product_detail:
             self.product_detail.validate()
+        if self.tag_options:
+            for k in self.tag_options:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.product_detail is not None:
             result['ProductDetail'] = self.product_detail.to_map()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
+        result['TagOptions'] = []
+        if self.tag_options is not None:
+            for k in self.tag_options:
+                result['TagOptions'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ProductDetail') is not None:
             temp_model = GetProductAsAdminResponseBodyProductDetail()
             self.product_detail = temp_model.from_map(m['ProductDetail'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        self.tag_options = []
+        if m.get('TagOptions') is not None:
+            for k in m.get('TagOptions'):
+                temp_model = GetProductAsAdminResponseBodyTagOptions()
+                self.tag_options.append(temp_model.from_map(k))
         return self
 
 
 class GetProductAsAdminResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -3033,26 +3745,26 @@
         has_default_launch_option: bool = None,
         product_arn: str = None,
         product_id: str = None,
         product_name: str = None,
         product_type: str = None,
         provider_name: str = None,
     ):
-        # The time when the product is created.
+        # The time when the product was created.
         # 
         # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.create_time = create_time
         # The description of the product.
         self.description = description
         # Indicates whether the default launch option exists. Valid values:
         # 
         # *   true: The default launch option exists. In this case, the PortfolioId parameter is not required when the product is launched or when the information about the product instance is updated.
         # *   false: The default launch option does not exist. In this case, the PortfolioId parameter is required when the product is launched or when the information about the product instance is updated. For more information about how to obtain the value of the PortfolioId parameter, see [ListLaunchOptions](~~ListLaunchOptions~~).
         # 
-        # >  If the product is added to only one product portfolio, the default launch option exists. If the product is added to multiple product portfolios, multiple launch options exist at the same time. However, no default launch options exist.
+        # > If the product is added to only one product portfolio, the default launch option exists. If the product is added to multiple product portfolios, multiple launch options exist at the same time. However, no default launch options exist.
         self.has_default_launch_option = has_default_launch_option
         # The Alibaba Cloud Resource Name (ARN) of the product.
         self.product_arn = product_arn
         # The ID of the product.
         self.product_id = product_id
         # The name of the product.
         self.product_name = product_name
@@ -3234,17 +3946,17 @@
         template_url: str = None,
     ):
         # Indicates whether the product version is visible to end users. Valid values:
         # 
         # *   true: The product version is visible to end users. This is the default value.
         # *   false: The product version is invisible to end users.
         self.active = active
-        # The time when the product version is created.
+        # The time when the product version was created.
         # 
-        # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
+        # The time follows the ISO 8601 standard in the YYYY-MM-DDThh:mm:ssZ format. The time is displayed in UTC.
         self.create_time = create_time
         # The description of the product version.
         self.description = description
         # The recommendation information. Valid values:
         # 
         # *   Default: No recommendation information is provided. This is the default value.
         # *   Recommended: the recommendation version.
@@ -3444,35 +4156,35 @@
         provisioned_product_name: str = None,
         provisioned_product_type: str = None,
         stack_id: str = None,
         stack_region_id: str = None,
         status: str = None,
         status_message: str = None,
     ):
-        # The time when the product instance is created.
+        # The time when the product instance was created.
         # 
         # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.create_time = create_time
-        # The ID of the task that is last run on the product instance.
+        # The ID of the task that was last run on the product instance.
         # 
         # The task can be one of the following types:
         # 
-        # *   LaunchProduct: launches the product.
-        # *   UpdateProvisionedProduct: updates the information about the product instance.
-        # *   TerminateProvisionedProduct: terminates the product instance.
+        # *   LaunchProduct: a task that launches the product.
+        # *   UpdateProvisionedProduct: a task that updates the information about the product instance.
+        # *   TerminateProvisionedProduct: a task that terminates the product instance.
         self.last_provisioning_task_id = last_provisioning_task_id
-        # The ID of the last task successfully run on the product instance.
+        # The ID of the last task that was successfully run on the product instance.
         # 
         # The task can be one of the following types:
         # 
-        # *   LaunchProduct: launches the product.
-        # *   UpdateProvisionedProduct: updates the information about the product instance.
-        # *   TerminateProvisionedProduct: terminates the product instance.
+        # *   LaunchProduct: a task that launches the product.
+        # *   UpdateProvisionedProduct: a task that updates the information about the product instance.
+        # *   TerminateProvisionedProduct: a task that terminates the product instance.
         self.last_successful_provisioning_task_id = last_successful_provisioning_task_id
-        # The ID of the task that is last run.
+        # The ID of the task that was last run.
         self.last_task_id = last_task_id
         # The ID of the RAM entity to which the product instance belongs.
         self.owner_principal_id = owner_principal_id
         # The type of the Resource Access Management (RAM) entity to which the product instance belongs. Valid values:
         # 
         # *   RamUser: a RAM user
         # *   RamRole: a RAM role
@@ -3491,29 +4203,29 @@
         self.provisioned_product_arn = provisioned_product_arn
         # The ID of the product instance.
         self.provisioned_product_id = provisioned_product_id
         # The name of the product instance.
         self.provisioned_product_name = provisioned_product_name
         # The type of the product instance.
         # 
-        # The value is fixed as RosStack, which indicates a ROS stack.
+        # The value is fixed as RosStack, which indicates an ROS stack.
         self.provisioned_product_type = provisioned_product_type
         # The ID of the Resource Orchestration Service (ROS) stack.
         self.stack_id = stack_id
         # The ID of the region to which the ROS stack belongs.
         self.stack_region_id = stack_region_id
         # The state of the product instance. Valid values:
         # 
-        # *   Available: The product instance is available.
-        # *   UnderChange: The information about the product instance is being changed.
+        # *   Available: The product instance was available.
+        # *   UnderChange: The information about the product instance was being changed.
         # *   Error: An exception occurred on the product instance.
         self.status = status
-        # The message that is returned for the state.
+        # The message that is returned for the status of the product instance.
         # 
-        # >  This parameter is returned only when Error is returned for the Status parameter.
+        # > This parameter is returned only when Error is returned for the Status parameter.
         self.status_message = status_message
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4576,14 +5288,171 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetProvisionedProductPlanResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetTagOptionRequest(TeaModel):
+    def __init__(
+        self,
+        tag_option_id: str = None,
+    ):
+        self.tag_option_id = tag_option_id
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
+        if self.tag_option_id is not None:
+            result['TagOptionId'] = self.tag_option_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TagOptionId') is not None:
+            self.tag_option_id = m.get('TagOptionId')
+        return self
+
+
+class GetTagOptionResponseBodyTagOptionDetail(TeaModel):
+    def __init__(
+        self,
+        active: bool = None,
+        key: str = None,
+        owner: str = None,
+        tag_option_id: str = None,
+        value: str = None,
+    ):
+        self.active = active
+        self.key = key
+        self.owner = owner
+        self.tag_option_id = tag_option_id
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
+        if self.active is not None:
+            result['Active'] = self.active
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.owner is not None:
+            result['Owner'] = self.owner
+        if self.tag_option_id is not None:
+            result['TagOptionId'] = self.tag_option_id
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Active') is not None:
+            self.active = m.get('Active')
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Owner') is not None:
+            self.owner = m.get('Owner')
+        if m.get('TagOptionId') is not None:
+            self.tag_option_id = m.get('TagOptionId')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class GetTagOptionResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        tag_option_detail: GetTagOptionResponseBodyTagOptionDetail = None,
+    ):
+        self.request_id = request_id
+        self.tag_option_detail = tag_option_detail
+
+    def validate(self):
+        if self.tag_option_detail:
+            self.tag_option_detail.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.tag_option_detail is not None:
+            result['TagOptionDetail'] = self.tag_option_detail.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TagOptionDetail') is not None:
+            temp_model = GetTagOptionResponseBodyTagOptionDetail()
+            self.tag_option_detail = temp_model.from_map(m['TagOptionDetail'])
+        return self
+
+
+class GetTagOptionResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetTagOptionResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetTagOptionResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetTaskRequest(TeaModel):
     def __init__(
         self,
         task_id: str = None,
     ):
         # The ID of the task.
         self.task_id = task_id
@@ -4611,24 +5480,24 @@
 class GetTaskResponseBodyTaskDetailLogTerraformLogs(TeaModel):
     def __init__(
         self,
         command: str = None,
         content: str = None,
         stream: str = None,
     ):
-        # The name of the Terraform command. Valid values:
+        # The name of the Terraform command that is run. Valid values:
         # 
         # *   apply
         # *   plan
         # *   destroy
         # *   version
         # 
         # For more information about Terraform commands, see [Basic CLI Features](https://www.terraform.io/cli/commands).
         self.command = command
-        # The content of the output stream that is returned after you run the command.
+        # The content of the output stream that is returned after the command is run.
         self.content = content
         # The output stream. Valid values:
         # 
         # *   stdout: a standard output stream
         # *   stderr: a standard error stream
         self.stream = stream
 
@@ -4661,15 +5530,15 @@
 
 
 class GetTaskResponseBodyTaskDetailLog(TeaModel):
     def __init__(
         self,
         terraform_logs: List[GetTaskResponseBodyTaskDetailLogTerraformLogs] = None,
     ):
-        # An array that consists of Terraform logs.
+        # The Terraform logs.
         self.terraform_logs = terraform_logs
 
     def validate(self):
         if self.terraform_logs:
             for k in self.terraform_logs:
                 if k:
                     k.validate()
@@ -4699,19 +5568,19 @@
 class GetTaskResponseBodyTaskDetailOutputs(TeaModel):
     def __init__(
         self,
         description: str = None,
         output_key: str = None,
         output_value: str = None,
     ):
-        # The description of the parameter that is specified in the output of the template.
+        # The description of the output parameter for the template.
         self.description = description
-        # The name of the parameter that is specified in the output of the template.
+        # The name of the output parameter for the template.
         self.output_key = output_key
-        # The value of the parameter that is specified in the output of the template.
+        # The value of the output parameter for the template.
         self.output_value = output_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4740,17 +5609,17 @@
 
 class GetTaskResponseBodyTaskDetailParameters(TeaModel):
     def __init__(
         self,
         parameter_key: str = None,
         parameter_value: str = None,
     ):
-        # The name of the parameter in the template.
+        # The name of the input parameter for the template.
         self.parameter_key = parameter_key
-        # The value of the parameter in the template.
+        # The value of the input parameter for the template.
         self.parameter_value = parameter_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4775,21 +5644,15 @@
 
 class GetTaskResponseBodyTaskDetailTaskTags(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # The tag key of the custom tag.
-        # 
-        # The tag key can be up to 128 characters in length, and cannot start with `acs:` or `aliyun`. The tag key cannot contain `http://` or `https://`.
         self.key = key
-        # The tag value of the custom tag.
-        # 
-        # The tag value can be up to 128 characters in length, and cannot start with `acs:`. The tag value cannot contain `http://` or `https://`.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4835,51 +5698,50 @@
     ):
         # The time when the task was created.
         # 
         # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.create_time = create_time
         # The logs of the product instance.
         self.log = log
-        # An array that consists of the parameters specified in the output of the template.
+        # The output parameters of the template.
         self.outputs = outputs
-        # An array that consists of the parameters in the template.
+        # The input parameters of the template.
         self.parameters = parameters
         # The ID of the product portfolio.
         self.portfolio_id = portfolio_id
         # The ID of the product.
         self.product_id = product_id
         # The name of the product.
         self.product_name = product_name
         # The ID of the product version.
         self.product_version_id = product_version_id
-        # The name for the version of the product.
+        # The name of the product version.
         self.product_version_name = product_version_name
         # The ID of the product instance.
         self.provisioned_product_id = provisioned_product_id
         # The name of the product instance.
         self.provisioned_product_name = provisioned_product_name
-        # The status of the task. Valid values:
+        # The state of the task. Valid values:
         # 
         # *   Succeeded: The task was successful.
-        # *   InProgress: The task is in progress.
+        # *   InProgress: The task was in progress.
         # *   Failed: The task failed.
         self.status = status
-        # The message that is returned for the state.
+        # The message that is returned for the status of the task.
         # 
         # > This parameter is returned only when Failed is returned for the Status parameter.
         self.status_message = status_message
         # The ID of the task.
         self.task_id = task_id
-        # An array consisting of custom tags that are specified by the end user.
         self.task_tags = task_tags
         # The type of the task. Valid values:
         # 
-        # *   LaunchProduct: launches the product.
-        # *   UpdateProvisionedProduct: updates the information about the product instance.
-        # *   TerminateProvisionedProduct: terminates the product instance.
+        # *   LaunchProduct: a task that launches the product.
+        # *   UpdateProvisionedProduct: a task that updates the information about the product instance.
+        # *   TerminateProvisionedProduct: a task that terminates the product instance.
         self.task_type = task_type
         # The time when the task was last modified.
         # 
         # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.update_time = update_time
 
     def validate(self):
@@ -4999,15 +5861,15 @@
     def __init__(
         self,
         request_id: str = None,
         task_detail: GetTaskResponseBodyTaskDetail = None,
     ):
         # The ID of the request.
         self.request_id = request_id
-        # The details of the download task.
+        # The details of the task.
         self.task_detail = task_detail
 
     def validate(self):
         if self.task_detail:
             self.task_detail.validate()
 
     def to_map(self):
@@ -5480,35 +6342,35 @@
         page_number: int = None,
         page_size: int = None,
         product_id: str = None,
         scope: str = None,
         sort_by: str = None,
         sort_order: str = None,
     ):
-        # The filter condition.
+        # The filter conditions.
         self.filters = filters
         # The number of the page to return.
         # 
         # Pages start from page 1. Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page.
         # 
-        # Valid values: 1 to 100. Minimum value: 1. Default value: 10.
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
         # The ID of the product.
         self.product_id = product_id
         # The query scope. Valid values:
         # 
         # *   Local: the product portfolios that are created by using the current account. This is the default value.
         # *   Import: the product portfolios that are imported from other accounts.
-        # *   All: All available product portfolios.
+        # *   All: all available product portfolios.
         self.scope = scope
         # The field that is used to sort the queried data.
         # 
-        # The value is fixed as CreateTime, which specifies the creation time of product portfolios.
+        # The value is fixed as CreateTime, which specifies the time when the product portfolio was created.
         self.sort_by = sort_by
         # The order in which you want to sort the queried data. Valid values:
         # 
         # *   Asc: the ascending order
         # *   Desc: the descending order
         self.sort_order = sort_order
 
@@ -5570,15 +6432,15 @@
         create_time: str = None,
         description: str = None,
         portfolio_arn: str = None,
         portfolio_id: str = None,
         portfolio_name: str = None,
         provider_name: str = None,
     ):
-        # The time when the product portfolio is created.
+        # The time when the product portfolio was created.
         # 
         # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.create_time = create_time
         # The description of the product portfolio.
         self.description = description
         # The Alibaba Cloud Resource Name (ARN) of the product portfolio.
         self.portfolio_arn = portfolio_arn
@@ -5638,15 +6500,15 @@
         request_id: str = None,
         total_count: int = None,
     ):
         # The page number of the returned page.
         self.page_number = page_number
         # The number of entries returned per page.
         self.page_size = page_size
-        # An array that consists of the product portfolios.
+        # The product portfolios.
         self.portfolio_details = portfolio_details
         # The ID of the request.
         self.request_id = request_id
         # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
@@ -5805,15 +6667,15 @@
 
 class ListPrincipalsResponseBody(TeaModel):
     def __init__(
         self,
         principals: List[ListPrincipalsResponseBodyPrincipals] = None,
         request_id: str = None,
     ):
-        # An array that consists of RAM entities.
+        # The RAM entities.
         self.principals = principals
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.principals:
             for k in self.principals:
@@ -5891,15 +6753,15 @@
 
 
 class ListProductVersionsRequest(TeaModel):
     def __init__(
         self,
         product_id: str = None,
     ):
-        # The ID of the product to which the product version belongs.
+        # The ID of the product.
         self.product_id = product_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5927,40 +6789,40 @@
         guidance: str = None,
         product_id: str = None,
         product_version_id: str = None,
         product_version_name: str = None,
         template_type: str = None,
         template_url: str = None,
     ):
-        # Indicates whether the product version is visible to end users. Valid values:
+        # Indicates whether the product version is enabled. Valid values:
         # 
-        # true: The product version is visible to end users. This is the default value. false: The product version is invisible to end users.
+        # true: The product version is enabled. This is the default value. false: The product version is disabled.
         self.active = active
-        # The time when the product version is created.
+        # The time when the product version was created.
         # 
         # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.create_time = create_time
         # The description of the product version.
         self.description = description
         # The recommendation information. Valid values:
         # 
         # *   Default: No recommendation information is provided. This is the default value.
-        # *   Recommended: the recommendation version.
+        # *   Recommended: the recommended version.
         # *   Latest: the latest version.
-        # *   Deprecated: the version that is about to be deprecated.
+        # *   Deprecated: the version that is about to be discontinued.
         self.guidance = guidance
         # The ID of the product to which the product version belongs.
         self.product_id = product_id
         # The ID of the product version.
         self.product_version_id = product_version_id
         # The name of the product version.
         self.product_version_name = product_version_name
         # The type of the template.
         # 
-        # The value is fixed as RosTerraformTemplate, which indicates that the Terraform template is supported by Resource Orchestration Service (ROS).
+        # The value is fixed as RosTerraformTemplate, which indicates the Terraform template that is supported by Resource Orchestration Service (ROS).
         self.template_type = template_type
         # The URL of the template.
         self.template_url = template_url
 
     def validate(self):
         pass
 
@@ -6015,15 +6877,15 @@
 
 class ListProductVersionsResponseBody(TeaModel):
     def __init__(
         self,
         product_version_details: List[ListProductVersionsResponseBodyProductVersionDetails] = None,
         request_id: str = None,
     ):
-        # An array that consists of the product versions.
+        # The versions of the product.
         self.product_version_details = product_version_details
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.product_version_details:
             for k in self.product_version_details:
@@ -6145,37 +7007,37 @@
         page_number: int = None,
         page_size: int = None,
         portfolio_id: str = None,
         scope: str = None,
         sort_by: str = None,
         sort_order: str = None,
     ):
-        # An array that consists of filter conditions.
+        # The filter conditions.
         self.filters = filters
         # The number of the page to return.
         # 
         # Pages start from page 1. Default value: 1.
         self.page_number = page_number
-        # The number of entries returned per page.
+        # The number of entries to return on each page.
         # 
-        # Valid values: 1 to 100. Pages start from page 1. Default value: 10.
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
         # The ID of the product portfolio.
         self.portfolio_id = portfolio_id
         # The query scope. Valid values:
         # 
         # *   Local: the products that are created by using the current account. This is the default value.
         # *   Import: the products that are imported from other accounts.
         # *   All: all available products.
         self.scope = scope
-        # The information based on which you want to sort the products.
+        # The field that is used to sort the queried data.
         # 
-        # The value is fixed as CreateTime, which specifies the creation time of products.
+        # Set the value to CreateTime, which specifies the time when the product was created.
         self.sort_by = sort_by
-        # The order in which you want to sort the query results. Valid values:
+        # The order in which you want to sort the queried data. Valid values:
         # 
         # *   Asc: the ascending order
         # *   Desc: the descending order
         self.sort_order = sort_order
 
     def validate(self):
         if self.filters:
@@ -6250,15 +7112,15 @@
         self.product_arn = product_arn
         # The ID of the product.
         self.product_id = product_id
         # The name of the product.
         self.product_name = product_name
         # The type of the product.
         # 
-        # The value is fixed as Ros, which specifies Resource Orchestration Service (ROS).
+        # The value is fixed as Ros, which indicates Resource Orchestration Service (ROS).
         self.product_type = product_type
         # The provider of the product.
         self.provider_name = provider_name
 
     def validate(self):
         pass
 
@@ -6308,19 +7170,19 @@
         self,
         page_number: int = None,
         page_size: int = None,
         product_details: List[ListProductsAsAdminResponseBodyProductDetails] = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The number of the returned page.
+        # The page number of the returned page.
         self.page_number = page_number
         # The number of entries returned per page.
         self.page_size = page_size
-        # An array that consists of products.
+        # The products.
         self.product_details = product_details
         # The ID of the request.
         self.request_id = request_id
         # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
@@ -6454,27 +7316,27 @@
         self,
         filters: List[ListProductsAsEndUserRequestFilters] = None,
         page_number: int = None,
         page_size: int = None,
         sort_by: str = None,
         sort_order: str = None,
     ):
-        # An array that consists of filter conditions.
+        # The filter conditions.
         self.filters = filters
         # The number of the page to return.
         # 
         # Pages start from page 1. Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page.
         # 
-        # Valid values: 1 to 100. Minimum value: 1. Default value: 10.
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
         # The field that is used to sort the queried data.
         # 
-        # The value is fixed as CreateTime, which specifies the creation time of products.
+        # Set the value to CreateTime, which specifies the time when the product was created.
         self.sort_by = sort_by
         # The order in which you want to sort the queried data. Valid values:
         # 
         # *   Asc: the ascending order
         # *   Desc: the descending order
         self.sort_order = sort_order
 
@@ -6530,26 +7392,26 @@
         has_default_launch_option: bool = None,
         product_arn: str = None,
         product_id: str = None,
         product_name: str = None,
         product_type: str = None,
         provider_name: str = None,
     ):
-        # The time when the product is created.
+        # The time when the product was created.
         # 
         # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.create_time = create_time
         # The description of the product.
         self.description = description
         # Indicates whether the default launch option exists. Valid values:
         # 
         # *   true: The default launch option exists. In this case, the PortfolioId parameter is not required when the product is launched or when the information about the product instance is updated.
         # *   false: The default launch option does not exist. In this case, the PortfolioId parameter is required when the product is launched or when the information about the product instance is updated. For more information about how to obtain the value of the PortfolioId parameter, see [ListLaunchOptions](~~ListLaunchOptions~~).
         # 
-        # >  If the product is added to only one product portfolio, the default launch option exists. If the product is added to multiple product portfolios, multiple launch options exist at the same time. However, no default launch options exist.
+        # > If the product is added to only one product portfolio, the default launch option exists. If the product is added to multiple product portfolios, multiple launch options exist at the same time. However, no default launch options exist.
         self.has_default_launch_option = has_default_launch_option
         # The Alibaba Cloud Resource Name (ARN) of the product.
         self.product_arn = product_arn
         # The ID of the product.
         self.product_id = product_id
         # The name of the product.
         self.product_name = product_name
@@ -6617,19 +7479,19 @@
         request_id: str = None,
         total_count: int = None,
     ):
         # The page number of the returned page.
         self.page_number = page_number
         # The number of entries returned per page.
         self.page_size = page_size
-        # An array that consists of products.
+        # The products.
         self.product_summaries = product_summaries
         # The ID of the request.
         self.request_id = request_id
-        # The total number of returned rows.
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.product_summaries:
             for k in self.product_summaries:
                 if k:
                     k.validate()
@@ -7466,27 +8328,27 @@
         sort_order: str = None,
     ):
         # The access filter. Valid values:
         # 
         # *   User: queries the product instances that are created by the current requester. This is the default value.
         # *   Account: queries the product instances that belong to the current Alibaba Cloud account.
         self.access_level_filter = access_level_filter
-        # The filter condition.
+        # The filter conditions.
         self.filters = filters
         # The number of the page to return.
         # 
         # Pages start from page 1. Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page.
         # 
-        # Valid values: 1 to 100. Minimum value: 1. Default value: 10.
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
         # The field that is used to sort the queried data.
         # 
-        # The value is fixed as CreateTime, which specifies the creation time of product instances.
+        # Set the value to CreateTime, which specifies the time when the product instance was created.
         self.sort_by = sort_by
         # The order in which you want to sort the queried data. Valid values:
         # 
         # *   Asc: the ascending order
         # *   Desc: the descending order
         self.sort_order = sort_order
 
@@ -7557,35 +8419,35 @@
         provisioned_product_name: str = None,
         provisioned_product_type: str = None,
         stack_id: str = None,
         stack_region_id: str = None,
         status: str = None,
         status_message: str = None,
     ):
-        # The time when the product instance is created.
+        # The time when the product instance was created.
         # 
         # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.create_time = create_time
-        # The ID of the task that is last run on the product instance.
+        # The ID of the task that was last run on the product instance.
         # 
         # The task can be one of the following types:
         # 
-        # *   LaunchProduct: launches the product.
-        # *   UpdateProvisionedProduct: updates the information about the product instance.
-        # *   TerminateProvisionedProduct: terminates the product instance.
+        # *   LaunchProduct: a task that launches the product.
+        # *   UpdateProvisionedProduct: a task that updates the information about the product instance.
+        # *   TerminateProvisionedProduct: a task that terminates the product instance.
         self.last_provisioning_task_id = last_provisioning_task_id
-        # The ID of the last task successfully run on the product instance.
+        # The ID of the last task that was successfully run on the product instance.
         # 
         # The task can be one of the following types:
         # 
-        # *   LaunchProduct: launches the product.
-        # *   UpdateProvisionedProduct: updates the information about the product instance.
-        # *   TerminateProvisionedProduct: terminates the product instance.
+        # *   LaunchProduct: a task that launches the product.
+        # *   UpdateProvisionedProduct: a task that updates the information about the product instance.
+        # *   TerminateProvisionedProduct: a task that terminates the product instance.
         self.last_successful_provisioning_task_id = last_successful_provisioning_task_id
-        # The ID of the task that is last run.
+        # The ID of the task that was last run.
         self.last_task_id = last_task_id
         # The ID of the RAM entity to which the product instance belongs.
         self.owner_principal_id = owner_principal_id
         # The type of the Resource Access Management (RAM) entity to which the product instance belongs. Valid values:
         # 
         # *   RamUser: a RAM user
         # *   RamRole: a RAM role
@@ -7604,29 +8466,29 @@
         self.provisioned_product_arn = provisioned_product_arn
         # The ID of the product instance.
         self.provisioned_product_id = provisioned_product_id
         # The name of the product instance.
         self.provisioned_product_name = provisioned_product_name
         # The type of the product instance.
         # 
-        # The value is fixed as RosStack, which indicates a ROS stack.
+        # The value is fixed as RosStack, which indicates an ROS stack.
         self.provisioned_product_type = provisioned_product_type
         # The ID of the Resource Orchestration Service (ROS) stack.
         self.stack_id = stack_id
         # The ID of the region to which the ROS stack belongs.
         self.stack_region_id = stack_region_id
         # The state of the product instance. Valid values:
         # 
-        # *   Available: The product instance is available.
-        # *   UnderChange: The information about the product instance is being changed.
+        # *   Available: The product instance was available.
+        # *   UnderChange: The information about the product instance was being changed.
         # *   Error: An exception occurred on the product instance.
         self.status = status
-        # The description of the state.
+        # The message that is returned for the status of the product instance.
         # 
-        # >  This parameter is returned only when Error is returned for the Status parameter.
+        # > This parameter is returned only when Error is returned for the Status parameter.
         self.status_message = status_message
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7726,15 +8588,15 @@
         request_id: str = None,
         total_count: int = None,
     ):
         # The page number of the returned page.
         self.page_number = page_number
         # The number of entries returned per page.
         self.page_size = page_size
-        # An array that consists of product instances.
+        # The product instances.
         self.provisioned_product_details = provisioned_product_details
         # The ID of the request.
         self.request_id = request_id
         # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
@@ -7869,15 +8731,15 @@
 
 class ListRegionsResponseBody(TeaModel):
     def __init__(
         self,
         regions: List[ListRegionsResponseBodyRegions] = None,
         request_id: str = None,
     ):
-        # An array that consists of regions.
+        # The details of regions.
         self.regions = regions
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.regions:
             for k in self.regions:
@@ -7950,14 +8812,516 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListRegionsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListResourcesForTagOptionRequest(TeaModel):
+    def __init__(
+        self,
+        page_number: int = None,
+        page_size: int = None,
+        resource_type: str = None,
+        tag_option_id: str = None,
+    ):
+        self.page_number = page_number
+        self.page_size = page_size
+        self.resource_type = resource_type
+        self.tag_option_id = tag_option_id
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
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        if self.tag_option_id is not None:
+            result['TagOptionId'] = self.tag_option_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        if m.get('TagOptionId') is not None:
+            self.tag_option_id = m.get('TagOptionId')
+        return self
+
+
+class ListResourcesForTagOptionResponseBodyResourceDetails(TeaModel):
+    def __init__(
+        self,
+        create_time: str = None,
+        description: str = None,
+        resource_arn: str = None,
+        resource_id: str = None,
+        resource_name: str = None,
+    ):
+        self.create_time = create_time
+        self.description = description
+        self.resource_arn = resource_arn
+        self.resource_id = resource_id
+        self.resource_name = resource_name
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
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.resource_arn is not None:
+            result['ResourceArn'] = self.resource_arn
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_name is not None:
+            result['ResourceName'] = self.resource_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('ResourceArn') is not None:
+            self.resource_arn = m.get('ResourceArn')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceName') is not None:
+            self.resource_name = m.get('ResourceName')
+        return self
+
+
+class ListResourcesForTagOptionResponseBody(TeaModel):
+    def __init__(
+        self,
+        page_number: int = None,
+        page_size: int = None,
+        request_id: str = None,
+        resource_details: List[ListResourcesForTagOptionResponseBodyResourceDetails] = None,
+        total_count: int = None,
+    ):
+        self.page_number = page_number
+        self.page_size = page_size
+        self.request_id = request_id
+        self.resource_details = resource_details
+        self.total_count = total_count
+
+    def validate(self):
+        if self.resource_details:
+            for k in self.resource_details:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['ResourceDetails'] = []
+        if self.resource_details is not None:
+            for k in self.resource_details:
+                result['ResourceDetails'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.resource_details = []
+        if m.get('ResourceDetails') is not None:
+            for k in m.get('ResourceDetails'):
+                temp_model = ListResourcesForTagOptionResponseBodyResourceDetails()
+                self.resource_details.append(temp_model.from_map(k))
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListResourcesForTagOptionResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListResourcesForTagOptionResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListResourcesForTagOptionResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListTagOptionsRequestFilters(TeaModel):
+    def __init__(
+        self,
+        active: bool = None,
+        full_text_search: str = None,
+        key: str = None,
+        value: str = None,
+    ):
+        self.active = active
+        self.full_text_search = full_text_search
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
+        if self.active is not None:
+            result['Active'] = self.active
+        if self.full_text_search is not None:
+            result['FullTextSearch'] = self.full_text_search
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Active') is not None:
+            self.active = m.get('Active')
+        if m.get('FullTextSearch') is not None:
+            self.full_text_search = m.get('FullTextSearch')
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListTagOptionsRequest(TeaModel):
+    def __init__(
+        self,
+        filters: ListTagOptionsRequestFilters = None,
+        page_number: int = None,
+        page_size: int = None,
+        sort_by: str = None,
+        sort_order: str = None,
+    ):
+        self.filters = filters
+        self.page_number = page_number
+        self.page_size = page_size
+        self.sort_by = sort_by
+        self.sort_order = sort_order
+
+    def validate(self):
+        if self.filters:
+            self.filters.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.filters is not None:
+            result['Filters'] = self.filters.to_map()
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.sort_by is not None:
+            result['SortBy'] = self.sort_by
+        if self.sort_order is not None:
+            result['SortOrder'] = self.sort_order
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Filters') is not None:
+            temp_model = ListTagOptionsRequestFilters()
+            self.filters = temp_model.from_map(m['Filters'])
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('SortBy') is not None:
+            self.sort_by = m.get('SortBy')
+        if m.get('SortOrder') is not None:
+            self.sort_order = m.get('SortOrder')
+        return self
+
+
+class ListTagOptionsShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        filters_shrink: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        sort_by: str = None,
+        sort_order: str = None,
+    ):
+        self.filters_shrink = filters_shrink
+        self.page_number = page_number
+        self.page_size = page_size
+        self.sort_by = sort_by
+        self.sort_order = sort_order
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
+        if self.filters_shrink is not None:
+            result['Filters'] = self.filters_shrink
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.sort_by is not None:
+            result['SortBy'] = self.sort_by
+        if self.sort_order is not None:
+            result['SortOrder'] = self.sort_order
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Filters') is not None:
+            self.filters_shrink = m.get('Filters')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('SortBy') is not None:
+            self.sort_by = m.get('SortBy')
+        if m.get('SortOrder') is not None:
+            self.sort_order = m.get('SortOrder')
+        return self
+
+
+class ListTagOptionsResponseBodyTagOptionDetails(TeaModel):
+    def __init__(
+        self,
+        active: bool = None,
+        key: str = None,
+        owner: str = None,
+        tag_option_id: str = None,
+        value: str = None,
+    ):
+        self.active = active
+        self.key = key
+        self.owner = owner
+        self.tag_option_id = tag_option_id
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
+        if self.active is not None:
+            result['Active'] = self.active
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.owner is not None:
+            result['Owner'] = self.owner
+        if self.tag_option_id is not None:
+            result['TagOptionId'] = self.tag_option_id
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Active') is not None:
+            self.active = m.get('Active')
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Owner') is not None:
+            self.owner = m.get('Owner')
+        if m.get('TagOptionId') is not None:
+            self.tag_option_id = m.get('TagOptionId')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListTagOptionsResponseBody(TeaModel):
+    def __init__(
+        self,
+        page_number: int = None,
+        page_size: int = None,
+        request_id: str = None,
+        tag_option_details: List[ListTagOptionsResponseBodyTagOptionDetails] = None,
+        total_count: int = None,
+    ):
+        self.page_number = page_number
+        self.page_size = page_size
+        self.request_id = request_id
+        self.tag_option_details = tag_option_details
+        self.total_count = total_count
+
+    def validate(self):
+        if self.tag_option_details:
+            for k in self.tag_option_details:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['TagOptionDetails'] = []
+        if self.tag_option_details is not None:
+            for k in self.tag_option_details:
+                result['TagOptionDetails'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.tag_option_details = []
+        if m.get('TagOptionDetails') is not None:
+            for k in m.get('TagOptionDetails'):
+                temp_model = ListTagOptionsResponseBodyTagOptionDetails()
+                self.tag_option_details.append(temp_model.from_map(k))
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListTagOptionsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListTagOptionsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListTagOptionsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListTasksRequest(TeaModel):
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         provisioned_product_id: str = None,
         sort_by: str = None,
@@ -7965,21 +9329,21 @@
     ):
         # The number of the page to return.
         # 
         # Pages start from page 1. Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page.
         # 
-        # Valid values: 1 to 100. Minimum value: 1. Default value: 10.
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
         # The ID of the product instance.
         self.provisioned_product_id = provisioned_product_id
         # The field that is used to sort the queried data.
         # 
-        # The value is fixed as CreateTime, which specifies the creation time of tasks.
+        # Set the value to CreateTime, which specifies the time when the task was created.
         self.sort_by = sort_by
         # The order in which you want to sort the queried data. Valid values:
         # 
         # *   Asc: the ascending order
         # *   Desc: the descending order
         self.sort_order = sort_order
 
@@ -8022,24 +9386,24 @@
 class ListTasksResponseBodyTaskDetailsLogTerraformLogs(TeaModel):
     def __init__(
         self,
         command: str = None,
         content: str = None,
         stream: str = None,
     ):
-        # The name of the Terraform command. Valid values:
+        # The name of the Terraform command that is run. Valid values:
         # 
         # *   apply
         # *   plan
         # *   destroy
         # *   version
         # 
         # For more information about Terraform commands, see [Basic CLI Features](https://www.terraform.io/cli/commands).
         self.command = command
-        # The content of the output stream that is returned after you run the command.
+        # The content of the output stream that is returned after the command is run.
         self.content = content
         # The output stream. Valid values:
         # 
         # *   stdout: a standard output stream
         # *   stderr: a standard error stream
         self.stream = stream
 
@@ -8072,15 +9436,15 @@
 
 
 class ListTasksResponseBodyTaskDetailsLog(TeaModel):
     def __init__(
         self,
         terraform_logs: List[ListTasksResponseBodyTaskDetailsLogTerraformLogs] = None,
     ):
-        # An array that consists of Terraform logs.
+        # The Terraform logs.
         self.terraform_logs = terraform_logs
 
     def validate(self):
         if self.terraform_logs:
             for k in self.terraform_logs:
                 if k:
                     k.validate()
@@ -8110,19 +9474,19 @@
 class ListTasksResponseBodyTaskDetailsOutputs(TeaModel):
     def __init__(
         self,
         description: str = None,
         output_key: str = None,
         output_value: str = None,
     ):
-        # The description of the parameter that is specified in the output of the template.
+        # The description of the output parameter for the template.
         self.description = description
-        # The name of the parameter that is specified in the output of the template.
+        # The name of the output parameter for the template.
         self.output_key = output_key
-        # The value of the parameter that is specified in the output of the template.
+        # The value of the output parameter for the template.
         self.output_value = output_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8151,17 +9515,17 @@
 
 class ListTasksResponseBodyTaskDetailsParameters(TeaModel):
     def __init__(
         self,
         parameter_key: str = None,
         parameter_value: str = None,
     ):
-        # The name of the parameter in the template.
+        # The name of the input parameter for the template.
         self.parameter_key = parameter_key
-        # The value of the parameter in the template.
+        # The value of the input parameter for the template.
         self.parameter_value = parameter_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8200,55 +9564,55 @@
         provisioned_product_name: str = None,
         status: str = None,
         status_message: str = None,
         task_id: str = None,
         task_type: str = None,
         update_time: str = None,
     ):
-        # The time when the task is created.
+        # The time when the task was created.
         # 
         # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.create_time = create_time
         # The logs of the product instance.
         self.log = log
-        # An array that consists of the parameters specified in the output of the template.
+        # The output parameters of the template.
         self.outputs = outputs
-        # An array that consists of the parameters in the template. The parameters are specified by the administrator.
+        # The input parameters of the template.
         self.parameters = parameters
         # The ID of the product portfolio.
         self.portfolio_id = portfolio_id
         # The ID of the product.
         self.product_id = product_id
         # The name of the product.
         self.product_name = product_name
         # The ID of the product version.
         self.product_version_id = product_version_id
-        # The name for the version of the product.
+        # The name of the product version.
         self.product_version_name = product_version_name
         # The ID of the product instance.
         self.provisioned_product_id = provisioned_product_id
         # The name of the product instance.
         self.provisioned_product_name = provisioned_product_name
         # The state of the task. Valid values:
         # 
-        # *   Succeeded: The task is successful.
-        # *   InProgress: The task is in progress.
+        # *   Succeeded: The task was successful.
+        # *   InProgress: The task was in progress.
         # *   Failed: The task failed.
         self.status = status
-        # The message that is returned for the state.
+        # The message that is returned for the status of the task.
         # 
-        # >  This parameter is returned only when Failed is returned for the Status parameter.
+        # > This parameter is returned only when Failed is returned for the Status parameter.
         self.status_message = status_message
         # The ID of the task.
         self.task_id = task_id
         # The type of the task. Valid values:
         # 
-        # *   LaunchProduct: launches the product.
-        # *   UpdateProvisionedProduct: updates the information about the product instance.
-        # *   TerminateProvisionedProduct: terminates the product instance.
+        # *   LaunchProduct: a task that launches the product.
+        # *   UpdateProvisionedProduct: a task that updates the information about the product instance.
+        # *   TerminateProvisionedProduct: a task that terminates the product instance.
         self.task_type = task_type
         # The time when the task was last modified.
         # 
         # The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.update_time = update_time
 
     def validate(self):
@@ -8362,17 +9726,17 @@
     ):
         # The page number of the returned page.
         self.page_number = page_number
         # The number of entries returned per page.
         self.page_size = page_size
         # The ID of the request.
         self.request_id = request_id
-        # An array that consists of tasks.
+        # The tasks.
         self.task_details = task_details
-        # The total number of returned rows.
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.task_details:
             for k in self.task_details:
                 if k:
                     k.validate()
@@ -8562,15 +9926,15 @@
 class UpdateConstraintRequest(TeaModel):
     def __init__(
         self,
         config: str = None,
         constraint_id: str = None,
         description: str = None,
     ):
-        # The configuration of the constraint.
+        # The configurations of the constraint.
         # 
         # Format: { "LocalRoleName": "\<role_name>" }.
         self.config = config
         # The ID of the constraint.
         self.constraint_id = constraint_id
         # The description of the constraint.
         # 
@@ -8957,29 +10321,29 @@
         self,
         active: bool = None,
         description: str = None,
         guidance: str = None,
         product_version_id: str = None,
         product_version_name: str = None,
     ):
-        # Specifies whether the product version is visible to end users. Valid values:
+        # Specifies whether to enable the product version. Valid values:
         # 
-        # *   true: The product version is visible to end users. This is the default value.
-        # *   false: The product version is invisible to end users.
+        # *   true: enables the product version. This is the default value.
+        # *   false: disables the product version.
         self.active = active
         # The description of the product version.
         # 
         # The value must be 1 to 128 characters in length.
         self.description = description
         # The recommendation information. Valid values:
         # 
         # *   Default: No recommendation information is provided. This is the default value.
-        # *   Recommended: the recommendation version.
+        # *   Recommended: the recommended version.
         # *   Latest: the latest version.
-        # *   Deprecated: the version that is about to be deprecated.
+        # *   Deprecated: the version that is about to be discontinued.
         self.guidance = guidance
         # The ID of the product version.
         self.product_version_id = product_version_id
         # The name of the product version.
         # 
         # The value must be 1 to 128 characters in length.
         self.product_version_name = product_version_name
@@ -9101,17 +10465,17 @@
 
 class UpdateProvisionedProductRequestParameters(TeaModel):
     def __init__(
         self,
         parameter_key: str = None,
         parameter_value: str = None,
     ):
-        # The name of the parameter in the template.
+        # The name of the input parameter for the template.
         self.parameter_key = parameter_key
-        # The value of the parameter in the template.
+        # The value of the input parameter for the template.
         self.parameter_value = parameter_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9136,15 +10500,21 @@
 
 class UpdateProvisionedProductRequestTags(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # The tag key of the custom tag.
+        # 
+        # The tag key must be 1 to 128 characters in length and cannot contain `http://` or `https://`. It cannot start with `acs:` or `aliyun`.
         self.key = key
+        # The tag value of the custom tag.
+        # 
+        # The tag value can be up to 128 characters in length and cannot start with `acs:`. It cannot contain `http://` or `https://`.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9173,33 +10543,43 @@
         parameters: List[UpdateProvisionedProductRequestParameters] = None,
         portfolio_id: str = None,
         product_id: str = None,
         product_version_id: str = None,
         provisioned_product_id: str = None,
         tags: List[UpdateProvisionedProductRequestTags] = None,
     ):
-        # An array that consists of the parameters in the template. The parameters are specified by the administrator.
+        # The input parameters of the template.
         # 
         # You can specify up to 200 parameters.
         # 
-        # > - This parameter is optional. If you specify the Parameters parameter, you must specify the ParameterKey and ParameterValue parameters.
-        # > - If the values of the ProductVersionId and Parameters parameters are not changed, you are not allowed to update the information about the product instance.
+        # > 
+        # *   This parameter is optional. If you specify the Parameters parameter, you must specify the ParameterKey and ParameterValue parameters.
+        # > 
+        # *   If the values of the ProductVersionId and Parameters parameters are not changed, you are not allowed to update the information about the product instance.
         self.parameters = parameters
         # The ID of the product portfolio.
         # 
-        # >  If the PortfolioId parameter is not required, you do not need to specify the PortfolioId parameter. If the PortfolioId parameter is required, you must specify the PortfolioId parameter. For more information about how to obtain the value of the PortfolioId parameter, see [ListLaunchOptions](~~ListLaunchOptions~~).
+        # > The PortfolioId parameter is not required if the default launch option exists. The PortfolioId parameter is required if the default launch option does not exist. For more information about how to obtain the value of the PortfolioId parameter, see [ListLaunchOptions](~~ListLaunchOptions~~).
         self.portfolio_id = portfolio_id
         # The ID of the product.
         self.product_id = product_id
         # The ID of the product version.
         # 
-        # >  If the values of the ProductVersionId and Parameters parameters are not changed, the information about the product instance cannot be updated.
+        # > If the values of the ProductVersionId and Parameters parameters are not changed, the information about the product instance cannot be updated.
         self.product_version_id = product_version_id
         # The ID of the product instance.
         self.provisioned_product_id = provisioned_product_id
+        # The input custom tags.
+        # 
+        # Maximum value of N: 20.
+        # 
+        # > 
+        # *   The Tags parameter is optional. If you need to specify the Tags parameter, you must specify the Tags.N.Key and Tags.N.Value parameters.
+        # > 
+        # *   The tag is propagated to each stack resource that supports the tag feature.
         self.tags = tags
 
     def validate(self):
         if self.parameters:
             for k in self.parameters:
                 if k:
                     k.validate()
@@ -9559,7 +10939,176 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpdateProvisionedProductPlanResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateTagOptionRequest(TeaModel):
+    def __init__(
+        self,
+        active: bool = None,
+        tag_option_id: str = None,
+        value: str = None,
+    ):
+        self.active = active
+        self.tag_option_id = tag_option_id
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
+        if self.active is not None:
+            result['Active'] = self.active
+        if self.tag_option_id is not None:
+            result['TagOptionId'] = self.tag_option_id
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Active') is not None:
+            self.active = m.get('Active')
+        if m.get('TagOptionId') is not None:
+            self.tag_option_id = m.get('TagOptionId')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class UpdateTagOptionResponseBodyTagOptionDetail(TeaModel):
+    def __init__(
+        self,
+        active: bool = None,
+        key: str = None,
+        owner: str = None,
+        tag_option_id: str = None,
+        value: str = None,
+    ):
+        self.active = active
+        self.key = key
+        self.owner = owner
+        self.tag_option_id = tag_option_id
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
+        if self.active is not None:
+            result['Active'] = self.active
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.owner is not None:
+            result['Owner'] = self.owner
+        if self.tag_option_id is not None:
+            result['TagOptionId'] = self.tag_option_id
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Active') is not None:
+            self.active = m.get('Active')
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Owner') is not None:
+            self.owner = m.get('Owner')
+        if m.get('TagOptionId') is not None:
+            self.tag_option_id = m.get('TagOptionId')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class UpdateTagOptionResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        tag_option_detail: UpdateTagOptionResponseBodyTagOptionDetail = None,
+    ):
+        self.request_id = request_id
+        self.tag_option_detail = tag_option_detail
+
+    def validate(self):
+        if self.tag_option_detail:
+            self.tag_option_detail.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.tag_option_detail is not None:
+            result['TagOptionDetail'] = self.tag_option_detail.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TagOptionDetail') is not None:
+            temp_model = UpdateTagOptionResponseBodyTagOptionDetail()
+            self.tag_option_detail = temp_model.from_map(m['TagOptionDetail'])
+        return self
+
+
+class UpdateTagOptionResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateTagOptionResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateTagOptionResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_servicecatalog20210901-1.1.3/alibabacloud_servicecatalog20210901.egg-info/PKG-INFO` & `alibabacloud_servicecatalog20210901-1.1.4/alibabacloud_servicecatalog20210901.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-servicecatalog20210901
-Version: 1.1.3
+Version: 1.1.4
 Summary: Alibaba Cloud servicecatalog (20210901) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_servicecatalog20210901-1.1.3/setup.py` & `alibabacloud_servicecatalog20210901-1.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_servicecatalog20210901.
 
-Created on 20/03/2023
+Created on 17/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_servicecatalog20210901"
 NAME = "alibabacloud_servicecatalog20210901" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud servicecatalog (20210901) SDK Library for Python"
```

