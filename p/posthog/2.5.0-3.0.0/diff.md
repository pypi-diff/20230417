# Comparing `tmp/posthog-2.5.0.tar.gz` & `tmp/posthog-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posthog-2.5.0.tar", last modified: Mon Apr 10 19:14:04 2023, max compression
+gzip compressed data, was "posthog-3.0.0.tar", last modified: Mon Apr 17 11:08:00 2023, max compression
```

## Comparing `posthog-2.5.0.tar` & `posthog-3.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:14:04.455840 posthog-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-04-10 19:13:52.000000 posthog-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-10 19:13:52.000000 posthog-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-10 19:14:04.455840 posthog-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2207 2023-04-10 19:13:52.000000 posthog-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:14:04.451840 posthog-2.5.0/posthog/
--rw-r--r--   0 runner    (1001) docker     (122)    12456 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24749 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)    10569 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/poller.py
--rw-r--r--   0 runner    (1001) docker     (122)     3536 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/request.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:14:04.451840 posthog-2.5.0/posthog/sentry/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/sentry/django.py
--rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/sentry/posthog_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:14:04.455840 posthog-2.5.0/posthog/test/
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20666 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6325 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/test/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)   125788 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/test/test_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/test/test_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/test/test_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-04-10 19:13:52.000000 posthog-2.5.0/posthog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:14:04.451840 posthog-2.5.0/posthog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-10 19:14:04.000000 posthog-2.5.0/posthog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-10 19:14:04.000000 posthog-2.5.0/posthog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 19:14:04.000000 posthog-2.5.0/posthog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-04-10 19:14:04.000000 posthog-2.5.0/posthog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-10 19:14:04.000000 posthog-2.5.0/posthog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-04-10 19:13:52.000000 posthog-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-04-10 19:14:04.455840 posthog-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-04-10 19:13:52.000000 posthog-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:08:00.917886 posthog-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-04-17 11:07:46.000000 posthog-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-17 11:07:46.000000 posthog-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-17 11:08:00.917886 posthog-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2207 2023-04-17 11:07:46.000000 posthog-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:08:00.913886 posthog-3.0.0/posthog/
+-rw-r--r--   0 runner    (1001) docker     (122)    13467 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26356 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10569 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/poller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3536 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/request.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:08:00.913886 posthog-3.0.0/posthog/sentry/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/sentry/django.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/sentry/posthog_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:08:00.917886 posthog-3.0.0/posthog/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25975 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6325 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/test/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)   127297 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/test/test_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/test/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/test/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:08:00.913886 posthog-3.0.0/posthog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-17 11:08:00.000000 posthog-3.0.0/posthog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-17 11:08:00.000000 posthog-3.0.0/posthog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 11:08:00.000000 posthog-3.0.0/posthog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-04-17 11:08:00.000000 posthog-3.0.0/posthog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-17 11:08:00.000000 posthog-3.0.0/posthog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-04-17 11:07:46.000000 posthog-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-04-17 11:08:00.917886 posthog-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-04-17 11:07:46.000000 posthog-3.0.0/setup.py
```

### Comparing `posthog-2.5.0/LICENSE` & `posthog-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `posthog-2.5.0/PKG-INFO` & `posthog-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posthog
-Version: 2.5.0
+Version: 3.0.0
 Summary: Integrate PostHog into any python application.
 Home-page: https://github.com/posthog/posthog-python
 Author: Posthog
 Author-email: hey@posthog.com
 Maintainer: PostHog
 Maintainer-email: hey@posthog.com
 License: MIT License
```

### Comparing `posthog-2.5.0/README.md` & `posthog-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `posthog-2.5.0/posthog/__init__.py` & `posthog-3.0.0/posthog/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,27 +13,29 @@
 debug = False  # type: bool
 send = True  # type: bool
 sync_mode = False  # type: bool
 disabled = False  # type: bool
 personal_api_key = None  # type: str
 project_api_key = None  # type: str
 poll_interval = 30  # type: int
+disable_geoip = True  # type: bool
 
 default_client = None
 
 
 def capture(
     distinct_id,  # type: str
     event,  # type: str
     properties=None,  # type: Optional[Dict]
     context=None,  # type: Optional[Dict]
     timestamp=None,  # type: Optional[datetime.datetime]
     uuid=None,  # type: Optional[str]
     groups=None,  # type: Optional[Dict]
     send_feature_flags=False,
+    disable_geoip=None,  # type: Optional[bool]
 ):
     # type: (...) -> None
     """
     Capture allows you to capture anything a user does within your system, which you can later use in PostHog to find patterns in usage, work out which features to improve or where people are giving up.
 
     A `capture` call requires
     - `distinct id` which uniquely identifies your user
@@ -58,23 +60,25 @@
         event=event,
         properties=properties,
         context=context,
         timestamp=timestamp,
         uuid=uuid,
         groups=groups,
         send_feature_flags=send_feature_flags,
+        disable_geoip=disable_geoip,
     )
 
 
 def identify(
     distinct_id,  # type: str
     properties=None,  # type: Optional[Dict]
     context=None,  # type: Optional[Dict]
     timestamp=None,  # type: Optional[datetime.datetime]
     uuid=None,  # type: Optional[str]
+    disable_geoip=None,  # type: Optional[bool]
 ):
     # type: (...) -> None
     """
     Identify lets you add metadata on your users so you can more easily identify who they are in PostHog, and even do things like segment users by these properties.
 
     An `identify` call requires
     - `distinct id` which uniquely identifies your user
