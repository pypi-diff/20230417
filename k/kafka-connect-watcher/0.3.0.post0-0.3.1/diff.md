# Comparing `tmp/kafka_connect_watcher-0.3.0.post0.tar.gz` & `tmp/kafka_connect_watcher-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka_connect_watcher-0.3.0.post0.tar", max compression
+gzip compressed data, was "kafka_connect_watcher-0.3.1.tar", max compression
```

## Comparing `kafka_connect_watcher-0.3.0.post0.tar` & `kafka_connect_watcher-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      944 2023-02-28 14:05:27.479088 kafka_connect_watcher-0.3.0.post0/README.rst
--rw-r--r--   0        0        0      195 2023-03-22 22:05:51.891302 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/__init__.py
--rw-r--r--   0        0        0     4038 2023-03-15 14:40:57.739243 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/aws_emf.py
--rw-r--r--   0        0        0     6192 2023-03-22 21:01:49.774003 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/aws_sns/__init__.py
--rw-r--r--   0        0        0      107 2023-03-20 14:52:32.551851 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/aws_sns/default.j2
--rw-r--r--   0        0        0      140 2023-03-20 14:10:44.078719 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/aws_sns/email.j2
--rw-r--r--   0        0        0       80 2023-03-20 14:45:41.271914 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/aws_sns/sms.j2
--rw-r--r--   0        0        0      616 2023-02-28 16:04:00.414003 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/cli.py
--rw-r--r--   0        0        0     3466 2023-03-20 15:50:03.131477 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/cluster.py
--rw-r--r--   0        0        0     5075 2023-03-22 20:06:47.639263 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/config.py
--rw-r--r--   0        0        0     2571 2023-03-22 21:01:49.767003 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/connectors_eval.py
--rw-r--r--   0        0        0     8064 2023-03-22 20:17:29.774964 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/error_rules.py
--rw-r--r--   0        0        0     1204 2022-08-08 20:12:17.351935 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/logger.py
--rw-r--r--   0        0        0      918 2023-03-22 21:01:49.737002 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/notifications.py
--rw-r--r--   0        0        0      254 2023-01-23 17:30:58.219507 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/threads_settings.py
--rw-r--r--   0        0        0      492 2023-01-23 08:58:32.729607 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/tools.py
--rw-r--r--   0        0        0     8149 2023-03-22 21:20:00.602403 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/watcher-config.spec.json
--rw-r--r--   0        0        0     4550 2023-03-22 21:01:49.755003 kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/watcher.py
--rw-r--r--   0        0        0     2501 2023-03-22 22:05:51.891302 kafka_connect_watcher-0.3.0.post0/pyproject.toml
--rw-r--r--   0        0        0     2169 1970-01-01 00:00:00.000000 kafka_connect_watcher-0.3.0.post0/setup.py
--rw-r--r--   0        0        0     2486 1970-01-01 00:00:00.000000 kafka_connect_watcher-0.3.0.post0/PKG-INFO
+-rw-r--r--   0        0        0      944 2023-02-28 14:05:27.479088 kafka_connect_watcher-0.3.1/README.rst
+-rw-r--r--   0        0        0      189 2023-04-17 15:35:02.457313 kafka_connect_watcher-0.3.1/kafka_connect_watcher/__init__.py
+-rw-r--r--   0        0        0     4038 2023-03-15 14:40:57.739243 kafka_connect_watcher-0.3.1/kafka_connect_watcher/aws_emf.py
+-rw-r--r--   0        0        0     5383 2023-04-17 15:31:09.335440 kafka_connect_watcher-0.3.1/kafka_connect_watcher/aws_sns/__init__.py
+-rw-r--r--   0        0        0      107 2023-03-20 14:52:32.551851 kafka_connect_watcher-0.3.1/kafka_connect_watcher/aws_sns/default.j2
+-rw-r--r--   0        0        0      140 2023-03-20 14:10:44.078719 kafka_connect_watcher-0.3.1/kafka_connect_watcher/aws_sns/email.j2
+-rw-r--r--   0        0        0       80 2023-03-20 14:45:41.271914 kafka_connect_watcher-0.3.1/kafka_connect_watcher/aws_sns/sms.j2
+-rw-r--r--   0        0        0      616 2023-02-28 16:04:00.414003 kafka_connect_watcher-0.3.1/kafka_connect_watcher/cli.py
+-rw-r--r--   0        0        0     3466 2023-03-20 15:50:03.131477 kafka_connect_watcher-0.3.1/kafka_connect_watcher/cluster.py
+-rw-r--r--   0        0        0     5075 2023-03-22 20:06:47.639263 kafka_connect_watcher-0.3.1/kafka_connect_watcher/config.py
+-rw-r--r--   0        0        0     2571 2023-03-22 21:01:49.767003 kafka_connect_watcher-0.3.1/kafka_connect_watcher/connectors_eval.py
+-rw-r--r--   0        0        0     8064 2023-03-22 20:17:29.774964 kafka_connect_watcher-0.3.1/kafka_connect_watcher/error_rules.py
+-rw-r--r--   0        0        0     1928 2023-04-17 15:32:30.604442 kafka_connect_watcher-0.3.1/kafka_connect_watcher/logger.py
+-rw-r--r--   0        0        0      918 2023-03-22 21:01:49.737002 kafka_connect_watcher-0.3.1/kafka_connect_watcher/notifications.py
+-rw-r--r--   0        0        0      254 2023-01-23 17:30:58.219507 kafka_connect_watcher-0.3.1/kafka_connect_watcher/threads_settings.py
+-rw-r--r--   0        0        0      492 2023-01-23 08:58:32.729607 kafka_connect_watcher-0.3.1/kafka_connect_watcher/tools.py
+-rw-r--r--   0        0        0     8149 2023-03-23 13:26:18.128320 kafka_connect_watcher-0.3.1/kafka_connect_watcher/watcher-config.spec.json
+-rw-r--r--   0        0        0     4674 2023-04-17 15:24:05.452215 kafka_connect_watcher-0.3.1/kafka_connect_watcher/watcher.py
+-rw-r--r--   0        0        0     2489 2023-04-17 15:35:02.457313 kafka_connect_watcher-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2163 1970-01-01 00:00:00.000000 kafka_connect_watcher-0.3.1/setup.py
+-rw-r--r--   0        0        0     2480 1970-01-01 00:00:00.000000 kafka_connect_watcher-0.3.1/PKG-INFO
```

### Comparing `kafka_connect_watcher-0.3.0.post0/README.rst` & `kafka_connect_watcher-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/aws_emf.py` & `kafka_connect_watcher-0.3.1/kafka_connect_watcher/aws_emf.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/aws_sns/__init__.py` & `kafka_connect_watcher-0.3.1/kafka_connect_watcher/aws_sns/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,17 +41,14 @@
             "email": pkg_files("kafka_connect_watcher").joinpath("aws_sns/email.j2"),
             "sms": pkg_files("kafka_connect_watcher").joinpath("aws_sns/sms.j2"),
         }
         self.ignore_errors = keyisset("ignore_errors", self.definition)
         self._messages_templates: dict = {}
         self.import_jinja2_templates()
 
