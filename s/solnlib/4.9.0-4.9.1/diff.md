# Comparing `tmp/solnlib-4.9.0.tar.gz` & `tmp/solnlib-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solnlib-4.9.0.tar", max compression
+gzip compressed data, was "solnlib-4.9.1.tar", max compression
```

## Comparing `solnlib-4.9.0.tar` & `solnlib-4.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11341 2022-12-12 14:07:25.006034 solnlib-4.9.0/LICENSE
--rw-r--r--   0        0        0     1215 2022-12-12 14:08:27.806233 solnlib-4.9.0/pyproject.toml
--rw-r--r--   0        0        0     1244 2022-12-12 14:08:27.802233 solnlib-4.9.0/solnlib/__init__.py
--rw-r--r--   0        0        0     2735 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/_utils.py
--rw-r--r--   0        0        0     5901 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/acl.py
--rw-r--r--   0        0        0    16897 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/conf_manager.py
--rw-r--r--   0        0        0    13862 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/credentials.py
--rw-r--r--   0        0        0     3974 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/file_monitor.py
--rw-r--r--   0        0        0     5050 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/hec_config.py
--rw-r--r--   0        0        0     7269 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/log.py
--rw-r--r--   0        0        0     1186 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/modular_input/__init__.py
--rw-r--r--   0        0        0     8688 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/modular_input/checkpointer.py
--rw-r--r--   0        0        0     7869 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/modular_input/event.py
--rw-r--r--   0        0        0    15634 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/modular_input/event_writer.py
--rw-r--r--   0        0        0    17930 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/modular_input/modular_input.py
--rw-r--r--   0        0        0     4059 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/net_utils.py
--rw-r--r--   0        0        0     3214 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/orphan_process_monitor.py
--rw-r--r--   0        0        0     1158 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/pattern.py
--rw-r--r--   0        0        0     7856 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/server_info.py
--rw-r--r--   0        0        0     7235 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/splunk_rest_client.py
--rw-r--r--   0        0        0     7887 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/splunkenv.py
--rw-r--r--   0        0        0     4664 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/time_parser.py
--rw-r--r--   0        0        0     9968 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/timer_queue.py
--rw-r--r--   0        0        0    29171 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/user_access.py
--rw-r--r--   0        0        0     5251 2022-12-12 14:07:25.006034 solnlib-4.9.0/solnlib/utils.py
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 solnlib-4.9.0/setup.py
--rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 solnlib-4.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-02-03 13:59:56.427687 solnlib-4.9.1/LICENSE
+-rw-r--r--   0        0        0     1184 2023-02-03 14:00:52.194906 solnlib-4.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1244 2023-02-03 14:00:52.190905 solnlib-4.9.1/solnlib/__init__.py
+-rw-r--r--   0        0        0     2735 2023-02-03 13:59:56.427687 solnlib-4.9.1/solnlib/_utils.py
+-rw-r--r--   0        0        0     5901 2023-02-03 13:59:56.427687 solnlib-4.9.1/solnlib/acl.py
+-rw-r--r--   0        0        0    16897 2023-02-03 13:59:56.427687 solnlib-4.9.1/solnlib/conf_manager.py
+-rw-r--r--   0        0        0    13862 2023-02-03 13:59:56.427687 solnlib-4.9.1/solnlib/credentials.py
+-rw-r--r--   0        0        0     3974 2023-02-03 13:59:56.427687 solnlib-4.9.1/solnlib/file_monitor.py
+-rw-r--r--   0        0        0     5050 2023-02-03 13:59:56.427687 solnlib-4.9.1/solnlib/hec_config.py
+-rw-r--r--   0        0        0     7269 2023-02-03 13:59:56.427687 solnlib-4.9.1/solnlib/log.py
+-rw-r--r--   0        0        0     1186 2023-02-03 13:59:56.427687 solnlib-4.9.1/solnlib/modular_input/__init__.py
+-rw-r--r--   0        0        0     8688 2023-02-03 13:59:56.431687 solnlib-4.9.1/solnlib/modular_input/checkpointer.py
+-rw-r--r--   0        0        0     7869 2023-02-03 13:59:56.431687 solnlib-4.9.1/solnlib/modular_input/event.py
+-rw-r--r--   0        0        0    15634 2023-02-03 13:59:56.431687 solnlib-4.9.1/solnlib/modular_input/event_writer.py
+-rw-r--r--   0        0        0    17930 2023-02-03 13:59:56.431687 solnlib-4.9.1/solnlib/modular_input/modular_input.py
+-rw-r--r--   0        0        0     4059 2023-02-03 13:59:56.431687 solnlib-4.9.1/solnlib/net_utils.py
+-rw-r--r--   0        0        0     3214 2023-02-03 13:59:56.431687 solnlib-4.9.1/solnlib/orphan_process_monitor.py
+-rw-r--r--   0        0        0     1158 2023-02-03 13:59:56.431687 solnlib-4.9.1/solnlib/pattern.py
+-rw-r--r--   0        0        0     7856 2023-02-03 13:59:56.431687 solnlib-4.9.1/solnlib/server_info.py
+-rw-r--r--   0        0        0     7235 2023-02-03 13:59:56.431687 solnlib-4.9.1/solnlib/splunk_rest_client.py
+-rw-r--r--   0        0        0     7887 2023-02-03 13:59:56.431687 solnlib-4.9.1/solnlib/splunkenv.py
+-rw-r--r--   0        0        0     4664 2023-02-03 13:59:56.431687 solnlib-4.9.1/solnlib/time_parser.py
+-rw-r--r--   0        0        0     9968 2023-02-03 13:59:56.431687 solnlib-4.9.1/solnlib/timer_queue.py
+-rw-r--r--   0        0        0    29171 2023-02-03 13:59:56.431687 solnlib-4.9.1/solnlib/user_access.py
+-rw-r--r--   0        0        0     5251 2023-02-03 13:59:56.431687 solnlib-4.9.1/solnlib/utils.py
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 solnlib-4.9.1/setup.py
+-rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 solnlib-4.9.1/PKG-INFO
```

### Comparing `solnlib-4.9.0/LICENSE` & `solnlib-4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/pyproject.toml` & `solnlib-4.9.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 [tool.poetry]
 name = "solnlib"
