# Comparing `tmp/tencentcloud-sdk-python-bmlb-3.0.873.tar.gz` & `tmp/tencentcloud-sdk-python-bmlb-3.0.874.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-bmlb-3.0.873.tar", last modified: Fri Apr 14 00:20:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-bmlb-3.0.874.tar", last modified: Mon Apr 17 00:21:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-bmlb-3.0.873.tar` & `tencentcloud-sdk-python-bmlb-3.0.874.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud/bmlb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud/bmlb/v20180625/
--rw-r--r--   0 root         (0) root         (0)    47086 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud/bmlb/v20180625/bmlb_client.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud/bmlb/v20180625/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud/bmlb/v20180625/__init__.py
--rw-r--r--   0 root         (0) root         (0)   202561 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud/bmlb/v20180625/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud/bmlb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud_sdk_python_bmlb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud_sdk_python_bmlb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud_sdk_python_bmlb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud_sdk_python_bmlb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 00:20:25.000000 tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud_sdk_python_bmlb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud/bmlb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud/bmlb/v20180625/
+-rw-r--r--   0 root         (0) root         (0)    47086 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud/bmlb/v20180625/bmlb_client.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud/bmlb/v20180625/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud/bmlb/v20180625/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   202561 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud/bmlb/v20180625/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud/bmlb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud_sdk_python_bmlb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud_sdk_python_bmlb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud_sdk_python_bmlb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud_sdk_python_bmlb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 00:21:35.000000 tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud_sdk_python_bmlb.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-bmlb-3.0.873/README.rst` & `tencentcloud-sdk-python-bmlb-3.0.874/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud/bmlb/v20180625/bmlb_client.py` & `tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud/bmlb/v20180625/bmlb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud/bmlb/v20180625/errorcodes.py` & `tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud/bmlb/v20180625/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud/bmlb/v20180625/models.py` & `tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud/bmlb/v20180625/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud/__init__.py` & `tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-bmlb-3.0.873/PKG-INFO` & `tencentcloud-sdk-python-bmlb-3.0.874/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bmlb
-Version: 3.0.873
+Version: 3.0.874
 Summary: Tencent Cloud Bmlb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bmlb-3.0.873/setup.py` & `tencentcloud-sdk-python-bmlb-3.0.874/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmlb-3.0.873/tencentcloud_sdk_python_bmlb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-bmlb-3.0.874/tencentcloud_sdk_python_bmlb.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bmlb
-Version: 3.0.873
+Version: 3.0.874
 Summary: Tencent Cloud Bmlb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