@@ -91,23 +95,25 @@
     _proxy(
         "identify",
         distinct_id=distinct_id,
         properties=properties,
         context=context,
         timestamp=timestamp,
         uuid=uuid,
+        disable_geoip=disable_geoip,
     )
 
 
 def set(
     distinct_id,  # type: str
     properties=None,  # type: Optional[Dict]
     context=None,  # type: Optional[Dict]
     timestamp=None,  # type: Optional[datetime.datetime]
     uuid=None,  # type: Optional[str]
+    disable_geoip=None,  # type: Optional[bool]
 ):
     # type: (...) -> None
     """
     Set properties on a user record.
     This will overwrite previous people property values, just like `identify`.
 
      A `set` call requires
@@ -124,23 +130,25 @@
     _proxy(
         "set",
         distinct_id=distinct_id,
         properties=properties,
         context=context,
         timestamp=timestamp,
         uuid=uuid,
+        disable_geoip=disable_geoip,
     )
 
 
 def set_once(
     distinct_id,  # type: str
     properties=None,  # type: Optional[Dict]
     context=None,  # type: Optional[Dict]
     timestamp=None,  # type: Optional[datetime.datetime]
     uuid=None,  # type: Optional[str]
+    disable_geoip=None,  # type: Optional[bool]
 ):
     # type: (...) -> None
     """
     Set properties on a user record, only if they do not yet exist.
     This will not overwrite previous people property values, unlike `identify`.
 
      A `set_once` call requires
@@ -157,24 +165,26 @@
     _proxy(
         "set_once",
         distinct_id=distinct_id,
         properties=properties,
         context=context,
         timestamp=timestamp,
         uuid=uuid,
+        disable_geoip=disable_geoip,
     )
 
 
 def group_identify(
     group_type,  # type: str
     group_key,  # type: str
     properties=None,  # type: Optional[Dict]
     context=None,  # type: Optional[Dict]
     timestamp=None,  # type: Optional[datetime.datetime]
     uuid=None,  # type: Optional[str]
+    disable_geoip=None,  # type: Optional[bool]
 ):
     # type: (...) -> None
     """
     Set properties on a group
 
      A `group_identify` call requires
      - `group_type` type of your group
@@ -192,23 +202,25 @@
         "group_identify",
         group_type=group_type,
         group_key=group_key,
         properties=properties,
         context=context,
         timestamp=timestamp,
         uuid=uuid,
+        disable_geoip=disable_geoip,
     )
 
 
 def alias(
     previous_id,  # type: str
     distinct_id,  # type: str
     context=None,  # type: Optional[Dict]
     timestamp=None,  # type: Optional[datetime.datetime]
     uuid=None,  # type: Optional[str]
+    disable_geoip=None,  # type: Optional[bool]
 ):
     # type: (...) -> None
     """
     To marry up whatever a user does before they sign up or log in with what they do after you need to make an alias call. This will allow you to answer questions like "Which marketing channels leads to users churning after a month?" or "What do users do on our website before signing up?"
 
     In a purely back-end implementation, this means whenever an anonymous user does something, you'll want to send a session ID ([Django](https://stackoverflow.com/questions/526179/in-django-how-can-i-find-out-the-request-session-sessionid-and-use-it-as-a-vari), [Flask](https://stackoverflow.com/questions/15156132/flask-login-how-to-get-session-id)) with the capture call. Then, when that users signs up, you want to do an alias call with the session ID and the newly created user ID.
 
@@ -226,25 +238,27 @@
     _proxy(
         "alias",
         previous_id=previous_id,
         distinct_id=distinct_id,
         context=context,
         timestamp=timestamp,
         uuid=uuid,
+        disable_geoip=disable_geoip,
     )
 
 
 def feature_enabled(
     key,  # type: str
     distinct_id,  # type: str
     groups={},  # type: dict
     person_properties={},  # type: dict
     group_properties={},  # type: dict
     only_evaluate_locally=False,  # type: bool
     send_feature_flag_events=True,  # type: bool
+    disable_geoip=None,  # type: Optional[bool]
 ):
     # type: (...) -> bool
     """
     Use feature flags to enable or disable features for users.
 
     For example:
     ```python
@@ -261,25 +275,27 @@
         key=key,
         distinct_id=distinct_id,
         groups=groups,
         person_properties=person_properties,
         group_properties=group_properties,
         only_evaluate_locally=only_evaluate_locally,
         send_feature_flag_events=send_feature_flag_events,
+        disable_geoip=disable_geoip,
     )
 
 
 def get_feature_flag(
     key,  # type: str
     distinct_id,  # type: str
     groups={},  # type: dict
     person_properties={},  # type: dict
     group_properties={},  # type: dict
     only_evaluate_locally=False,  # type: bool
     send_feature_flag_events=True,  # type: bool
+    disable_geoip=None,  # type: Optional[bool]
 ):
     """
     Get feature flag variant for users. Used with experiments.
     Example:
     ```python
     if posthog.get_feature_flag('beta-feature', 'distinct_id') == 'test-variant':
         # do test variant code
@@ -304,23 +320,25 @@
         key=key,
         distinct_id=distinct_id,
         groups=groups,
         person_properties=person_properties,
         group_properties=group_properties,
         only_evaluate_locally=only_evaluate_locally,
         send_feature_flag_events=send_feature_flag_events,
+        disable_geoip=disable_geoip,
     )
 
 
 def get_all_flags(
     distinct_id,  # type: str
     groups={},  # type: dict
     person_properties={},  # type: dict
     group_properties={},  # type: dict
     only_evaluate_locally=False,  # type: bool
+    disable_geoip=None,  # type: Optional[bool]
 ):
     """
     Get all flags for a given user.
     Example:
     ```python
     flags = posthog.get_all_flags('distinct_id')
     ```
@@ -330,54 +348,59 @@
     return _proxy(
         "get_all_flags",
         distinct_id=distinct_id,
         groups=groups,
         person_properties=person_properties,
         group_properties=group_properties,
         only_evaluate_locally=only_evaluate_locally,
+        disable_geoip=disable_geoip,
     )
 
 
 def get_feature_flag_payload(
     key,
     distinct_id,
     match_value=None,
     groups={},
     person_properties={},
     group_properties={},
     only_evaluate_locally=False,
     send_feature_flag_events=True,
+    disable_geoip=None,  # type: Optional[bool]
 ):
     return _proxy(
         "get_feature_flag_payload",
         key=key,
         distinct_id=distinct_id,
         match_value=match_value,
         groups=groups,
         person_properties=person_properties,
         group_properties=group_properties,
         only_evaluate_locally=only_evaluate_locally,
         send_feature_flag_events=send_feature_flag_events,
+        disable_geoip=disable_geoip,
     )
 
 
 def get_all_flags_and_payloads(
     distinct_id,
     groups={},
     person_properties={},
     group_properties={},
     only_evaluate_locally=False,
+    disable_geoip=None,  # type: Optional[bool]
 ):
     return _proxy(
         "get_all_flags_and_payloads",
         distinct_id=distinct_id,
         groups=groups,
         person_properties=person_properties,
         group_properties=group_properties,
         only_evaluate_locally=only_evaluate_locally,
+        disable_geoip=disable_geoip,
     )
 
 
 def page(*args, **kwargs):
     """Send a page call."""
     _proxy("page", *args, **kwargs)
 
@@ -414,14 +437,15 @@
             on_error=on_error,
             send=send,
             sync_mode=sync_mode,
             personal_api_key=personal_api_key,
             project_api_key=project_api_key,
             poll_interval=poll_interval,
             disabled=disabled,
+            disable_geoip=disable_geoip,
         )
 
     # always set incase user changes it
     default_client.disabled = disabled
     default_client.debug = debug
 
     fn = getattr(default_client, method)
```

