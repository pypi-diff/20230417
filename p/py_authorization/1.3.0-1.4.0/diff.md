# Comparing `tmp/py_authorization-1.3.0.tar.gz` & `tmp/py_authorization-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_authorization-1.3.0.tar", last modified: Mon Dec  5 14:02:31 2022, max compression
+gzip compressed data, was "py_authorization-1.4.0.tar", last modified: Mon Apr 17 17:47:44 2023, max compression
```

## Comparing `py_authorization-1.3.0.tar` & `py_authorization-1.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      119 2022-12-05 13:46:55.559068 py_authorization-1.3.0/.gitignore
--rw-r--r--   0        0        0       78 2022-11-09 13:19:55.248285 py_authorization-1.3.0/.isort.cfg
--rw-r--r--   0        0        0     1041 2022-11-09 13:19:55.248556 py_authorization-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      788 2022-11-03 12:45:18.023657 py_authorization-1.3.0/.vscode/settings.json
--rw-r--r--   0        0        0     1065 2022-11-07 19:18:16.174174 py_authorization-1.3.0/LICENSE
--rw-r--r--   0        0        0       23 2022-11-07 19:18:32.779163 py_authorization-1.3.0/README.md
--rwxr-xr-x   0        0        0      579 2022-11-09 13:19:55.248866 py_authorization-1.3.0/bin/new_line_check.sh
--rwxr-xr-x   0        0        0      481 2022-11-09 13:19:55.249149 py_authorization-1.3.0/bin/pdb_check.sh
--rw-r--r--   0        0        0      523 2022-12-05 13:53:13.424437 py_authorization-1.3.0/py_authorization/__init__.py
--rw-r--r--   0        0        0    11250 2022-12-02 18:45:28.351112 py_authorization-1.3.0/py_authorization/authorization.py
--rw-r--r--   0        0        0      325 2022-11-30 16:12:25.600432 py_authorization-1.3.0/py_authorization/context.py
--rw-r--r--   0        0        0      398 2022-11-04 03:50:18.628749 py_authorization-1.3.0/py_authorization/policy.py
--rw-r--r--   0        0        0      455 2022-11-07 19:13:47.101298 py_authorization-1.3.0/py_authorization/policy_strategy.py
--rw-r--r--   0        0        0      619 2022-11-30 16:12:25.600829 py_authorization-1.3.0/py_authorization/policy_strategy_builder.py
--rw-r--r--   0        0        0        0 2022-11-07 15:50:03.558350 py_authorization-1.3.0/py_authorization/py.typed
--rw-r--r--   0        0        0     5538 2022-11-04 03:48:00.918664 py_authorization-1.3.0/py_authorization/sql_parser.py
--rw-r--r--   0        0        0      135 2022-12-02 12:53:12.500907 py_authorization-1.3.0/py_authorization/user.py
--rw-r--r--   0        0        0      616 2022-12-05 13:51:43.790025 py_authorization-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      190 2022-12-05 13:35:32.334246 py_authorization-1.3.0/requirements.txt
--rw-r--r--   0        0        0      377 2022-11-03 14:55:31.590784 py_authorization-1.3.0/setup.cfg
--rw-r--r--   0        0        0      309 2022-11-07 15:54:53.936572 py_authorization-1.3.0/setup.py
--rw-r--r--   0        0        0      106 2022-11-10 14:34:34.500890 py_authorization-1.3.0/tests/conftest.py
--rw-r--r--   0        0        0     5728 2022-11-30 16:12:25.601244 py_authorization-1.3.0/tests/test_authorization.py
--rw-r--r--   0        0        0     3181 2022-11-30 16:12:25.601396 py_authorization-1.3.0/tests/test_policy_finder.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 py_authorization-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      119 2022-12-05 13:46:55.559068 py_authorization-1.4.0/.gitignore
+-rw-r--r--   0        0        0       78 2022-11-09 13:19:55.248285 py_authorization-1.4.0/.isort.cfg
+-rw-r--r--   0        0        0     1041 2022-11-09 13:19:55.248556 py_authorization-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      788 2022-11-03 12:45:18.023657 py_authorization-1.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1065 2022-11-07 19:18:16.174174 py_authorization-1.4.0/LICENSE
+-rw-r--r--   0        0        0       23 2022-11-07 19:18:32.779163 py_authorization-1.4.0/README.md
+-rwxr-xr-x   0        0        0      579 2022-11-09 13:19:55.248866 py_authorization-1.4.0/bin/new_line_check.sh
+-rwxr-xr-x   0        0        0      481 2022-11-09 13:19:55.249149 py_authorization-1.4.0/bin/pdb_check.sh
+-rw-r--r--   0        0        0      523 2023-04-17 17:43:28.478172 py_authorization-1.4.0/py_authorization/__init__.py
+-rw-r--r--   0        0        0    11250 2023-02-20 17:33:40.883491 py_authorization-1.4.0/py_authorization/authorization.py
+-rw-r--r--   0        0        0      325 2022-11-30 16:12:25.600432 py_authorization-1.4.0/py_authorization/context.py
+-rw-r--r--   0        0        0      398 2022-11-04 03:50:18.628749 py_authorization-1.4.0/py_authorization/policy.py
+-rw-r--r--   0        0        0      455 2022-11-07 19:13:47.101298 py_authorization-1.4.0/py_authorization/policy_strategy.py
+-rw-r--r--   0        0        0      619 2022-11-30 16:12:25.600829 py_authorization-1.4.0/py_authorization/policy_strategy_builder.py
+-rw-r--r--   0        0        0        0 2022-11-07 15:50:03.558350 py_authorization-1.4.0/py_authorization/py.typed
+-rw-r--r--   0        0        0     5538 2022-11-04 03:48:00.918664 py_authorization-1.4.0/py_authorization/sql_parser.py
+-rw-r--r--   0        0        0      128 2023-04-17 17:11:09.746541 py_authorization-1.4.0/py_authorization/user.py
+-rw-r--r--   0        0        0      383 2022-12-05 14:25:45.789192 py_authorization-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      179 2022-12-05 14:05:43.744172 py_authorization-1.4.0/requirements.txt
+-rw-r--r--   0        0        0      377 2022-11-03 14:55:31.590784 py_authorization-1.4.0/setup.cfg
+-rw-r--r--   0        0        0      309 2022-12-05 14:25:51.504916 py_authorization-1.4.0/setup.py
+-rw-r--r--   0        0        0      106 2022-11-10 14:34:34.500890 py_authorization-1.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     5906 2023-04-17 17:36:34.843037 py_authorization-1.4.0/tests/test_authorization.py
+-rw-r--r--   0        0        0     3304 2023-04-17 17:35:45.267432 py_authorization-1.4.0/tests/test_policy_finder.py
+-rw-r--r--   0        0        0      230 1970-01-01 00:00:00.000000 py_authorization-1.4.0/PKG-INFO
```

### Comparing `py_authorization-1.3.0/.pre-commit-config.yaml` & `py_authorization-1.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py_authorization-1.3.0/.vscode/settings.json` & `py_authorization-1.4.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `py_authorization-1.3.0/LICENSE` & `py_authorization-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_authorization-1.3.0/bin/new_line_check.sh` & `py_authorization-1.4.0/bin/new_line_check.sh`

 * *Files identical despite different names*

