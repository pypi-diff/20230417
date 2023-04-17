# Comparing `tmp/tencentcloud-sdk-python-cdn-3.0.873.tar.gz` & `tmp/tencentcloud-sdk-python-cdn-3.0.874.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.873.tar", last modified: Fri Apr 14 00:24:06 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.874.tar", last modified: Mon Apr 17 00:23:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdn-3.0.873.tar` & `tencentcloud-sdk-python-cdn-3.0.874.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/tencentcloud/cdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/tencentcloud/cdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)    21844 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/tencentcloud/cdn/v20180606/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    80657 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)   568032 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/tencentcloud_sdk_python_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-14 00:24:06.000000 tencentcloud-sdk-python-cdn-3.0.873/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/tencentcloud/cdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/tencentcloud/cdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)    21844 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/tencentcloud/cdn/v20180606/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    80657 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   568035 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/tencentcloud_sdk_python_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-17 00:23:31.000000 tencentcloud-sdk-python-cdn-3.0.874/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.873/README.rst` & `tencentcloud-sdk-python-cdn-3.0.874/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.873/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdn-3.0.874/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdn-3.0.873/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-cdn-3.0.874/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.873/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-cdn-3.0.874/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.873/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-cdn-3.0.874/tencentcloud/cdn/v20180606/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10838,19 +10838,19 @@
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class Origin(AbstractModel):
     """源站配置复杂类型，支持以下配置：
     + 源站指定为单个域名
-    + 源站指定为多个 IP，可配置端口（1~65535），可配置权重（1~100），格式为 IP:端口:权重
+    + 源站指定为多个 IP，可配置端口（1\~65535），可配置权重（1\~100），格式为 IP:端口:权重
     + 回源域名配置
     + 对象存储（COS）作为源站
     + 热备源站指定为单个域名
-    + 热备源站指定为多个 IP，可配置端口（1~65535），暂不支持权重配置
+    + 热备源站指定为多个 IP，可配置端口（1\~65535），暂不支持权重配置
     + 热备源站回源域名配置
 
     """
 
     def __init__(self):
         r"""
         :param Origins: 主源站列表
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.873/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.874/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.873
+Version: 3.0.874
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.873/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.874/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.873
+Version: 3.0.874
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.873/setup.py` & `tencentcloud-sdk-python-cdn-3.0.874/setup.py`

 * *Files identical despite different names*

