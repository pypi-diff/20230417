# Comparing `tmp/electrickiwi-api-0.8.0.tar.gz` & `tmp/electrickiwi-api-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electrickiwi-api-0.8.0.tar", last modified: Sat Mar 18 19:58:27 2023, max compression
+gzip compressed data, was "electrickiwi-api-0.8.1.tar", last modified: Mon Apr 17 06:54:20 2023, max compression
```

## Comparing `electrickiwi-api-0.8.0.tar` & `electrickiwi-api-0.8.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-18 19:58:27.671961 electrickiwi-api-0.8.0/
--rw-rw-r--   0 michael   (1000) michael   (1000)    35149 2022-10-20 08:35:26.000000 electrickiwi-api-0.8.0/LICENSE
--rw-rw-r--   0 michael   (1000) michael   (1000)     1899 2023-03-18 19:58:27.671961 electrickiwi-api-0.8.0/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     1678 2023-03-18 19:58:13.000000 electrickiwi-api-0.8.0/README.md
--rw-rw-r--   0 michael   (1000) michael   (1000)      914 2023-03-18 19:58:13.000000 electrickiwi-api-0.8.0/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)      177 2023-03-18 19:58:27.671961 electrickiwi-api-0.8.0/setup.cfg
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-18 19:58:27.668961 electrickiwi-api-0.8.0/src/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-18 19:58:27.670961 electrickiwi-api-0.8.0/src/electrickiwi_api/
--rw-rw-r--   0 michael   (1000) michael   (1000)      428 2023-03-18 19:58:13.000000 electrickiwi-api-0.8.0/src/electrickiwi_api/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9022 2023-03-18 19:41:23.000000 electrickiwi-api-0.8.0/src/electrickiwi_api/api.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1499 2022-10-27 20:38:47.000000 electrickiwi-api-0.8.0/src/electrickiwi_api/auth.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      375 2022-10-26 00:12:16.000000 electrickiwi-api-0.8.0/src/electrickiwi_api/exceptions.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    21327 2023-03-18 19:41:23.000000 electrickiwi-api-0.8.0/src/electrickiwi_api/model.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-18 19:58:27.670961 electrickiwi-api-0.8.0/src/electrickiwi_api.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1899 2023-03-18 19:58:27.000000 electrickiwi-api-0.8.0/src/electrickiwi_api.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)      439 2023-03-18 19:58:27.000000 electrickiwi-api-0.8.0/src/electrickiwi_api.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-03-18 19:58:27.000000 electrickiwi-api-0.8.0/src/electrickiwi_api.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       15 2023-03-18 19:58:27.000000 electrickiwi-api-0.8.0/src/electrickiwi_api.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       17 2023-03-18 19:58:27.000000 electrickiwi-api-0.8.0/src/electrickiwi_api.egg-info/top_level.txt
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-03-18 19:58:27.670961 electrickiwi-api-0.8.0/tests/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1382 2022-12-16 23:22:54.000000 electrickiwi-api-0.8.0/tests/test_instance.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-17 06:54:20.202879 electrickiwi-api-0.8.1/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    35149 2022-10-20 08:35:26.000000 electrickiwi-api-0.8.1/LICENSE
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1899 2023-04-17 06:54:20.202879 electrickiwi-api-0.8.1/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1678 2023-03-18 19:58:13.000000 electrickiwi-api-0.8.1/README.md
+-rw-rw-r--   0 michael   (1000) michael   (1000)      914 2023-04-17 06:53:36.000000 electrickiwi-api-0.8.1/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)      177 2023-04-17 06:54:20.203879 electrickiwi-api-0.8.1/setup.cfg
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-17 06:54:20.199879 electrickiwi-api-0.8.1/src/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-17 06:54:20.201879 electrickiwi-api-0.8.1/src/electrickiwi_api/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      428 2023-03-18 19:58:13.000000 electrickiwi-api-0.8.1/src/electrickiwi_api/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9031 2023-04-17 05:33:03.000000 electrickiwi-api-0.8.1/src/electrickiwi_api/api.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1499 2022-10-27 20:38:47.000000 electrickiwi-api-0.8.1/src/electrickiwi_api/auth.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      483 2023-03-22 18:50:16.000000 electrickiwi-api-0.8.1/src/electrickiwi_api/exceptions.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    21334 2023-04-17 05:26:30.000000 electrickiwi-api-0.8.1/src/electrickiwi_api/model.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-17 06:54:20.202879 electrickiwi-api-0.8.1/src/electrickiwi_api.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1899 2023-04-17 06:54:20.000000 electrickiwi-api-0.8.1/src/electrickiwi_api.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)      439 2023-04-17 06:54:20.000000 electrickiwi-api-0.8.1/src/electrickiwi_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-04-17 06:54:20.000000 electrickiwi-api-0.8.1/src/electrickiwi_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       15 2023-04-17 06:54:20.000000 electrickiwi-api-0.8.1/src/electrickiwi_api.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       17 2023-04-17 06:54:20.000000 electrickiwi-api-0.8.1/src/electrickiwi_api.egg-info/top_level.txt
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-17 06:54:20.202879 electrickiwi-api-0.8.1/tests/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1382 2022-12-16 23:22:54.000000 electrickiwi-api-0.8.1/tests/test_instance.py
```

### Comparing `electrickiwi-api-0.8.0/LICENSE` & `electrickiwi-api-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `electrickiwi-api-0.8.0/PKG-INFO` & `electrickiwi-api-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrickiwi-api
-Version: 0.8.0
+Version: 0.8.1
 Author-email: Michael Arthur <michael@jumblesoft.co.nz>
 License: GNU-3.0
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Electric Kiwi Python API
```

