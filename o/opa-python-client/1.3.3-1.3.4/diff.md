# Comparing `tmp/OPA-python-client-1.3.3.tar.gz` & `tmp/opa_python_client-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OPA-python-client-1.3.3.tar", last modified: Mon May  2 13:51:53 2022, max compression
+gzip compressed data, was "opa_python_client-1.3.4.tar", max compression
```

## Comparing `OPA-python-client-1.3.3.tar` & `opa_python_client-1.3.4.tar`

### file list

```diff
@@ -1,21 +1,8 @@
-drwxr-xr-x   0 tural      (501) staff       (20)        0 2022-05-02 13:51:53.725077 OPA-python-client-1.3.3/
--rw-r--r--   0 tural      (501) staff       (20)     1078 2022-03-21 16:37:50.000000 OPA-python-client-1.3.3/LICENCE.md
-drwxr-xr-x   0 tural      (501) staff       (20)        0 2022-05-02 13:51:53.723567 OPA-python-client-1.3.3/OPA_python_client.egg-info/
--rw-r--r--   0 tural      (501) staff       (20)     7758 2022-05-02 13:51:53.000000 OPA-python-client-1.3.3/OPA_python_client.egg-info/PKG-INFO
--rw-r--r--   0 tural      (501) staff       (20)      409 2022-05-02 13:51:53.000000 OPA-python-client-1.3.3/OPA_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 tural      (501) staff       (20)        1 2022-05-02 13:51:53.000000 OPA-python-client-1.3.3/OPA_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 tural      (501) staff       (20)       71 2022-05-02 13:51:53.000000 OPA-python-client-1.3.3/OPA_python_client.egg-info/requires.txt
--rw-r--r--   0 tural      (501) staff       (20)       11 2022-05-02 13:51:53.000000 OPA-python-client-1.3.3/OPA_python_client.egg-info/top_level.txt
--rw-r--r--   0 tural      (501) staff       (20)     7758 2022-05-02 13:51:53.724961 OPA-python-client-1.3.3/PKG-INFO
--rw-r--r--   0 tural      (501) staff       (20)     7021 2022-03-21 16:37:50.000000 OPA-python-client-1.3.3/README.md
-drwxr-xr-x   0 tural      (501) staff       (20)        0 2022-05-02 13:51:53.723938 OPA-python-client-1.3.3/opa_client/
-drwxr-xr-x   0 tural      (501) staff       (20)        0 2022-05-02 13:51:53.724472 OPA-python-client-1.3.3/opa_client/OpaExceptions/
--rw-r--r--   0 tural      (501) staff       (20)     3004 2022-03-21 16:37:50.000000 OPA-python-client-1.3.3/opa_client/OpaExceptions/OpaExceptions.py
--rw-r--r--   0 tural      (501) staff       (20)      290 2022-03-21 16:37:50.000000 OPA-python-client-1.3.3/opa_client/OpaExceptions/__init__.py
--rw-r--r--   0 tural      (501) staff       (20)      129 2022-03-21 16:37:50.000000 OPA-python-client-1.3.3/opa_client/__init__.py
--rw-r--r--   0 tural      (501) staff       (20)    23023 2022-05-02 13:49:40.000000 OPA-python-client-1.3.3/opa_client/opa.py
-drwxr-xr-x   0 tural      (501) staff       (20)        0 2022-05-02 13:51:53.724697 OPA-python-client-1.3.3/opa_client/test/
--rw-r--r--   0 tural      (501) staff       (20)        0 2022-03-21 16:37:50.000000 OPA-python-client-1.3.3/opa_client/test/__init__.py
--rw-r--r--   0 tural      (501) staff       (20)     2997 2022-03-22 08:50:53.000000 OPA-python-client-1.3.3/opa_client/test/test_opa.py
--rw-r--r--   0 tural      (501) staff       (20)       38 2022-05-02 13:51:53.725118 OPA-python-client-1.3.3/setup.cfg
--rw-r--r--   0 tural      (501) staff       (20)     1176 2022-05-02 13:49:31.000000 OPA-python-client-1.3.3/setup.py
+-rw-r--r--   0        0        0     7870 2023-04-17 06:13:13.235711 opa_python_client-1.3.4/README.md
+-rw-r--r--   0        0        0      100 2023-04-17 06:13:13.235848 opa_python_client-1.3.4/opa_client/__init__.py
+-rw-r--r--   0        0        0     3039 2023-04-17 06:13:13.235942 opa_python_client-1.3.4/opa_client/errors.py
+-rw-r--r--   0        0        0    20776 2023-04-17 06:13:13.236194 opa_python_client-1.3.4/opa_client/opa.py
+-rw-r--r--   0        0        0        0 2022-03-21 16:37:50.641920 opa_python_client-1.3.4/opa_client/test/__init__.py
+-rw-r--r--   0        0        0     3843 2023-04-17 06:13:13.238585 opa_python_client-1.3.4/opa_client/test/test_opa.py
+-rw-r--r--   0        0        0     1179 2023-04-17 06:14:50.257160 opa_python_client-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     9056 1970-01-01 00:00:00.000000 opa_python_client-1.3.4/PKG-INFO
```

### Comparing `OPA-python-client-1.3.3/OPA_python_client.egg-info/PKG-INFO` & `opa_python_client-1.3.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,35 @@
-Metadata-Version: 2.1
-Name: OPA-python-client
-Version: 1.3.3
-Summary: Client for connection to the OPA service
-Home-page: https://github.com/Turall/OPA-python-client.git
-Author: Tural Muradov
-Author-email: tural_m@hotmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENCE.md
-
 # Python Open Policy Agent (OPA) Client 
 