### Comparing `py_authorization-1.3.0/py_authorization/__init__.py` & `py_authorization-1.4.0/py_authorization/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Easily manage authorization complex logic"""
 
-__version__ = "1.3.0"
+__version__ = "1.4.0"
 
 from .authorization import Authorization, CheckResponse
 from .context import Context
 from .policy import Policy, Strategy
 from .policy_strategy import PolicyStrategy
 from .policy_strategy_builder import PolicyStrategyBuilder, StrategyMapper
 from .user import User
```

### Comparing `py_authorization-1.3.0/py_authorization/authorization.py` & `py_authorization-1.4.0/py_authorization/authorization.py`

 * *Files identical despite different names*

### Comparing `py_authorization-1.3.0/py_authorization/policy_strategy_builder.py` & `py_authorization-1.4.0/py_authorization/policy_strategy_builder.py`

 * *Files identical despite different names*

### Comparing `py_authorization-1.3.0/py_authorization/sql_parser.py` & `py_authorization-1.4.0/py_authorization/sql_parser.py`

 * *Files identical despite different names*

### Comparing `py_authorization-1.3.0/tests/test_authorization.py` & `py_authorization-1.4.0/tests/test_authorization.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,31 +40,35 @@
     roles=[Role.VIEWER],
     actions=[Action.READ],
     strategies=[Strategy("TestStrategy")],
 )
 
 
 def test_authorization_evaluates_simple_policy() -> None:
-    authorization = Authorization(policies=[admin_policy], strategy_mapper_callable=Mock(return_value={}))
+    authorization = Authorization(
+        policies=[admin_policy], strategy_mapper_callable=Mock(return_value={})
+    )
     form = Mock()
-    user = User(role=Role.ADMIN)
+    user = User(role=Role.ADMIN, id=None)
     resp = authorization.apply_policies_to_one(
         user=user,
         entity=form,
         resource_to_check="Form",
         action=Action.CREATE,
     )
 
     assert_that(resp).is_equal_to(form)
 
 
 def test_authorization_evaluates_simple_policy_and_rejects_the_object() -> None:
-    authorization = Authorization(policies=[admin_policy], strategy_mapper_callable=Mock(return_value={}))
+    authorization = Authorization(
+        policies=[admin_policy], strategy_mapper_callable=Mock(return_value={})
+    )
     form = Mock()
-    user = User(role=Role.VIEWER)
+    user = User(role=Role.VIEWER, id=None)
 
     resp = authorization.apply_policies_to_one(
         user=user,
         entity=form,
         resource_to_check="Form",
         action=Action.CREATE,
     )
@@ -73,30 +77,32 @@
 
 
 def test_authorization_evaluates_simple_policy_multiple_objects() -> None:
     authorization = Authorization(
         policies=[admin_policy], strategy_mapper_callable=Mock(return_value={})
     )
     forms = [Mock(), Mock()]
-    user = User(role=Role.ADMIN)
+    user = User(role=Role.ADMIN, id=None)
 
     resp = authorization.apply_policies_to_many(
         user=user,
         entities=forms,
         resource_to_check="Form",
         action=Action.CREATE,
     )
 
     assert_that(resp).is_equal_to(forms)
 
 
 def test_authorization_evaluates_simple_policy_and_reject_multiple_objects() -> None:
-    authorization = Authorization(policies=[admin_policy], strategy_mapper_callable=Mock(return_value={}))
+    authorization = Authorization(
+        policies=[admin_policy], strategy_mapper_callable=Mock(return_value={})
+    )
     forms = [Mock(), Mock()]
-    user = User(role=Role.VIEWER)
+    user = User(role=Role.VIEWER, id=None)
 
     resp = authorization.apply_policies_to_many(
         user=user,
         entities=forms,
         resource_to_check="Form",
         action=Action.CREATE,
     )
@@ -108,19 +114,20 @@
     class TestStrategy(PolicyStrategy):
         def apply_policies_to_entity(self, entity: T, context: Context) -> Optional[T]:
             mock = cast(Mock, entity)
             return mock if mock.id == 2 else None
 
     strategy_mapper: StrategyMapper = {"TestStrategy": TestStrategy}
     authorization = Authorization(
-        policies=[strategy_policy], strategy_mapper_callable=Mock(return_value=strategy_mapper)
+        policies=[strategy_policy],
+        strategy_mapper_callable=Mock(return_value=strategy_mapper),
     )
 
     forms = [Mock(id=1), Mock(id=2)]
-    user = User(role=Role.VIEWER)
+    user = User(role=Role.VIEWER, id=None)
 
     resp = authorization.apply_policies_to_many(
         user=user,
         entities=forms,
         resource_to_check="Form",
         action=Action.READ,
     )
@@ -134,48 +141,54 @@
         def apply_policies_to_entity(self, entity: T, context: Context) -> Optional[T]:
             mock = cast(Mock, entity)
             return mock if mock.id == 2 else None
 
     strategy_mapper: StrategyMapper = {"TestStrategy": TestStrategy}
     authorization = Authorization(
         policies=[admin_policy],
-        strategy_mapper_callable=Mock(return_value=strategy_mapper)
+        strategy_mapper_callable=Mock(return_value=strategy_mapper),
     )
     form = Mock()
-    user = User(role=Role.ADMIN)
+    user = User(role=Role.ADMIN, id=None)
 
     resp = authorization.apply_policies_to_one(
         user=user,
         entity=form,
         resource_to_check="Form",
         action=Action.CREATE,
     )
 
     assert_that(resp).is_equal_to(form)
 
 
 def test_authorization_evaluates_simple_policy_query() -> None:
-    authorization = Authorization(policies=[admin_policy], strategy_mapper_callable=Mock(return_value={}))
+    authorization = Authorization(
+        policies=[admin_policy], strategy_mapper_callable=Mock(return_value={})
+    )
     query = Mock()
-    user = User(role=Role.ADMIN)
+    user = User(role=Role.ADMIN, id=None)
 
     resp = authorization.apply_policies_to_query(
         user=user,
         query=query,
         action=Action.CREATE,
         resources_to_check=["Form"],
     )
 
     assert_that(resp).is_equal_to(query)
 
 
-def test_authorization_evaluates_simple_policy_query_and_apply_empty_filter_when_is_rejected() -> None:
-    authorization = Authorization(policies=[admin_policy], strategy_mapper_callable=Mock(return_value={}))
+def test_authorization_evaluates_simple_policy_query_and_apply_empty_filter_when_is_rejected() -> (
+    None
+):
+    authorization = Authorization(
+        policies=[admin_policy], strategy_mapper_callable=Mock(return_value={})
+    )
     query = Mock()
-    user = User(role=Role.VIEWER)
+    user = User(role=Role.VIEWER, id=None)
 
     resp = authorization.apply_policies_to_query(
         user=user,
         query=query,
         action=Action.CREATE,
         resources_to_check=["Form"],
     )
