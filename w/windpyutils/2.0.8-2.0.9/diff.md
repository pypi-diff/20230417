# Comparing `tmp/windpyutils-2.0.8.tar.gz` & `tmp/windpyutils-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/minerva1/nlp-2/homes/idocekal/windPyUtils/dist/tmpu15sh6l9/windpyutils-2.0.8.tar", last modified: Mon Jun 27 13:20:48 2022, max compression
+gzip compressed data, was "windpyutils-2.0.9.tar", last modified: Thu Jun 30 14:53:11 2022, max compression
```

## Comparing `windpyutils-2.0.8.tar` & `windpyutils-2.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwx---   0 idocekal (35695) proj06     (435)        0 2022-06-27 13:20:48.000000 windpyutils-2.0.8/
--rw-rw----   0 idocekal (35695) proj06     (435)     1211 2022-05-31 11:17:31.000000 windpyutils-2.0.8/LICENSE
--rw-rw----   0 idocekal (35695) proj06     (435)      353 2022-06-27 13:20:48.000000 windpyutils-2.0.8/PKG-INFO
--rw-rw----   0 idocekal (35695) proj06     (435)       41 2022-05-31 11:17:31.000000 windpyutils-2.0.8/README.md
--rw-rw----   0 idocekal (35695) proj06     (435)       38 2022-06-27 13:20:48.000000 windpyutils-2.0.8/setup.cfg
--rw-rw----   0 idocekal (35695) proj06     (435)      736 2022-06-27 13:20:14.000000 windpyutils-2.0.8/setup.py
-drwxrwx---   0 idocekal (35695) proj06     (435)        0 2022-06-27 13:20:48.000000 windpyutils-2.0.8/windpyutils/
--rw-rw----   0 idocekal (35695) proj06     (435)       83 2022-05-31 11:17:31.000000 windpyutils-2.0.8/windpyutils/__init__.py
--rw-rw----   0 idocekal (35695) proj06     (435)      493 2022-05-31 11:17:31.000000 windpyutils-2.0.8/windpyutils/args.py
--rw-rw----   0 idocekal (35695) proj06     (435)     5713 2022-05-31 11:17:31.000000 windpyutils-2.0.8/windpyutils/buffers.py
--rw-rw----   0 idocekal (35695) proj06     (435)     1982 2022-05-31 11:17:31.000000 windpyutils-2.0.8/windpyutils/config.py
--rw-rw----   0 idocekal (35695) proj06     (435)     3695 2022-05-31 11:17:31.000000 windpyutils-2.0.8/windpyutils/design_patterns.py
--rw-rw----   0 idocekal (35695) proj06     (435)    24440 2022-06-27 13:14:11.000000 windpyutils-2.0.8/windpyutils/files.py
--rw-rw----   0 idocekal (35695) proj06     (435)     7566 2022-06-27 11:17:24.000000 windpyutils-2.0.8/windpyutils/generic.py
--rw-rw----   0 idocekal (35695) proj06     (435)      752 2022-05-31 11:17:31.000000 windpyutils-2.0.8/windpyutils/logger.py
--rw-rw----   0 idocekal (35695) proj06     (435)     1006 2022-05-31 11:17:31.000000 windpyutils-2.0.8/windpyutils/metrics.py
--rw-rw----   0 idocekal (35695) proj06     (435)     3028 2022-05-31 11:17:31.000000 windpyutils-2.0.8/windpyutils/mocking.py
-drwxrwx---   0 idocekal (35695) proj06     (435)        0 2022-06-27 13:20:48.000000 windpyutils-2.0.8/windpyutils/parallel/
--rw-rw----   0 idocekal (35695) proj06     (435)       83 2022-05-31 11:17:31.000000 windpyutils-2.0.8/windpyutils/parallel/__init__.py
--rw-rw----   0 idocekal (35695) proj06     (435)     1615 2022-05-31 11:17:31.000000 windpyutils-2.0.8/windpyutils/parallel/maps.py
--rw-rw----   0 idocekal (35695) proj06     (435)     4949 2022-05-31 11:17:31.000000 windpyutils-2.0.8/windpyutils/parallel/own_proc_pools.py
--rw-rw----   0 idocekal (35695) proj06     (435)     3915 2022-05-31 11:17:31.000000 windpyutils-2.0.8/windpyutils/parallel/pools.py
--rw-rw----   0 idocekal (35695) proj06     (435)     2488 2022-05-31 11:17:31.000000 windpyutils-2.0.8/windpyutils/parallel/workers.py
-drwxrwx---   0 idocekal (35695) proj06     (435)        0 2022-06-27 13:20:48.000000 windpyutils-2.0.8/windpyutils/structures/
--rw-rw----   0 idocekal (35695) proj06     (435)       83 2022-05-31 11:17:31.000000 windpyutils-2.0.8/windpyutils/structures/__init__.py
--rw-rw----   0 idocekal (35695) proj06     (435)     2079 2022-05-31 11:17:31.000000 windpyutils-2.0.8/windpyutils/structures/circular_buffer.py
--rw-rw----   0 idocekal (35695) proj06     (435)     1261 2022-05-31 11:17:32.000000 windpyutils-2.0.8/windpyutils/structures/data_classes.py
--rw-rw----   0 idocekal (35695) proj06     (435)     3530 2022-05-31 11:17:32.000000 windpyutils-2.0.8/windpyutils/structures/maps.py
--rw-rw----   0 idocekal (35695) proj06     (435)    14149 2022-05-31 11:17:32.000000 windpyutils-2.0.8/windpyutils/structures/span_set.py
-drwxrwx---   0 idocekal (35695) proj06     (435)        0 2022-06-27 13:20:48.000000 windpyutils-2.0.8/windpyutils/visual/
--rw-rw----   0 idocekal (35695) proj06     (435)       83 2022-05-31 11:17:32.000000 windpyutils-2.0.8/windpyutils/visual/__init__.py
--rw-rw----   0 idocekal (35695) proj06     (435)     7600 2022-05-31 11:17:32.000000 windpyutils-2.0.8/windpyutils/visual/text.py
-drwxrwx---   0 idocekal (35695) proj06     (435)        0 2022-06-27 13:20:48.000000 windpyutils-2.0.8/windpyutils.egg-info/
--rw-rw----   0 idocekal (35695) proj06     (435)      353 2022-06-27 13:20:47.000000 windpyutils-2.0.8/windpyutils.egg-info/PKG-INFO
--rw-rw----   0 idocekal (35695) proj06     (435)      801 2022-06-27 13:20:47.000000 windpyutils-2.0.8/windpyutils.egg-info/SOURCES.txt
--rw-rw----   0 idocekal (35695) proj06     (435)        1 2022-06-27 13:20:47.000000 windpyutils-2.0.8/windpyutils.egg-info/dependency_links.txt
--rw-rw----   0 idocekal (35695) proj06     (435)       12 2022-06-27 13:20:47.000000 windpyutils-2.0.8/windpyutils.egg-info/top_level.txt
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2022-06-30 14:53:11.505962 windpyutils-2.0.9/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1211 2020-04-08 13:35:58.000000 windpyutils-2.0.9/LICENSE
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      353 2022-06-30 14:53:11.505962 windpyutils-2.0.9/PKG-INFO
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       41 2020-04-08 13:37:13.000000 windpyutils-2.0.9/README.md
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       38 2022-06-30 14:53:11.505962 windpyutils-2.0.9/setup.cfg
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      736 2022-06-30 14:52:30.000000 windpyutils-2.0.9/setup.py
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2022-06-30 14:53:11.505962 windpyutils-2.0.9/windpyutils/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       83 2020-04-08 13:35:58.000000 windpyutils-2.0.9/windpyutils/__init__.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      493 2020-08-26 11:10:16.000000 windpyutils-2.0.9/windpyutils/args.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     5713 2022-06-16 18:18:06.000000 windpyutils-2.0.9/windpyutils/buffers.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1982 2021-04-15 10:19:16.000000 windpyutils-2.0.9/windpyutils/config.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3695 2021-04-06 08:19:25.000000 windpyutils-2.0.9/windpyutils/design_patterns.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)    24467 2022-06-30 14:52:05.000000 windpyutils-2.0.9/windpyutils/files.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     7566 2022-06-13 13:18:19.000000 windpyutils-2.0.9/windpyutils/generic.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      752 2021-03-02 12:31:15.000000 windpyutils-2.0.9/windpyutils/logger.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1006 2021-01-28 08:31:28.000000 windpyutils-2.0.9/windpyutils/metrics.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3028 2021-01-28 08:31:28.000000 windpyutils-2.0.9/windpyutils/mocking.py
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2022-06-30 14:53:11.505962 windpyutils-2.0.9/windpyutils/parallel/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       83 2020-09-23 13:11:41.000000 windpyutils-2.0.9/windpyutils/parallel/__init__.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1615 2021-12-04 05:25:16.000000 windpyutils-2.0.9/windpyutils/parallel/maps.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     4949 2022-06-23 11:48:43.000000 windpyutils-2.0.9/windpyutils/parallel/own_proc_pools.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3915 2021-12-05 12:20:53.000000 windpyutils-2.0.9/windpyutils/parallel/pools.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2488 2021-12-04 05:09:40.000000 windpyutils-2.0.9/windpyutils/parallel/workers.py
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2022-06-30 14:53:11.505962 windpyutils-2.0.9/windpyutils/structures/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       83 2020-04-08 13:35:58.000000 windpyutils-2.0.9/windpyutils/structures/__init__.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2079 2021-01-28 08:18:57.000000 windpyutils-2.0.9/windpyutils/structures/circular_buffer.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1261 2021-01-28 08:19:42.000000 windpyutils-2.0.9/windpyutils/structures/data_classes.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3530 2021-01-28 08:23:10.000000 windpyutils-2.0.9/windpyutils/structures/maps.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)    14149 2021-01-28 08:24:17.000000 windpyutils-2.0.9/windpyutils/structures/span_set.py
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2022-06-30 14:53:11.505962 windpyutils-2.0.9/windpyutils/visual/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       83 2021-02-05 08:18:17.000000 windpyutils-2.0.9/windpyutils/visual/__init__.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     7600 2022-05-26 13:14:45.000000 windpyutils-2.0.9/windpyutils/visual/text.py
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2022-06-30 14:53:11.505962 windpyutils-2.0.9/windpyutils.egg-info/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      353 2022-06-30 14:53:11.000000 windpyutils-2.0.9/windpyutils.egg-info/PKG-INFO
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      801 2022-06-30 14:53:11.000000 windpyutils-2.0.9/windpyutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)        1 2022-06-30 14:53:11.000000 windpyutils-2.0.9/windpyutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       12 2022-06-30 14:53:11.000000 windpyutils-2.0.9/windpyutils.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `windpyutils-2.0.8/LICENSE` & `windpyutils-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/setup.py` & `windpyutils-2.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='windpyutils',
-    version='2.0.8',
+    version='2.0.9',
     description='Useful tools for Python projects.',
     long_description_content_type="text/markdown",
     long_description=README,
     license='The Unlicense',
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     author='Martin Dočekal',
     keywords=['utils', 'general usage'],
```