-        self._session = Session()
-        self._session_expiry = None
-
     def __repr__(self):
         return f"sns.{self.name}"
 
     def import_jinja2_templates(self) -> None:
         if keyisset("template", self.definition):
             self._templates_definitions.update(self.definition["template"])
         for message_type, template_path in self._templates_definitions.items():
@@ -135,35 +132,19 @@
                 )
                 if not self.ignore_errors:
                     raise
         self.publish(subject, messages)
 
     @property
     def session(self) -> Session:
-        """
-        Sets the boto3 session up
-        If role_arn is set, we assume_role to get the session, and keep track of expiry. If at execution the expiry
-        passed, re-assume to a new session and get new credentials.
-        Otherwise, use the default Session() set at __init__
-        """
         if keyisset("role_arn", self.definition):
-            if (
-                self._session
-                and self._session_expiry
-                and (dt.now()) < self._session_expiry
-            ):
-                return self._session
-            else:
-                self._session, details = get_assume_role_session(
-                    Session(),
-                    self.definition["role_arn"],
-                    set_else_none(
-                        "role_session_name",
-                        self.definition,
-                        f"KafkaConnectWatcher{self.name}",
-                    ),
-                    include_full_return=True,
-                    DurationSeconds=3600,
+            return get_assume_role_session(
+                Session(),
+                self.definition["role_arn"],
+                set_else_none(
+                    "role_session_name",
+                    self.definition,
+                    f"KafkaConnectWatcher{self.name}",
                 )
-                self._session_expiry = details["Credentials"]["Expiration"]
+            )
         else:
-            return self._session
+            return Session()
```

### Comparing `kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/cli.py` & `kafka_connect_watcher-0.3.1/kafka_connect_watcher/cli.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/cluster.py` & `kafka_connect_watcher-0.3.1/kafka_connect_watcher/cluster.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/config.py` & `kafka_connect_watcher-0.3.1/kafka_connect_watcher/config.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/connectors_eval.py` & `kafka_connect_watcher-0.3.1/kafka_connect_watcher/connectors_eval.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/error_rules.py` & `kafka_connect_watcher-0.3.1/kafka_connect_watcher/error_rules.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/notifications.py` & `kafka_connect_watcher-0.3.1/kafka_connect_watcher/notifications.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/watcher-config.spec.json` & `kafka_connect_watcher-0.3.1/kafka_connect_watcher/watcher-config.spec.json`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.0.post0/kafka_connect_watcher/watcher.py` & `kafka_connect_watcher-0.3.1/kafka_connect_watcher/watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,18 @@
                 LOG.info(
                     "Clusters processing finished - {}s".format(
                         (dt.now() - now).total_seconds()
                     )
                 )
                 if config.emf_watcher_config:
                     handle_watcher_emf(config, self)
-                sleep(config.scan_intervals)
+                for _second in range(1, config.scan_intervals):
+                    sleep(1)
+                    if not self.keep_running:
+                        break
                 self.metrics.update(
                     {"connect_clusters_healthy": 0, "connect_clusters_unhealthy": 0}
                 )
                 LOG.debug("Watcher metrics: {}".format(self.metrics))
         except KeyboardInterrupt:
             self.keep_running = False
             LOG.debug("\rExited due to Keyboard interrupt")
```

### Comparing `kafka_connect_watcher-0.3.0.post0/pyproject.toml` & `kafka_connect_watcher-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kafka-connect-watcher"
-version = "0.3.0.post0"
+version = "0.3.1"
 description = "Kafka Connect active watcher"
 authors = ["John \"Preston\" Mille <john@ews-network.net>"]
 readme = "README.rst"
 license = "MPL-2.0"
 keywords = ["kafka", "connect", "monitoring", "observability"]
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -83,15 +83,15 @@
   "*/cli.py"
 ]
 
 [tool.tbump]
 github_url = "https://github.com/johnpreston/kafka-connect-watcher"
 
 [tool.tbump.version]