-version = "4.9.0"
+version = "4.9.1"
 description = "The Splunk Software Development Kit for Splunk Solutions"
 authors = ["Splunk <addonfactory@splunk.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/splunk/addonfactory-solutions-library-python"
 
 [tool.poetry.dependencies]
 python = "^3.7"
@@ -31,13 +31,10 @@
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 mkdocs = "^1.4.2"
 mkdocs-material = "^8.5.10"
 mkdocstrings = "0.18.0"
 
-[tool.isort]
-profile = "black"
-
 [build-system]
 requires = ["poetry>=1.0.0"]
-build-backend = "poetry.masonry.api"
+build-backend = "poetry.masonry.api"
```

### Comparing `solnlib-4.9.0/solnlib/__init__.py` & `solnlib-4.9.1/solnlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,8 +50,8 @@
     "splunkenv",
     "time_parser",
     "timer_queue",
     "user_access",
     "utils",
 ]
 
-__version__ = "4.9.0"
+__version__ = "4.9.1"
```

### Comparing `solnlib-4.9.0/solnlib/_utils.py` & `solnlib-4.9.1/solnlib/_utils.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/acl.py` & `solnlib-4.9.1/solnlib/acl.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/conf_manager.py` & `solnlib-4.9.1/solnlib/conf_manager.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/credentials.py` & `solnlib-4.9.1/solnlib/credentials.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/file_monitor.py` & `solnlib-4.9.1/solnlib/file_monitor.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/hec_config.py` & `solnlib-4.9.1/solnlib/hec_config.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/log.py` & `solnlib-4.9.1/solnlib/log.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/modular_input/__init__.py` & `solnlib-4.9.1/solnlib/modular_input/__init__.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/modular_input/checkpointer.py` & `solnlib-4.9.1/solnlib/modular_input/checkpointer.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/modular_input/event.py` & `solnlib-4.9.1/solnlib/modular_input/event.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/modular_input/event_writer.py` & `solnlib-4.9.1/solnlib/modular_input/event_writer.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/modular_input/modular_input.py` & `solnlib-4.9.1/solnlib/modular_input/modular_input.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/net_utils.py` & `solnlib-4.9.1/solnlib/net_utils.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/orphan_process_monitor.py` & `solnlib-4.9.1/solnlib/orphan_process_monitor.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/pattern.py` & `solnlib-4.9.1/solnlib/pattern.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/server_info.py` & `solnlib-4.9.1/solnlib/server_info.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/splunk_rest_client.py` & `solnlib-4.9.1/solnlib/splunk_rest_client.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/splunkenv.py` & `solnlib-4.9.1/solnlib/splunkenv.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/time_parser.py` & `solnlib-4.9.1/solnlib/time_parser.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/timer_queue.py` & `solnlib-4.9.1/solnlib/timer_queue.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/user_access.py` & `solnlib-4.9.1/solnlib/user_access.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/solnlib/utils.py` & `solnlib-4.9.1/solnlib/utils.py`

 * *Files identical despite different names*

### Comparing `solnlib-4.9.0/setup.py` & `solnlib-4.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['defusedxml>=0.7.1,<0.8.0',
  'requests>=2.28.0,<3.0.0',
  'sortedcontainers>=2.2,<3.0',
  'splunk-sdk>=1.6.18']
 
 setup_kwargs = {
     'name': 'solnlib',
-    'version': '4.9.0',
+    'version': '4.9.1',
     'description': 'The Splunk Software Development Kit for Splunk Solutions',
     'long_description': 'None',
     'author': 'Splunk',
     'author_email': 'addonfactory@splunk.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/splunk/addonfactory-solutions-library-python',
```

### Comparing `solnlib-4.9.0/PKG-INFO` & `solnlib-4.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solnlib
-Version: 4.9.0
+Version: 4.9.1
 Summary: The Splunk Software Development Kit for Splunk Solutions
 Home-page: https://github.com/splunk/addonfactory-solutions-library-python
 License: Apache-2.0
 Author: Splunk
 Author-email: addonfactory@splunk.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