### Comparing `posthog-2.5.0/posthog/client.py` & `posthog-3.0.0/posthog/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         sync_mode=False,
         timeout=15,
         thread=1,
         poll_interval=30,
         personal_api_key=None,
         project_api_key=None,
         disabled=False,
+        disable_geoip=True,
     ):
         self.queue = queue.Queue(max_queue_size)
 
         # api_key: This should be the Team API Key (token), public
         self.api_key = project_api_key or api_key
 
         require("api_key", self.api_key, string_types)
@@ -67,14 +68,15 @@
         self.feature_flags_by_key = None
         self.group_type_mapping = None
         self.cohorts = None
         self.poll_interval = poll_interval
         self.poller = None
         self.distinct_ids_feature_flags_reported = SizeLimitedDict(MAX_DICT_SIZE, set)
         self.disabled = disabled
+        self.disable_geoip = disable_geoip
 
         # personal_api_key: This should be a generated Personal API Key, private
         self.personal_api_key = personal_api_key
         if debug:
             # Ensures that debug level messages are logged when debug mode is on.
             # Otherwise, defaults to WARNING level. See https://docs.python.org/3/howto/logging.html#what-happens-if-no-configuration-is-provided
             logging.basicConfig()
@@ -108,58 +110,70 @@
                 )
                 self.consumers.append(consumer)
 
                 # if we've disabled sending, just don't start the consumer
                 if send:
                     consumer.start()
 
-    def identify(self, distinct_id=None, properties=None, context=None, timestamp=None, uuid=None):
+    def identify(self, distinct_id=None, properties=None, context=None, timestamp=None, uuid=None, disable_geoip=None):
         properties = properties or {}
         context = context or {}
         require("distinct_id", distinct_id, ID_TYPES)
         require("properties", properties, dict)
 
         msg = {
             "timestamp": timestamp,
             "context": context,
             "distinct_id": distinct_id,
             "$set": properties,
             "event": "$identify",
             "uuid": uuid,
         }
 
-        return self._enqueue(msg)
+        return self._enqueue(msg, disable_geoip)
 
-    def get_feature_variants(self, distinct_id, groups=None, person_properties=None, group_properties=None):
-        resp_data = self.get_decide(distinct_id, groups, person_properties, group_properties)
+    def get_feature_variants(
+        self, distinct_id, groups=None, person_properties=None, group_properties=None, disable_geoip=None
+    ):
+        resp_data = self.get_decide(distinct_id, groups, person_properties, group_properties, disable_geoip)
         return resp_data["featureFlags"]
 
-    def _get_active_feature_variants(self, distinct_id, groups=None, person_properties=None, group_properties=None):
-        feature_variants = self.get_feature_variants(distinct_id, groups, person_properties, group_properties)
+    def _get_active_feature_variants(
+        self, distinct_id, groups=None, person_properties=None, group_properties=None, disable_geoip=None
+    ):
+        feature_variants = self.get_feature_variants(
+            distinct_id, groups, person_properties, group_properties, disable_geoip
+        )
         return {
             k: v for (k, v) in feature_variants.items() if v is not False
         }  # explicitly test for false to account for values that may seem falsy (ex: 0)
 
