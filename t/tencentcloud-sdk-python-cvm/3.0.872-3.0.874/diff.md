# Comparing `tmp/tencentcloud-sdk-python-cvm-3.0.872.tar.gz` & `tmp/tencentcloud-sdk-python-cvm-3.0.874.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.872.tar", last modified: Thu Apr 13 00:30:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.874.tar", last modified: Mon Apr 17 00:26:41 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cvm-3.0.872.tar` & `tencentcloud-sdk-python-cvm-3.0.874.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/
--rw-r--r--   0 root         (0) root         (0)   119282 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/cvm_client.py
--rw-r--r--   0 root         (0) root         (0)    42551 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   429673 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud_sdk_python_cvm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/tencentcloud/cvm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/tencentcloud/cvm/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   119282 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/tencentcloud/cvm/v20170312/cvm_client.py
+-rw-r--r--   0 root         (0) root         (0)    42551 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/tencentcloud/cvm/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/tencentcloud/cvm/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   429673 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/tencentcloud/cvm/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/tencentcloud/cvm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/tencentcloud_sdk_python_cvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 00:26:41.000000 tencentcloud-sdk-python-cvm-3.0.874/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.872/README.rst` & `tencentcloud-sdk-python-cvm-3.0.874/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/cvm_client.py` & `tencentcloud-sdk-python-cvm-3.0.874/tencentcloud/cvm/v20170312/cvm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cvm-3.0.874/tencentcloud/cvm/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/models.py` & `tencentcloud-sdk-python-cvm-3.0.874/tencentcloud/cvm/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cvm-3.0.874/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.872'
+__version__ = '3.0.874'
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.872/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.874/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.872
+Version: 3.0.874
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.872/setup.py` & `tencentcloud-sdk-python-cvm-3.0.874/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.872/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.874/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.872
+Version: 3.0.874
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

