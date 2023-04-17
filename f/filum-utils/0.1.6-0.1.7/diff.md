# Comparing `tmp/filum-utils-0.1.6.tar.gz` & `tmp/filum-utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filum-utils-0.1.6.tar", last modified: Thu Mar 23 11:55:07 2023, max compression
+gzip compressed data, was "filum-utils-0.1.7.tar", last modified: Mon Apr 17 13:36:06 2023, max compression
```

## Comparing `filum-utils-0.1.6.tar` & `filum-utils-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-03-23 11:55:07.750614 filum-utils-0.1.6/
--rw-r--r--   0 hip        (502) staff       (20)      373 2023-03-23 11:55:07.750464 filum-utils-0.1.6/PKG-INFO
-drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-03-23 11:55:07.747161 filum-utils-0.1.6/filum_utils/
--rw-r--r--   0 hip        (502) staff       (20)      419 2023-03-20 07:08:14.000000 filum-utils-0.1.6/filum_utils/__init__.py
-drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-03-23 11:55:07.750256 filum-utils-0.1.6/filum_utils/clients/
--rw-r--r--   0 hip        (502) staff       (20)        0 2023-02-16 04:07:46.000000 filum-utils-0.1.6/filum_utils/clients/__init__.py
--rw-r--r--   0 hip        (502) staff       (20)     1327 2023-02-16 04:07:46.000000 filum-utils-0.1.6/filum_utils/clients/action.py
--rw-r--r--   0 hip        (502) staff       (20)       77 2023-02-16 04:07:46.000000 filum-utils-0.1.6/filum_utils/clients/analytics.py
--rw-r--r--   0 hip        (502) staff       (20)     1200 2023-02-16 04:07:46.000000 filum-utils-0.1.6/filum_utils/clients/common.py
--rw-r--r--   0 hip        (502) staff       (20)     8673 2023-03-22 08:59:51.000000 filum-utils-0.1.6/filum_utils/clients/connection.py
--rw-r--r--   0 hip        (502) staff       (20)     2189 2023-02-16 04:07:46.000000 filum-utils-0.1.6/filum_utils/clients/filum.py
--rw-r--r--   0 hip        (502) staff       (20)     1403 2023-02-16 04:07:46.000000 filum-utils-0.1.6/filum_utils/clients/log.py
--rw-r--r--   0 hip        (502) staff       (20)     2729 2023-03-20 16:41:50.000000 filum-utils-0.1.6/filum_utils/clients/mini_app.py
--rw-r--r--   0 hip        (502) staff       (20)     1806 2023-02-16 04:07:54.000000 filum-utils-0.1.6/filum_utils/clients/notification.py
--rw-r--r--   0 hip        (502) staff       (20)     1387 2023-03-14 11:31:26.000000 filum-utils-0.1.6/filum_utils/clients/subscription.py
--rw-r--r--   0 hip        (502) staff       (20)    15671 2023-03-23 11:54:40.000000 filum-utils-0.1.6/filum_utils/clients/subscription_object.py
--rw-r--r--   0 hip        (502) staff       (20)     1276 2023-03-14 11:31:26.000000 filum-utils-0.1.6/filum_utils/config.py
--rw-r--r--   0 hip        (502) staff       (20)      483 2023-03-20 11:48:27.000000 filum-utils-0.1.6/filum_utils/enums.py
--rw-r--r--   0 hip        (502) staff       (20)      182 2023-02-16 04:07:46.000000 filum-utils-0.1.6/filum_utils/errors.py
-drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-03-23 11:55:07.747870 filum-utils-0.1.6/filum_utils.egg-info/
--rw-r--r--   0 hip        (502) staff       (20)      373 2023-03-23 11:55:07.000000 filum-utils-0.1.6/filum_utils.egg-info/PKG-INFO
--rw-r--r--   0 hip        (502) staff       (20)      633 2023-03-23 11:55:07.000000 filum-utils-0.1.6/filum_utils.egg-info/SOURCES.txt
--rw-r--r--   0 hip        (502) staff       (20)        1 2023-03-23 11:55:07.000000 filum-utils-0.1.6/filum_utils.egg-info/dependency_links.txt
--rw-r--r--   0 hip        (502) staff       (20)       61 2023-03-23 11:55:07.000000 filum-utils-0.1.6/filum_utils.egg-info/requires.txt
--rw-r--r--   0 hip        (502) staff       (20)       12 2023-03-23 11:55:07.000000 filum-utils-0.1.6/filum_utils.egg-info/top_level.txt
--rw-r--r--   0 hip        (502) staff       (20)       38 2023-03-23 11:55:07.750664 filum-utils-0.1.6/setup.cfg
--rw-r--r--   0 hip        (502) staff       (20)      839 2023-03-23 11:54:57.000000 filum-utils-0.1.6/setup.py
+drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-04-17 13:36:06.474290 filum-utils-0.1.7/
+-rw-r--r--   0 hip        (502) staff       (20)      373 2023-04-17 13:36:06.474071 filum-utils-0.1.7/PKG-INFO
+drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-04-17 13:36:06.470595 filum-utils-0.1.7/filum_utils/
+-rw-r--r--   0 hip        (502) staff       (20)      419 2023-04-17 13:34:58.000000 filum-utils-0.1.7/filum_utils/__init__.py
+drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-04-17 13:36:06.473842 filum-utils-0.1.7/filum_utils/clients/
+-rw-r--r--   0 hip        (502) staff       (20)        0 2023-02-16 04:07:46.000000 filum-utils-0.1.7/filum_utils/clients/__init__.py
+-rw-r--r--   0 hip        (502) staff       (20)     1327 2023-02-16 04:07:46.000000 filum-utils-0.1.7/filum_utils/clients/action.py
+-rw-r--r--   0 hip        (502) staff       (20)       77 2023-02-16 04:07:46.000000 filum-utils-0.1.7/filum_utils/clients/analytics.py
+-rw-r--r--   0 hip        (502) staff       (20)     1200 2023-02-16 04:07:46.000000 filum-utils-0.1.7/filum_utils/clients/common.py
+-rw-r--r--   0 hip        (502) staff       (20)     8680 2023-04-17 13:35:10.000000 filum-utils-0.1.7/filum_utils/clients/connection.py
+-rw-r--r--   0 hip        (502) staff       (20)     2189 2023-02-16 04:07:46.000000 filum-utils-0.1.7/filum_utils/clients/filum.py
+-rw-r--r--   0 hip        (502) staff       (20)     1403 2023-02-16 04:07:46.000000 filum-utils-0.1.7/filum_utils/clients/log.py
+-rw-r--r--   0 hip        (502) staff       (20)     2865 2023-04-17 13:35:10.000000 filum-utils-0.1.7/filum_utils/clients/mini_app.py
+-rw-r--r--   0 hip        (502) staff       (20)     1806 2023-02-16 04:07:54.000000 filum-utils-0.1.7/filum_utils/clients/notification.py
+-rw-r--r--   0 hip        (502) staff       (20)     1387 2023-04-17 13:34:58.000000 filum-utils-0.1.7/filum_utils/clients/subscription.py
+-rw-r--r--   0 hip        (502) staff       (20)    16248 2023-04-17 13:35:10.000000 filum-utils-0.1.7/filum_utils/clients/subscription_object.py
+-rw-r--r--   0 hip        (502) staff       (20)     1276 2023-04-17 13:34:58.000000 filum-utils-0.1.7/filum_utils/config.py
+-rw-r--r--   0 hip        (502) staff       (20)      483 2023-04-17 13:34:58.000000 filum-utils-0.1.7/filum_utils/enums.py
+-rw-r--r--   0 hip        (502) staff       (20)      182 2023-02-16 04:07:46.000000 filum-utils-0.1.7/filum_utils/errors.py
+drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-04-17 13:36:06.471489 filum-utils-0.1.7/filum_utils.egg-info/
+-rw-r--r--   0 hip        (502) staff       (20)      373 2023-04-17 13:36:06.000000 filum-utils-0.1.7/filum_utils.egg-info/PKG-INFO
+-rw-r--r--   0 hip        (502) staff       (20)      633 2023-04-17 13:36:06.000000 filum-utils-0.1.7/filum_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 hip        (502) staff       (20)        1 2023-04-17 13:36:06.000000 filum-utils-0.1.7/filum_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 hip        (502) staff       (20)       61 2023-04-17 13:36:06.000000 filum-utils-0.1.7/filum_utils.egg-info/requires.txt
+-rw-r--r--   0 hip        (502) staff       (20)       12 2023-04-17 13:36:06.000000 filum-utils-0.1.7/filum_utils.egg-info/top_level.txt
+-rw-r--r--   0 hip        (502) staff       (20)       38 2023-04-17 13:36:06.474352 filum-utils-0.1.7/setup.cfg
+-rw-r--r--   0 hip        (502) staff       (20)      839 2023-04-17 13:35:47.000000 filum-utils-0.1.7/setup.py
```

### Comparing `filum-utils-0.1.6/filum_utils/clients/action.py` & `filum-utils-0.1.7/filum_utils/clients/action.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.6/filum_utils/clients/common.py` & `filum-utils-0.1.7/filum_utils/clients/common.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.6/filum_utils/clients/connection.py` & `filum-utils-0.1.7/filum_utils/clients/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             "data_value": value
         },
         auth=HTTPBasicAuth(config.APPSTORE_USERNAME, config.APPSTORE_PASSWORD)
     )
     return response.json()
 
 
