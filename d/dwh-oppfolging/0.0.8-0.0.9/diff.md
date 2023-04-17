# Comparing `tmp/dwh_oppfolging-0.0.8.tar.gz` & `tmp/dwh_oppfolging-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwh_oppfolging-0.0.8.tar", max compression
+gzip compressed data, was "dwh_oppfolging-0.0.9.tar", max compression
```

## Comparing `dwh_oppfolging-0.0.8.tar` & `dwh_oppfolging-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1063 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/LICENSE
--rw-r--r--   0        0        0       23 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/README.md
--rw-r--r--   0        0        0        0 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/__init__.py
--rw-r--r--   0        0        0        0 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/apis/__init__.py
--rw-r--r--   0        0        0     6715 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/apis/brreg_api_v1.py
--rw-r--r--   0        0        0     1837 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/apis/brreg_api_v1_structs.py
--rw-r--r--   0        0        0      268 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/apis/kafka_api_v1.py
--rw-r--r--   0        0        0     7348 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/apis/oracle_api_v1.py
--rw-r--r--   0        0        0      865 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/apis/secrets_api_v1.py
--rw-r--r--   0        0        0     8538 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/apis/ssb_api_v1.py
--rw-r--r--   0        0        0      429 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/apis/ssb_api_v1_structs.py
--rw-r--r--   0        0        0        0 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/db/__init__.py
--rw-r--r--   0        0        0     2008 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/db/sql.py
--rw-r--r--   0        0        0      511 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/db/table.py
--rw-r--r--   0        0        0      771 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/misc/__init__.py
--rw-r--r--   0        0        0     1669 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/misc/datatypes.py
--rw-r--r--   0        0        0     2565 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/dwh_oppfolging/misc/transforms.py
--rw-r--r--   0        0        0      936 2023-01-10 15:20:14.822138 dwh_oppfolging-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 dwh_oppfolging-0.0.8/setup.py
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 dwh_oppfolging-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/LICENSE
+-rw-r--r--   0        0        0       23 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/README.md
+-rw-r--r--   0        0        0        0 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/__init__.py
+-rw-r--r--   0        0        0     6715 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/brreg_api_v1.py
+-rw-r--r--   0        0        0     1837 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/brreg_api_v1_structs.py
+-rw-r--r--   0        0        0      268 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/kafka_api_v1.py
+-rw-r--r--   0        0        0     7371 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/oracle_api_v1.py
+-rw-r--r--   0        0        0      865 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/secrets_api_v1.py
+-rw-r--r--   0        0        0     8538 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/ssb_api_v1.py
+-rw-r--r--   0        0        0      429 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/ssb_api_v1_structs.py
+-rw-r--r--   0        0        0        0 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/db/__init__.py
+-rw-r--r--   0        0        0     2008 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/db/sql.py
+-rw-r--r--   0        0        0      511 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/db/table.py
+-rw-r--r--   0        0        0      771 2023-01-11 09:28:29.550086 dwh_oppfolging-0.0.9/dwh_oppfolging/misc/__init__.py
+-rw-r--r--   0        0        0     1669 2023-01-11 09:28:29.550086 dwh_oppfolging-0.0.9/dwh_oppfolging/misc/datatypes.py
+-rw-r--r--   0        0        0     2565 2023-01-11 09:28:29.550086 dwh_oppfolging-0.0.9/dwh_oppfolging/misc/transforms.py
+-rw-r--r--   0        0        0      936 2023-01-11 09:28:29.550086 dwh_oppfolging-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 dwh_oppfolging-0.0.9/setup.py
+-rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 dwh_oppfolging-0.0.9/PKG-INFO
```

### Comparing `dwh_oppfolging-0.0.8/LICENSE` & `dwh_oppfolging-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.8/dwh_oppfolging/apis/brreg_api_v1.py` & `dwh_oppfolging-0.0.9/dwh_oppfolging/apis/brreg_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.8/dwh_oppfolging/apis/brreg_api_v1_structs.py` & `dwh_oppfolging-0.0.9/dwh_oppfolging/apis/brreg_api_v1_structs.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.8/dwh_oppfolging/apis/oracle_api_v1.py` & `dwh_oppfolging-0.0.9/dwh_oppfolging/apis/oracle_api_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     # No return value implies default type handling
     return None
 
 
 def create_oracle_connection(user: str):
     """creates oracle connection with db access
     you have to call .commit() yourself"""
-
+    user = user.upper()
     oracle_secrets = get_secrets()["ORACLE_ONPREM"][os.environ["ORACLE_ENV"]]
     con = oracledb.connect(  # type: ignore
         user=oracle_secrets[user+"_USER"],
         password=oracle_secrets[user+"_PW"],
         dsn=oracle_secrets["DSN"],
         encoding="utf-8",
         nencoding="utf-8",
```

### Comparing `dwh_oppfolging-0.0.8/dwh_oppfolging/apis/secrets_api_v1.py` & `dwh_oppfolging-0.0.9/dwh_oppfolging/apis/secrets_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.8/dwh_oppfolging/apis/ssb_api_v1.py` & `dwh_oppfolging-0.0.9/dwh_oppfolging/apis/ssb_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.8/dwh_oppfolging/db/sql.py` & `dwh_oppfolging-0.0.9/dwh_oppfolging/db/sql.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.8/dwh_oppfolging/misc/__init__.py` & `dwh_oppfolging-0.0.9/dwh_oppfolging/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.8/dwh_oppfolging/misc/datatypes.py` & `dwh_oppfolging-0.0.9/dwh_oppfolging/misc/datatypes.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.8/dwh_oppfolging/misc/transforms.py` & `dwh_oppfolging-0.0.9/dwh_oppfolging/misc/transforms.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.8/pyproject.toml` & `dwh_oppfolging-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dwh-oppfolging"
-version = "0.0.8"
+version = "0.0.9"
 description = "Oppfolging python package for DWH ETL"
 authors = ["Team Oppfolging"]
 packages = [{include = "dwh_oppfolging"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 oracledb = "^1.2.1"
```

### Comparing `dwh_oppfolging-0.0.8/setup.py` & `dwh_oppfolging-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['google-cloud-secret-manager>=2.12.6,<3.0.0',
  'ijson>=3.1.4,<4.0.0',
  'oracledb>=1.2.1,<2.0.0',
  'pendulum>=2.1.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'dwh-oppfolging',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Oppfolging python package for DWH ETL',
     'long_description': 'None',
     'author': 'Team Oppfolging',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

