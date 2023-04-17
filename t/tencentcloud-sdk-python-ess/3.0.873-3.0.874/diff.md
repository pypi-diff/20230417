# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.873.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.874.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.873.tar", last modified: Fri Apr 14 00:37:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.874.tar", last modified: Mon Apr 17 00:29:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.873.tar` & `tencentcloud-sdk-python-ess-3.0.874.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    47020 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23577 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   212473 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-14 00:37:10.000000 tencentcloud-sdk-python-ess-3.0.873/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    47020 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23577 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   212520 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.873/README.rst` & `tencentcloud-sdk-python-ess-3.0.874/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.873/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.874/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.873/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.873/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.873/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1303,15 +1303,15 @@
 class CreateFlowRemindsResponse(AbstractModel):
     """CreateFlowReminds返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param RemindFlowRecords: 签署连接过期时间字符串：年月日-时分秒
+        :param RemindFlowRecords: 催办合同详情列表
         :type RemindFlowRecords: list of RemindFlowRecords
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.RemindFlowRecords = None
         self.RequestId = None
 
@@ -4113,21 +4113,26 @@
         :param FlowId: 合同(流程)的Id
         :type FlowId: str
         :param FlowName: 合同(流程)的名字
         :type FlowName: str
         :param FlowType: 合同(流程)的类型
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowType: str
-        :param FlowStatus: 合同(流程)的状态
-1：未签署
-2：部分签署
-3：已退回
-4：完成签署
-5：已过期
-6：已取消
+        :param FlowStatus: 流程状态
+- 0 还没有发起
+- 1 未签署
+- 2 部分签署
+- 3 已退回
+- 4 完成签署
+- 5 已过期
+- 6 已取消
+- 7 还没有预发起
+- 8 等待填写
+- 9 部分填写
+- 10 拒填
         :type FlowStatus: int
         :param FlowMessage: 合同(流程)的信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowMessage: str
         :param FlowDescription: 流程的描述
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowDescription: str
```

### Comparing `tencentcloud-sdk-python-ess-3.0.873/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.874/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.873
+Version: 3.0.874
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.873/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.874/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.873
+Version: 3.0.874
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.873/setup.py` & `tencentcloud-sdk-python-ess-3.0.874/setup.py`

 * *Files identical despite different names*