-def get_connections_by_source_id(source_id: int, organization_id: str):
+def get_connections_by_source_id(source_id: int, organization_id: str = None):
     response = requests.request(
         method="GET",
         url=config.APPSTORE_BASE_URL + "/source/installed-sources",
         params={
             "source_id": source_id,
             "organization_id": organization_id
         },
```

### Comparing `filum-utils-0.1.6/filum_utils/clients/filum.py` & `filum-utils-0.1.7/filum_utils/clients/filum.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.6/filum_utils/clients/log.py` & `filum-utils-0.1.7/filum_utils/clients/log.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.6/filum_utils/clients/mini_app.py` & `filum-utils-0.1.7/filum_utils/clients/mini_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 
         self.log_client = LogClient()
 
     def get_data(self, key: str):
         data = self.installed_mini_app.get("data")
         return data and data.get(key)
 
+    def get_service_account_info(self):
+        return self.installed_mini_app and self.installed_mini_app.get("service_account_info")
+
     def update_data(self, updated_data: Dict[str, Any]):
         self.installed_mini_app = self._request(
             method="PUT",
             endpoint=f"/internal/installed-mini-apps/{self.installed_mini_app['id']}/data",
             data=updated_data
         )
```

### Comparing `filum-utils-0.1.6/filum_utils/clients/notification.py` & `filum-utils-0.1.7/filum_utils/clients/notification.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.6/filum_utils/clients/subscription.py` & `filum-utils-0.1.7/filum_utils/clients/subscription.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.6/filum_utils/clients/subscription_object.py` & `filum-utils-0.1.7/filum_utils/clients/subscription_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 ActionType = Dict[str, Any]
 AutomatedActionType = Dict[str, Any]
 CampaignType = Dict[str, Any]
 EventType = Optional[Dict[str, Any]]
 ObjectType = Optional[Dict[str, Any]]
 UserType = Optional[Dict[str, Any]]
 SubscriptionDataType = Optional[Dict[str, Any]]
+ConnectionsType = Optional[List[Dict[str, Any]]]
 
 
 class BaseSubscriptionObjectClient(ABC):
     def __init__(self, subscription_id: int):
         self.subscription_client = SubscriptionClient(subscription_id)
         self.action_client = ActionClient(action_id=self.subscription_client.get_action_id())
         self.filum_client = FilumClient()
@@ -190,36 +191,39 @@
                 title=f"{self.automated_action.get('name')} failed to run",
                 subtitle=error.get("notification_message") or NOTIFICATION_ERROR_MESSAGE_MAPPINGS[error["type"]],
             )
 
     def handle_transactional_trigger(
         self,
         process_transactional_fn: Callable[
-            [ActionType, AutomatedActionType, EventType, SubscriptionDataType],
+            [ActionType, AutomatedActionType, EventType, SubscriptionDataType, ConnectionsType],
             ProcessFunctionResponse
         ],
-        events: List[Dict[str, Any]]
+        events: List[Dict[str, Any]],
+        connections: List[Dict[str, Any]] = None
     ) -> TriggerFunctionResponse:
         for event in events:
             self._handle_trigger(
                 process_fn=process_transactional_fn,
-                data=event
+                data=event,
+                connections=connections
             )
 
         return {"is_finished": True}
 
     def handle_segment_users_on_demand_trigger(
         self,
         process_segment_user_fn: Callable[
-            [ActionType, AutomatedActionType, UserType, SubscriptionDataType],
+            [ActionType, AutomatedActionType, UserType, SubscriptionDataType, ConnectionsType],
             ProcessFunctionResponse
         ],
         properties: List[str] = None,
         required_properties: List[List[str]] = None,
-        last_current_index: int = None
+        last_current_index: int = None,
+        connections: List[Dict[str, Any]] = None
     ) -> TriggerFunctionResponse:
         if not last_current_index:
             last_current_index = 0
 
         subscription_data = self.get_subscription_data()
         current_index = subscription_data.get("last_current_index") or 0
         if current_index != last_current_index:
