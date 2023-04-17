# Comparing `tmp/mayalabs-0.0.7.tar.gz` & `tmp/mayalabs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayalabs-0.0.7.tar", last modified: Mon Apr 10 16:44:37 2023, max compression
+gzip compressed data, was "mayalabs-0.0.8.tar", last modified: Mon Apr 17 16:05:13 2023, max compression
```

## Comparing `mayalabs-0.0.7.tar` & `mayalabs-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-10 16:44:37.628879 mayalabs-0.0.7/
--rw-r--r--   0 shubham    (501) staff       (20)     1054 2023-03-28 13:53:19.000000 mayalabs-0.0.7/LICENCE
--rw-r--r--   0 shubham    (501) staff       (20)     4204 2023-04-10 16:44:37.628670 mayalabs-0.0.7/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)     3758 2023-04-10 16:43:43.000000 mayalabs-0.0.7/README.md
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-10 16:44:37.622902 mayalabs-0.0.7/mayalabs/
--rw-r--r--   0 shubham    (501) staff       (20)      364 2023-04-10 12:10:07.000000 mayalabs-0.0.7/mayalabs/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     4356 2023-04-10 14:24:50.000000 mayalabs-0.0.7/mayalabs/cli.py
--rw-r--r--   0 shubham    (501) staff       (20)      269 2023-03-29 17:04:56.000000 mayalabs-0.0.7/mayalabs/exceptions.py
--rw-r--r--   0 shubham    (501) staff       (20)     5947 2023-04-10 15:50:57.000000 mayalabs-0.0.7/mayalabs/function.py
--rw-r--r--   0 shubham    (501) staff       (20)     1142 2023-04-06 10:29:10.000000 mayalabs-0.0.7/mayalabs/mayalabs.py
--rw-r--r--   0 shubham    (501) staff       (20)    15585 2023-04-10 12:10:07.000000 mayalabs-0.0.7/mayalabs/session.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-10 16:44:37.627020 mayalabs-0.0.7/mayalabs/utils/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2023-03-27 23:24:06.000000 mayalabs-0.0.7/mayalabs/utils/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     1249 2023-04-10 12:10:07.000000 mayalabs-0.0.7/mayalabs/utils/defaults.py
--rw-r--r--   0 shubham    (501) staff       (20)     5196 2023-03-27 23:24:06.000000 mayalabs-0.0.7/mayalabs/utils/general.py
--rw-r--r--   0 shubham    (501) staff       (20)     1434 2023-03-29 17:05:06.000000 mayalabs-0.0.7/mayalabs/utils/log.py
--rw-r--r--   0 shubham    (501) staff       (20)      202 2023-03-29 17:04:56.000000 mayalabs-0.0.7/mayalabs/utils/logging.py
--rw-r--r--   0 shubham    (501) staff       (20)     3973 2023-03-27 23:24:06.000000 mayalabs-0.0.7/mayalabs/utils/name_gen.py
--rw-r--r--   0 shubham    (501) staff       (20)     7923 2023-04-10 12:10:07.000000 mayalabs-0.0.7/mayalabs/utils/pac_engine.py
--rw-r--r--   0 shubham    (501) staff       (20)      628 2023-03-29 10:15:45.000000 mayalabs-0.0.7/mayalabs/utils/poll.py
--rw-r--r--   0 shubham    (501) staff       (20)     5181 2023-04-10 16:17:26.000000 mayalabs-0.0.7/mayalabs/utils/websocket.py
--rw-r--r--   0 shubham    (501) staff       (20)    17204 2023-04-10 16:09:47.000000 mayalabs-0.0.7/mayalabs/worker.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-10 16:44:37.624674 mayalabs-0.0.7/mayalabs.egg-info/
--rw-r--r--   0 shubham    (501) staff       (20)     4204 2023-04-10 16:44:37.000000 mayalabs-0.0.7/mayalabs.egg-info/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)      713 2023-04-10 16:44:37.000000 mayalabs-0.0.7/mayalabs.egg-info/SOURCES.txt
--rw-r--r--   0 shubham    (501) staff       (20)        1 2023-04-10 16:44:37.000000 mayalabs-0.0.7/mayalabs.egg-info/dependency_links.txt
--rw-r--r--   0 shubham    (501) staff       (20)       46 2023-04-10 16:44:37.000000 mayalabs-0.0.7/mayalabs.egg-info/entry_points.txt
--rw-r--r--   0 shubham    (501) staff       (20)       84 2023-04-10 16:44:37.000000 mayalabs-0.0.7/mayalabs.egg-info/requires.txt
--rw-r--r--   0 shubham    (501) staff       (20)       35 2023-04-10 16:44:37.000000 mayalabs-0.0.7/mayalabs.egg-info/top_level.txt
--rw-r--r--   0 shubham    (501) staff       (20)      837 2023-04-10 16:44:13.000000 mayalabs-0.0.7/pyproject.toml
--rw-r--r--   0 shubham    (501) staff       (20)       38 2023-04-10 16:44:37.628948 mayalabs-0.0.7/setup.cfg
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-10 16:44:37.627979 mayalabs-0.0.7/tests/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2023-04-10 12:10:07.000000 mayalabs-0.0.7/tests/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)      701 2023-04-10 16:40:37.000000 mayalabs-0.0.7/tests/example_1.py
--rw-r--r--   0 shubham    (501) staff       (20)     1373 2023-04-10 12:10:07.000000 mayalabs-0.0.7/tests/example_2.py
--rw-r--r--   0 shubham    (501) staff       (20)      947 2023-04-10 12:10:07.000000 mayalabs-0.0.7/tests/example_3.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-10 16:44:37.628409 mayalabs-0.0.7/usage/
--rw-r--r--   0 shubham    (501) staff       (20)      169 2023-04-10 12:10:07.000000 mayalabs-0.0.7/usage/function.py
--rw-r--r--   0 shubham    (501) staff       (20)      414 2023-04-10 12:10:07.000000 mayalabs-0.0.7/usage/sql_test.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-17 16:05:13.921157 mayalabs-0.0.8/
+-rw-r--r--   0 shubham    (501) staff       (20)     1054 2023-03-28 13:53:19.000000 mayalabs-0.0.8/LICENCE
+-rw-r--r--   0 shubham    (501) staff       (20)     3633 2023-04-17 16:05:13.920974 mayalabs-0.0.8/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)     3187 2023-04-17 12:33:36.000000 mayalabs-0.0.8/README.md
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-17 16:05:13.912380 mayalabs-0.0.8/examples/
+-rw-r--r--   0 shubham    (501) staff       (20)      644 2023-04-13 07:38:39.000000 mayalabs-0.0.8/examples/add_to_google_sheet.py
+-rw-r--r--   0 shubham    (501) staff       (20)      665 2023-04-13 07:38:39.000000 mayalabs-0.0.8/examples/native_memory.py
+-rw-r--r--   0 shubham    (501) staff       (20)      717 2023-04-13 07:38:39.000000 mayalabs-0.0.8/examples/web_scraping.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-17 16:05:13.914455 mayalabs-0.0.8/mayalabs/
+-rw-r--r--   0 shubham    (501) staff       (20)      364 2023-04-10 12:10:07.000000 mayalabs-0.0.8/mayalabs/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     8115 2023-04-14 14:01:06.000000 mayalabs-0.0.8/mayalabs/cli.py
+-rw-r--r--   0 shubham    (501) staff       (20)      269 2023-04-17 14:31:38.000000 mayalabs-0.0.8/mayalabs/exceptions.py
+-rw-r--r--   0 shubham    (501) staff       (20)     7959 2023-04-17 14:31:46.000000 mayalabs-0.0.8/mayalabs/function.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1142 2023-04-06 10:29:10.000000 mayalabs-0.0.8/mayalabs/mayalabs.py
+-rw-r--r--   0 shubham    (501) staff       (20)    13356 2023-04-17 12:33:00.000000 mayalabs-0.0.8/mayalabs/session.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-17 16:05:13.918459 mayalabs-0.0.8/mayalabs/utils/
+-rw-r--r--   0 shubham    (501) staff       (20)        0 2023-03-27 23:24:06.000000 mayalabs-0.0.8/mayalabs/utils/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1249 2023-04-10 12:10:07.000000 mayalabs-0.0.8/mayalabs/utils/defaults.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5315 2023-04-17 14:31:58.000000 mayalabs-0.0.8/mayalabs/utils/general.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1434 2023-03-29 17:05:06.000000 mayalabs-0.0.8/mayalabs/utils/log.py
+-rw-r--r--   0 shubham    (501) staff       (20)      202 2023-03-29 17:04:56.000000 mayalabs-0.0.8/mayalabs/utils/logging.py
+-rw-r--r--   0 shubham    (501) staff       (20)     3973 2023-03-27 23:24:06.000000 mayalabs-0.0.8/mayalabs/utils/name_gen.py
+-rw-r--r--   0 shubham    (501) staff       (20)     7923 2023-04-10 12:10:07.000000 mayalabs-0.0.8/mayalabs/utils/pac_engine.py
+-rw-r--r--   0 shubham    (501) staff       (20)      628 2023-03-29 10:15:45.000000 mayalabs-0.0.8/mayalabs/utils/poll.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5181 2023-04-13 12:38:22.000000 mayalabs-0.0.8/mayalabs/utils/websocket.py
+-rw-r--r--   0 shubham    (501) staff       (20)    19095 2023-04-17 14:31:00.000000 mayalabs-0.0.8/mayalabs/worker.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-17 16:05:13.915635 mayalabs-0.0.8/mayalabs.egg-info/
+-rw-r--r--   0 shubham    (501) staff       (20)     3633 2023-04-17 16:05:13.000000 mayalabs-0.0.8/mayalabs.egg-info/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)      796 2023-04-17 16:05:13.000000 mayalabs-0.0.8/mayalabs.egg-info/SOURCES.txt
+-rw-r--r--   0 shubham    (501) staff       (20)        1 2023-04-17 16:05:13.000000 mayalabs-0.0.8/mayalabs.egg-info/dependency_links.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       46 2023-04-17 16:05:13.000000 mayalabs-0.0.8/mayalabs.egg-info/entry_points.txt
+-rw-r--r--   0 shubham    (501) staff       (20)      106 2023-04-17 16:05:13.000000 mayalabs-0.0.8/mayalabs.egg-info/requires.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       35 2023-04-17 16:05:13.000000 mayalabs-0.0.8/mayalabs.egg-info/top_level.txt
+-rw-r--r--   0 shubham    (501) staff       (20)      874 2023-04-17 16:02:31.000000 mayalabs-0.0.8/pyproject.toml
+-rw-r--r--   0 shubham    (501) staff       (20)       38 2023-04-17 16:05:13.921208 mayalabs-0.0.8/setup.cfg
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-17 16:05:13.919843 mayalabs-0.0.8/tests/
+-rw-r--r--   0 shubham    (501) staff       (20)        0 2023-04-10 12:10:07.000000 mayalabs-0.0.8/tests/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)      641 2023-04-17 16:03:07.000000 mayalabs-0.0.8/tests/example_1.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1313 2023-04-17 16:03:43.000000 mayalabs-0.0.8/tests/example_2.py
+-rw-r--r--   0 shubham    (501) staff       (20)      887 2023-04-17 16:04:03.000000 mayalabs-0.0.8/tests/example_3.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-17 16:05:13.920651 mayalabs-0.0.8/usage/
+-rw-r--r--   0 shubham    (501) staff       (20)      169 2023-04-10 12:10:07.000000 mayalabs-0.0.8/usage/function.py
+-rw-r--r--   0 shubham    (501) staff       (20)      414 2023-04-10 12:10:07.000000 mayalabs-0.0.8/usage/sql_test.py
```

### Comparing `mayalabs-0.0.7/LICENCE` & `mayalabs-0.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.7/PKG-INFO` & `mayalabs-0.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: mayalabs
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python SDK for Maya Labs' natural language programming paradigm
 Author-email: Maya Support <humans@mayalabs.io>
 Maintainer-email: Maya Support <humans@mayalabs.io>
 Project-URL: homepage, https://mayalabs.io
 Project-URL: repository, https://github.com/mayahq/mayalabs-sdk-python
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENCE
 
 # Maya Labs : Program machines using natural language.
 
 The Maya Labs Python SDK provides easy async access to our PAC-1 program synthesis engine, with a CLI to instruct and generate programs from instructions in natural language.
 