-    def get_feature_payloads(self, distinct_id, groups=None, person_properties=None, group_properties=None):
-        resp_data = self.get_decide(distinct_id, groups, person_properties, group_properties)
+    def get_feature_payloads(
+        self, distinct_id, groups=None, person_properties=None, group_properties=None, disable_geoip=None
+    ):
+        resp_data = self.get_decide(distinct_id, groups, person_properties, group_properties, disable_geoip)
         return resp_data["featureFlagPayloads"]
 
-    def get_decide(self, distinct_id, groups=None, person_properties=None, group_properties=None):
+    def get_decide(self, distinct_id, groups=None, person_properties=None, group_properties=None, disable_geoip=None):
         require("distinct_id", distinct_id, ID_TYPES)
 
+        if disable_geoip is None:
+            disable_geoip = self.disable_geoip
+
         if groups:
             require("groups", groups, dict)
         else:
             groups = {}
 
         request_data = {
             "distinct_id": distinct_id,
             "groups": groups,
             "person_properties": person_properties,
             "group_properties": group_properties,
+            "disable_geoip": disable_geoip,
         }
         resp_data = decide(self.api_key, self.host, timeout=10, **request_data)
 
         return resp_data
 
     def capture(
         self,
@@ -167,14 +181,15 @@
         event=None,
         properties=None,
         context=None,
         timestamp=None,
         uuid=None,
         groups=None,
         send_feature_flags=False,
+        disable_geoip=None,
     ):
         properties = properties or {}
         context = context or {}
         require("distinct_id", distinct_id, ID_TYPES)
         require("properties", properties, dict)
         require("event", event, string_types)
 
@@ -189,59 +204,68 @@
 
         if groups:
             require("groups", groups, dict)
             msg["properties"]["$groups"] = groups
 
         if send_feature_flags:
             try:
-                feature_variants = self._get_active_feature_variants(distinct_id, groups)
+                feature_variants = self._get_active_feature_variants(distinct_id, groups, disable_geoip=disable_geoip)
             except Exception as e:
                 self.log.exception(f"[FEATURE FLAGS] Unable to get feature variants: {e}")
             else:
                 for feature, variant in feature_variants.items():
                     msg["properties"]["$feature/{}".format(feature)] = variant
                 msg["properties"]["$active_feature_flags"] = list(feature_variants.keys())
 
-        return self._enqueue(msg)
+        return self._enqueue(msg, disable_geoip)
 
-    def set(self, distinct_id=None, properties=None, context=None, timestamp=None, uuid=None):
+    def set(self, distinct_id=None, properties=None, context=None, timestamp=None, uuid=None, disable_geoip=None):
         properties = properties or {}
         context = context or {}
         require("distinct_id", distinct_id, ID_TYPES)
         require("properties", properties, dict)
 
         msg = {
             "timestamp": timestamp,
             "context": context,
             "distinct_id": distinct_id,
             "$set": properties,
             "event": "$set",
             "uuid": uuid,
         }
 
-        return self._enqueue(msg)
+        return self._enqueue(msg, disable_geoip)
 
-    def set_once(self, distinct_id=None, properties=None, context=None, timestamp=None, uuid=None):
+    def set_once(self, distinct_id=None, properties=None, context=None, timestamp=None, uuid=None, disable_geoip=None):
         properties = properties or {}
         context = context or {}
         require("distinct_id", distinct_id, ID_TYPES)
         require("properties", properties, dict)
 
         msg = {
             "timestamp": timestamp,
             "context": context,
             "distinct_id": distinct_id,
             "$set_once": properties,
             "event": "$set_once",
             "uuid": uuid,
         }
 
-        return self._enqueue(msg)
+        return self._enqueue(msg, disable_geoip)
 
-    def group_identify(self, group_type=None, group_key=None, properties=None, context=None, timestamp=None, uuid=None):
+    def group_identify(
+        self,
+        group_type=None,
+        group_key=None,
+        properties=None,
+        context=None,
+        timestamp=None,
+        uuid=None,
+        disable_geoip=None,
+    ):
         properties = properties or {}
         context = context or {}
         require("group_type", group_type, ID_TYPES)
         require("group_key", group_key, ID_TYPES)
         require("properties", properties, dict)
 
         msg = {
@@ -253,17 +277,17 @@
             },
             "distinct_id": "${}_{}".format(group_type, group_key),
             "timestamp": timestamp,
             "context": context,
             "uuid": uuid,
         }
 
-        return self._enqueue(msg)
+        return self._enqueue(msg, disable_geoip)
 
-    def alias(self, previous_id=None, distinct_id=None, context=None, timestamp=None, uuid=None):
+    def alias(self, previous_id=None, distinct_id=None, context=None, timestamp=None, uuid=None, disable_geoip=None):
         context = context or {}
 
         require("previous_id", previous_id, ID_TYPES)
         require("distinct_id", distinct_id, ID_TYPES)
 
         msg = {
             "properties": {
@@ -272,17 +296,19 @@
             },
             "timestamp": timestamp,
             "context": context,
             "event": "$create_alias",
             "distinct_id": previous_id,
         }
 
-        return self._enqueue(msg)
+        return self._enqueue(msg, disable_geoip)
 
-    def page(self, distinct_id=None, url=None, properties=None, context=None, timestamp=None, uuid=None):
+    def page(
+        self, distinct_id=None, url=None, properties=None, context=None, timestamp=None, uuid=None, disable_geoip=None
+    ):
         properties = properties or {}
         context = context or {}
 
         require("distinct_id", distinct_id, ID_TYPES)
         require("properties", properties, dict)
 
         require("url", url, string_types)
@@ -293,17 +319,17 @@
             "properties": properties,
             "timestamp": timestamp,
             "context": context,
             "distinct_id": distinct_id,
             "uuid": uuid,
         }
 