@@ -245,57 +249,67 @@
         total_processed_users = 0
         for user in users:
             current_index += 1
             total_processed_users += 1
 
             self._handle_trigger(
                 process_fn=process_segment_user_fn,
-                data=user
+                data=user,
+                connections=connections
             )
 
         if total_processed_users >= config.SEGMENT_RECORD_LIMIT:
             self.update_subscription_data({"last_current_index": current_index})
             self.action_client.sync({
                 "subscription_id": self.subscription_client.subscription["id"],
                 "last_current_index": last_current_index
             })
 
             return {"is_finished": False}
 
         return {"is_finished": True}
 
-    def handle_object_on_demand_trigger(self, process_segment_fn: Callable[
-        [ActionType, AutomatedActionType, ObjectType, SubscriptionDataType],
-        ProcessFunctionResponse
-    ]) -> TriggerFunctionResponse:
+    def handle_object_on_demand_trigger(
+        self,
+        process_segment_fn: Callable[
+            [ActionType, AutomatedActionType, ObjectType, SubscriptionDataType, ConnectionsType],
+            ProcessFunctionResponse
+        ],
+        connections: List[Dict[str, Any]] = None
+    ) -> TriggerFunctionResponse:
 
         context_type = self.get_context_type()
 
         data = {}
         if context_type == Object.SEGMENT:
             data = self.filum_client.get_segment(
                 segment_id=self.get_context_id(),
                 organization=self.subscription_client.get_organization()
             )
         elif context_type == Object.CAMPAIGN:
             data = self.filum_client.get_campaign(campaign_id=self.get_context_id())
 
         self._handle_trigger(
             process_fn=process_segment_fn,
-            data=data
+            data=data,
+            connections=connections
         )
 
         return {"is_finished": True}
 
