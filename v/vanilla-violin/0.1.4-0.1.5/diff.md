# Comparing `tmp/vanilla_violin-0.1.4.tar.gz` & `tmp/vanilla_violin-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanilla_violin-0.1.4.tar", last modified: Thu Apr 13 13:44:08 2023, max compression
+gzip compressed data, was "vanilla_violin-0.1.5.tar", last modified: Mon Apr 17 14:53:52 2023, max compression
```

## Comparing `vanilla_violin-0.1.4.tar` & `vanilla_violin-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:44:08.503652 vanilla_violin-0.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      380 2023-04-13 13:44:08.503652 vanilla_violin-0.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 13:44:08.503652 vanilla_violin-0.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:44:08.498652 vanilla_violin-0.1.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/tests/test_gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:44:08.498652 vanilla_violin-0.1.4/vanilla_violin/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/vanilla_violin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:44:08.502652 vanilla_violin-0.1.4/vanilla_violin/aws/
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/vanilla_violin/aws/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4734 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/vanilla_violin/aws/aws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:44:08.502652 vanilla_violin-0.1.4/vanilla_violin/gitlab/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/vanilla_violin/gitlab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9944 2023-04-13 13:43:42.000000 vanilla_violin-0.1.4/vanilla_violin/gitlab/gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:44:08.501652 vanilla_violin-0.1.4/vanilla_violin.egg-info/
--rw-r--r--   0 root         (0) root         (0)      380 2023-04-13 13:44:08.000000 vanilla_violin-0.1.4/vanilla_violin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-13 13:44:08.000000 vanilla_violin-0.1.4/vanilla_violin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 13:44:08.000000 vanilla_violin-0.1.4/vanilla_violin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-13 13:44:08.000000 vanilla_violin-0.1.4/vanilla_violin.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-13 13:44:08.000000 vanilla_violin-0.1.4/vanilla_violin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-13 13:44:08.000000 vanilla_violin-0.1.4/vanilla_violin.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:53:52.816419 vanilla_violin-0.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-04-17 14:53:26.000000 vanilla_violin-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      380 2023-04-17 14:53:52.815419 vanilla_violin-0.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-04-17 14:53:26.000000 vanilla_violin-0.1.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 14:53:52.816419 vanilla_violin-0.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-17 14:53:26.000000 vanilla_violin-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:53:52.811418 vanilla_violin-0.1.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-04-17 14:53:26.000000 vanilla_violin-0.1.5/tests/test_gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:53:52.811418 vanilla_violin-0.1.5/vanilla_violin/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-17 14:53:26.000000 vanilla_violin-0.1.5/vanilla_violin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:53:52.814418 vanilla_violin-0.1.5/vanilla_violin/aws/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-17 14:53:26.000000 vanilla_violin-0.1.5/vanilla_violin/aws/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4734 2023-04-17 14:53:26.000000 vanilla_violin-0.1.5/vanilla_violin/aws/aws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:53:52.815419 vanilla_violin-0.1.5/vanilla_violin/gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-17 14:53:26.000000 vanilla_violin-0.1.5/vanilla_violin/gitlab/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11571 2023-04-17 14:53:26.000000 vanilla_violin-0.1.5/vanilla_violin/gitlab/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:53:52.813418 vanilla_violin-0.1.5/vanilla_violin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      380 2023-04-17 14:53:52.000000 vanilla_violin-0.1.5/vanilla_violin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-17 14:53:52.000000 vanilla_violin-0.1.5/vanilla_violin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 14:53:52.000000 vanilla_violin-0.1.5/vanilla_violin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-17 14:53:52.000000 vanilla_violin-0.1.5/vanilla_violin.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-17 14:53:52.000000 vanilla_violin-0.1.5/vanilla_violin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-17 14:53:52.000000 vanilla_violin-0.1.5/vanilla_violin.egg-info/top_level.txt
```

### Comparing `vanilla_violin-0.1.4/LICENSE` & `vanilla_violin-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vanilla_violin-0.1.4/tests/test_gitlab.py` & `vanilla_violin-0.1.5/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `vanilla_violin-0.1.4/vanilla_violin/aws/aws.py` & `vanilla_violin-0.1.5/vanilla_violin/aws/aws.py`

 * *Files identical despite different names*

### Comparing `vanilla_violin-0.1.4/vanilla_violin/gitlab/gitlab.py` & `vanilla_violin-0.1.5/vanilla_violin/gitlab/gitlab.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,25 +166,88 @@
       headers=self.request_headers
     )
     return {
       'text': json.loads(response.text),
       'status_code': response.status_code
     }
 
+  def get_pipelines(self, project_id):
+    
+    response = requests.get(
+      f'{self.base_url}{self.api_url}projects/{project_id}/pipelines',
+      headers=self.request_headers
+    )
+    return {
+      'text': json.loads(response.text),
+      'status_code': response.status_code
+    }
+
+  def get_latest_pipeline_id(self, project_id, ref='main'):
+    
+    response = self.get_pipelines(project_id)['text']
+
+    for pipe in response:
+      if pipe['ref'] == ref:
+        return pipe['id']
+
+    return None
+
+  def get_pipeline_jobs(self, project_id, pipeline_id):
+
+    response = requests.get(
+      f'{self.base_url}{self.api_url}projects/{project_id}/pipelines/{pipeline_id}/jobs',
+      headers=self.request_headers
+    )
+    return {
+      'text': json.loads(response.text),
+      'status_code': response.status_code
+    }
+
+  def get_job_id(self, project_id, pipeline_id, job_name):
+
+    response = self.get_pipeline_jobs(project_id, pipeline_id)['text']
+
+    for job in response:
+      if job['name'] == job_name:
+        return job['id']
+
+    return None
+    
+
+  def run_job(self, project_id, job_id):
+    
+    response = requests.post(
+      f'{self.base_url}{self.api_url}projects/{project_id}/jobs/{job_id}/play',
+      headers=self.request_headers,
+    )
+    return {
+      'text': json.loads(response.text),
+      'status_code': response.status_code
+    }
+
   def trigger_pipeline(self, project_id, ref='main'):
 
     response = requests.post(
       f'{self.base_url}{self.api_url}projects/{project_id}/pipeline?ref={ref}',
       headers=self.request_headers,
     )
     return {
       'text': json.loads(response.text),
       'status_code': response.status_code
     }
 
+  def run_pipeline_job(self, url, job_name):
+
+    proj_id = self.get_project_id(url)
+    pipe_id = self.get_latest_pipeline_id(proj_id)
+    job_id = self.get_job_id(proj_id, pipe_id, job_name)
+    response = self.run_job(proj_id, job_id)
+
+    return response
+
   def create_pages_domain_if_available(self, project_id, domain, auto_ssl_enabled = True):
 
     print('--- BUILDING PAGES ---')
     pages_create = self.create_pages_domain(project_id, domain, auto_ssl_enabled)
 
     if pages_create['status_code'] == 404:
       print(f"--- {pages_create['text']['message']}")
```