-current = "0.3.0.post0"
+current = "0.3.1"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `kafka_connect_watcher-0.3.0.post0/setup.py` & `kafka_connect_watcher-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 {'console_scripts': ['kafka-connect-watcher = '
                      'kafka_connect_watcher.cli:start_watcher',
                      'kafka_connect_watcher = '
                      'kafka_connect_watcher.cli:start_watcher']}
 
 setup_kwargs = {
     'name': 'kafka-connect-watcher',
-    'version': '0.3.0.post0',
+    'version': '0.3.1',
     'description': 'Kafka Connect active watcher',
     'long_description': '\n===========================================\nKafka Connect Watcher\n===========================================\n\nService that will actively probe and monitor your Kafka connect clusters using the Connect API.\nIt can report metrics to AWS CloudWatch (Prometheus coming) using `AWS EMF`_ to allow creating alerts\nand alarms.\n\nFeatures\n=========\n\n* Scan multiple clusters at once\n* Implement different remediation rules\n* Include/Exclude lists for connectors to evaluate/ignore\n\nRoadmap\n=========\n\n* Prometheus support\n* Multiple channels of alerts (i.e. webhooks)\n\n\nSystems recommendations\n------------------------------\n\nWhen using multiple clusters, we recommend to provide multiple CPUs to the service as it\nhas multi-threading enabled, allowing for parallel processing of clusters & their respective connectors.\n\n\n.. _AWS EMF: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Embedded_Metric_Format_Specification.html\n',
     'author': 'John "Preston" Mille',
     'author_email': 'john@ews-network.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kafka_connect_watcher-0.3.0.post0/PKG-INFO` & `kafka_connect_watcher-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-connect-watcher
-Version: 0.3.0.post0
+Version: 0.3.1
 Summary: Kafka Connect active watcher
 License: MPL-2.0
 Keywords: kafka,connect,monitoring,observability
 Author: John "Preston" Mille
 Author-email: john@ews-network.net
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

