# Comparing `tmp/commonX-0.3.9.tar.gz` & `tmp/commonX-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\commonX-0.3.9.tar", last modified: Thu Apr  6 14:14:39 2023, max compression
+gzip compressed data, was "dist\commonX-0.4.0.tar", last modified: Mon Apr 17 10:48:06 2023, max compression
```

## Comparing `commonX-0.3.9.tar` & `commonX-0.4.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 14:14:39.000000 commonX-0.3.9/
--rw-rw-rw-   0        0        0      714 2023-04-06 14:14:39.000000 commonX-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0       77 2023-04-06 14:13:41.000000 commonX-0.3.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 14:14:39.000000 commonX-0.3.9/common/
--rw-rw-rw-   0        0        0       86 2023-04-06 14:13:41.000000 commonX-0.3.9/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:14:39.000000 commonX-0.3.9/common/base/
--rw-rw-rw-   0        0        0      622 2023-04-06 14:13:41.000000 commonX-0.3.9/common/base/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-04-06 14:13:41.000000 commonX-0.3.9/common/base/entity.py
--rw-rw-rw-   0        0        0      359 2023-04-06 14:13:41.000000 commonX-0.3.9/common/base/factory.py
--rw-rw-rw-   0        0        0     2927 2023-04-06 14:13:41.000000 commonX-0.3.9/common/base/genor.py
--rw-rw-rw-   0        0        0     2916 2023-04-06 14:13:41.000000 commonX-0.3.9/common/base/hook.py
--rw-rw-rw-   0        0        0     4135 2023-04-06 14:13:41.000000 commonX-0.3.9/common/base/logger.py
--rw-rw-rw-   0        0        0     5710 2023-04-06 14:13:41.000000 commonX-0.3.9/common/base/mapper.py
--rw-rw-rw-   0        0        0     8399 2023-04-06 14:13:41.000000 commonX-0.3.9/common/base/multi_task.py
--rw-rw-rw-   0        0        0     5182 2023-04-06 14:13:41.000000 commonX-0.3.9/common/base/packer.py
--rw-rw-rw-   0        0        0     1968 2023-04-06 14:13:41.000000 commonX-0.3.9/common/base/registry.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:14:39.000000 commonX-0.3.9/common/ext/
--rw-rw-rw-   0        0        0      187 2023-04-06 14:13:41.000000 commonX-0.3.9/common/ext/__init__.py
--rw-rw-rw-   0        0        0     2174 2023-04-06 14:13:41.000000 commonX-0.3.9/common/ext/cookie_parser.py
--rw-rw-rw-   0        0        0     3845 2023-04-06 14:13:41.000000 commonX-0.3.9/common/ext/iphone_client.py
--rw-rw-rw-   0        0        0      220 2023-04-06 14:13:41.000000 commonX-0.3.9/common/ext/ocr_support.py
--rw-rw-rw-   0        0        0     1862 2023-04-06 14:13:41.000000 commonX-0.3.9/common/ext/qq_email.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:14:39.000000 commonX-0.3.9/common/postman/
--rw-rw-rw-   0        0        0       87 2023-04-06 14:13:41.000000 commonX-0.3.9/common/postman/__init__.py
--rw-rw-rw-   0        0        0     4861 2023-04-06 14:13:41.000000 commonX-0.3.9/common/postman/postman_api.py
--rw-rw-rw-   0        0        0     3316 2023-04-06 14:13:41.000000 commonX-0.3.9/common/postman/postman_impl.py
--rw-rw-rw-   0        0        0     3308 2023-04-06 14:13:41.000000 commonX-0.3.9/common/postman/postman_proxy.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:14:39.000000 commonX-0.3.9/common/util/
--rw-rw-rw-   0        0        0      246 2023-04-06 14:13:41.000000 commonX-0.3.9/common/util/__init__.py
--rw-rw-rw-   0        0        0      791 2023-04-06 14:13:41.000000 commonX-0.3.9/common/util/args_util.py
--rw-rw-rw-   0        0        0     2176 2023-04-06 14:13:41.000000 commonX-0.3.9/common/util/assert_util.py
--rw-rw-rw-   0        0        0     3273 2023-04-06 14:13:41.000000 commonX-0.3.9/common/util/decorator_util.py
--rw-rw-rw-   0        0        0     4855 2023-04-06 14:13:41.000000 commonX-0.3.9/common/util/file_util.py
--rw-rw-rw-   0        0        0     2765 2023-04-06 14:13:41.000000 commonX-0.3.9/common/util/json_util.py
--rw-rw-rw-   0        0        0     6494 2023-04-06 14:13:41.000000 commonX-0.3.9/common/util/requests_util.py
--rw-rw-rw-   0        0        0     4426 2023-04-06 14:13:41.000000 commonX-0.3.9/common/util/sys_util.py
--rw-rw-rw-   0        0        0      898 2023-04-06 14:13:41.000000 commonX-0.3.9/common/util/time_util.py
--rw-rw-rw-   0        0        0      715 2023-04-06 14:13:41.000000 commonX-0.3.9/common/util/typing_util.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:14:39.000000 commonX-0.3.9/commonX.egg-info/
--rw-rw-rw-   0        0        0      714 2023-04-06 14:14:39.000000 commonX-0.3.9/commonX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      896 2023-04-06 14:14:39.000000 commonX-0.3.9/commonX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 14:14:39.000000 commonX-0.3.9/commonX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-06 14:14:39.000000 commonX-0.3.9/commonX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 14:14:39.000000 commonX-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1089 2023-04-06 14:13:41.000000 commonX-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:48:06.000000 commonX-0.4.0/
+-rw-rw-rw-   0        0        0      714 2023-04-17 10:48:06.000000 commonX-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       77 2023-04-11 16:54:05.000000 commonX-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 10:48:06.000000 commonX-0.4.0/common/
+-rw-rw-rw-   0        0        0       86 2023-04-11 16:54:05.000000 commonX-0.4.0/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:48:06.000000 commonX-0.4.0/common/base/
+-rw-rw-rw-   0        0        0      622 2023-04-11 16:54:05.000000 commonX-0.4.0/common/base/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-04-11 16:54:05.000000 commonX-0.4.0/common/base/entity.py
+-rw-rw-rw-   0        0        0      359 2023-04-11 16:54:05.000000 commonX-0.4.0/common/base/factory.py
+-rw-rw-rw-   0        0        0     2927 2023-04-11 16:54:05.000000 commonX-0.4.0/common/base/genor.py
+-rw-rw-rw-   0        0        0     2916 2023-04-11 16:54:05.000000 commonX-0.4.0/common/base/hook.py
+-rw-rw-rw-   0        0        0     4135 2023-04-11 16:54:05.000000 commonX-0.4.0/common/base/logger.py
+-rw-rw-rw-   0        0        0     5710 2023-04-11 16:54:05.000000 commonX-0.4.0/common/base/mapper.py
+-rw-rw-rw-   0        0        0     8399 2023-04-11 16:54:05.000000 commonX-0.4.0/common/base/multi_task.py
+-rw-rw-rw-   0        0        0     5182 2023-04-11 16:54:05.000000 commonX-0.4.0/common/base/packer.py
+-rw-rw-rw-   0        0        0     1968 2023-04-11 16:54:05.000000 commonX-0.4.0/common/base/registry.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:48:06.000000 commonX-0.4.0/common/ext/
+-rw-rw-rw-   0        0        0      187 2023-04-11 16:54:05.000000 commonX-0.4.0/common/ext/__init__.py
+-rw-rw-rw-   0        0        0     2174 2023-04-11 16:54:05.000000 commonX-0.4.0/common/ext/cookie_parser.py
+-rw-rw-rw-   0        0        0     3845 2023-04-11 16:54:05.000000 commonX-0.4.0/common/ext/iphone_client.py
+-rw-rw-rw-   0        0        0      220 2023-04-11 16:54:05.000000 commonX-0.4.0/common/ext/ocr_support.py
+-rw-rw-rw-   0        0        0     1862 2023-04-11 16:54:05.000000 commonX-0.4.0/common/ext/qq_email.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:48:06.000000 commonX-0.4.0/common/postman/
+-rw-rw-rw-   0        0        0       87 2023-04-11 16:54:05.000000 commonX-0.4.0/common/postman/__init__.py
+-rw-rw-rw-   0        0        0     5086 2023-04-11 16:54:05.000000 commonX-0.4.0/common/postman/postman_api.py
+-rw-rw-rw-   0        0        0     3316 2023-04-11 16:54:05.000000 commonX-0.4.0/common/postman/postman_impl.py
+-rw-rw-rw-   0        0        0     3865 2023-04-11 16:54:05.000000 commonX-0.4.0/common/postman/postman_proxy.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:48:06.000000 commonX-0.4.0/common/util/
+-rw-rw-rw-   0        0        0      246 2023-04-11 16:54:05.000000 commonX-0.4.0/common/util/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-04-11 16:54:05.000000 commonX-0.4.0/common/util/args_util.py
+-rw-rw-rw-   0        0        0     2176 2023-04-11 16:54:05.000000 commonX-0.4.0/common/util/assert_util.py
+-rw-rw-rw-   0        0        0     3273 2023-04-11 16:54:05.000000 commonX-0.4.0/common/util/decorator_util.py
+-rw-rw-rw-   0        0        0     4855 2023-04-11 16:54:05.000000 commonX-0.4.0/common/util/file_util.py
+-rw-rw-rw-   0        0        0     2765 2023-04-11 16:54:05.000000 commonX-0.4.0/common/util/json_util.py
+-rw-rw-rw-   0        0        0     6494 2023-04-11 16:54:05.000000 commonX-0.4.0/common/util/requests_util.py
+-rw-rw-rw-   0        0        0     4616 2023-04-11 16:54:05.000000 commonX-0.4.0/common/util/sys_util.py
+-rw-rw-rw-   0        0        0      898 2023-04-11 16:54:05.000000 commonX-0.4.0/common/util/time_util.py
+-rw-rw-rw-   0        0        0      715 2023-04-11 16:54:05.000000 commonX-0.4.0/common/util/typing_util.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:48:06.000000 commonX-0.4.0/commonX.egg-info/
+-rw-rw-rw-   0        0        0      714 2023-04-17 10:48:06.000000 commonX-0.4.0/commonX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      896 2023-04-17 10:48:06.000000 commonX-0.4.0/commonX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 10:48:06.000000 commonX-0.4.0/commonX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 10:48:06.000000 commonX-0.4.0/commonX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 10:48:06.000000 commonX-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1089 2023-04-11 16:54:05.000000 commonX-0.4.0/setup.py
```

### Comparing `commonX-0.3.9/PKG-INFO` & `commonX-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.3.9
+Version: 0.4.0
 Summary: python common toolkit
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `commonX-0.3.9/common/base/__init__.py` & `commonX-0.4.0/common/base/__init__.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/base/entity.py` & `commonX-0.4.0/common/base/entity.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/base/genor.py` & `commonX-0.4.0/common/base/genor.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/base/hook.py` & `commonX-0.4.0/common/base/hook.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/base/logger.py` & `commonX-0.4.0/common/base/logger.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/base/mapper.py` & `commonX-0.4.0/common/base/mapper.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/base/multi_task.py` & `commonX-0.4.0/common/base/multi_task.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/base/packer.py` & `commonX-0.4.0/common/base/packer.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/base/registry.py` & `commonX-0.4.0/common/base/registry.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/ext/cookie_parser.py` & `commonX-0.4.0/common/ext/cookie_parser.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/ext/iphone_client.py` & `commonX-0.4.0/common/ext/iphone_client.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/ext/qq_email.py` & `commonX-0.4.0/common/ext/qq_email.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/postman/postman_api.py` & `commonX-0.4.0/common/postman/postman_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,22 @@
     def create(cls, clazz=None, **kwargs):
         if clazz is None:
             from .postman_impl import RequestsPostman
             clazz = RequestsPostman
 
         return clazz(kwargs)
 
+    def get_root_postman(self):
+        from .postman_proxy import PostmanProxy
+        if isinstance(self, PostmanProxy):
+            return self.postman.get_root_postman()
+        return self
+
+    # proxy method
+
     def with_fix_url(self, url: str):
         from .postman_proxy import FixUrlPostman
         return FixUrlPostman(self, url)
 
     def with_retry(self, retry_times, clazz=None):
         if clazz is None:
             from .postman_proxy import RetryPostman
@@ -88,19 +96,20 @@
         from .postman_proxy import MultiPartPostman
         return MultiPartPostman(self)
 
     def with_wrap_resp(self, clazz=None):
         from .postman_proxy import WrapRespPostman
         return WrapRespPostman(self, clazz)
 
-    def get_root_postman(self):
-        from .postman_proxy import PostmanProxy
-        if isinstance(self, PostmanProxy):
-            return self.postman.get_root_postman()
-        return self
+    def with_redirect_catching(self, clazz=None):
+        if clazz is None:
+            from .postman_proxy import RedirectPostman
+            clazz = RedirectPostman
+
+        return clazz(self)
 
 
 class AbstractPostman(Postman):
 
     @classmethod
     def create(cls, **kwargs):
         return cls(kwargs)
```

