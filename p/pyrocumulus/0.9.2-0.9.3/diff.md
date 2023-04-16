# Comparing `tmp/pyrocumulus-0.9.2.tar.gz` & `tmp/pyrocumulus-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrocumulus-0.9.2.tar", last modified: Fri Dec 29 23:10:01 2017, max compression
+gzip compressed data, was "dist/pyrocumulus-0.9.3.tar", last modified: Wed Apr 25 05:28:06 2018, max compression
```

## Comparing `pyrocumulus-0.9.2.tar` & `pyrocumulus-0.9.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2017-12-29 23:10:01.000000 pyrocumulus-0.9.2/
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2017-12-29 23:10:01.000000 pyrocumulus-0.9.2/pyrocumulus/
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2017-12-29 23:10:01.000000 pyrocumulus-0.9.2/pyrocumulus/commands/
--rw-r--r--   0 juca      (1000) juca      (1000)     6322 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/commands/base.py
--rw-r--r--   0 juca      (1000) juca      (1000)     7297 2017-12-29 21:26:44.000000 pyrocumulus-0.9.2/pyrocumulus/commands/runtornado.py
--rw-r--r--   0 juca      (1000) juca      (1000)      915 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/commands/test.py
--rw-r--r--   0 juca      (1000) juca      (1000)       23 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/commands/__init__.py
--rw-r--r--   0 juca      (1000) juca      (1000)     4443 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/commands/authcli.py
--rw-r--r--   0 juca      (1000) juca      (1000)     3914 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/commands/createproject.py
--rw-r--r--   0 juca      (1000) juca      (1000)    10538 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/converters.py
--rw-r--r--   0 juca      (1000) juca      (1000)     3545 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/auth.py
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2017-12-29 23:10:01.000000 pyrocumulus-0.9.2/pyrocumulus/web/
--rw-r--r--   0 juca      (1000) juca      (1000)     3886 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/web/mixins.py
--rw-r--r--   0 juca      (1000) juca      (1000)    22203 2017-12-29 22:16:43.000000 pyrocumulus-0.9.2/pyrocumulus/web/handlers.py
--rw-r--r--   0 juca      (1000) juca      (1000)     2143 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/web/decorators.py
--rw-r--r--   0 juca      (1000) juca      (1000)     2000 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/web/metaclasses.py
--rw-r--r--   0 juca      (1000) juca      (1000)     4720 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/web/operationmappers.py
--rw-r--r--   0 juca      (1000) juca      (1000)       24 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/web/__init__.py
--rw-r--r--   0 juca      (1000) juca      (1000)     3955 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/web/applications.py
--rw-r--r--   0 juca      (1000) juca      (1000)     3656 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/web/template.py
--rw-r--r--   0 juca      (1000) juca      (1000)      708 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/web/request_handlers.py
--rw-r--r--   0 juca      (1000) juca      (1000)     5453 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/web/urlmappers.py
--rw-r--r--   0 juca      (1000) juca      (1000)     2016 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/testing.py
--rw-r--r--   0 juca      (1000) juca      (1000)     5282 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/parsers.py
--rw-r--r--   0 juca      (1000) juca      (1000)     1859 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/conf.py
--rw-r--r--   0 juca      (1000) juca      (1000)     1594 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/utils.py
--rw-r--r--   0 juca      (1000) juca      (1000)      770 2017-12-29 23:09:26.000000 pyrocumulus-0.9.2/pyrocumulus/__init__.py
--rw-r--r--   0 juca      (1000) juca      (1000)     1546 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/db.py
--rw-r--r--   0 juca      (1000) juca      (1000)     1211 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/pyrocumulus/exceptions.py
--rw-r--r--   0 juca      (1000) juca      (1000)     2368 2017-11-16 21:33:32.000000 pyrocumulus-0.9.2/setup.py
--rw-r--r--   0 juca      (1000) juca      (1000)      387 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/README
--rw-r--r--   0 juca      (1000) juca      (1000)     1483 2017-12-29 23:10:01.000000 pyrocumulus-0.9.2/PKG-INFO
--rw-r--r--   0 juca      (1000) juca      (1000)       38 2017-12-29 23:10:01.000000 pyrocumulus-0.9.2/setup.cfg
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2017-12-29 23:10:01.000000 pyrocumulus-0.9.2/script/
--rw-r--r--   0 juca      (1000) juca      (1000)      123 2017-10-12 03:55:42.000000 pyrocumulus-0.9.2/script/pyrocumulus
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2017-12-29 23:10:01.000000 pyrocumulus-0.9.2/pyrocumulus.egg-info/
--rw-r--r--   0 juca      (1000) juca      (1000)        1 2017-12-29 23:10:01.000000 pyrocumulus-0.9.2/pyrocumulus.egg-info/dependency_links.txt
--rw-r--r--   0 juca      (1000) juca      (1000)     1483 2017-12-29 23:10:01.000000 pyrocumulus-0.9.2/pyrocumulus.egg-info/PKG-INFO
--rw-r--r--   0 juca      (1000) juca      (1000)      910 2017-12-29 23:10:01.000000 pyrocumulus-0.9.2/pyrocumulus.egg-info/SOURCES.txt
--rw-r--r--   0 juca      (1000) juca      (1000)       61 2017-12-29 23:10:01.000000 pyrocumulus-0.9.2/pyrocumulus.egg-info/requires.txt
--rw-r--r--   0 juca      (1000) juca      (1000)       12 2017-12-29 23:10:01.000000 pyrocumulus-0.9.2/pyrocumulus.egg-info/top_level.txt
+drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2018-04-25 05:28:06.000000 pyrocumulus-0.9.3/
+drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2018-04-25 05:28:06.000000 pyrocumulus-0.9.3/pyrocumulus/
+drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2018-04-25 05:28:06.000000 pyrocumulus-0.9.3/pyrocumulus/commands/
+-rw-r--r--   0 juca      (1000) juca      (1000)     6322 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/commands/base.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     7295 2018-04-25 05:18:03.000000 pyrocumulus-0.9.3/pyrocumulus/commands/runtornado.py
+-rw-r--r--   0 juca      (1000) juca      (1000)      915 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/commands/test.py
+-rw-r--r--   0 juca      (1000) juca      (1000)       23 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/commands/__init__.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     4443 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/commands/authcli.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     3914 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/commands/createproject.py
+-rw-r--r--   0 juca      (1000) juca      (1000)    10538 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/converters.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     3545 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/auth.py
+drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2018-04-25 05:28:06.000000 pyrocumulus-0.9.3/pyrocumulus/web/
+-rw-r--r--   0 juca      (1000) juca      (1000)     3886 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/web/mixins.py
+-rw-r--r--   0 juca      (1000) juca      (1000)    22203 2017-12-29 22:16:43.000000 pyrocumulus-0.9.3/pyrocumulus/web/handlers.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     2143 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/web/decorators.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     2000 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/web/metaclasses.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     4720 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/web/operationmappers.py
+-rw-r--r--   0 juca      (1000) juca      (1000)       24 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/web/__init__.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     3955 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/web/applications.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     3656 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/web/template.py
+-rw-r--r--   0 juca      (1000) juca      (1000)      708 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/web/request_handlers.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     5453 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/web/urlmappers.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     2016 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/testing.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     5282 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/parsers.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     1859 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/conf.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     1602 2018-04-25 05:22:09.000000 pyrocumulus-0.9.3/pyrocumulus/utils.py
+-rw-r--r--   0 juca      (1000) juca      (1000)      770 2018-04-25 05:26:10.000000 pyrocumulus-0.9.3/pyrocumulus/__init__.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     1546 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/db.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     1211 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/pyrocumulus/exceptions.py
+-rw-r--r--   0 juca      (1000) juca      (1000)     2368 2017-11-16 21:33:32.000000 pyrocumulus-0.9.3/setup.py
+-rw-r--r--   0 juca      (1000) juca      (1000)      387 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/README
+-rw-r--r--   0 juca      (1000) juca      (1000)     1483 2018-04-25 05:28:06.000000 pyrocumulus-0.9.3/PKG-INFO
+-rw-r--r--   0 juca      (1000) juca      (1000)       38 2018-04-25 05:28:06.000000 pyrocumulus-0.9.3/setup.cfg
+drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2018-04-25 05:28:06.000000 pyrocumulus-0.9.3/script/
+-rw-r--r--   0 juca      (1000) juca      (1000)      123 2017-10-12 03:55:42.000000 pyrocumulus-0.9.3/script/pyrocumulus
+drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2018-04-25 05:28:06.000000 pyrocumulus-0.9.3/pyrocumulus.egg-info/
+-rw-r--r--   0 juca      (1000) juca      (1000)        1 2018-04-25 05:28:06.000000 pyrocumulus-0.9.3/pyrocumulus.egg-info/dependency_links.txt
+-rw-r--r--   0 juca      (1000) juca      (1000)     1483 2018-04-25 05:28:06.000000 pyrocumulus-0.9.3/pyrocumulus.egg-info/PKG-INFO
+-rw-r--r--   0 juca      (1000) juca      (1000)      910 2018-04-25 05:28:06.000000 pyrocumulus-0.9.3/pyrocumulus.egg-info/SOURCES.txt
+-rw-r--r--   0 juca      (1000) juca      (1000)       61 2018-04-25 05:28:06.000000 pyrocumulus-0.9.3/pyrocumulus.egg-info/requires.txt
+-rw-r--r--   0 juca      (1000) juca      (1000)       12 2018-04-25 05:28:06.000000 pyrocumulus-0.9.3/pyrocumulus.egg-info/top_level.txt
```

### Comparing `pyrocumulus-0.9.2/pyrocumulus/commands/base.py` & `pyrocumulus-0.9.3/pyrocumulus/commands/base.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/commands/runtornado.py` & `pyrocumulus-0.9.3/pyrocumulus/commands/runtornado.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
          'kwargs': {'default': False, 'help': 'kill tornado server',
                     'action': 'store_true'}},
         # --asyncio
         {'args': ('--asyncio',),
          'kwargs': {'default': False, 'help': 'Use asyncio main loop',
                     'action': 'store_true'}},
         # --log-level
