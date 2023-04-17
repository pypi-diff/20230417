# Comparing `tmp/tencentcloud-sdk-python-trp-3.0.873.tar.gz` & `tmp/tencentcloud-sdk-python-trp-3.0.874.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trp-3.0.873.tar", last modified: Fri Apr 14 01:00:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trp-3.0.874.tar", last modified: Mon Apr 17 00:53:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trp-3.0.873.tar` & `tencentcloud-sdk-python-trp-3.0.874.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:00:22.000000 tencentcloud-sdk-python-trp-3.0.873/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-14 01:00:21.000000 tencentcloud-sdk-python-trp-3.0.873/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:00:22.000000 tencentcloud-sdk-python-trp-3.0.873/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:00:22.000000 tencentcloud-sdk-python-trp-3.0.873/tencentcloud/trp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:00:22.000000 tencentcloud-sdk-python-trp-3.0.873/tencentcloud/trp/v20210515/
--rw-r--r--   0 root         (0) root         (0)      992 2023-04-14 01:00:21.000000 tencentcloud-sdk-python-trp-3.0.873/tencentcloud/trp/v20210515/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 01:00:21.000000 tencentcloud-sdk-python-trp-3.0.873/tencentcloud/trp/v20210515/__init__.py
--rw-r--r--   0 root         (0) root         (0)   130963 2023-04-14 01:00:21.000000 tencentcloud-sdk-python-trp-3.0.873/tencentcloud/trp/v20210515/models.py
--rw-r--r--   0 root         (0) root         (0)    39990 2023-04-14 01:00:21.000000 tencentcloud-sdk-python-trp-3.0.873/tencentcloud/trp/v20210515/trp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 01:00:21.000000 tencentcloud-sdk-python-trp-3.0.873/tencentcloud/trp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-14 01:00:21.000000 tencentcloud-sdk-python-trp-3.0.873/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 01:00:22.000000 tencentcloud-sdk-python-trp-3.0.873/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-14 01:00:21.000000 tencentcloud-sdk-python-trp-3.0.873/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-14 01:00:22.000000 tencentcloud-sdk-python-trp-3.0.873/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:00:22.000000 tencentcloud-sdk-python-trp-3.0.873/tencentcloud_sdk_python_trp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 01:00:22.000000 tencentcloud-sdk-python-trp-3.0.873/tencentcloud_sdk_python_trp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-14 01:00:22.000000 tencentcloud-sdk-python-trp-3.0.873/tencentcloud_sdk_python_trp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 01:00:22.000000 tencentcloud-sdk-python-trp-3.0.873/tencentcloud_sdk_python_trp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 01:00:22.000000 tencentcloud-sdk-python-trp-3.0.873/tencentcloud_sdk_python_trp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/
+-rw-r--r--   0 root         (0) root         (0)      992 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   132410 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/models.py
+-rw-r--r--   0 root         (0) root         (0)    40986 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/trp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud_sdk_python_trp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud_sdk_python_trp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud_sdk_python_trp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud_sdk_python_trp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud_sdk_python_trp.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-trp-3.0.873/README.rst` & `tencentcloud-sdk-python-trp-3.0.874/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.873/tencentcloud/trp/v20210515/errorcodes.py` & `tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.873/tencentcloud/trp/v20210515/models.py` & `tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2625,14 +2625,65 @@
                 obj = TraceCode()
                 obj._deserialize(item)
                 self.TraceCodes.append(obj)
         self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeTraceDataByIdRequest(AbstractModel):
+    """DescribeTraceDataById请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: 溯源ID
+        :type Id: str
+        :param CorpId: 企业ID
+        :type CorpId: int
+        """
+        self.Id = None
+        self.CorpId = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        self.CorpId = params.get("CorpId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeTraceDataByIdResponse(AbstractModel):
+    """DescribeTraceDataById返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TraceData: 无
+        :type TraceData: :class:`tencentcloud.trp.v20210515.models.TraceData`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TraceData = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("TraceData") is not None:
+            self.TraceData = TraceData()
+            self.TraceData._deserialize(params.get("TraceData"))
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeTraceDataListRequest(AbstractModel):
     """DescribeTraceDataList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-trp-3.0.873/tencentcloud/trp/v20210515/trp_client.py` & `tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/trp_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -805,14 +805,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeTraceDataById(self, request):
+        """查询溯源ID查溯源信息，通常溯源信息跟生产批次绑定，即一个批次的所有溯源信息都是一样的
+
+        :param request: Request instance for DescribeTraceDataById.
+        :type request: :class:`tencentcloud.trp.v20210515.models.DescribeTraceDataByIdRequest`
+        :rtype: :class:`tencentcloud.trp.v20210515.models.DescribeTraceDataByIdResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeTraceDataById", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeTraceDataByIdResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeTraceDataList(self, request):
         """查询溯源信息，通常溯源信息跟生产批次绑定，即一个批次的所有溯源信息都是一样的
 
         :param request: Request instance for DescribeTraceDataList.
         :type request: :class:`tencentcloud.trp.v20210515.models.DescribeTraceDataListRequest`
         :rtype: :class:`tencentcloud.trp.v20210515.models.DescribeTraceDataListResponse`
```

### Comparing `tencentcloud-sdk-python-trp-3.0.873/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trp-3.0.874/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.873'
+__version__ = '3.0.874'
```

### Comparing `tencentcloud-sdk-python-trp-3.0.873/PKG-INFO` & `tencentcloud-sdk-python-trp-3.0.874/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trp
-Version: 3.0.873
+Version: 3.0.874
 Summary: Tencent Cloud Trp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trp-3.0.873/setup.py` & `tencentcloud-sdk-python-trp-3.0.874/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.873/tencentcloud_sdk_python_trp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trp-3.0.874/tencentcloud_sdk_python_trp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trp
-Version: 3.0.873
+Version: 3.0.874
 Summary: Tencent Cloud Trp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