### Comparing `commonX-0.3.9/common/postman/postman_impl.py` & `commonX-0.4.0/common/postman/postman_impl.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/postman/postman_proxy.py` & `commonX-0.4.0/common/postman/postman_proxy.py`

 * *Files 21% similar despite different names*

```diff
@@ -100,7 +100,25 @@
         self.WrapResp = wrap_resp_class
 
     def get(self, *args, **kwargs):
         return self.WrapResp(super().get(*args, **kwargs))
 
     def post(self, *args, **kwargs):
         return self.WrapResp(super().post(*args, **kwargs))
+
+
+# noinspection PyMethodMayBeStatic
+class RedirectPostman(PostmanProxy):
+
+    def request(self, args, kwargs, method):
+        kwargs.setdefault("allow_redirects", False)
+        resp = method(*args, **kwargs)
+        return self.get_redirect_url_from_resp(resp)
+
+    def get_redirect_url_from_resp(self, resp):
+        return resp.headers['Location']
+
+    def get(self, *args, **kwargs):
+        return self.request(args, kwargs, super().get)
+
+    def post(self, *args, **kwargs):
+        return self.request(args, kwargs, super().post)
```

### Comparing `commonX-0.3.9/common/util/args_util.py` & `commonX-0.4.0/common/util/args_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/util/assert_util.py` & `commonX-0.4.0/common/util/assert_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/util/decorator_util.py` & `commonX-0.4.0/common/util/decorator_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/util/file_util.py` & `commonX-0.4.0/common/util/file_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/util/json_util.py` & `commonX-0.4.0/common/util/json_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/util/requests_util.py` & `commonX-0.4.0/common/util/requests_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/util/sys_util.py` & `commonX-0.4.0/common/util/sys_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -162,16 +162,27 @@
 
 
 def traceback_print_exec():
     import traceback
     traceback.print_exc()
 
 
+def str_to_line_iter(lines: str):
+    for line in lines.strip().splitlines():
+        line = line.strip()
+        if line != '':
+            yield line
+
+
 def str_to_list(lines: str):
-    return [line.strip() for line in lines.strip().split('\n') if line.strip() != '']
+    return list(str_to_line_iter(lines))
+
+
+def str_to_set(lines: str):
+    return set(str_to_line_iter(lines))
 
 
 def show_bytecodes():
     from dis import dis
     try:
         dis(paste_from_clip())
     except:
```

### Comparing `commonX-0.3.9/common/util/time_util.py` & `commonX-0.4.0/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/common/util/typing_util.py` & `commonX-0.4.0/common/util/typing_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/commonX.egg-info/PKG-INFO` & `commonX-0.4.0/commonX.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.3.9
+Version: 0.4.0
 Summary: python common toolkit
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `commonX-0.3.9/commonX.egg-info/SOURCES.txt` & `commonX-0.4.0/commonX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commonX-0.3.9/setup.py` & `commonX-0.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
-VERSION = '0.3.9'
+VERSION = '0.4.0'
 DESCRIPTION = 'python common toolkit'
 
 setup(
     name='commonX',
     version=VERSION,
     description=DESCRIPTION,
     author='hect0x7',
```