-        return self._enqueue(msg)
+        return self._enqueue(msg, disable_geoip)
 
-    def _enqueue(self, msg):
+    def _enqueue(self, msg, disable_geoip):
         """Push a new `msg` onto the queue, return `(success, msg)`"""
 
         if self.disabled:
             return False, "disabled"
 
         timestamp = msg["timestamp"]
         if timestamp is None:
@@ -323,14 +349,20 @@
                 msg["uuid"] = stringify_id(uuid)
 
         if not msg.get("properties"):
             msg["properties"] = {}
         msg["properties"]["$lib"] = "posthog-python"
         msg["properties"]["$lib_version"] = VERSION
 
+        if disable_geoip is None:
+            disable_geoip = self.disable_geoip
+
+        if disable_geoip:
+            msg["properties"]["$geoip_disable"] = True
+
         msg["distinct_id"] = stringify_id(msg.get("distinct_id", None))
 
         msg = clean(msg)
         self.log.debug("queueing: %s", msg)
 
         # if send is False, return msg as if it was successfully queued
         if not self.send:
@@ -466,23 +498,25 @@
         distinct_id,
         *,
         groups={},
         person_properties={},
         group_properties={},
         only_evaluate_locally=False,
         send_feature_flag_events=True,
+        disable_geoip=None,
     ):
         response = self.get_feature_flag(
             key,
             distinct_id,
             groups=groups,
             person_properties=person_properties,
             group_properties=group_properties,
             only_evaluate_locally=only_evaluate_locally,
             send_feature_flag_events=send_feature_flag_events,
+            disable_geoip=disable_geoip,
         )
 
         if response is None:
             return None
         return bool(response)
 
     def get_feature_flag(
@@ -491,14 +525,15 @@
         distinct_id,
         *,
         groups={},
         person_properties={},
         group_properties={},
         only_evaluate_locally=False,
         send_feature_flag_events=True,
+        disable_geoip=None,
     ):
         require("key", key, string_types)
         require("distinct_id", distinct_id, ID_TYPES)
         require("groups", groups, dict)
 
         if self.feature_flags is None and self.personal_api_key:
             self.load_feature_flags()
@@ -524,15 +559,19 @@
                         self.log.exception(f"[FEATURE FLAGS] Error while computing variant locally: {e}")
                         continue
 
         flag_was_locally_evaluated = response is not None
         if not flag_was_locally_evaluated and not only_evaluate_locally:
             try:
                 feature_flags = self.get_feature_variants(
-                    distinct_id, groups=groups, person_properties=person_properties, group_properties=group_properties
+                    distinct_id,
+                    groups=groups,
+                    person_properties=person_properties,
+                    group_properties=group_properties,
+                    disable_geoip=disable_geoip,
                 )
                 response = feature_flags.get(key)
                 if response is None:
                     response = False
                 self.log.debug(f"Successfully computed flag remotely: #{key} -> #{response}")
             except Exception as e:
                 self.log.exception(f"[FEATURE FLAGS] Unable to get flag remotely: {e}")
@@ -547,14 +586,15 @@
                 "$feature_flag_called",
                 {
                     "$feature_flag": key,
                     "$feature_flag_response": response,
                     "locally_evaluated": flag_was_locally_evaluated,
                 },
                 groups=groups,
+                disable_geoip=disable_geoip,
             )
             self.distinct_ids_feature_flags_reported[distinct_id].add(feature_flag_reported_key)
         return response
 
     def get_feature_flag_payload(
         self,
         key,
@@ -562,33 +602,37 @@
         *,
         match_value=None,
         groups={},
         person_properties={},
         group_properties={},
         only_evaluate_locally=False,
         send_feature_flag_events=True,
+        disable_geoip=None,
     ):
         if match_value is None:
             match_value = self.get_feature_flag(
                 key,
                 distinct_id,
                 groups=groups,
                 person_properties=person_properties,
                 group_properties=group_properties,
                 send_feature_flag_events=send_feature_flag_events,
                 only_evaluate_locally=True,
+                disable_geoip=disable_geoip,
             )
 
         response = None
 
         if match_value is not None:
             response = self._compute_payload_locally(key, match_value)
 
         if response is None and not only_evaluate_locally:
-            decide_payloads = self.get_feature_payloads(distinct_id, groups, person_properties, group_properties)
+            decide_payloads = self.get_feature_payloads(
+                distinct_id, groups, person_properties, group_properties, disable_geoip
+            )
             response = decide_payloads.get(str(key).lower(), None)
 
         return response
 
     def _compute_payload_locally(self, key, match_value):
         payload = None
 
