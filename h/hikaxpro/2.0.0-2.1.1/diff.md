# Comparing `tmp/hikaxpro-2.0.0.tar.gz` & `tmp/hikaxpro-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikaxpro-2.0.0.tar", last modified: Wed Apr  5 16:46:43 2023, max compression
+gzip compressed data, was "hikaxpro-2.1.1.tar", last modified: Sun Apr 16 22:08:05 2023, max compression
```

## Comparing `hikaxpro-2.0.0.tar` & `hikaxpro-2.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:46:43.882422 hikaxpro-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-05 16:46:43.882422 hikaxpro-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 16:46:43.882422 hikaxpro-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:46:43.882422 hikaxpro-2.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/src/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:46:43.882422 hikaxpro-2.0.0/src/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/src/errors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:46:43.882422 hikaxpro-2.0.0/src/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/src/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/src/helpers/sha256.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/src/helpers/xmlBuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:46:43.882422 hikaxpro-2.0.0/src/hikaxpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-05 16:46:43.000000 hikaxpro-2.0.0/src/hikaxpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-05 16:46:43.000000 hikaxpro-2.0.0/src/hikaxpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 16:46:43.000000 hikaxpro-2.0.0/src/hikaxpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-05 16:46:43.000000 hikaxpro-2.0.0/src/hikaxpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-05 16:46:43.000000 hikaxpro-2.0.0/src/hikaxpro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/src/hikaxpro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:46:43.882422 hikaxpro-2.0.0/src/models/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/src/models/SessionLogin.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/src/models/SessionLoginCap.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:46:43.882422 hikaxpro-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/tests/test_hikaxpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-05 16:46:33.000000 hikaxpro-2.0.0/tests/test_xmlBuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:08:05.825503 hikaxpro-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-16 22:08:05.825503 hikaxpro-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 22:08:05.825503 hikaxpro-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:08:05.821502 hikaxpro-2.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/src/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:08:05.821502 hikaxpro-2.1.1/src/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/src/errors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:08:05.821502 hikaxpro-2.1.1/src/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/src/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/src/helpers/sha256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/src/helpers/xmlBuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:08:05.821502 hikaxpro-2.1.1/src/hikaxpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-16 22:08:05.000000 hikaxpro-2.1.1/src/hikaxpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-16 22:08:05.000000 hikaxpro-2.1.1/src/hikaxpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:08:05.000000 hikaxpro-2.1.1/src/hikaxpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-16 22:08:05.000000 hikaxpro-2.1.1/src/hikaxpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 22:08:05.000000 hikaxpro-2.1.1/src/hikaxpro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/src/hikaxpro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:08:05.825503 hikaxpro-2.1.1/src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/src/models/SessionLogin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/src/models/SessionLoginCap.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:08:05.825503 hikaxpro-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/tests/test_hikaxpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-16 22:07:52.000000 hikaxpro-2.1.1/tests/test_xmlBuilder.py
```

### Comparing `hikaxpro-2.0.0/LICENSE` & `hikaxpro-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.0.0/PKG-INFO` & `hikaxpro-2.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: hikaxpro
-Version: 2.0.0
+Version: 2.1.1
 Summary: Hikvision AX Pro alarm kit ISAPI integration for home assistant alarm panel
 Author-email: Günkut Zeybek <gunkut.zeybek@gmail.com>, Petr Leo Compel <petrleocompel@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2022 smartha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Project-URL: repository, https://github.com/petrleocompel/hikaxpro/
 Keywords: hikvision,ISAPI,homeassistant
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `hikaxpro-2.0.0/pyproject.toml` & `hikaxpro-2.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hikaxpro"
-version = "2.0.0"
+version = "2.1.1"
 description = "Hikvision AX Pro alarm kit ISAPI integration for home assistant alarm panel"
 readme = "README.md"
 authors = [
     { name = "Günkut Zeybek", email = "gunkut.zeybek@gmail.com" },
     { name = "Petr Leo Compel", email = "petrleocompel@gmail.com" }
 ]
 license = { file = "LICENSE" }
@@ -19,19 +19,22 @@
 ]
 keywords = ["hikvision", "ISAPI", "homeassistant"]
 dependencies = [
     "requests"    
 ]
 requires-python = ">=3.9"
 
+[project.urls]
+repository = "https://github.com/petrleocompel/hikaxpro/"
+
 [project.optional-dependencies]
 dev = ["pytest", "requests_mock"]
 
 [tool.bumpver]
-current_version = "2.0.0"
+current_version = "2.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore: release version {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `hikaxpro-2.0.0/src/consts.py` & `hikaxpro-2.1.1/src/consts.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 class Endpoints:
     Session_Capabilities = "/ISAPI/Security/sessionLogin/capabilities?username="
     Session_Login = "/ISAPI/Security/sessionLogin"