### Comparing `electrickiwi-api-0.8.0/README.md` & `electrickiwi-api-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `electrickiwi-api-0.8.0/pyproject.toml` & `electrickiwi-api-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "electrickiwi-api"
-version     = "0.8.0"
+version     = "0.8.1"
 license     = {text = "GNU-3.0"}
 description = ""
 readme      = "README.md"
 authors     = [
     {name = "Michael Arthur", email = "michael@jumblesoft.co.nz"}
 ]
```

### Comparing `electrickiwi-api-0.8.0/src/electrickiwi_api/api.py` & `electrickiwi-api-0.8.1/src/electrickiwi_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,16 @@
         raise ApiException(f"Error request failed: {status}")
 
 
 class ElectricKiwiApi:
     """Electric Kiwi API"""
 
     def __init__(self, auth: AbstractAuth) -> None:
-        self.connection_id = None
-        self.customer_number = None
+        self.connection_id: int = None
+        self.customer_number: int = None
         self.auth = auth
 
     async def set_active_session(self) -> None:
         resp = await self.auth.request("get", ElectricKiwiEndpoint.session)
         check_status(resp.status)
 
         customer_session = Session.from_dict(await resp.json())
@@ -99,15 +99,15 @@
 
     async def get_billing_frequency(self) -> BillingFrequency:
         billing_frequency = await self.auth.request("get", ElectricKiwiEndpoint.billingFrequency.format(
             customerNumber=self.customer_number))
         check_status(billing_frequency.status)
         return BillingFrequency.from_dict(await billing_frequency.json())
 
-    # @paginated(by_query_params=get_next_page)
+    #@paginated(by_query_params=get_next_page)
     async def get_billing_bills(self, limit = 5, offset = 0) -> Bills:
         billing_bills = await self.auth.request("get", ElectricKiwiEndpoint.billingBills.format(customerNumber=self.customer_number, limit=limit, offset=offset))
         check_status(billing_bills.status)
         return Bills.from_dict(await billing_bills.json())
 
     async def get_billing_bill(self, bill_id) -> Bill:
         billing_bill = await self.auth.request("get",
```

### Comparing `electrickiwi-api-0.8.0/src/electrickiwi_api/auth.py` & `electrickiwi-api-0.8.1/src/electrickiwi_api/auth.py`

 * *Files identical despite different names*

### Comparing `electrickiwi-api-0.8.0/src/electrickiwi_api/model.py` & `electrickiwi-api-0.8.1/src/electrickiwi_api/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,15 +680,15 @@
             _is_active,
             _subscriptions,
         )
 
 
 @dataclass
 class Session:
-    customer: List[Customer]
+    customer: List[SessionCustomer]
     customer_numbers: List[int]
     type: str
 
     @staticmethod
     def from_dict(session_data: Any) -> "Session":
         session = session_data.get("data")
         _customer = [SessionCustomer.from_dict(y) for y in session.get("customer")]
```

### Comparing `electrickiwi-api-0.8.0/src/electrickiwi_api.egg-info/PKG-INFO` & `electrickiwi-api-0.8.1/src/electrickiwi_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrickiwi-api
-Version: 0.8.0
+Version: 0.8.1
 Author-email: Michael Arthur <michael@jumblesoft.co.nz>
 License: GNU-3.0
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Electric Kiwi Python API
```

### Comparing `electrickiwi-api-0.8.0/tests/test_instance.py` & `electrickiwi-api-0.8.1/tests/test_instance.py`

 * *Files identical despite different names*