### Comparing `windpyutils-2.0.8/windpyutils/buffers.py` & `windpyutils-2.0.9/windpyutils/buffers.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils/config.py` & `windpyutils-2.0.9/windpyutils/config.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils/design_patterns.py` & `windpyutils-2.0.9/windpyutils/design_patterns.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils/files.py` & `windpyutils-2.0.9/windpyutils/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,14 +275,15 @@
             self._opened_in_process_with_id = os.getpid()
         return self
 
     def close(self):
         if self.file is not None:
             self.mm.close()
             self.file.close()
+            self.mm = None
             self.file = None
             self._opened_in_process_with_id = None
 
     def _file_seek(self, offset: int):
         self._reopen_if_needed()
         self.mm.seek(offset)
```

### Comparing `windpyutils-2.0.8/windpyutils/generic.py` & `windpyutils-2.0.9/windpyutils/generic.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils/logger.py` & `windpyutils-2.0.9/windpyutils/logger.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils/metrics.py` & `windpyutils-2.0.9/windpyutils/metrics.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils/mocking.py` & `windpyutils-2.0.9/windpyutils/mocking.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils/parallel/maps.py` & `windpyutils-2.0.9/windpyutils/parallel/maps.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils/parallel/own_proc_pools.py` & `windpyutils-2.0.9/windpyutils/parallel/own_proc_pools.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils/parallel/pools.py` & `windpyutils-2.0.9/windpyutils/parallel/pools.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils/parallel/workers.py` & `windpyutils-2.0.9/windpyutils/parallel/workers.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils/structures/circular_buffer.py` & `windpyutils-2.0.9/windpyutils/structures/circular_buffer.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils/structures/data_classes.py` & `windpyutils-2.0.9/windpyutils/structures/data_classes.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils/structures/maps.py` & `windpyutils-2.0.9/windpyutils/structures/maps.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils/structures/span_set.py` & `windpyutils-2.0.9/windpyutils/structures/span_set.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils/visual/text.py` & `windpyutils-2.0.9/windpyutils/visual/text.py`

 * *Files identical despite different names*

### Comparing `windpyutils-2.0.8/windpyutils.egg-info/SOURCES.txt` & `windpyutils-2.0.9/windpyutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