@@ -187,18 +200,19 @@
 def test_authorization_applies_policy_with_strategy_to_query() -> None:
     class TestStrategy(PolicyStrategy):
         def apply_policies_to_query(self, query: Query, context: Context) -> Query:
             query.filter("test_filter")
 
     strategy_mapper: StrategyMapper = {"TestStrategy": TestStrategy}
     authorization = Authorization(
-        policies=[strategy_policy], strategy_mapper_callable=Mock(return_value=strategy_mapper)
+        policies=[strategy_policy],
+        strategy_mapper_callable=Mock(return_value=strategy_mapper),
     )
     query = Mock()
-    user = User(role=Role.VIEWER)
+    user = User(role=Role.VIEWER, id=None)
 
     authorization.apply_policies_to_query(
         user=user,
         query=query,
         action=Action.READ,
         resources_to_check=["Form"],
     )
```

### Comparing `py_authorization-1.3.0/tests/test_policy_finder.py` & `py_authorization-1.4.0/tests/test_policy_finder.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,92 +33,101 @@
     resources=["Deal"],
     roles=[Role.EDITOR, Role.ADMIN],
     actions=[Action.UPDATE],
 )
 
 
 def test_find_wildcard_policy() -> None:
-    authorization = Authorization(policies=[wildcard_policy], strategy_mapper_callable=Mock(return_value={}))
-    user = User(role=Role.ADMIN)
+    authorization = Authorization(
+        policies=[wildcard_policy], strategy_mapper_callable=Mock(return_value={})
+    )
+    user = User(role=Role.ADMIN, id=None)
 
     resp = authorization._get_policy(
         user=user,
         resource_to_access="Form",
         action=Action.READ,
         sub_action=None,
     )
 
     assert_that(resp).is_equal_to(wildcard_policy)
 
 
 def test_find_viewer_policy() -> None:
     authorization = Authorization(
-        policies=[viewer_policy, wildcard_policy], strategy_mapper_callable=Mock(return_value={})
+        policies=[viewer_policy, wildcard_policy],
+        strategy_mapper_callable=Mock(return_value={}),
     )
-    user = User(role=Role.VIEWER)
+    user = User(role=Role.VIEWER, id=None)
 
     resp = authorization._get_policy(
         user=user,
         resource_to_access="Form",
         action=Action.READ,
         sub_action=None,
     )
 
     assert_that(resp).is_equal_to(viewer_policy)
 
 
 def test_find_no_policy_when_role_doesnt_match() -> None:
-    authorization = Authorization(policies=[viewer_policy], strategy_mapper_callable=Mock(return_value={}))
-    user = User(role=Role.EDITOR)
+    authorization = Authorization(
+        policies=[viewer_policy], strategy_mapper_callable=Mock(return_value={})
+    )
+    user = User(role=Role.EDITOR, id=None)
 
     resp = authorization._get_policy(
         user=user,
         resource_to_access="Form",
         action=Action.READ,
         sub_action=None,
     )
 
     assert_that(resp).is_none()
 
 
 def test_find_form_policy() -> None:
     authorization = Authorization(
-        policies=[form_policy, viewer_policy, wildcard_policy], strategy_mapper_callable=Mock(return_value={})
+        policies=[form_policy, viewer_policy, wildcard_policy],
+        strategy_mapper_callable=Mock(return_value={}),
     )
-    user = User(role=Role.ADMIN)
+    user = User(role=Role.ADMIN, id=None)
 
     resp = authorization._get_policy(
         user=user,
         resource_to_access="Form",
         action=Action.READ,
         sub_action=None,
     )
 
     assert_that(resp).is_equal_to(form_policy)
 
 
 def test_find_no_policy_when_resource_is_not_found() -> None:
-    authorization = Authorization(policies=[form_policy], strategy_mapper_callable=Mock(return_value={}))
-    user = User(role=Role.ADMIN)
+    authorization = Authorization(
+        policies=[form_policy], strategy_mapper_callable=Mock(return_value={})
+    )
+    user = User(role=Role.ADMIN, id=None)
 
     resp = authorization._get_policy(
         user=user,
         resource_to_access="Submissions",
         action=Action.READ,
         sub_action=None,
     )
 
     assert_that(resp).is_none()
 
 
 def test_find_update_policy() -> None:
     authorization = Authorization(
-        policies=[update_policy, wildcard_policy], strategy_mapper_callable=Mock(return_value={})
+        policies=[update_policy, wildcard_policy],
+        strategy_mapper_callable=Mock(return_value={}),
     )
-    user = User(role=Role.EDITOR)
+    user = User(role=Role.EDITOR, id=None)
 
     resp = authorization._get_policy(
         user=user,
         resource_to_access="Form",
         action=Action.UPDATE,
         sub_action=None,
     )
```