@@ -598,37 +642,56 @@
         flag_definition = self.feature_flags_by_key.get(key) or {}
         flag_filters = flag_definition.get("filters") or {}
         flag_payloads = flag_filters.get("payloads") or {}
         payload = flag_payloads.get(str(match_value).lower(), None)
         return payload
 
     def get_all_flags(
-        self, distinct_id, *, groups={}, person_properties={}, group_properties={}, only_evaluate_locally=False
+        self,
+        distinct_id,
+        *,
+        groups={},
+        person_properties={},
+        group_properties={},
+        only_evaluate_locally=False,
+        disable_geoip=None,
     ):
         flags = self.get_all_flags_and_payloads(
             distinct_id,
             groups=groups,
             person_properties=person_properties,
             group_properties=group_properties,
             only_evaluate_locally=only_evaluate_locally,
+            disable_geoip=disable_geoip,
         )
         return flags["featureFlags"]
 
     def get_all_flags_and_payloads(
-        self, distinct_id, *, groups={}, person_properties={}, group_properties={}, only_evaluate_locally=False
+        self,
+        distinct_id,
+        *,
+        groups={},
+        person_properties={},
+        group_properties={},
+        only_evaluate_locally=False,
+        disable_geoip=None,
     ):
         flags, payloads, fallback_to_decide = self._get_all_flags_and_payloads_locally(
             distinct_id, groups=groups, person_properties=person_properties, group_properties=group_properties
         )
         response = {"featureFlags": flags, "featureFlagPayloads": payloads}
 
         if fallback_to_decide and not only_evaluate_locally:
             try:
                 flags_and_payloads = self.get_decide(
-                    distinct_id, groups=groups, person_properties=person_properties, group_properties=group_properties
+                    distinct_id,
+                    groups=groups,
+                    person_properties=person_properties,
+                    group_properties=group_properties,
+                    disable_geoip=disable_geoip,
                 )
                 response = flags_and_payloads
             except Exception as e:
                 self.log.exception(f"[FEATURE FLAGS] Unable to get feature flags and payloads: {e}")
 
         return response
```

### Comparing `posthog-2.5.0/posthog/consumer.py` & `posthog-3.0.0/posthog/consumer.py`

 * *Files identical despite different names*

### Comparing `posthog-2.5.0/posthog/feature_flags.py` & `posthog-3.0.0/posthog/feature_flags.py`

 * *Files identical despite different names*

### Comparing `posthog-2.5.0/posthog/poller.py` & `posthog-3.0.0/posthog/poller.py`

 * *Files identical despite different names*

### Comparing `posthog-2.5.0/posthog/request.py` & `posthog-3.0.0/posthog/request.py`

 * *Files identical despite different names*

### Comparing `posthog-2.5.0/posthog/sentry/django.py` & `posthog-3.0.0/posthog/sentry/django.py`

 * *Files identical despite different names*

### Comparing `posthog-2.5.0/posthog/sentry/posthog_integration.py` & `posthog-3.0.0/posthog/sentry/posthog_integration.py`

 * *Files identical despite different names*

### Comparing `posthog-2.5.0/posthog/test/test_client.py` & `posthog-3.0.0/posthog/test/test_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -108,16 +108,26 @@
     @mock.patch("posthog.client.decide")
     def test_get_active_feature_flags(self, patch_decide):
         patch_decide.return_value = {
             "featureFlags": {"beta-feature": "random-variant", "alpha-feature": True, "off-feature": False}
         }
 
         client = Client(FAKE_TEST_API_KEY, on_error=self.set_fail, personal_api_key=FAKE_TEST_API_KEY)
-        variants = client._get_active_feature_variants("some_id", None, None, None)
+        variants = client._get_active_feature_variants("some_id", None, None, None, False)
         self.assertEqual(variants, {"beta-feature": "random-variant", "alpha-feature": True})
+        patch_decide.assert_called_with(
+            "random_key",
+            None,
+            timeout=10,
+            distinct_id="some_id",
+            groups={},
+            person_properties=None,
+            group_properties=None,
+            disable_geoip=False,
+        )
 
     @mock.patch("posthog.client.decide")
     def test_basic_capture_with_feature_flags_returns_active_only(self, patch_decide):
         patch_decide.return_value = {
             "featureFlags": {"beta-feature": "random-variant", "alpha-feature": True, "off-feature": False}
         }
 
@@ -127,21 +137,69 @@
         self.assertTrue(success)
         self.assertFalse(self.failed)
 
         self.assertEqual(msg["event"], "python test event")
         self.assertTrue(isinstance(msg["timestamp"], str))
         self.assertIsNone(msg.get("uuid"))
         self.assertEqual(msg["distinct_id"], "distinct_id")
+        self.assertTrue(msg["properties"]["$geoip_disable"])
         self.assertEqual(msg["properties"]["$lib"], "posthog-python")
         self.assertEqual(msg["properties"]["$lib_version"], VERSION)
         self.assertEqual(msg["properties"]["$feature/beta-feature"], "random-variant")
         self.assertEqual(msg["properties"]["$feature/alpha-feature"], True)
         self.assertEqual(msg["properties"]["$active_feature_flags"], ["beta-feature", "alpha-feature"])
 
         self.assertEqual(patch_decide.call_count, 1)
+        patch_decide.assert_called_with(
+            "random_key",
+            None,
+            timeout=10,
+            distinct_id="distinct_id",
+            groups={},
+            person_properties=None,
+            group_properties=None,
+            disable_geoip=True,
+        )
+
+    @mock.patch("posthog.client.decide")
+    def test_basic_capture_with_feature_flags_and_disable_geoip_returns_correctly(self, patch_decide):
+        patch_decide.return_value = {
+            "featureFlags": {"beta-feature": "random-variant", "alpha-feature": True, "off-feature": False}
+        }
+
+        client = Client(
+            FAKE_TEST_API_KEY, on_error=self.set_fail, personal_api_key=FAKE_TEST_API_KEY, disable_geoip=True
+        )
+        success, msg = client.capture("distinct_id", "python test event", send_feature_flags=True, disable_geoip=False)
+        client.flush()
+        self.assertTrue(success)
+        self.assertFalse(self.failed)
+
+        self.assertEqual(msg["event"], "python test event")
+        self.assertTrue(isinstance(msg["timestamp"], str))
+        self.assertIsNone(msg.get("uuid"))
+        self.assertTrue("$geoip_disable" not in msg["properties"])
+        self.assertEqual(msg["distinct_id"], "distinct_id")
+        self.assertEqual(msg["properties"]["$lib"], "posthog-python")
+        self.assertEqual(msg["properties"]["$lib_version"], VERSION)
+        self.assertEqual(msg["properties"]["$feature/beta-feature"], "random-variant")
+        self.assertEqual(msg["properties"]["$feature/alpha-feature"], True)
+        self.assertEqual(msg["properties"]["$active_feature_flags"], ["beta-feature", "alpha-feature"])
+
+        self.assertEqual(patch_decide.call_count, 1)
+        patch_decide.assert_called_with(
+            "random_key",
+            None,
+            timeout=10,
+            distinct_id="distinct_id",
+            groups={},
+            person_properties=None,
+            group_properties=None,
+            disable_geoip=False,
+        )
 
     @mock.patch("posthog.client.decide")
     def test_basic_capture_with_feature_flags_switched_off_doesnt_send_them(self, patch_decide):
         patch_decide.return_value = {"featureFlags": {"beta-feature": "random-variant"}}
 
         client = Client(FAKE_TEST_API_KEY, on_error=self.set_fail, personal_api_key=FAKE_TEST_API_KEY)
         success, msg = client.capture("distinct_id", "python test event", send_feature_flags=False)
