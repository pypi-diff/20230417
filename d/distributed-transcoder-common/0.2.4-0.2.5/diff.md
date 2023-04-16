# Comparing `tmp/distributed-transcoder-common-0.2.4.tar.gz` & `tmp/distributed-transcoder-common-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distributed-transcoder-common-0.2.4.tar", max compression
+gzip compressed data, was "distributed-transcoder-common-0.2.5.tar", max compression
```

## Comparing `distributed-transcoder-common-0.2.4.tar` & `distributed-transcoder-common-0.2.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       86 2023-04-04 05:32:08.748355 distributed-transcoder-common-0.2.4/distributed_transcoder_common/__init__.py
--rw-r--r--   0        0        0      416 2023-04-04 05:06:21.155583 distributed-transcoder-common-0.2.4/distributed_transcoder_common/message_types.py
--rw-r--r--   0        0        0     1907 2023-04-16 03:00:08.313542 distributed-transcoder-common-0.2.4/distributed_transcoder_common/models.py
--rw-r--r--   0        0        0      390 2023-04-16 03:00:55.472977 distributed-transcoder-common-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      695 2023-04-16 03:00:59.864056 distributed-transcoder-common-0.2.4/setup.py
--rw-r--r--   0        0        0      422 2023-04-16 03:00:59.864263 distributed-transcoder-common-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-04-04 05:32:08.748355 distributed-transcoder-common-0.2.5/distributed_transcoder_common/__init__.py
+-rw-r--r--   0        0        0      416 2023-04-04 05:06:21.155583 distributed-transcoder-common-0.2.5/distributed_transcoder_common/message_types.py
+-rw-r--r--   0        0        0     1909 2023-04-16 03:05:30.465666 distributed-transcoder-common-0.2.5/distributed_transcoder_common/models.py
+-rw-r--r--   0        0        0      390 2023-04-16 03:05:51.801176 distributed-transcoder-common-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      695 2023-04-16 03:05:56.123516 distributed-transcoder-common-0.2.5/setup.py
+-rw-r--r--   0        0        0      422 2023-04-16 03:05:56.123715 distributed-transcoder-common-0.2.5/PKG-INFO
```

### Comparing `distributed-transcoder-common-0.2.4/distributed_transcoder_common/models.py` & `distributed-transcoder-common-0.2.5/distributed_transcoder_common/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     class PydanticMeta:
         exclude = ("jobs",)
 
 
 class Job(Model):
     STATE_QUEUED = "queued"
     STATE_IN_PROGRESS = "in-progress"
-    STATE_FINISHED = "finished"
+    STATE_COMPLETED = "completed"
     STATE_FAILED = "failed"
     STATE_CANCELLED = "cancelled"
 
     id = fields.UUIDField(pk=True)
     job_id = fields.CharField(max_length=50, unique=True)
     input_s3_path = fields.CharField(max_length=255)
     output_s3_path = fields.CharField(max_length=255)
```

### Comparing `distributed-transcoder-common-0.2.4/setup.py` & `distributed-transcoder-common-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['tortoise-orm>=0.19.3,<0.20.0']
 
 setup_kwargs = {
     'name': 'distributed-transcoder-common',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'A common library for for the distributed transcoder project',
     'long_description': None,
     'author': 'Eric Volpert',
     'author_email': 'ericvolp12@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