+    Session_Logout = "/ISAPI/Security/sessionLogout"
     Alarm_Disarm = "/ISAPI/SecurityCP/control/disarm/{}"
     Alarm_ArmAway = "/ISAPI/SecurityCP/control/arm/{}?ways=away"
     Alarm_ArmHome = "/ISAPI/SecurityCP/control/arm/{}?ways=stay"
     SubSystemStatus = "/ISAPI/SecurityCP/status/subSystems"
     AlertStream = "/ISAPI/Event/notification/alertStream"
     DetectorConfig = "/ISAPI/SecurityCP/BasicParam/DetectorCfg"
     DetectorConfigCap = "/ISAPI/SecurityCP/BasicParam/DetectorCfg/capabilities"
```

### Comparing `hikaxpro-2.0.0/src/helpers/sha256.py` & `hikaxpro-2.1.1/src/helpers/sha256.py`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.0.0/src/helpers/xmlBuilder.py` & `hikaxpro-2.1.1/src/helpers/xmlBuilder.py`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.0.0/src/hikaxpro.egg-info/PKG-INFO` & `hikaxpro-2.1.1/src/hikaxpro.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: hikaxpro
-Version: 2.0.0
+Version: 2.1.1
 Summary: Hikvision AX Pro alarm kit ISAPI integration for home assistant alarm panel
 Author-email: Günkut Zeybek <gunkut.zeybek@gmail.com>, Petr Leo Compel <petrleocompel@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2022 smartha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Project-URL: repository, https://github.com/petrleocompel/hikaxpro/
 Keywords: hikvision,ISAPI,homeassistant
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `hikaxpro-2.0.0/src/hikaxpro.py` & `hikaxpro-2.1.1/src/hikaxpro.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,23 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class HikAxPro:
     """HikVisison Ax Pro Alarm panel coordinator."""
 
-    def __init__(self, host, username, password):
+    host: str
+    username: str
+    password: str
+    _cookie: Optional[str] = None
+
+    def __init__(self, host: str, username: str, password: str):
         self.host = host
         self.username = username
         self.password = password
-        self.cookie = ''
 
     def get_session_params(self):
         q_user = urllib.parse.quote(self.username)
         # q_password = urllib.parse.quote(self.password)
         # TODO needs basic auth ?
         # response = \
         #  requests.get(f"http://{q_user}:{q_password}@{self.host}{consts.Endpoints.Session_Capabilities}{q_user}")
@@ -62,15 +66,15 @@
         root = ElementTree.fromstring(xml_data)
         namespaces = {'xmlns': consts.XML_SCHEMA}
 
         session_id = HikAxPro._root_get_value(root, namespaces, "xmlns:sessionID")
         challenge = HikAxPro._root_get_value(root, namespaces, "xmlns:challenge")
         salt = HikAxPro._root_get_value(root, namespaces, "xmlns:salt")
         salt2 = HikAxPro._root_get_value(root, namespaces, "xmlns:salt2")
-        is_irreversible = HikAxPro._root_get_value(root, namespaces, "xmlns:isIrreversible", False)
+        is_irreversible = True if HikAxPro._root_get_value(root, namespaces, "xmlns:isIrreversible", False) == 'true' else False
         iterations = HikAxPro._root_get_value(root, namespaces, "xmlns:iterations")
         if iterations is not None:
             iterations = int(iterations)
         session_cap = SessionLoginCap.SessionLoginCap(
             session_id=session_id,
             challenge=challenge,
             salt=salt,
@@ -126,55 +130,87 @@
                 if cookie is None:
                     root = ElementTree.fromstring(login_response.text)
                     namespaces = {'xmlns': consts.XML_SCHEMA}
                     session_id = HikAxPro._root_get_value(root, namespaces, "xmlns:sessionID")
                     if session_id is not None:
                         cookie = "WebSession=" + session_id
                 else:
-                    self.cookie = cookie.split(";")[0]
+                    self._cookie = cookie.split(";")[0]
 
                 if cookie is None:
                     raise Exception("No cookie provided")
 
-                self.cookie = cookie
+                self._cookie = cookie
                 result = True
         except Exception as e:
             _LOGGER.error("Error in parsing response", exc_info=e)
             result = False
+            self._cookie = None
 
         return result
 
+    def logout(self):
+        response = self._base_json_request(f"http://{self.host}{consts.Endpoints.Session_Logout}", method=consts.Method.PUT)
+        if response.status_code != 200:
+            raise errors.UnexpectedResponseCodeError(response.status_code, response.text)
+        self._cookie = ''
+        return response.status_code == 200
+
+    def is_logged_in(self):
+        return self._cookie is not None
+
     @staticmethod
     def build_url(endpoint: str, is_json: bool = False):
         param_prefix = "&" if "?" in endpoint else "?"
         return f"{endpoint}{param_prefix}format=json" if is_json else endpoint
 
-    def _base_json_request(self, url: str, method: consts.Method = consts.Method.GET):
+    def _base_json_request(self, url: str, method: consts.Method = consts.Method.GET, data=None):
         endpoint = self.build_url(url, True)
-        response = self.make_request(endpoint, method, is_json=True)
+        response = self.make_request(endpoint, method, is_json=True, data=data)
 
         if response.status_code != 200:
             raise errors.UnexpectedResponseCodeError(response.status_code, response.text)
         if response.status_code == 200:
             return response.json()
 
-    def arm_home(self, sub_id: Optional[int] = None):
+    def arm_home(self, sub_id: Optional[int] = None, code: Optional[str] = None):
         sid = "0xffffffff" if sub_id is None else str(sub_id)
+        data = None
+        if code is None:
+            data = {
+              "Operate": {
+                "moduleOperateCode": code
+              }
+            }
         return self._base_json_request(f"http://{self.host}{consts.Endpoints.Alarm_ArmHome.replace('{}', sid)}",
-                                       method=consts.Method.PUT)
+                                       method=consts.Method.PUT, data=data)
 
-    def arm_away(self, sub_id: Optional[int] = None):
+    def arm_away(self, sub_id: Optional[int] = None, code: Optional[str] = None):
         sid = "0xffffffff" if sub_id is None else str(sub_id)
+        data = None
+        if code is None:
+            data = {
+              "Operate": {
+                "moduleOperateCode": code
+              }
+            }
         return self._base_json_request(f"http://{self.host}{consts.Endpoints.Alarm_ArmAway.replace('{}', sid)}",
-                                       method=consts.Method.PUT)
+                                       method=consts.Method.PUT, data=data)
 
-    def disarm(self, sub_id: Optional[int] = None):
+    def disarm(self, sub_id: Optional[int] = None, code: Optional[str] = None):
         sid = "0xffffffff" if sub_id is None else str(sub_id)
+        data = None
+        if code is None:
+            data = {
+              "Operate": {
+                "moduleOperateCode": code
+              }
+            }
         return self._base_json_request(f"http://{self.host}{consts.Endpoints.Alarm_Disarm.replace('{}', sid)}",
-                                       method=consts.Method.PUT)
+                                       method=consts.Method.PUT, data=data)
 
     def subsystem_status(self):
         return self._base_json_request(f"http://{self.host}{consts.Endpoints.SubSystemStatus}")
 
     def peripherals_status(self):
         return self._base_json_request(f"http://{self.host}{consts.Endpoints.PeripheralsStatus}")
 
@@ -240,26 +276,26 @@
     def keypad_status(self):
         return self._base_json_request(f"http://{self.host}{consts.Endpoints.KeypadStatus}")
 
     def repeater_status(self):
         return self._base_json_request(f"http://{self.host}{consts.Endpoints.RepeaterStatus}")
 
     def make_request(self, endpoint, method, data=None, is_json=False):
-        headers = {"Cookie": self.cookie}
+        headers = {"Cookie": self._cookie}
 
         if method == consts.Method.GET:
             response = requests.get(endpoint, headers=headers)
         elif method == consts.Method.POST:
             if is_json:
                 response = requests.post(endpoint, json=data, headers=headers)
             else:
                 response = requests.post(endpoint, data=data, headers=headers)
         elif method == consts.Method.PUT:
             if is_json:
-                response = requests.post(endpoint, json=data, headers=headers)
+                response = requests.put(endpoint, json=data, headers=headers)
             else:
                 response = requests.put(endpoint, data=data, headers=headers)
         else:
             return None
 
         if response.status_code == 401:
             self.connect()
```

### Comparing `hikaxpro-2.0.0/tests/test_hikaxpro.py` & `hikaxpro-2.1.1/tests/test_hikaxpro.py`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.0.0/tests/test_xmlBuilder.py` & `hikaxpro-2.1.1/tests/test_xmlBuilder.py`

 * *Files identical despite different names*