+[![MIT licensed](https://img.shields.io/github/license/Turall/OPA-python-client)](https://raw.githubusercontent.com/Turall/OPA-python-client/master/LICENSE)
+[![GitHub stars](https://img.shields.io/github/stars/Turall/OPA-python-client.svg)](https://github.com/Turall/OPA-python-client/stargazers)
+[![GitHub forks](https://img.shields.io/github/forks/Turall/OPA-python-client.svg)](https://github.com/Turall/OPA-python-client/network)
+[![GitHub issues](https://img.shields.io/github/issues-raw/Turall/OPA-python-client)](https://github.com/Turall/OPA-python-client/issues)
 [![Downloads](https://pepy.tech/badge/opa-python-client)](https://pepy.tech/project/opa-python-client)
 
+
 See offical documentation page [Open Policy Agent](https://www.openpolicyagent.org/docs/latest/)
 
 
 ### Installation ###
 
 ```sh
- $ pip install OPA-python-client
+$ pip install OPA-python-client
 ```
 
+Alternatively, if you prefer to use `poetry` for package dependencies:
+
+```bash
+$ poetry shell
+$ poetry add OPA-python-client
+```
 
 
 
-## Usage Examples ##
+## Usage Examples 
 
 ```python
 >>> from opa_client.opa import OpaClient
 >>> client = OpaClient() # default host='localhost', port=8181, version='v1'
 >>> client.check_connection()
 'Yes I"m here :)'
 >>>  test_policy = """
@@ -64,32 +54,31 @@
 True
 >>> check_data = {"input": {"message": "hello"}}
 >>> client.check_permission(input_data=check_data, policy_name="testpolicy", rule_name="hello")
 {'result': True}
 ```
 
 
-### Connection to OPA service ###
+### Connection to OPA service
 
 ```python
 from opa_client.opa import OpaClient
 
 client = OpaClient() # default host='localhost', port=8181, version='v1'
 
 client.check_connection() # response is  Yes I'm here :)
 
 # Ensure the connection is closed correctly by deleting the client
 del client
 ```
 
 
-### Connection to OPA service with SSL ###
+### Connection to OPA service with SSL
 
 ```python
-
 from opa_client.opa import OpaClient
 
 
 client = OpaClient(
     host="https://192.168.99.100",
     port=8181,
     version="v1",
@@ -99,71 +88,64 @@
 
 client.check_connection() # response is  Yes I'm here :)
 
 del client
 ```
 
 
-
-
-### Update policy from rego file ###
+### Update policy from rego file
 
 ```python
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 client.update_opa_policy_fromfile("/your/path/filename.rego", endpoint="fromfile") # response is True
 
 client.get_policies_list() # response is ["fromfile"]
 
 del client
 ```
 
 
-### Update policy from URL ###
+### Update policy from URL
 
 ```python
-
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 
 client.update_opa_policy_fromurl("http://opapolicyurlexample.test/example.rego", endpoint="fromurl") # response is True
 
 client.get_policies_list() # response is ["fromfile","fromurl"]
 
 del client
 ```
 
 
-### Delete policy ###
+### Delete policy
 
 
 ```python
-
-
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 client.delete_opa_policy("fromfile") # response is True
 
 client.get_policies_list() # response is [] 
 
 del client
 ```
 
-### Get raw data from OPA service ###
+### Get raw data from OPA service
 
 
 ```python
-
-
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 print(client.get_opa_raw_data("testapi/testdata"))  # response is {'result': ['world', 'hello']}
 
 # You can use query params for additional info
@@ -176,69 +158,63 @@
 print(client.get_opa_raw_data("userinfo",query_params={"metrics": True})) 
 
 # response is {'metrics': {'counter_server_query_cache_hit': 0, 'timer_rego_external_resolve_ns': 231, 'timer_rego_input_parse_ns': 381, 'timer_rego_query_compile_ns': 40173, 'timer_rego_query_eval_ns': 12674, 'timer_rego_query_parse_ns': 5692, 'timer_server_handler_ns': 83490}, 'result': {'user_roles': {'alice': ['admin'], 'bob': ['employee', 'billing'], 'eve': ['customer']}}}
 
 del client
 ```
 
-### Save policy to file from OPA service ###
-
 
-```python
+### Save policy to file from OPA service
 
 
+```python
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 client.opa_policy_to_file(policy_name="fromurl",path="/your/path",filename="example.rego")  # response is True
 
 del client
 ```
 
-### Delete data from OPA service ###
 
-
-```python
+### Delete data from OPA service
 
 
+```python
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 client.delete_opa_data("testapi")  # response is True
 
 del client
 ```
 
 
-### Information about policy path and rules ###
+### Information about policy path and rules
 
 
 ```python
-
-
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 client.get_policies_info()
 
 # response is {'testpolicy': {'path': ['http://your-opa-service/v1/data/play'], 'rules': ['http://your-opa-service/v1/data/play/hello']}
 
 del client
 ```
 
 
-### Check permissions ###
+### Check permissions
 
 
 ```python
-
-
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 permission_you_want_check = {"input": {"message": "hello"}}
 client.check_permission(input_data=permission_you_want_check, policy_name="testpolicy", rule_name="hello")
 
@@ -267,15 +243,14 @@
     m := input.message
     m == "world"
 }
 """
 
 check_data = {"message": "world"}
 client.check_policy_rule(input_data=check_data, package_path="play", rule_name="hello") # response {'result': True}
-
 ```
 
 ### Execute an Ad-hoc Query
 
 ```python
 from opa_client.opa import OpaClient
 
@@ -303,33 +278,32 @@
 # execute query 
 print(client.ad_hoc_query(query_params={"q": "data.userinfo.user_roles[name]"})) 
 # response is {'result': [{'name': 'eve'}, {'name': 'alice'}, {'name': 'bob'}]}
 
 #you can send body request
 print(client.ad_hoc_query(body={"query": "data.userinfo.user_roles[name] "})) 
 # response is {'result': [{'name': 'eve'}, {'name': 'alice'}, {'name': 'bob'}]}
-
 ```
 
 ### Check OPA healthy. If you want check bundels or plugins, add query params for this.
 
 ```python
 from opa_client.opa import OpaClient
 
 client = OpaClient()
 
 print(client.check_health()) # response is  True or False
 print(client.check_health({"bundle": True})) # response is  True or False
 # If your diagnostic url different than default url, you can provide it.
 print(client.check_health(diagnostic_url="http://localhost:8282/health"))  # response is  True or False
 print(client.check_health(query={"bundle": True}, diagnostic_url="http://localhost:8282/health"))  # response is  True or False
-
 ```
 
 
-# Contributing #
-
-#### Free to open issue and send PR ####
+# Contributing
 
-### OPA-python-client  supports Python >= 3.5
+Fell free to open issue and send pull request.
 
+Thanks To [Contributors](https://github.com/Turall/OPA-python-client/graphs/contributors).
+Contributions of any kind are welcome!
 
+Before you start please read [CONTRIBUTING](https://github.com/Turall/OPA-python-client/blob/master/CONTRIBUTING.md)
```

### Comparing `OPA-python-client-1.3.3/PKG-INFO` & `opa_python_client-1.3.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,64 @@
 Metadata-Version: 2.1
-Name: OPA-python-client
-Version: 1.3.3
+Name: opa-python-client
+Version: 1.3.4
 Summary: Client for connection to the OPA service
-Home-page: https://github.com/Turall/OPA-python-client.git
+Home-page: https://github.com/Turall/OPA-python-client
+License: MIT
 Author: Tural Muradov
 Author-email: tural_m@hotmail.com
-License: MIT
-Platform: UNKNOWN
+Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Dist: certifi (>=2022.5.18,<2023.0.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: types-requests (>=2.27.30,<3.0.0)
+Requires-Dist: urllib3 (>=1.26.9,<2.0.0)
+Requires-Dist: user-agent (>=0.1.10,<0.2.0)
+Project-URL: Repository, https://github.com/Turall/OPA-python-client
 Description-Content-Type: text/markdown
-License-File: LICENCE.md
 
 # Python Open Policy Agent (OPA) Client 
 
+[![MIT licensed](https://img.shields.io/github/license/Turall/OPA-python-client)](https://raw.githubusercontent.com/Turall/OPA-python-client/master/LICENSE)
+[![GitHub stars](https://img.shields.io/github/stars/Turall/OPA-python-client.svg)](https://github.com/Turall/OPA-python-client/stargazers)
+[![GitHub forks](https://img.shields.io/github/forks/Turall/OPA-python-client.svg)](https://github.com/Turall/OPA-python-client/network)
+[![GitHub issues](https://img.shields.io/github/issues-raw/Turall/OPA-python-client)](https://github.com/Turall/OPA-python-client/issues)
 [![Downloads](https://pepy.tech/badge/opa-python-client)](https://pepy.tech/project/opa-python-client)
 
+
 See offical documentation page [Open Policy Agent](https://www.openpolicyagent.org/docs/latest/)
 
 
 ### Installation ###
 
 ```sh
- $ pip install OPA-python-client
+$ pip install OPA-python-client
 ```
 
+Alternatively, if you prefer to use `poetry` for package dependencies:
+
+```bash
+$ poetry shell
+$ poetry add OPA-python-client
+```
 
 
 
-## Usage Examples ##
+## Usage Examples 
 
 ```python
 >>> from opa_client.opa import OpaClient
 >>> client = OpaClient() # default host='localhost', port=8181, version='v1'
 >>> client.check_connection()
 'Yes I"m here :)'
 >>>  test_policy = """
@@ -64,32 +83,31 @@
 True
 >>> check_data = {"input": {"message": "hello"}}
 >>> client.check_permission(input_data=check_data, policy_name="testpolicy", rule_name="hello")
 {'result': True}
 ```
 
 
-### Connection to OPA service ###
+### Connection to OPA service
 
 ```python
 from opa_client.opa import OpaClient
 
 client = OpaClient() # default host='localhost', port=8181, version='v1'
 
 client.check_connection() # response is  Yes I'm here :)
 
 # Ensure the connection is closed correctly by deleting the client
 del client
 ```
 
 
-### Connection to OPA service with SSL ###
+### Connection to OPA service with SSL
 
 ```python
-
 from opa_client.opa import OpaClient
 
 
 client = OpaClient(
     host="https://192.168.99.100",
     port=8181,
     version="v1",
@@ -99,71 +117,64 @@
 
 client.check_connection() # response is  Yes I'm here :)
 
 del client
 ```
 
 
-
-
-### Update policy from rego file ###
+### Update policy from rego file
 
 ```python
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 client.update_opa_policy_fromfile("/your/path/filename.rego", endpoint="fromfile") # response is True
 
 client.get_policies_list() # response is ["fromfile"]
 
 del client
 ```
 
 
-### Update policy from URL ###
+### Update policy from URL
 
 ```python
-
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 
 client.update_opa_policy_fromurl("http://opapolicyurlexample.test/example.rego", endpoint="fromurl") # response is True
 
 client.get_policies_list() # response is ["fromfile","fromurl"]
 
 del client
 ```
 
 
-### Delete policy ###
+### Delete policy
 
 
 ```python
-
-
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 client.delete_opa_policy("fromfile") # response is True
 
 client.get_policies_list() # response is [] 
 
 del client
 ```
 
-### Get raw data from OPA service ###
+### Get raw data from OPA service
 
 
 ```python
-
-
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 print(client.get_opa_raw_data("testapi/testdata"))  # response is {'result': ['world', 'hello']}
 
 # You can use query params for additional info
@@ -176,69 +187,63 @@
 print(client.get_opa_raw_data("userinfo",query_params={"metrics": True})) 
 
 # response is {'metrics': {'counter_server_query_cache_hit': 0, 'timer_rego_external_resolve_ns': 231, 'timer_rego_input_parse_ns': 381, 'timer_rego_query_compile_ns': 40173, 'timer_rego_query_eval_ns': 12674, 'timer_rego_query_parse_ns': 5692, 'timer_server_handler_ns': 83490}, 'result': {'user_roles': {'alice': ['admin'], 'bob': ['employee', 'billing'], 'eve': ['customer']}}}
 
 del client
 ```
 
-### Save policy to file from OPA service ###
-
 
-```python
+### Save policy to file from OPA service
 
 
+```python
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 client.opa_policy_to_file(policy_name="fromurl",path="/your/path",filename="example.rego")  # response is True
 
 del client
 ```
 
-### Delete data from OPA service ###
 
-
-```python
+### Delete data from OPA service
 
 
+```python
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 client.delete_opa_data("testapi")  # response is True
 
 del client
 ```
 
 
-### Information about policy path and rules ###
+### Information about policy path and rules
 
 
 ```python
-
-
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 client.get_policies_info()
 
 # response is {'testpolicy': {'path': ['http://your-opa-service/v1/data/play'], 'rules': ['http://your-opa-service/v1/data/play/hello']}
 
 del client
 ```
 
 
-### Check permissions ###
+### Check permissions
 
 
 ```python
-
-
 from opa_client.opa import OpaClient
 
 client = OpaClient() 
 
 permission_you_want_check = {"input": {"message": "hello"}}
 client.check_permission(input_data=permission_you_want_check, policy_name="testpolicy", rule_name="hello")
 
@@ -267,15 +272,14 @@
     m := input.message
     m == "world"
 }
 """
 
 check_data = {"message": "world"}
 client.check_policy_rule(input_data=check_data, package_path="play", rule_name="hello") # response {'result': True}
-
 ```
 
 ### Execute an Ad-hoc Query
 
 ```python
 from opa_client.opa import OpaClient
 
@@ -303,33 +307,33 @@
 # execute query 
 print(client.ad_hoc_query(query_params={"q": "data.userinfo.user_roles[name]"})) 
 # response is {'result': [{'name': 'eve'}, {'name': 'alice'}, {'name': 'bob'}]}
 
 #you can send body request
 print(client.ad_hoc_query(body={"query": "data.userinfo.user_roles[name] "})) 
 # response is {'result': [{'name': 'eve'}, {'name': 'alice'}, {'name': 'bob'}]}
-
 ```
 
 ### Check OPA healthy. If you want check bundels or plugins, add query params for this.
 
 ```python
 from opa_client.opa import OpaClient
 
 client = OpaClient()
 
 print(client.check_health()) # response is  True or False
 print(client.check_health({"bundle": True})) # response is  True or False
 # If your diagnostic url different than default url, you can provide it.
 print(client.check_health(diagnostic_url="http://localhost:8282/health"))  # response is  True or False
 print(client.check_health(query={"bundle": True}, diagnostic_url="http://localhost:8282/health"))  # response is  True or False
-
 ```
 
 
-# Contributing #
+# Contributing
 
-#### Free to open issue and send PR ####
+Fell free to open issue and send pull request.
 
-### OPA-python-client  supports Python >= 3.5
+Thanks To [Contributors](https://github.com/Turall/OPA-python-client/graphs/contributors).
+Contributions of any kind are welcome!
 
+Before you start please read [CONTRIBUTING](https://github.com/Turall/OPA-python-client/blob/master/CONTRIBUTING.md)
```

### Comparing `OPA-python-client-1.3.3/opa_client/OpaExceptions/OpaExceptions.py` & `opa_python_client-1.3.4/opa_client/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,116 +1,106 @@
 class ConnectionsError(Exception):
-    """
+    def __init__(self, expression, message):
+        """
         expression -- input expression in which the error occurred
         message -- explanation of the error
-    """
-
-    def __init__(self, expression, message):
+        """
         self.expression = expression
         self.message = message
 
 
 class QueryExecuteError(Exception):
-    """
+    def __init__(self, expression, message):
+        """
         expression -- input expression in which the error occurred
         message -- explanation of the error
-    """
-
-    def __init__(self, expression, message):
+        """
         self.expression = expression
         self.message = message
 
 
 class PolicyNotFoundError(Exception):
-    """
+    def __init__(self, expression, message):
+        """
         expression -- input expression in which the error occurred
         message -- explanation of the error
-    """
-
-    def __init__(self, expression, message):
+        """
         self.expression = expression
         self.message = message
 
 
 class CheckPermissionError(Exception):
-    """
+    def __init__(self, expression, message):
+        """
         expression -- input expression in which the error occurred
         message -- explanation of the error
-    """
-
-    def __init__(self, expression, message):
+        """
         self.expression = expression
         self.message = message
 
 
 class DeleteDataError(Exception):
-    """
+    def __init__(self, expression, message):
+        """
         expression -- input expression in which the error occurred
         message -- explanation of the error
-    """
-
-    def __init__(self, expression, message):
+        """
         self.expression = expression
         self.message = message
 
 
 class DeletePolicyError(Exception):
-    """
+    def __init__(self, expression, message):
+        """
         expression -- input expression in which the error occurred
         message -- explanation of the error
-    """
-
-    def __init__(self, expression, message):
+        """
         self.expression = expression
         self.message = message
 
 
 class PathNotFoundError(Exception):
-    """
+    def __init__(self, expression, message):
+        """
         expression -- input expression in which the error occurred
         message -- explanation of the error
-    """
-
-    def __init__(self, expression, message):
+        """
         self.expression = expression
         self.message = message
 
 
 class RegoParseError(Exception):
-    """
+    def __init__(self, expression, message):
+        """
         expression -- input expression in which the error occurred
         message -- explanation of the error
-    """
-
-    def __init__(self, expression, message):
+        """
         self.expression = expression
         self.message = message
 
 
 class SSLError(Exception):
-    """
+    def __init__(self, expression, message):
+        """
         expression -- input expression in which the error occurred
         message -- explanation of the error
-    """
-
-    def __init__(self, expression, message):
+        """
         self.expression = expression
         self.message = message
 
 
 class FileError(ValueError):
-    """
+    def __init__(self, expression, message):
+        """
         expression -- input expression in which the error occurred
         message -- explanation of the error
-    """
-    def __init__(self, expression, message):
+        """
         self.expression = expression
         self.message = message
 
 
 class TypeExecption(TypeError):
-    """
-        expression -- input expression in which the error occurred
-        message -- explanation of the error
-    """
     def __init__(self, expression):
+        """
+        expression -- input expression in which the error occurred
+        """
         self.expression = expression
```

### Comparing `OPA-python-client-1.3.3/opa_client/opa.py` & `opa_python_client-1.3.4/opa_client/opa.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,117 +4,124 @@
 # \ \  \|\  \   \ \  \|\  \ \ \  \|\  \    #
 #  \ \  \\\  \   \ \   ____\ \ \   __  \   #
 #   \ \  \\\  \   \ \  \___|  \ \  \ \  \  #
 #    \ \_______\   \ \__\      \ \__\ \__\ #
 #     \|_______|    \|__|       \|__|\|__| #
 ############################################
 
-import requests
-import urllib3
 import json
 import os
-from user_agent import generate_user_agent
-from typing import Union, Dict
+from typing import Dict, Union
 from urllib.parse import urlencode
-from .OpaExceptions import (CheckPermissionError,
-                            ConnectionsError, DeleteDataError,
-                            DeletePolicyError, PathNotFoundError,
-                            PolicyNotFoundError, RegoParseError,
-                            SSLError, FileError, TypeExecption,
-                            QueryExecuteError)
 
-__version__ = "1.3.3"
-__author__ = "Tural Muradov"
+import requests
+import urllib3
+from user_agent import generate_user_agent
+
+from .errors import (
+    CheckPermissionError,
+    ConnectionsError,
+    DeleteDataError,
+    DeletePolicyError,
+    FileError,
+    PathNotFoundError,
+    PolicyNotFoundError,
+    QueryExecuteError,
+    RegoParseError,
+    SSLError,
+    TypeExecption,
+)
+
+__version__ = '1.3.3'
+__author__ = 'Tural Muradov'
 __license__ = 'MIT'
 
 
 class OpaClient:
-    """ OpaClient client object to connect and manipulate OPA service.
-        ```
-        The class object holds session information necesseary to connect OPA service.
-        param :: host : to connect OPA service ,defaults to localhost
-        type  :: host: str
-        param :: port : to connect OPA service ,defaults to 8181
-        type  :: port : str or int
-        param :: version : provided REST API version by OPA,defaults to v1
-        type  :: version : str
-        param :: ssl : verify ssl certificates for https requests,defaults to False
-        type  :: ssl : bool
-        param :: cert : path to client certificate information to use for mutual TLS authentification
-        type  :: cert : str
-        param :: headers :  dictionary of headers to send, defaults to None
-        ```
-
+    """OpaClient client object to connect and manipulate OPA service.
+    ```
+    The class object holds session information necesseary to connect OPA service.
+    param :: host : to connect OPA service ,defaults to localhost
+    type  :: host: str
+    param :: port : to connect OPA service ,defaults to 8181
+    type  :: port : str or int
+    param :: version : provided REST API version by OPA,defaults to v1
+    type  :: version : str
+    param :: ssl : verify ssl certificates for https requests,defaults to False
+    type  :: ssl : bool
+    param :: cert : path to client certificate information to use for mutual TLS authentification
+    type  :: cert : str
+    param :: headers :  dictionary of headers to send, defaults to None
+    ```
     """
 
     def __init__(
         self,
-        host: str = "localhost",
+        host: str = 'localhost',
         port: int = 8181,
-        version: str = "v1",
+        version: str = 'v1',
         ssl: bool = False,
         cert: Union[None, str] = None,
         headers: Union[None, dict] = None,
         **kwargs,
     ):
         host = host.lstrip()
         self.__port = port
         self.__version = version
-        self.__policy_root = "{}/policies/{}"
-        self.__data_root = "{}/data/{}"
+        self.__policy_root = '{}/policies/{}'
+        self.__data_root = '{}/data/{}'
         self.__secure = False
-        self.__schema = "http://"
-        self.retries = kwargs.get("retries", 2)
-        self.timeout = kwargs.get("timeout", 1.5)
+        self.__schema = 'http://'
+        self.retries = kwargs.get('retries', 2)
+        self.timeout = kwargs.get('timeout', 1.5)
 
         if not isinstance(self.__port, int):
-            raise TypeError("The port must be integer")
+            raise TypeError('The port must be integer')
 
         if ssl:
             self.__ssl = ssl
             self.__cert = cert
             self.__secure = True
-            self.__schema = "https://"
+            self.__schema = 'https://'
 
         if not cert and ssl is True:
-            raise SSLError("ssl=True", "Make sure you  provide cert file")
+            raise SSLError('ssl=True', 'Make sure you  provide cert file')
 
-        if host.startswith("https://"):
+        if host.startswith('https://'):
             self.__host = host
-            self.__root_url = "{}:{}/{}".format(self.__host, self.__port,
-                                                self.__version)
+            self.__root_url = '{}:{}/{}'.format(self.__host, self.__port, self.__version)
 
-        elif host.startswith("http://"):
+        elif host.startswith('http://'):
             self.__host = host
             if self.__secure:
                 raise SSLError(
-                    "ssl=True",
-                    "With ssl enabled not possible to have connection with http",
+                    'ssl=True',
+                    'With ssl enabled not possible to have connection with http',
                 )
 
-            self.__root_url = "{}:{}/{}".format(self.__host, self.__port,
-                                                self.__version)
+            self.__root_url = '{}:{}/{}'.format(self.__host, self.__port, self.__version)
 
         else:
             self.__host = host
 
-            self.__root_url = "{}{}:{}/{}".format(self.__schema, self.__host,
-                                                  self.__port, self.__version)
+            self.__root_url = '{}{}:{}/{}'.format(
+                self.__schema, self.__host, self.__port, self.__version
+            )
 
         if headers:
             self.__headers = requests.utils.default_headers()
             self.__headers.update({**headers})
         else:
             self.__headers = requests.utils.default_headers()
 
-            self.__headers.update({"User-Agent": generate_user_agent()})
+            self.__headers.update({'User-Agent': generate_user_agent()})
 
         if self.__secure:
             self.__manager = urllib3.PoolManager(
-                cert_reqs="CERT_REQUIRED",
+                cert_reqs='CERT_REQUIRED',
                 assert_hostname=False,
                 ca_certs=self.__cert,
                 headers=self.__headers,
             )
             self.__session = self.__manager.request
         else:
             self.__manager = urllib3.PoolManager(headers=self.__headers)
@@ -130,473 +137,430 @@
         try:
             self.__manager.clear()
         except:  # noqa: E722
             pass
 
     def check_connection(self):
         """
-            Checks whether established connection config True or not.
-            if not properly configured will raise an ConnectionError.
+        Checks whether established connection config True or not.
+        if not properly configured will raise an ConnectionError.
         """
 
-        url = self.__policy_root.format(self.__root_url, "")
+        url = self.__policy_root.format(self.__root_url, '')
         try:
-            response = self.__session(
-                "GET", url, retries=self.retries, timeout=self.timeout)
+            response = self.__session('GET', url, retries=self.retries, timeout=self.timeout)
             if response.status == 200:
                 return "Yes I'm here :)"
 
         except Exception:
-            raise ConnectionsError("service unreachable",
-                                   "check config and try again")
+            raise ConnectionsError('service unreachable', 'check config and try again')
 
-        raise ConnectionsError("service unreachable",
-                               "check config and try again")
+        raise ConnectionsError('service unreachable', 'check config and try again')
 
     def check_health(self, query: Dict[str, bool] = None, diagnostic_url: str = None) -> bool:
         """
-            Check OPA healthy. If you want check bundels or plugins, add query params for this.
-            If your diagnostic url different than default url, you can provide it.
-            ```
-            param :: query : it is the url query string. default None
-            param :: diagnostic_url : OPA diagnostic url
-
-            example:
-                print(client.check_health())
-                print(client.check_health({"bundle": True}))
-                print(client.check_health(diagnostic_url="http://localhost:8282/health"))
-                print(client.check_health(query={"bundle": True}, diagnostic_url="http://localhost:8282/health"))
+        Check OPA healthy. If you want check bundels or plugins, add query params for this.
+        If your diagnostic url different than default url, you can provide it.
+        ```
+        param :: query : it is the url query string. default None
+        param :: diagnostic_url : OPA diagnostic url
 
+        example:
+            print(client.check_health())
+            print(client.check_health({"bundle": True}))
+            print(client.check_health(diagnostic_url="http://localhost:8282/health"))
+            print(client.check_health(
+                query={"bundle": True}, diagnostic_url="http://localhost:8282/health")
+            )
         """
         if diagnostic_url:
             url = diagnostic_url
         else:
-            url = "{}{}:{}/{}".format(self.__schema, self.__host,
-                                      self.__port, "health")
+            url = '{}{}:{}/{}'.format(self.__schema, self.__host, self.__port, 'health')
         if query:
             url = self.prepare_args(url, query)
-        response = self.__session(
-            "GET", url, retries=self.retries, timeout=self.timeout)
+        response = self.__session('GET', url, retries=self.retries, timeout=self.timeout)
         if response.status == 200:
             return True
         return False
 
     def get_policies_list(self) -> list:
-        """ Returns all  OPA policies in the service"""
+        """Returns all  OPA policies in the service"""
 
         return self.__get_policies_list()
 
     def get_policies_info(self) -> dict:
-        """ 
-            Returns information about each policy, including
-            policy path and policy rules
+        """
+        Returns information about each policy, including
+        policy path and policy rules
         """
         return self.__get_policies_info()
 
-    def update_opa_policy_fromstring(self, new_policy: str,
-                                     endpoint: str) -> bool:
-        """ Write your rego policy with using python string type and update your OPA policies.
-            ```
-            param :: new_policy : is the name of your new defined  rego policy. 
-            param :: endpoint : is the path of your new policy in OPA
-
-            example:
-                new_policy=
-                    package play
-
-                    default hello = false
-
-                    hello {
-                        m := input.message
-                        m == "world"
-                    }
-                client = OpaClient()
-                client.update_opa_policy_fromstring(new_policy,'exampleapi')
-            ```
+    def update_opa_policy_fromstring(self, new_policy: str, endpoint: str) -> bool:
+        """Write your rego policy with using python string type and update your OPA policies.
+        ```
+        param :: new_policy : is the name of your new defined  rego policy.
+        param :: endpoint : is the path of your new policy in OPA
 
+        example:
+            new_policy=
+                package play
+
+                default hello = false
+
+                hello {
+                    m := input.message
+                    m == "world"
+                }
+            client = OpaClient()
+            client.update_opa_policy_fromstring(new_policy,'exampleapi')
+        ```
         """
 
         return self.__update_opa_policy_fromstring(new_policy, endpoint)
 
     def update_opa_policy_fromfile(self, filepath: str, endpoint: str) -> bool:
-        """ Write your rego policy to file and update your OPA policies. """
+        """Write your rego policy to file and update your OPA policies."""
 
         return self.__update_opa_policy_fromfile(filepath, endpoint)
 
     def update_opa_policy_fromurl(self, url: str, endpoint: str) -> bool:
         """Update your OPA policies from internet."""
 
         return self.__update_opa_policy_fromurl(url, endpoint)
 
     def update_or_create_opa_data(self, new_data: dict, endpoint: str) -> bool:
-        """ Updates existing data or create new data for policy.
-            ```
-            param :: new_data : name of defined data
-            type  :: new_data : dict
-            param :: endpoint : is the path of your new data or existing one in OPA 
-            type  :: endpoint : str
-            example:
-                my_policy_list = [
-                    {"resource": "/api/someapi", "identity": "your_identity", "method": "PUT"},
-                    {"resource": "/api/someapi", "identity": "your_identity", "method": "GET"},
-                ]
-
-                client = OpaClient()
-                client.update_or_create_opa_data(my_policy_list,'exampledata/accesses')
-            ```
+        """Updates existing data or create new data for policy.
+        ```
+        param :: new_data : name of defined data
+        type  :: new_data : dict
+        param :: endpoint : is the path of your new data or existing one in OPA
+        type  :: endpoint : str
+        example:
+            my_policy_list = [
+                {"resource": "/api/someapi", "identity": "your_identity", "method": "PUT"},
+                {"resource": "/api/someapi", "identity": "your_identity", "method": "GET"},
+            ]
+
+            client = OpaClient()
+            client.update_or_create_opa_data(my_policy_list,'exampledata/accesses')
+        ```
         """
 
         return self.__update_opa_data(new_data, endpoint)
 
-    def get_opa_raw_data(self, data_name: str = "", query_params: Dict[str, bool] = dict()) -> dict:
-        """ Returns OPA raw data in string type 
-            ```
-            param :: data_name : OPA data name you want get
-            param :: query_params : query params in url for more information about metrics
-            ```
+    def get_opa_raw_data(self, data_name: str = '', query_params: Dict[str, bool] = dict()) -> dict:
+        """Returns OPA raw data in string type
+        ```
+        param :: data_name : OPA data name you want get
+        param :: query_params : query params in url for more information about metrics
+        ```
         """
         return self.__get_opa_raw_data(data_name, query_params)
 
-    def opa_policy_to_file(self,
-                           policy_name: str,
-                           path: Union[str, None] = None,
-                           filename: str = "opa_policy.rego"):
-        """ Write OPA service policy to the  file.
+    def opa_policy_to_file(
+        self, policy_name: str, path: Union[str, None] = None, filename: str = 'opa_policy.rego'
+    ):
+        """Write OPA service policy to the  file.
         ```
-            param :: policy_name : name of OPA policy
-            type  :: policy_name : str
+        param :: policy_name : name of OPA policy
+        type  :: policy_name : str
 
-            param :: path : path to save file ,default current path
-            type  :: path : str
+        param :: path : path to save file ,default current path
+        type  :: path : str
 
-            param :: filename : name of the file,default opa_policy.rego
-            type  :: filename : str
+        param :: filename : name of the file,default opa_policy.rego
+        type  :: filename : str
         ```
-
         """
         return self.__opa_policy_to_file(policy_name, path, filename)
 
     def get_opa_policy(self, policy_name: str) -> dict:
-        """Returns full info about policy, provided OPA service """
+        """Returns full info about policy, provided OPA service"""
 
         return self.__get_opa_policy(policy_name)
 
     def delete_opa_policy(self, policy_name: str) -> bool:
-        """ Deletes given OPA policy name """
+        """Deletes given OPA policy name"""
 
         return self.__delete_opa_policy(policy_name)
 
     def delete_opa_data(self, data_name: str) -> bool:
-        """ Deletes given OPA policy data name """
+        """Deletes given OPA policy data name"""
 
         return self.__delete_opa_data(data_name)
 
-    def check_permission(self, input_data: dict, policy_name: str,
-                         rule_name: str, query_params: Dict[str, bool] = dict()) -> dict:
+    def check_permission(
+        self,
+        input_data: dict,
+        policy_name: str,
+        rule_name: str,
+        query_params: Dict[str, bool] = dict(),
+    ) -> dict:
         """
         ```
-            params :: input_data    : data which you want check permission
-                type   :: input_data  : dict
+        params :: input_data    : data which you want check permission
+            type   :: input_data  : dict
 
-            params :: policy_name   : the name of policy resource
-                type   :: policy_name  : str
+        params :: policy_name   : the name of policy resource
+            type   :: policy_name  : str
 
-            params :: rule_name   : the name included in the policy
-                type   :: rule_name  : str
-            param :: query_params : query params in url for more information about metrics
-                type :: query_params : dict
+        params :: rule_name   : the name included in the policy
+            type   :: rule_name  : str
+        param :: query_params : query params in url for more information about metrics
+            type :: query_params : dict
         ```
         """
 
         return self.__check(input_data, policy_name, rule_name, query_params)
 
-    def check_policy_rule(self,
-                          input_data: dict,
-                          package_path: str,
-                          rule_name: str = None) -> dict:
+    def check_policy_rule(self, input_data: dict, package_path: str, rule_name: str = None) -> dict:
         """
         Queries a package rule with the given input data
         """
 
         return self.__query(input_data, package_path, rule_name)
 
     def ad_hoc_query(self, *, query_params: Dict[str, str] = None, body: Dict[str, str] = None):
-        """ Execute an ad-hoc query and return bindings for variables found in the query. 
+        """Execute an ad-hoc query and return bindings for variables found in the query.
         ```
-            param :: query_params for sending query string in url
-            param :: body  for sending query in request body
-
+        param :: query_params for sending query string in url
+        param :: body  for sending query in request body
         ```
         """
 
-        url = "{}{}:{}/{}/{}".format(self.__schema, self.__host,
-                                     self.__port, "v1", "query")
+        url = '{}{}:{}/{}/{}'.format(self.__schema, self.__host, self.__port, 'v1', 'query')
         if body:
-            encoded_json = json.dumps(body).encode("utf-8")
+            encoded_json = json.dumps(body).encode('utf-8')
             response = self.__session(
-                "POST",
+                'POST',
                 url,
                 body=encoded_json,
                 retries=self.retries,
                 timeout=self.timeout,
             )
         elif query_params:
             url = self.prepare_args(url, query_params)
-            response = self.__session("GET",
-                                      url,
-                                      retries=self.retries,
-                                      timeout=self.timeout)
-        data = json.loads(response.data.decode("utf-8"))
+            response = self.__session('GET', url, retries=self.retries, timeout=self.timeout)
+        data = json.loads(response.data.decode('utf-8'))
         if response.status == 200:
             return data
 
-        raise QueryExecuteError(data.get("code"), data.get("message"))
+        raise QueryExecuteError(data.get('code'), data.get('message'))
 
     def prepare_args(self, url: str, query_params: dict) -> str:
         if query_params:
             query_params = urlencode(query_params)
-            url = url + "?" + query_params
+            url = url + '?' + query_params
         return url
 
     def __get_opa_raw_data(self, data_name: str, query_params: Dict[str, bool]):
         url = self.__data_root.format(self.__root_url, data_name)
         url = self.prepare_args(url, query_params)
-        response = self.__session("GET",
-                                  url,
-                                  retries=self.retries,
-                                  timeout=self.timeout)
+        response = self.__session('GET', url, retries=self.retries, timeout=self.timeout)
         code = response.status
-        response = json.loads(response.data.decode("utf-8"))
-        return response if code == 200 else (code, "not found")
+        response = json.loads(response.data.decode('utf-8'))
+        return response if code == 200 else (code, 'not found')
 
     def __update_opa_data(self, new_data: dict, endpoint: str):
         url = self.__data_root.format(self.__root_url, endpoint)
 
-        encoded_json = json.dumps(new_data).encode("utf-8")
+        encoded_json = json.dumps(new_data).encode('utf-8')
         response = self.__session(
-            "PUT",
+            'PUT',
             url,
             body=encoded_json,
             retries=self.retries,
             timeout=self.timeout,
         )
         code = response.status
         return True if code == 204 else False
 
     def __update_opa_policy_fromfile(self, filepath: str, endpoint: str):
 
         if os.path.isfile(filepath):
-            with open(filepath, "r") as rf:
+            with open(filepath, 'r') as rf:
                 return self.__update_opa_policy_fromstring(rf.read(), endpoint)
 
-        raise FileError(f"{filepath}",
-                        "is not a file, make sure you provide a file")
+        raise FileError(f'{filepath}', 'is not a file, make sure you provide a file')
 
-    def __update_opa_policy_fromstring(self, new_policy: str,
-                                       endpoint: str) -> bool:
+    def __update_opa_policy_fromstring(self, new_policy: str, endpoint: str) -> bool:
 
         if not isinstance(new_policy, str) or not isinstance(endpoint, str):
-            raise TypeExecption(f"{new_policy} is not string type")
+            raise TypeExecption(f'{new_policy} is not string type')
 
         if new_policy:
             url = self.__policy_root.format(self.__root_url, endpoint)
 
             response = self.__session(
-                "PUT",
+                'PUT',
                 url,
                 body=new_policy.encode(),
                 headers=self.__headers,
                 retries=self.retries,
                 timeout=self.timeout,
             )
 
             if response.status == 200:
                 return True
 
-            raise RegoParseError(
-                response.status,
-                json.loads(response.data.decode())
-            )
+            raise RegoParseError(response.status, json.loads(response.data.decode()))
 
         return False
 
     def __get_opa_policy(self, policy_name: str) -> dict:
         url = self.__policy_root.format(self.__root_url, policy_name)
 
-        response = self.__session("GET",
-                                  url,
-                                  retries=self.retries,
-                                  timeout=self.timeout)
-        data = json.loads(response.data.decode("utf-8"))
+        response = self.__session('GET', url, retries=self.retries, timeout=self.timeout)
+        data = json.loads(response.data.decode('utf-8'))
         if response.status == 200:
 
             return data
 
-        raise PolicyNotFoundError(data.get("code"), data.get("message"))
+        raise PolicyNotFoundError(data.get('code'), data.get('message'))
 
     def __update_opa_policy_fromurl(self, url: str, endpoint: str) -> bool:
         response = requests.get(url, headers=self.__headers)
         return self.__update_opa_policy_fromstring(response.text, endpoint)
 
-    def __opa_policy_to_file(self, policy_name: str, path: Union[str, None],
-                             filename: str) -> bool:
+    def __opa_policy_to_file(self, policy_name: str, path: Union[str, None], filename: str) -> bool:
         raw_policy = self.__get_opa_policy(policy_name)
         if isinstance(raw_policy, dict):
             try:
                 if path:
-
-                    with open(f"{path}/{filename}", "wb") as wr:
-                        wr.write(raw_policy.get("result").get("raw").encode())
+                    with open(f'{path}/{filename}', 'wb') as wr:
+                        wr.write(raw_policy.get('result').get('raw').encode())
                 else:
-                    with open(filename, "wb") as wr:
-                        wr.write(raw_policy.get("result").get("raw").encode())
+                    with open(filename, 'wb') as wr:
+                        wr.write(raw_policy.get('result').get('raw').encode())
                 return True
 
             except:  # noqa: E722
-                raise PathNotFoundError("error when write file",
-                                        "path not found")
+                raise PathNotFoundError('error when write file', 'path not found')
 
     def __delete_opa_policy(self, policy_name: str) -> bool:
         url = self.__policy_root.format(self.__root_url, policy_name)
 
-        response = self.__session("DELETE",
-                                  url,
-                                  retries=self.retries,
-                                  timeout=self.timeout)
-        data = json.loads(response.data.decode("utf-8"))
+        response = self.__session('DELETE', url, retries=self.retries, timeout=self.timeout)
+        data = json.loads(response.data.decode('utf-8'))
         if response.status == 200:
             return True
 
-        raise DeletePolicyError(data.get("code"), data.get("message"))
+        raise DeletePolicyError(data.get('code'), data.get('message'))
 
     def __get_policies_list(self) -> list:
-        url = self.__policy_root.format(self.__root_url, "")
+        url = self.__policy_root.format(self.__root_url, '')
         temp = []
-        response = self.__session("GET",
-                                  url,
-                                  retries=self.retries,
-                                  timeout=self.timeout,
-                                  headers=self.__headers)
+        response = self.__session(
+            'GET', url, retries=self.retries, timeout=self.timeout, headers=self.__headers
+        )
 
         response = json.loads(response.data.decode())
 
-        for policy in response.get("result"):
-            if policy.get("id"):
-                temp.append(policy.get("id"))
+        for policy in response.get('result'):
+            if policy.get('id'):
+                temp.append(policy.get('id'))
 
         return temp
 
     def __delete_opa_data(self, data_name: str) -> bool:
         url = self.__data_root.format(self.__root_url, data_name)
 
-        response = self.__session("DELETE",
-                                  url,
-                                  retries=self.retries,
-                                  timeout=self.timeout)
+        response = self.__session('DELETE', url, retries=self.retries, timeout=self.timeout)
         if response.data:
-            data = json.loads(response.data.decode("utf-8"))
+            data = json.loads(response.data.decode('utf-8'))
         if response.status == 204:
             return True
 
-        raise DeleteDataError(data.get("code"), data.get("message"))
+        raise DeleteDataError(data.get('code'), data.get('message'))
 
     def __get_policies_info(self) -> dict:
-        url = self.__policy_root.format(self.__root_url, "")
-        policy = self.__session("GET",
-                                url,
-                                retries=self.retries,
-                                timeout=self.timeout,
-                                headers=self.__headers)
+        url = self.__policy_root.format(self.__root_url, '')
+        policy = self.__session(
+            'GET', url, retries=self.retries, timeout=self.timeout, headers=self.__headers
+        )
 
         policy = json.loads(policy.data.decode())
-        result = policy.get("result")
+        result = policy.get('result')
 
         temp_dict = {}
         for policy in result:
             temp_policy = []
             temp_rules = []
-            temp_url = ""
+            temp_url = ''
             permission_url = self.__root_url
-            for path in policy.get("ast").get("package").get("path"):
-                permission_url += "/" + path.get("value")
+            for path in policy.get('ast').get('package').get('path'):
+                permission_url += '/' + path.get('value')
             temp_policy.append(permission_url)
-            for rule in policy.get("ast").get("rules"):
-                if not rule.get("default"):
-                    continue
+            
+            rules = list(set(
+                [rule.get("head").get("name") for rule in policy.get("ast").get("rules")]
+            ))
+            for rule in rules:
                 temp_url = permission_url
-                temp_url += "/" + rule.get("head").get("name")
+                temp_url += "/" + rule
                 temp_rules.append(temp_url)
-            temp_dict[policy.get("id")] = {
-                "path": temp_policy,
-                "rules": temp_rules
-            }
+                
+            temp_dict[policy.get('id')] = {'path': temp_policy, 'rules': temp_rules}
 
         return temp_dict
 
-    def __check(self, input_data: dict, policy_name: str,
-                rule_name: str, query_params: Dict[str, bool]) -> dict:
+    def __check(
+        self, input_data: dict, policy_name: str, rule_name: str, query_params: Dict[str, bool]
+    ) -> dict:
         url = self.__policy_root.format(self.__root_url, policy_name)
 
-        policy = self.__session("GET",
-                                url,
-                                headers=self.__headers,
-                                retries=self.retries,
-                                timeout=self.timeout)
-        policy = json.loads(policy.data.decode("utf-8"))
-        result = policy.get("result")
+        policy = self.__session(
+            'GET', url, headers=self.__headers, retries=self.retries, timeout=self.timeout
+        )
+        policy = json.loads(policy.data.decode('utf-8'))
+        result = policy.get('result')
         find = False
         permission_url = self.__root_url
         if result:
-            for path in result.get("ast").get("package").get("path"):
-                permission_url += "/" + path.get("value")
+            for path in result.get('ast').get('package').get('path'):
+                permission_url += '/' + path.get('value')
 
-            for rule in result.get("ast").get("rules"):
-                if not rule.get("default"):
-                    continue
-                if rule.get("head").get("name") == rule_name:
+            rules = [rule.get("head").get("name") for rule in result.get("ast").get("rules")]
+            if rule_name in rules:
+                permission_url += "/" + rule_name
+                find = True
 
-                    permission_url += "/" + rule.get("head").get("name")
-                    find = True
         if find:
-            encoded_json = json.dumps(input_data).encode("utf-8")
+            encoded_json = json.dumps(input_data).encode('utf-8')
             permission_url = self.prepare_args(permission_url, query_params)
-            response = self.__session("POST",
-                                      permission_url,
-                                      body=encoded_json,
-                                      retries=self.retries,
-                                      timeout=self.timeout)
+            response = self.__session(
+                'POST',
+                permission_url,
+                body=encoded_json,
+                retries=self.retries,
+                timeout=self.timeout,
+            )
             if response.data:
-                data = json.loads(response.data.decode("utf-8"))
+                data = json.loads(response.data.decode('utf-8'))
                 return data
 
-        raise CheckPermissionError(f"{rule_name} rule not found",
-                                   "path or rule name not correct")
+        raise CheckPermissionError(f'{rule_name} rule not found', 'policy or rule name not correct')
 
-    def __query(self,
-                input_data: dict,
-                package_path: str,
-                rule_name: str = None) -> dict:
+    def __query(self, input_data: dict, package_path: str, rule_name: str = None) -> dict:
         if '.' in package_path:
             package_path = package_path.replace('.', '/')
         if rule_name:
             package_path = package_path + '/' + rule_name
         url = self.__data_root.format(self.__root_url, package_path)
 
-        encoded_json = json.dumps({'input': input_data}).encode("utf-8")
-        response = self.__session("POST",
-                                  url,
-                                  body=encoded_json,
-                                  retries=self.retries,
-                                  timeout=self.timeout)
+        encoded_json = json.dumps({'input': input_data}).encode('utf-8')
+        response = self.__session(
+            'POST', url, body=encoded_json, retries=self.retries, timeout=self.timeout
+        )
         if response.data:
-            data = json.loads(response.data.decode("utf-8"))
+            data = json.loads(response.data.decode('utf-8'))
             return data
 
-        raise CheckPermissionError(f"{rule_name} rule not found",
-                                   "policy or rule name not correct")
+        raise CheckPermissionError(f'{rule_name} rule not found', 'policy or rule name not correct')
 
     @property
     def _host(self):
         return self.__host
 
     @property
     def _port(self):
```

### Comparing `OPA-python-client-1.3.3/opa_client/test/test_opa.py` & `opa_python_client-1.3.4/opa_client/test/test_opa.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,88 +1,108 @@
 # -*- coding: utf-8 -*-
 """
 Unit tests for the OpaClient.
-
 """
 
 
 from unittest import TestCase
+
+from opa_client.errors import DeleteDataError, DeletePolicyError
 from opa_client.opa import OpaClient
-from opa_client.OpaExceptions import DeleteDataError, DeletePolicyError
 
 
 class TestClient(TestCase):
-
     def setUp(self):
         """Set up the test  for OpaClient object"""
 
         self.myclient = OpaClient()
 
     def tearDown(self):
-        """ Close the connection to the OPA server by deleting the client"""
+        """Close the connection to the OPA server by deleting the client"""
         del self.myclient
 
     def test_client(self):
-        """Set up the test  for OpaClient object"""
+        """Set up the test for OpaClient object"""
 
-        client = OpaClient("localhost", 8181, "v1")
-        self.assertEqual("http://localhost:8181/v1", client._root_url)
+        client = OpaClient('localhost', 8181, 'v1')
+        self.assertEqual('http://localhost:8181/v1', client._root_url)
 
-        client = OpaClient("localhost", 8181, "v1")
-        self.assertEqual("http://localhost:8181/v1", client._root_url)
+        client = OpaClient('localhost', 8181, 'v1')
+        self.assertEqual('http://localhost:8181/v1', client._root_url)
 
         self.assertFalse(False, self.myclient._secure)
-        self.assertEqual("http://", self.myclient._schema)
-        self.assertEqual("v1", self.myclient._version)
-        self.assertEqual("localhost", self.myclient._host)
+        self.assertEqual('http://', self.myclient._schema)
+        self.assertEqual('v1', self.myclient._version)
+        self.assertEqual('localhost', self.myclient._host)
         self.assertEqual(8181, self.myclient._port)
 
+    def test_connection_to_opa(self):
+        self.assertEqual("Yes I'm here :)", self.myclient.check_connection())
+    
     def test_functions(self):
+        new_policy = """
+            package test.policy
 
-        self.assertEqual("Yes I'm here :)", self.myclient.check_connection())
-        self.assertEqual(list(), self.myclient.get_policies_list())
-            
-        self.assertEqual(dict(), self.myclient.get_policies_info())
-     
-        # _dict = {'test': {'path': [
-        #     'http://localhost:8181/v1/data/play'], 'rules': ['http://localhost:8181/v1/data/play/hello']}}
+            import data.test.acl
+            import input
 
-        # self.assertEqual(_dict, self.myclient.get_policies_info())
-    
-        new_policy = '''
-            package play
+            default allow = false
 
-            default hello = false
+            allow {
+                access := acl[input.user]
+                access[_] == input.access
+            }
 
-            hello {
-                m := input.message
-                m == "world"
+            authorized_users[user] {
+                access := acl[user]
+                access[_] == input.access
             }
-        '''
-        self.assertEqual(
-            True, self.myclient.update_opa_policy_fromstring(new_policy, "test"))
-
-        self.assertEqual(["test"], self.myclient.get_policies_list())
-        _dict = {'test': {'path': ['http://localhost:8181/v1/data/play'],
-                            'rules': ['http://localhost:8181/v1/data/play/hello']}}
-
-        self.assertEqual(_dict, self.myclient.get_policies_info())
-
-        my_policy_list = [
-            {"resource": "/api/someapi", "identity": "your_identity", "method": "PUT"},
-            {"resource": "/api/someapi", "identity": "your_identity", "method": "GET"},
-        ]
-
-        self.assertTrue(True, self.myclient.update_or_create_opa_data(
-            my_policy_list, 'exampledata/accesses'))
-        value = {'result': {'hello': False}}
-          
-        self.assertEqual(True, self.myclient.opa_policy_to_file("test"))
-       
-        self.assertEqual(value, self.myclient.get_opa_raw_data("play"))
-    
-        self.assertTrue(True, self.myclient.delete_opa_policy("test"))
+        """
+
+        _dict = {
+            'test': {
+                'path': ['http://localhost:8181/v1/data/test/policy'],
+                'rules': [
+                    'http://localhost:8181/v1/data/test/policy/allow',
+                    'http://localhost:8181/v1/data/test/policy/authorized_users'
+                ],
+            }
+        }
+
+        my_policy_list = {
+            "alice": ["read","write"],
+            "bob": ["read"]
+        }
+
+        self.assertEqual(list(), self.myclient.get_policies_list())
+        self.assertEqual(dict(), self.myclient.get_policies_info())
+        self.assertEqual(True, self.myclient.update_opa_policy_fromstring(new_policy, 'test'))
+        self.assertEqual(['test'], self.myclient.get_policies_list())
+        
+        policy_info = self.myclient.get_policies_info()
+        self.assertEqual(_dict['test']['path'], policy_info['test']['path'])
+        for rule in _dict['test']['rules']:
+            self.assertIn(rule, policy_info['test']['rules'])
+
+        self.assertTrue(
+            True, self.myclient.update_or_create_opa_data(my_policy_list, 'test/acl')
+        )
+
+        self.assertEqual(True, self.myclient.opa_policy_to_file('test'))
+
+        value = {'result': {'acl': {'alice': ['read', 'write'], 'bob': ['read']}, 'policy': {'allow': False, 'authorized_users': []}}}
+        self.assertEqual(value, self.myclient.get_opa_raw_data('test'))
+
+        _input_a = {"input": {"user": "alice", "access": "write"}}
+        _input_b = {"input": {"access": "read"}}
+        value_a = {"result": True}
+        value_b = {"result": ["alice", "bob"]}
+        self.assertEqual(value_a, self.myclient.check_permission(input_data=_input_a, policy_name="test", rule_name="allow"))
+        self.assertEqual(value_b, self.myclient.check_permission(input_data=_input_b, policy_name="test", rule_name="authorized_users"))
+
+        self.assertTrue(True, self.myclient.delete_opa_policy('test'))
         with self.assertRaises(DeletePolicyError):
-            self.myclient.delete_opa_policy("test")
+            self.myclient.delete_opa_policy('test')
 
+        self.assertTrue(True, self.myclient.delete_opa_data('test/acl'))
         with self.assertRaises(DeleteDataError):
-            self.myclient.delete_opa_data("play")
+            self.myclient.delete_opa_data('test/acl')
```