-    def _handle_trigger(self, process_fn: Callable, data: Dict[str, Any]):
+    def _handle_trigger(self, process_fn: Callable, data: Dict[str, Any], connections: List[Dict[str, Any]] = None):
+        if not connections:
+            connections = []
+
         params = {
             "action": self.action_client.action,
             "automated_action": self.automated_action,
             "data": data,
-            "subscription_data": self.get_subscription_data()
+            "subscription_data": self.get_subscription_data(),
+            "connections": connections
         }
 
         process_fn(**params)
 
     def _get_object_route(self):
         return {
             "path": RoutePath.AUTOMATED_ACTIONS_DETAIL,
@@ -372,15 +386,15 @@
                 title=f"{self.campaign.get('name')} failed to run",
                 subtitle=error.get("notification_message") or NOTIFICATION_ERROR_MESSAGE_MAPPINGS[error["type"]],
             )
 
     def handle_transactional_trigger(
         self,
         process_transactional_fn: [
-            [ActionType, CampaignType, EventType, SubscriptionDataType],
+            [ActionType, CampaignType, EventType, SubscriptionDataType, ConnectionsType],
             ProcessFunctionResponse
         ],
         events: List[Dict[str, Any]],
         connections: List[Dict[str, Any]] = None
     ) -> TriggerFunctionResponse:
         for event in events:
             self._handle_trigger(
@@ -390,15 +404,15 @@
             )
 
         return {"is_finished": True}
 
     def handle_segment_users_on_demand_trigger(
         self,
         process_segment_user_fn: [
-            [ActionType, CampaignType, UserType, SubscriptionDataType],
+            [ActionType, CampaignType, UserType, SubscriptionDataType, ConnectionsType],
             ProcessFunctionResponse
         ],
         properties: List[str] = None,
         required_properties: List[List[str]] = None,
         connections: List[Dict[str, Any]] = None,
         last_current_index: int = None
     ) -> TriggerFunctionResponse:
```

### Comparing `filum-utils-0.1.6/filum_utils/config.py` & `filum-utils-0.1.7/filum_utils/config.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.6/filum_utils.egg-info/SOURCES.txt` & `filum-utils-0.1.7/filum_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.6/setup.py` & `filum-utils-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 
 from setuptools import setup, find_packages
 
 sys.path.insert(0, os.path.join(os.path.dirname(__file__), 'filum_analytics'))
 
-VERSION = "0.1.6"
+VERSION = "0.1.7"
 DESCRIPTION = "Filum Utils"
 LONG_DESCRIPTION = "Filum Utils"
 
 install_requires = [
     "requests==2.25.1",
     "filum-analytics-python==1.1.1",
     "glom==20.11.0",
```