-        {'args': ('--log-level',),
+        {'args': ('--loglevel',),
          'kwargs': {'default': 'info', 'help': 'Log level',
                     'nargs': '?'}},
 
     ]
 
     def run(self):
         if self.asyncio:
@@ -123,15 +123,15 @@
         Fork twice and setsid
         """
         self._do_fork()
         os.setsid()
         self._do_fork()
 
     def _set_log_level(self):
-        logging.basicConfig(level=getattr(logging, self.log_level.upper()))
+        logging.basicConfig(level=getattr(logging, self.loglevel.upper()))
 
     def close_file_descriptors(self):
         """
         Closes stdin
         """
         # the `canonical` way of doing this is to close
         # all file descriptors, using RLIMIT_NOFILE.
```

### Comparing `pyrocumulus-0.9.2/pyrocumulus/commands/test.py` & `pyrocumulus-0.9.3/pyrocumulus/commands/test.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/commands/authcli.py` & `pyrocumulus-0.9.3/pyrocumulus/commands/authcli.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/commands/createproject.py` & `pyrocumulus-0.9.3/pyrocumulus/commands/createproject.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/converters.py` & `pyrocumulus-0.9.3/pyrocumulus/converters.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/auth.py` & `pyrocumulus-0.9.3/pyrocumulus/auth.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/web/mixins.py` & `pyrocumulus-0.9.3/pyrocumulus/web/mixins.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/web/handlers.py` & `pyrocumulus-0.9.3/pyrocumulus/web/handlers.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/web/decorators.py` & `pyrocumulus-0.9.3/pyrocumulus/web/decorators.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/web/metaclasses.py` & `pyrocumulus-0.9.3/pyrocumulus/web/metaclasses.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/web/operationmappers.py` & `pyrocumulus-0.9.3/pyrocumulus/web/operationmappers.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/web/applications.py` & `pyrocumulus-0.9.3/pyrocumulus/web/applications.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/web/template.py` & `pyrocumulus-0.9.3/pyrocumulus/web/template.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/web/request_handlers.py` & `pyrocumulus-0.9.3/pyrocumulus/web/request_handlers.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/web/urlmappers.py` & `pyrocumulus-0.9.3/pyrocumulus/web/urlmappers.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/testing.py` & `pyrocumulus-0.9.3/pyrocumulus/testing.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/parsers.py` & `pyrocumulus-0.9.3/pyrocumulus/parsers.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/conf.py` & `pyrocumulus-0.9.3/pyrocumulus/conf.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/utils.py` & `pyrocumulus-0.9.3/pyrocumulus/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 import sys
 import imp
 import inspect
 import bcrypt
 from pyrocumulus.conf import settings
 
+SALT_ROUNDS = 12
+
 
 def get_value_from_settings(key, default=None):
     value = getattr(settings, key, default)
     return value
 
 
 def fqualname(obj):
@@ -44,10 +46,10 @@
     mod = imp.importlib.import_module(mod)
     return getattr(mod, cls)
 
 
 def bcrypt_string(string, salt=None):
     encoding = sys.getdefaultencoding()
     if not salt:
-        salt = settings.BCRYPT_SALT.encode(encoding)
+        salt = bcrypt.gensalt(SALT_ROUNDS)
     encrypted = bcrypt.hashpw(string.encode(encoding), salt)
     return encrypted.decode()
```

### Comparing `pyrocumulus-0.9.2/pyrocumulus/__init__.py` & `pyrocumulus-0.9.3/pyrocumulus/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with pyrocumulus.  If not, see <http://www.gnu.org/licenses/>.
 
 
-VERSION = '0.9.2'
+VERSION = '0.9.3'
```

### Comparing `pyrocumulus-0.9.2/pyrocumulus/db.py` & `pyrocumulus-0.9.3/pyrocumulus/db.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/pyrocumulus/exceptions.py` & `pyrocumulus-0.9.3/pyrocumulus/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/setup.py` & `pyrocumulus-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyrocumulus-0.9.2/PKG-INFO` & `pyrocumulus-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyrocumulus
-Version: 0.9.2
+Version: 0.9.3
 Summary: 
 Glue-code to make (even more!) easy and fun work with mongoengine and tornado
 
 Home-page: https://gitorious.org/mongomotor
 Author: Juca Crispim
 Author-email: juca@poraodojuca.net
 License: UNKNOWN
```

### Comparing `pyrocumulus-0.9.2/pyrocumulus.egg-info/PKG-INFO` & `pyrocumulus-0.9.3/pyrocumulus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyrocumulus
-Version: 0.9.2
+Version: 0.9.3
 Summary: 
 Glue-code to make (even more!) easy and fun work with mongoengine and tornado
 
 Home-page: https://gitorious.org/mongomotor
 Author: Juca Crispim
 Author-email: juca@poraodojuca.net
 License: UNKNOWN
```

### Comparing `pyrocumulus-0.9.2/pyrocumulus.egg-info/SOURCES.txt` & `pyrocumulus-0.9.3/pyrocumulus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