@@ -301,14 +359,15 @@
             msg["properties"],
             {
                 "$group_type": "organization",
                 "$group_key": "id:5",
                 "$group_set": {},
                 "$lib": "posthog-python",
                 "$lib_version": VERSION,
+                "$geoip_disable": True,
             },
         )
         self.assertTrue(isinstance(msg["timestamp"], str))
         self.assertIsNone(msg.get("uuid"))
 
     def test_advanced_group_identify(self):
         success, msg = self.client.group_identify(
@@ -322,14 +381,15 @@
             msg["properties"],
             {
                 "$group_type": "organization",
                 "$group_key": "id:5",
                 "$group_set": {"trait": "value"},
                 "$lib": "posthog-python",
                 "$lib_version": VERSION,
+                "$geoip_disable": True,
             },
         )
         self.assertEqual(msg["timestamp"], "2014-09-03T00:00:00+00:00")
         self.assertEqual(msg["context"]["ip"], "192.168.0.1")
 
     def test_basic_alias(self):
         client = self.client
@@ -490,14 +550,82 @@
         success, msg = client.capture("distinct_id", "python test event")
         client.flush()
         self.assertFalse(success)
         self.assertFalse(self.failed)
 
         self.assertEqual(msg, "disabled")
 
+    def test_disable_geoip_default_on_events(self):
+        client = Client(FAKE_TEST_API_KEY, on_error=self.set_fail, disable_geoip=True)
+        _, capture_msg = client.capture("distinct_id", "python test event")
+        client.flush()
+        self.assertEqual(capture_msg["properties"]["$geoip_disable"], True)
+
+        _, identify_msg = client.identify("distinct_id", {"trait": "value"})
+        client.flush()
+        self.assertEqual(identify_msg["properties"]["$geoip_disable"], True)
+
+    def test_disable_geoip_override_on_events(self):
+        client = Client(FAKE_TEST_API_KEY, on_error=self.set_fail, disable_geoip=False)
+        _, capture_msg = client.set("distinct_id", {"a": "b", "c": "d"}, disable_geoip=True)
+        client.flush()
+        self.assertEqual(capture_msg["properties"]["$geoip_disable"], True)
+
+        _, identify_msg = client.page("distinct_id", "http://a.com", {"trait": "value"}, disable_geoip=False)
+        client.flush()
+        self.assertEqual("$geoip_disable" not in identify_msg["properties"], True)
+
+    def test_disable_geoip_method_overrides_init_on_events(self):
+        client = Client(FAKE_TEST_API_KEY, on_error=self.set_fail, disable_geoip=True)
+        _, msg = client.capture("distinct_id", "python test event", disable_geoip=False)
+        client.flush()
+        self.assertTrue("$geoip_disable" not in msg["properties"])
+
+    @mock.patch("posthog.client.decide")
+    def test_disable_geoip_default_on_decide(self, patch_decide):
+        patch_decide.return_value = {
+            "featureFlags": {"beta-feature": "random-variant", "alpha-feature": True, "off-feature": False}
+        }
+        client = Client(FAKE_TEST_API_KEY, on_error=self.set_fail, disable_geoip=False)
+        client.get_feature_flag("random_key", "some_id", disable_geoip=True)
+        patch_decide.assert_called_with(
+            "random_key",
+            None,
+            timeout=10,
+            distinct_id="some_id",
+            groups={},
+            person_properties={},
+            group_properties={},
+            disable_geoip=True,
+        )
+        patch_decide.reset_mock()
+        client.feature_enabled("random_key", "feature_enabled_distinct_id", disable_geoip=True)
+        patch_decide.assert_called_with(
+            "random_key",
+            None,
+            timeout=10,
+            distinct_id="feature_enabled_distinct_id",
+            groups={},
+            person_properties={},
+            group_properties={},
+            disable_geoip=True,
+        )
+        patch_decide.reset_mock()
+        client.get_all_flags_and_payloads("all_flags_payloads_id")
+        patch_decide.assert_called_with(
+            "random_key",
+            None,
+            timeout=10,
+            distinct_id="all_flags_payloads_id",
+            groups={},
+            person_properties={},
+            group_properties={},
+            disable_geoip=False,
+        )
+
     @mock.patch("posthog.client.Poller")
     @mock.patch("posthog.client.get")
     def test_call_identify_fails(self, patch_get, patch_poll):
         def raise_effect():
             raise Exception("http exception")
 
         patch_get.return_value.raiseError.side_effect = raise_effect