-Read more about PAC-1 on our [blog](https://mayalabs.io/pac-1).
 
 ## Installation
 
 ```
 pip install --upgrade mayalabs
 ```
 ## Preview
@@ -36,45 +35,40 @@
 ```
 
 Or set `mayalabs.api_key` to its value:
 
 ```
 import mayalabs
 
-mayalabs.api_key = "mayakey-$2a$10$Fk0gE5S8XA9D2Lyyns8Ia.cTQaZLXIELnobp1RtA.p9NxIILpBii2"
+mayalabs.api_key = "mayakey-..."
 
 script = """
 1. trigger on receive
-2. research {{topic}} on wikipedia
+2. research {{term}} on wikipedia
 3. extract 'title' and 'summary' from tabular data
-3. send response back
+4. send response back
 """
 
-function = mayalabs.Function.create(name="Scrape1", script=script)
+function = mayalabs.Function(name="Scrape2")
+# Creating new worker...
 
-function.deploy()
-# Generating program...
+function.update(script=script)
+# Generating program graph...
 # Starting worker...
 # Installing dependencies...
 # Deployed!
 
-output = function.call({"topic": "Dr. Vikram Sarabhai"})
+output = function.call({"term": "Dr. Vikram Sarabhai"})
 print(output)
 # finds and outputs title and summary from wikipedia results
 
 ```
 
 PAC-1 takes in steps written in English, writes & assembles a discrete program graph, and deploys ready-to-use software on our compute infrastructure, that you can call within your code. You can set up missing dependencies / visualize the flow of logic by following the link to flow-based editor it provides after deployment.
 
-To call the function with a different value, just initialize the function like this (remove the `.create`, but keep the same `name`) in the code above : 
-
-```
-function = mayalabs.Function(name="Scrape1", script=script)
-```
-
 ## Use Cases
 
 - [If...Then Conditionals and Looping](/EXAMPLES.md#ifthen-conditionals-and-looping)
 - [Custom Functions](/EXAMPLES.md#custom-functions)
 - [Web Scrapers](/EXAMPLES.md#web-scrapers)
 - [Repeating Workflows](/EXAMPLES.md#repeating-workflows)
 - [Custom Dashboards](/EXAMPLES.md#custom-dashboards)
@@ -92,34 +86,26 @@
 
 ```
 $ mayalabs instruct -c 'fetch Name and Email from gsheet, write function to merge all columns, and return data'
 ```
 
 And then use the generated script as function.
 
-## Development
-
-To test and develop natural language functions iteratively, just set environment variable `MAYA_ENVIRONMENT` to `development`.
-
-```
-os.environ["MAYA_ENVIRONMENT"] = "development"
-```
-
-This ensures our program synthesis engine only incremental generates and deploys changes you make to the script, instead of deploying from scratch.
+https://user-images.githubusercontent.com/52493077/231979284-a7d1c43d-f6c6-4726-89fe-28e103cd198f.mp4
 
 ## Requirements
 
 - Python 3.7.1+
 
 ## Issues
 
 All feedback and bug reports welcome! Report in the [issues section](https://github.com/mayahq/mayalabs-sdk-python/issues), or mail us at humans@mayalabs.io.
 
 Full list of capabilities and limits [here](https://docs.mayalabs.io/capabilities-and-limits).
 
 
 ## Roadmap
-- [ ] Cleaner logs and exception handling
+- [x] Cleaner logs and exception handling
 - [ ] Dependency configuration UX improvement
 - [ ] Import skill repositories for reusing skills created by user or present in store
 - [ ] Create and call downstream auto-deployed functions
 - [ ] Allow multi-profile and team profile access
```

### Comparing `mayalabs-0.0.7/README.md` & `mayalabs-0.0.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Maya Labs : Program machines using natural language.
 
 The Maya Labs Python SDK provides easy async access to our PAC-1 program synthesis engine, with a CLI to instruct and generate programs from instructions in natural language.
 
-Read more about PAC-1 on our [blog](https://mayalabs.io/pac-1).
 
 ## Installation
 
 ```
 pip install --upgrade mayalabs
 ```
 ## Preview
@@ -23,45 +22,40 @@
 ```
 
 Or set `mayalabs.api_key` to its value:
 
 ```
 import mayalabs
 
-mayalabs.api_key = "mayakey-$2a$10$Fk0gE5S8XA9D2Lyyns8Ia.cTQaZLXIELnobp1RtA.p9NxIILpBii2"
+mayalabs.api_key = "mayakey-..."
 
 script = """
 1. trigger on receive
-2. research {{topic}} on wikipedia
+2. research {{term}} on wikipedia
 3. extract 'title' and 'summary' from tabular data
-3. send response back
+4. send response back
 """
 
-function = mayalabs.Function.create(name="Scrape1", script=script)
+function = mayalabs.Function(name="Scrape2")
+# Creating new worker...
 
-function.deploy()
-# Generating program...
+function.update(script=script)
+# Generating program graph...
 # Starting worker...
 # Installing dependencies...
 # Deployed!
 
-output = function.call({"topic": "Dr. Vikram Sarabhai"})
+output = function.call({"term": "Dr. Vikram Sarabhai"})
 print(output)
 # finds and outputs title and summary from wikipedia results
 
 ```
 
 PAC-1 takes in steps written in English, writes & assembles a discrete program graph, and deploys ready-to-use software on our compute infrastructure, that you can call within your code. You can set up missing dependencies / visualize the flow of logic by following the link to flow-based editor it provides after deployment.
 
-To call the function with a different value, just initialize the function like this (remove the `.create`, but keep the same `name`) in the code above : 
-
-```
-function = mayalabs.Function(name="Scrape1", script=script)
-```
-
 ## Use Cases
 
 - [If...Then Conditionals and Looping](/EXAMPLES.md#ifthen-conditionals-and-looping)
 - [Custom Functions](/EXAMPLES.md#custom-functions)
 - [Web Scrapers](/EXAMPLES.md#web-scrapers)
 - [Repeating Workflows](/EXAMPLES.md#repeating-workflows)
 - [Custom Dashboards](/EXAMPLES.md#custom-dashboards)
@@ -79,34 +73,26 @@
 
 ```
 $ mayalabs instruct -c 'fetch Name and Email from gsheet, write function to merge all columns, and return data'
 ```
 
 And then use the generated script as function.
 
-## Development
-
-To test and develop natural language functions iteratively, just set environment variable `MAYA_ENVIRONMENT` to `development`.
-
-```
-os.environ["MAYA_ENVIRONMENT"] = "development"
-```
-
-This ensures our program synthesis engine only incremental generates and deploys changes you make to the script, instead of deploying from scratch.
+https://user-images.githubusercontent.com/52493077/231979284-a7d1c43d-f6c6-4726-89fe-28e103cd198f.mp4
 
 ## Requirements
 
 - Python 3.7.1+
 
 ## Issues
 
 All feedback and bug reports welcome! Report in the [issues section](https://github.com/mayahq/mayalabs-sdk-python/issues), or mail us at humans@mayalabs.io.
 
 Full list of capabilities and limits [here](https://docs.mayalabs.io/capabilities-and-limits).
 
 
 ## Roadmap
-- [ ] Cleaner logs and exception handling
+- [x] Cleaner logs and exception handling
 - [ ] Dependency configuration UX improvement
 - [ ] Import skill repositories for reusing skills created by user or present in store
 - [ ] Create and call downstream auto-deployed functions
 - [ ] Allow multi-profile and team profile access
```

### Comparing `mayalabs-0.0.7/mayalabs/mayalabs.py` & `mayalabs-0.0.8/mayalabs/mayalabs.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.7/mayalabs/session.py` & `mayalabs-0.0.8/mayalabs/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,15 +114,17 @@
             },
             'headers': {
                 'x-api-key': api_key,
             }
         }
         response = requests.request(**request)
         if response.status_code == 200:
-            return response.status_code
+            change_response = response.json()
+            change_status = change_response['response'].get('change_status', {}).get('is_changed', False)
+            return change_status
         else:
             raise HTTPError("Failed to update script")
 
     @authenticate
     async def deploy_session(session_id, workspace_id, api_key=None):
         data = {
             'session_id': session_id,
@@ -138,24 +140,25 @@
     def __init__(self, engine="pac-1"):
         self.id = None
         self.engine = engine
         self.script = ""
         self.worker : Worker = None
         self.steps = {}
         self.stitched_flow = []
+        self.changed = None
 
     @classmethod
     def new(cls, script=None):
-        if not isinstance(script, str):
-            error_log = [
-                "Argument must be a string.",
-                f"Received {type(script).__name__}, expected a string."]
-            raise IntegrityException(format_error_log(error_log))
+        # if not isinstance(script, str):
+        #     error_log = [
+        #         "Argument must be a string.",
+        #         f"Received {type(script).__name__}, expected a string."]
+        #     raise IntegrityException(format_error_log(error_log))
          
-        response = SessionClient.create_session(from_script=script)
+        response = SessionClient.create_session()
         session = cls()
         session.parse_obj(response['response'])
         return session
    
     @classmethod
     def get(cls, session_id=None):
         response = SessionClient.get_session(session_id=session_id)
@@ -207,15 +210,15 @@
         log(
             'Worker status:', started_status,
             prefix='mayalabs',
             prefix_color=Fore.BLACK
         )
         return
 
-    def deploy(self, worker_id=None):
+    def _deploy(self, worker_id=None, update=False):
         # Implement this method
         # print(worker_id)
         def run_asyncio_coroutine(coroutine):
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
             result = loop.run_until_complete(coroutine)
             loop.close()
@@ -234,79 +237,32 @@
         else:
             raise Exception("Error: Could not find worker")
         
         if self.worker:
             if self.worker.status != "STARTED":
                 log("Starting worker: ", self.worker.name, prefix='mayalabs')
                 self.worker.start()
-            # log(
-            #     Style.BRIGHT + Fore.CYAN + 'Generating program.' + Style.RESET_ALL,
-            #     prefix=self.worker.name,
-            #     prefix_color=self.worker.prefix_color
-            # )
-            
-            sessions = {}
-            try:
-                with open(MAYA_CACHE_FILE, "r") as f:
-                    file_content = f.read()
-                    try:
-                        sessions = json.loads(file_content)
-                    except Exception as err:
-                        print(err)
-                        sessions = None
-                    f.close()
-            except FileNotFoundError:
-                with open(MAYA_CACHE_FILE, "w+") as f:
-                    f.write("{}")
-                    f.seek(0)
-                    file_content = f.read()
-                    try:
-                        sessions = json.loads(file_content)
-                    except Exception as err:
-                        print(err)
-                        sessions = None
-                    f.close()
-            hash.update(self.script.encode())
-            received_script = hash.hexdigest()
             with concurrent.futures.ThreadPoolExecutor() as exec:
                 result_2 = exec.submit(self.check_worker_start)
-                if sessions is None or self.id not in sessions.keys() or (self.id in sessions.keys() and sessions[self.id] != received_script):
-                    if sessions is None:
-                        sessions = {}
-                        sessions[self.id] = received_script
-                        sessions_str = json.dumps(sessions)
-                        with open(MAYA_CACHE_FILE, "w") as f:
-                            f.write(sessions_str)
-                            f.close()
-                        sessions = None
-                        log(Style.BRIGHT + Fore.CYAN + 'Generating program.' + Style.RESET_ALL, prefix='mayalabs')
-                    elif self.id not in sessions.keys() or (self.id in sessions.keys() and sessions[self.id] != received_script):
-                        tmp = sessions[self.id] if self.id in sessions.keys() else ""
-                        sessions[self.id] = received_script
-                        sessions_str = json.dumps(sessions)
-                        with open(MAYA_CACHE_FILE, "w") as f:
-                            f.write(sessions_str)
-                            f.close()
-                        if tmp != "" and tmp != received_script:
-                            log(Style.BRIGHT + Fore.LIGHTYELLOW_EX + 'Found script change. Regenerating program' + Style.RESET_ALL, prefix='mayalabs')
-                            self.change()
-                        else:
-                            log(Style.BRIGHT + Fore.CYAN + 'Generating program...' + Style.RESET_ALL, prefix='mayalabs')
-                        sessions[self.id] = tmp
+                if (self.changed or self.changed is None):
+                    if self.changed:
+                        log(Style.BRIGHT + Fore.CYAN + 'Script change detected. Regenerating changes...' + Style.RESET_ALL, prefix='mayalabs')
+                    else:
+                        log(Style.BRIGHT + Fore.CYAN + 'Generating program...' + Style.RESET_ALL, prefix='mayalabs')
                     future_1 = exec.submit(run_asyncio_coroutine, self.generate_async())
                     future_1.result()
                     log(Style.BRIGHT + Fore.CYAN + 'Generation successful.' + Style.RESET_ALL, prefix='mayalabs')
                 else:
-                    log(Style.BRIGHT + Fore.LIGHTYELLOW_EX + 'No change detected in script. Skipping generation' + Style.RESET_ALL, prefix='mayalabs')
+                    log(Style.BRIGHT + Fore.CYAN + 'No change in script. Skipped regeneration' + Style.RESET_ALL, prefix='mayalabs')
                 result_2.result()
                 # report all tasks done
             
             # loop = asyncio.get_event_loop()
             async def async_wrapper():
-                if sessions is None or self.id not in sessions.keys() or (self.id in sessions.keys() and sessions[self.id] != received_script):
+                if update:
                     deploy_task = asyncio.create_task(SessionClient.deploy_session(self.id, self.worker.id))
                     log_task = asyncio.create_task(self.worker.ws_client.start_listener(events=deploy_events, log_prefix=f'{self.worker.name}'))
                     def stop_log_task(future):
                         log_task.cancel()
 
                     deploy_task.add_done_callback(stop_log_task)
                     log(
@@ -319,15 +275,15 @@
                         Style.BRIGHT + Fore.CYAN + 'Deploy successful.' + Style.RESET_ALL,
                         prefix = self.worker.name,
                         prefix_color = self.worker.prefix_color
                     )
 
                     return deploy_task.result()
                 else:
-                    log(Style.BRIGHT + Fore.LIGHTYELLOW_EX + 'No change detected in script. Skipping deploy' + Style.RESET_ALL, prefix='mayalabs')
+                    log(Style.BRIGHT + Fore.LIGHTYELLOW_EX + 'Update set to false. Skipping deploy' + Style.RESET_ALL, prefix='mayalabs')
                     return
             
             asyncio.run(async_wrapper())
 
             problems = self.worker.get_flow_problems()
             if len(problems) > 0:
                 log(
@@ -361,19 +317,21 @@
             
         else:
             raise Exception("Error: Could not find worker") 
 
     def delete(self):
         # Implement this method
         response = SessionClient.delete_session(self.id)
-        return print(response)
+        return response
     
     def change(self):
         # Implement this method
-        SessionClient.change_session(session_id=self.id, script=self.script)
+        change_response = SessionClient.change_session(session_id=self.id, script=self.script)
+        if change_response:
+            self.changed = change_response
         return
 
     def parse_obj(self, obj):
         self.id = obj['session_id']
         self.script = obj['recipe']
         self.steps = obj['steps']
         self.stitched_flow = obj['stitched_flow']
```

### Comparing `mayalabs-0.0.7/mayalabs/utils/defaults.py` & `mayalabs-0.0.8/mayalabs/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.7/mayalabs/utils/general.py` & `mayalabs-0.0.8/mayalabs/utils/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pydantic import BaseModel
 from typing import List, Optional, Dict
+from enum import Enum
 
 class StepContainer(BaseModel):
     """
     A container for the step object. 
     """
     id : Optional[str]
     type : Optional[str]
@@ -115,7 +116,12 @@
                     check = check_child_exists(child.children, id)
             return check
         if self.id == child_id:
             return True
         else:
             return check_child_exists(self.children, child_id)
 
+
+class Force(Enum):
+    normal = "normal"
+    redeploy = "redeploy"
+    regenerate = "regenerate"
```

### Comparing `mayalabs-0.0.7/mayalabs/utils/log.py` & `mayalabs-0.0.8/mayalabs/utils/log.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.7/mayalabs/utils/name_gen.py` & `mayalabs-0.0.8/mayalabs/utils/name_gen.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.7/mayalabs/utils/pac_engine.py` & `mayalabs-0.0.8/mayalabs/utils/pac_engine.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.7/mayalabs/utils/poll.py` & `mayalabs-0.0.8/mayalabs/utils/poll.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.7/mayalabs/utils/websocket.py` & `mayalabs-0.0.8/mayalabs/utils/websocket.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.7/mayalabs/worker.py` & `mayalabs-0.0.8/mayalabs/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import requests
+from requests.exceptions import SSLError
 import asyncio
 import aiohttp
 import json
 import time
 from urllib.parse import urlparse
 import traceback
 from .utils.poll import poll
@@ -31,14 +32,16 @@
         self.alias : str = None
         self.id : str = None
         self.url : str = None
         self.status : str = None
         self.session_id : str = None
         self.ws_client : WebsocketListener = None
         self.prefix_color = Fore.WHITE
+        self.locked: bool = False
+        self._reuse: bool = False
 
     def _init_from_api_response(self, response):
         self.name = response['name']
         self.alias = response['alias']
         self.id = response['_id']
         self.url = response['url']
         self.status = response['status']
@@ -73,14 +76,17 @@
 
     def delete(self):
         return WorkerClient.delete_worker(worker_id=self.id)
 
     def clear(self):
         pass
 
+    def get_health(self):
+        return WorkerClient.get_worker_health(worker_url=self.url)
+
     def update(self):
         if self.id is not None:
             response = WorkerClient.get_worker(worker_id=self.id)
             self.parse_obj(response['results'])
         else:
             raise Exception("Worker ID is not set")
         
@@ -239,14 +245,16 @@
         worker.url = obj.get('url', None)
         worker.status = obj.get('status', None)
         worker.name = obj.get('name', None)
         worker.alias = obj.get('alias', None)
         worker.session_id = obj.get('sessionId', None)
         worker_ws_url = worker.url.replace('https', 'wss') + '/comms'
         worker.ws_client = WebsocketListener(url=worker_ws_url)
+        worker.locked = obj.get('locked', False)
+        worker._reuse = obj.get('reuse', False)
         return worker
     
     @classmethod
     def new(cls, name, alias=None):
         worker = WorkerClient.create_worker(worker_name=name, alias=alias)
         return worker
     
@@ -490,7 +498,61 @@
     @authenticate
     async def get_required_fields(worker_url, api_key=None):
         msg = {}
         async with aiohttp.ClientSession(headers={ 'Authorization': f'Bearer {api_key}' }) as session:
             async with session.get(f"{worker_url}/required-fields", json=msg) as response:
                 response_json = await response.json()
                 return response_json
+
+    @staticmethod
+    def get_worker_health(worker_url):
+        # print(f"{worker_url}/health")
+        try:
+            response = requests.get(f"{worker_url}/health")
+            return response
+        except Exception as err:
+            if type(err) == SSLError:
+                response = {
+                    "status_code": 404
+                }
+                return response
+            else:
+                raise err
+    @staticmethod
+    @authenticate       
+    def lock_worker(worker_id, api_key=None):
+        api_base = default_api_base_url()
+        request = {
+                'url': f"{api_base}/app/v2/brains/{worker_id}",
+                'method': "put",
+                'headers': {
+                    'x-api-key': api_key,
+                },
+                'json': {
+                    "locked": True
+                }
+            }
+        try:
+            response = requests.request(**request)
+            return response
+        except Exception as e:
+            raise e
+        
+    @staticmethod
+    @authenticate       
+    def unlock_worker(worker_id, api_key=None):
+        api_base = default_api_base_url()
+        request = {
+                'url': f"{api_base}/app/v2/brains/{worker_id}",
+                'method': "put",
+                'headers': {
+                    'x-api-key': api_key,
+                },
+                'json': {
+                    "locked": False
+                }
+            }
+        try:
+            response = requests.request(**request)
+            return response
+        except Exception as e:
+            raise e
```

### Comparing `mayalabs-0.0.7/mayalabs.egg-info/PKG-INFO` & `mayalabs-0.0.8/mayalabs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: mayalabs
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python SDK for Maya Labs' natural language programming paradigm
 Author-email: Maya Support <humans@mayalabs.io>
 Maintainer-email: Maya Support <humans@mayalabs.io>
 Project-URL: homepage, https://mayalabs.io
 Project-URL: repository, https://github.com/mayahq/mayalabs-sdk-python
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENCE
 
 # Maya Labs : Program machines using natural language.
 
 The Maya Labs Python SDK provides easy async access to our PAC-1 program synthesis engine, with a CLI to instruct and generate programs from instructions in natural language.
 
-Read more about PAC-1 on our [blog](https://mayalabs.io/pac-1).
 
 ## Installation
 
 ```
 pip install --upgrade mayalabs
 ```
 ## Preview
@@ -36,45 +35,40 @@
 ```
 
 Or set `mayalabs.api_key` to its value:
 
 ```
 import mayalabs
 
-mayalabs.api_key = "mayakey-$2a$10$Fk0gE5S8XA9D2Lyyns8Ia.cTQaZLXIELnobp1RtA.p9NxIILpBii2"
+mayalabs.api_key = "mayakey-..."
 
 script = """
 1. trigger on receive
-2. research {{topic}} on wikipedia
+2. research {{term}} on wikipedia
 3. extract 'title' and 'summary' from tabular data
-3. send response back
+4. send response back
 """
 
-function = mayalabs.Function.create(name="Scrape1", script=script)
+function = mayalabs.Function(name="Scrape2")
+# Creating new worker...
 
-function.deploy()
-# Generating program...
+function.update(script=script)
+# Generating program graph...
 # Starting worker...
 # Installing dependencies...
 # Deployed!
 
-output = function.call({"topic": "Dr. Vikram Sarabhai"})
+output = function.call({"term": "Dr. Vikram Sarabhai"})
 print(output)
 # finds and outputs title and summary from wikipedia results
 
 ```
 
 PAC-1 takes in steps written in English, writes & assembles a discrete program graph, and deploys ready-to-use software on our compute infrastructure, that you can call within your code. You can set up missing dependencies / visualize the flow of logic by following the link to flow-based editor it provides after deployment.
 
-To call the function with a different value, just initialize the function like this (remove the `.create`, but keep the same `name`) in the code above : 
-
-```
-function = mayalabs.Function(name="Scrape1", script=script)
-```
-
 ## Use Cases
 
 - [If...Then Conditionals and Looping](/EXAMPLES.md#ifthen-conditionals-and-looping)
 - [Custom Functions](/EXAMPLES.md#custom-functions)
 - [Web Scrapers](/EXAMPLES.md#web-scrapers)
 - [Repeating Workflows](/EXAMPLES.md#repeating-workflows)
 - [Custom Dashboards](/EXAMPLES.md#custom-dashboards)
@@ -92,34 +86,26 @@
 
 ```
 $ mayalabs instruct -c 'fetch Name and Email from gsheet, write function to merge all columns, and return data'
 ```
 
 And then use the generated script as function.
 
-## Development
-
-To test and develop natural language functions iteratively, just set environment variable `MAYA_ENVIRONMENT` to `development`.
-
-```
-os.environ["MAYA_ENVIRONMENT"] = "development"
-```
-
-This ensures our program synthesis engine only incremental generates and deploys changes you make to the script, instead of deploying from scratch.
+https://user-images.githubusercontent.com/52493077/231979284-a7d1c43d-f6c6-4726-89fe-28e103cd198f.mp4
 
 ## Requirements
 
 - Python 3.7.1+
 
 ## Issues
 
 All feedback and bug reports welcome! Report in the [issues section](https://github.com/mayahq/mayalabs-sdk-python/issues), or mail us at humans@mayalabs.io.
 
 Full list of capabilities and limits [here](https://docs.mayalabs.io/capabilities-and-limits).
 
 
 ## Roadmap
-- [ ] Cleaner logs and exception handling
+- [x] Cleaner logs and exception handling
 - [ ] Dependency configuration UX improvement
 - [ ] Import skill repositories for reusing skills created by user or present in store
 - [ ] Create and call downstream auto-deployed functions
 - [ ] Allow multi-profile and team profile access
```

### Comparing `mayalabs-0.0.7/mayalabs.egg-info/SOURCES.txt` & `mayalabs-0.0.8/mayalabs.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 LICENCE
 README.md
 pyproject.toml
+examples/add_to_google_sheet.py
+examples/native_memory.py
+examples/web_scraping.py
 mayalabs/__init__.py
 mayalabs/cli.py
 mayalabs/exceptions.py
 mayalabs/function.py
 mayalabs/mayalabs.py
 mayalabs/session.py
 mayalabs/worker.py
```

### Comparing `mayalabs-0.0.7/pyproject.toml` & `mayalabs-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [project]
 name = "mayalabs"
-version = "0.0.7"
+version = "0.0.8"
 description = "Python SDK for Maya Labs' natural language programming paradigm"
 dependencies = [
     "requests",
     "pydantic",
     "websockets",
     "click",
     "colorama",
+    "halo",
+    "simple-term-menu",
     "aiohttp>=3.6,<4.0"
 ]
 requires-python = ">=3.6"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 authors=[
  {name="Maya Support", email="humans@mayalabs.io"}
@@ -34,8 +36,8 @@
 [project.urls]
 homepage = "https://mayalabs.io"
 repository = "https://github.com/mayahq/mayalabs-sdk-python"
 
 [project.optional-dependencies]
 test=[
   "pytest==7.2.1"
-]
+]
```

### Comparing `mayalabs-0.0.7/tests/example_1.py` & `mayalabs-0.0.8/tests/example_1.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,13 +12,12 @@
 5. if {{payload.num}} is less than 36
     - 5.1. go to step 3
 6. else if {{payload.num}} is more than 36
     - 6.1. print {{payload.num}}
 7. respond back with {{payload}}
     """
 def test_if_condition_with_loop():
-    os.environ['MAYA_ENVIRONMENT'] = "development"
-    func = mayalabs.Function.create(name='UniqueNewFunc01', script=script)
-    func.deploy()
+    func = mayalabs.Function(name='UniqueNewFunc01')
+    func.update(script=script)
     output = func.call(payload={"trigger": "this"})
     print(output)
     assert True if output['num'] == 36 else False
```

### Comparing `mayalabs-0.0.7/tests/example_2.py` & `mayalabs-0.0.8/tests/example_2.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
 script = """
 1. trigger on recieve
 3. run a custom function to 'to take a deeply nested JSON object {{payload.data}} and flatten it then return'
 4. send response back
 """
 def test_custom_function_generate():
-    os.environ['MAYA_ENVIRONMENT'] = "development"
 
-    func = mayalabs.Function.create(name='UniqueNewFunc02', script=script)
-    func.deploy()
+    func = mayalabs.Function(name='UniqueNewFunc02')
+    func.update(script=script)
     output = func.call(payload={"data": example_object})
     expected_return = ['id: 1', 'name: Alice', 'position: CEO', 'subordinates.0.id: 2', 'subordinates.0.name: Bob', 'subordinates.0.position: CTO', 'subordinates.0.subordinates.0.id: 4', 'subordinates.0.subordinates.0.name: David', 'subordinates.0.subordinates.0.position: Lead Developer', 'subordinates.1.id: 3', 'subordinates.1.name: Carol', 'subordinates.1.position: CFO']
     assert True if output == expected_return else False
```

### Comparing `mayalabs-0.0.7/tests/example_3.py` & `mayalabs-0.0.8/tests/example_3.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 4. type {{query}} in field with xpath //*[@aria-label="Search"]
 5. click button with xpath (//input[@aria-label="Google Search"])[2]
 6. wait for 10 seconds
 7. scrape '//h3[contains(text(), "Description")]/../span/text()' as 'description'
 8. send response back
     """
 def test_web_scrape_type_click():
-    os.environ['MAYA_ENVIRONMENT'] = "development"
-    func = mayalabs.Function.create(name='UniqueNewFunc03', script=script)
-    func.deploy()
+    func = mayalabs.Function(name='UniqueNewFunc03')
+    func.update(script=script)
     output = fn.call(payload={
             'url': 'wss://chrome.browserless.io?token=' + os.environ.get('BROWSERLESS_TOKEN', ''),
             'query': 'lionel messi'
         })
     try:
         assert True if len(output['scrapResults'].get('description')) > 0 else False
     except:
```

