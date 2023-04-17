# Comparing `tmp/tencentcloud-sdk-python-wss-3.0.873.tar.gz` & `tmp/tencentcloud-sdk-python-wss-3.0.874.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-wss-3.0.873.tar", last modified: Fri Apr 14 01:02:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-wss-3.0.874.tar", last modified: Mon Apr 17 00:54:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-wss-3.0.873.tar` & `tencentcloud-sdk-python-wss-3.0.874.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/tencentcloud_sdk_python_wss.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/tencentcloud_sdk_python_wss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/tencentcloud_sdk_python_wss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/tencentcloud_sdk_python_wss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/tencentcloud_sdk_python_wss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/tencentcloud/wss/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/tencentcloud/wss/v20180426/
--rw-r--r--   0 root         (0) root         (0)     3594 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/tencentcloud/wss/v20180426/wss_client.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/tencentcloud/wss/v20180426/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/tencentcloud/wss/v20180426/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15365 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/tencentcloud/wss/v20180426/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/tencentcloud/wss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-14 01:02:43.000000 tencentcloud-sdk-python-wss-3.0.873/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/tencentcloud_sdk_python_wss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/tencentcloud_sdk_python_wss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/tencentcloud_sdk_python_wss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/tencentcloud_sdk_python_wss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/tencentcloud_sdk_python_wss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/tencentcloud/wss/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/tencentcloud/wss/v20180426/
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/tencentcloud/wss/v20180426/wss_client.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/tencentcloud/wss/v20180426/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/tencentcloud/wss/v20180426/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15365 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/tencentcloud/wss/v20180426/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/tencentcloud/wss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-17 00:54:54.000000 tencentcloud-sdk-python-wss-3.0.874/setup.cfg
```

### Comparing `tencentcloud-sdk-python-wss-3.0.873/tencentcloud_sdk_python_wss.egg-info/PKG-INFO` & `tencentcloud-sdk-python-wss-3.0.874/tencentcloud_sdk_python_wss.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wss
-Version: 3.0.873
+Version: 3.0.874
 Summary: Tencent Cloud Wss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wss-3.0.873/README.rst` & `tencentcloud-sdk-python-wss-3.0.874/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wss-3.0.873/tencentcloud/__init__.py` & `tencentcloud-sdk-python-wss-3.0.874/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-wss-3.0.873/tencentcloud/wss/v20180426/wss_client.py` & `tencentcloud-sdk-python-wss-3.0.874/tencentcloud/wss/v20180426/wss_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wss-3.0.873/tencentcloud/wss/v20180426/errorcodes.py` & `tencentcloud-sdk-python-wss-3.0.874/tencentcloud/wss/v20180426/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wss-3.0.873/tencentcloud/wss/v20180426/models.py` & `tencentcloud-sdk-python-wss-3.0.874/tencentcloud/wss/v20180426/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wss-3.0.873/PKG-INFO` & `tencentcloud-sdk-python-wss-3.0.874/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wss
-Version: 3.0.873
+Version: 3.0.874
 Summary: Tencent Cloud Wss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wss-3.0.873/setup.py` & `tencentcloud-sdk-python-wss-3.0.874/setup.py`

 * *Files identical despite different names*