```

### Comparing `posthog-2.5.0/posthog/test/test_consumer.py` & `posthog-3.0.0/posthog/test/test_consumer.py`

 * *Files identical despite different names*

### Comparing `posthog-2.5.0/posthog/test/test_feature_flags.py` & `posthog-3.0.0/posthog/test/test_feature_flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1886,14 +1886,15 @@
         )
         self.assertEqual(patch_capture.call_count, 1)
         patch_capture.assert_called_with(
             "some-distinct-id",
             "$feature_flag_called",
             {"$feature_flag": "complex-flag", "$feature_flag_response": True, "locally_evaluated": True},
             groups={},
+            disable_geoip=None,
         )
         patch_capture.reset_mock()
 
         # called again for same user, shouldn't call capture again
         self.assertTrue(
             client.get_feature_flag(
                 "complex-flag", "some-distinct-id", person_properties={"region": "USA", "name": "Aloha"}
@@ -1910,14 +1911,15 @@
         )
         self.assertEqual(patch_capture.call_count, 1)
         patch_capture.assert_called_with(
             "some-distinct-id2",
             "$feature_flag_called",
             {"$feature_flag": "complex-flag", "$feature_flag_response": True, "locally_evaluated": True},
             groups={},
+            disable_geoip=None,
         )
         patch_capture.reset_mock()
 
         # called for different user, but send configuration is false, so should NOT call capture again
         self.assertTrue(
             client.get_feature_flag(
                 "complex-flag",
@@ -1942,14 +1944,53 @@
         self.assertEqual(patch_decide.call_count, 1)
         self.assertEqual(patch_capture.call_count, 1)
         patch_capture.assert_called_with(
             "some-distinct-id2",
             "$feature_flag_called",
             {"$feature_flag": "decide-flag", "$feature_flag_response": "decide-value", "locally_evaluated": False},
             groups={"organization": "org1"},
+            disable_geoip=None,
+        )
+
+    @mock.patch.object(Client, "capture")
+    @mock.patch("posthog.client.decide")
+    def test_disable_geoip_get_flag_capture_call(self, patch_decide, patch_capture):
+        patch_decide.return_value = {"featureFlags": {"decide-flag": "decide-value"}}
+        client = Client(FAKE_TEST_API_KEY, personal_api_key=FAKE_TEST_API_KEY, disable_geoip=True)
+        client.feature_flags = [
+            {
+                "id": 1,
+                "name": "Beta Feature",
+                "key": "complex-flag",
+                "is_simple_flag": False,
+                "active": True,
+                "filters": {
+                    "groups": [
+                        {
+                            "properties": [{"key": "region", "value": "USA"}],
+                            "rollout_percentage": 100,
+                        }
+                    ],
+                },
+            }
+        ]
+
+        client.get_feature_flag(
+            "complex-flag",
+            "some-distinct-id",
+            person_properties={"region": "USA", "name": "Aloha"},
+            disable_geoip=False,
+        )
+
+        patch_capture.assert_called_with(
+            "some-distinct-id",
+            "$feature_flag_called",
+            {"$feature_flag": "complex-flag", "$feature_flag_response": True, "locally_evaluated": True},
+            groups={},
+            disable_geoip=False,
         )
 
     @mock.patch("posthog.client.MAX_DICT_SIZE", 100)
     @mock.patch.object(Client, "capture")
     @mock.patch("posthog.client.decide")
     def test_capture_multiple_users_doesnt_out_of_memory(self, patch_decide, patch_capture):
         client = Client(FAKE_TEST_API_KEY, personal_api_key=FAKE_TEST_API_KEY)
@@ -1975,14 +2016,15 @@
             distinct_id = f"some-distinct-id{i}"
             client.get_feature_flag("complex-flag", distinct_id, person_properties={"region": "USA", "name": "Aloha"})
             patch_capture.assert_called_with(
                 distinct_id,
                 "$feature_flag_called",
                 {"$feature_flag": "complex-flag", "$feature_flag_response": True, "locally_evaluated": True},
                 groups={},
+                disable_geoip=None,
             )
 
             self.assertEqual(len(client.distinct_ids_feature_flags_reported), i % 100 + 1)
 
 
 class TestConsistency(unittest.TestCase):
     @classmethod
```

### Comparing `posthog-2.5.0/posthog/test/test_module.py` & `posthog-3.0.0/posthog/test/test_module.py`

 * *Files identical despite different names*

### Comparing `posthog-2.5.0/posthog/test/test_request.py` & `posthog-3.0.0/posthog/test/test_request.py`

 * *Files identical despite different names*

### Comparing `posthog-2.5.0/posthog/test/test_utils.py` & `posthog-3.0.0/posthog/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `posthog-2.5.0/posthog/utils.py` & `posthog-3.0.0/posthog/utils.py`

 * *Files identical despite different names*

### Comparing `posthog-2.5.0/posthog.egg-info/PKG-INFO` & `posthog-3.0.0/posthog.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posthog
-Version: 2.5.0
+Version: 3.0.0
 Summary: Integrate PostHog into any python application.
 Home-page: https://github.com/posthog/posthog-python
 Author: Posthog
 Author-email: hey@posthog.com
 Maintainer: PostHog
 Maintainer-email: hey@posthog.com
 License: MIT License
```

### Comparing `posthog-2.5.0/posthog.egg-info/SOURCES.txt` & `posthog-3.0.0/posthog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `posthog-2.5.0/setup.py` & `posthog-3.0.0/setup.py`

 * *Files identical despite different names*

