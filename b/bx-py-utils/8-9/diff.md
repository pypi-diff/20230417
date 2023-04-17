# Comparing `tmp/bx_py_utils-8.tar.gz` & `tmp/bx_py_utils-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bx_py_utils-8.tar", last modified: Mon Nov 30 15:00:25 2020, max compression
+gzip compressed data, was "bx_py_utils-9.tar", last modified: Tue Dec  1 10:30:17 2020, max compression
```

## Comparing `bx_py_utils-8.tar` & `bx_py_utils-9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1068 2020-10-06 11:18:24.585248 bx_py_utils-8/LICENSE
--rw-r--r--   0        0        0     1076 2020-11-11 13:09:04.294093 bx_py_utils-8/README.md
--rw-r--r--   0        0        0       18 2020-11-30 14:30:39.532191 bx_py_utils-8/bx_py_utils/__init__.py
--rw-r--r--   0        0        0      792 2020-11-20 07:55:57.394159 bx_py_utils-8/bx_py_utils/dict_utils.py
--rw-r--r--   0        0        0     2239 2020-10-29 14:48:12.468364 bx_py_utils-8/bx_py_utils/error_handling.py
--rw-r--r--   0        0        0     1207 2020-11-09 08:12:19.613621 bx_py_utils-8/bx_py_utils/filename.py
--rw-r--r--   0        0        0      586 2020-10-16 13:19:54.440559 bx_py_utils-8/bx_py_utils/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      591 2020-10-16 13:13:10.852321 bx_py_utils-8/bx_py_utils/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      574 2020-10-16 13:19:54.444559 bx_py_utils-8/bx_py_utils/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      579 2020-10-16 13:13:10.848321 bx_py_utils-8/bx_py_utils/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-10-06 11:34:03.065746 bx_py_utils-8/bx_py_utils/models/__init__.py
--rw-r--r--   0        0        0      945 2020-11-06 15:18:41.990070 bx_py_utils-8/bx_py_utils/models/manipulate.py
--rw-r--r--   0        0        0     1744 2020-10-16 13:05:21.808604 bx_py_utils-8/bx_py_utils/models/timetracking.py
--rw-r--r--   0        0        0        0 2020-11-11 13:06:05.859777 bx_py_utils-8/bx_py_utils/test_utils/__init__.py
--rw-r--r--   0        0        0      802 2020-11-11 13:07:27.819001 bx_py_utils-8/bx_py_utils/test_utils/datetime.py
--rw-r--r--   0        0        0     2667 2020-11-30 14:16:06.000000 bx_py_utils-8/bx_py_utils/test_utils/model_clean_assert.py
--rw-r--r--   0        0        0      926 2020-11-30 15:00:22.613205 bx_py_utils-8/pyproject.toml
--rw-r--r--   0        0        0     2000 2020-11-30 15:00:26.025094 bx_py_utils-8/setup.py
--rw-r--r--   0        0        0     1860 2020-11-30 15:00:26.025331 bx_py_utils-8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2020-10-06 11:18:24.585248 bx_py_utils-9/LICENSE
+-rw-r--r--   0        0        0     1076 2020-11-11 13:09:04.294093 bx_py_utils-9/README.md
+-rw-r--r--   0        0        0       18 2020-12-01 09:39:26.919684 bx_py_utils-9/bx_py_utils/__init__.py
+-rw-r--r--   0        0        0      792 2020-11-20 07:55:57.394159 bx_py_utils-9/bx_py_utils/dict_utils.py
+-rw-r--r--   0        0        0     2239 2020-10-29 14:48:12.468364 bx_py_utils-9/bx_py_utils/error_handling.py
+-rw-r--r--   0        0        0     1207 2020-11-09 08:12:19.613621 bx_py_utils-9/bx_py_utils/filename.py
+-rw-r--r--   0        0        0      586 2020-10-16 13:19:54.440559 bx_py_utils-9/bx_py_utils/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      591 2020-10-16 13:13:10.852321 bx_py_utils-9/bx_py_utils/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      574 2020-10-16 13:19:54.444559 bx_py_utils-9/bx_py_utils/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      579 2020-10-16 13:13:10.848321 bx_py_utils-9/bx_py_utils/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-10-06 11:34:03.065746 bx_py_utils-9/bx_py_utils/models/__init__.py
+-rw-r--r--   0        0        0     1155 2020-12-01 09:37:02.157158 bx_py_utils-9/bx_py_utils/models/manipulate.py
+-rw-r--r--   0        0        0     1744 2020-10-16 13:05:21.808604 bx_py_utils-9/bx_py_utils/models/timetracking.py
+-rw-r--r--   0        0        0        0 2020-11-11 13:06:05.859777 bx_py_utils-9/bx_py_utils/test_utils/__init__.py
+-rw-r--r--   0        0        0      802 2020-11-11 13:07:27.819001 bx_py_utils-9/bx_py_utils/test_utils/datetime.py
+-rw-r--r--   0        0        0     2667 2020-11-30 14:16:06.000000 bx_py_utils-9/bx_py_utils/test_utils/model_clean_assert.py
+-rw-r--r--   0        0        0      926 2020-12-01 10:30:13.639173 bx_py_utils-9/pyproject.toml
+-rw-r--r--   0        0        0     2000 2020-12-01 10:30:17.219518 bx_py_utils-9/setup.py
+-rw-r--r--   0        0        0     1860 2020-12-01 10:30:17.219777 bx_py_utils-9/PKG-INFO
```

### Comparing `bx_py_utils-8/LICENSE` & `bx_py_utils-9/LICENSE`

 * *Files identical despite different names*

### Comparing `bx_py_utils-8/README.md` & `bx_py_utils-9/README.md`

 * *Files identical despite different names*

### Comparing `bx_py_utils-8/bx_py_utils/dict_utils.py` & `bx_py_utils-9/bx_py_utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `bx_py_utils-8/bx_py_utils/error_handling.py` & `bx_py_utils-9/bx_py_utils/error_handling.py`

 * *Files identical despite different names*

### Comparing `bx_py_utils-8/bx_py_utils/filename.py` & `bx_py_utils-9/bx_py_utils/filename.py`

 * *Files identical despite different names*

### Comparing `bx_py_utils-8/bx_py_utils/locale/de/LC_MESSAGES/django.mo` & `bx_py_utils-9/bx_py_utils/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bx_py_utils-8/bx_py_utils/locale/de/LC_MESSAGES/django.po` & `bx_py_utils-9/bx_py_utils/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bx_py_utils-8/bx_py_utils/locale/en/LC_MESSAGES/django.mo` & `bx_py_utils-9/bx_py_utils/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bx_py_utils-8/bx_py_utils/locale/en/LC_MESSAGES/django.po` & `bx_py_utils-9/bx_py_utils/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bx_py_utils-8/bx_py_utils/models/manipulate.py` & `bx_py_utils-9/bx_py_utils/models/manipulate.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,24 +8,28 @@
 def create_or_update(*, ModelClass, lookup, **values):
     """
     Create a new model instance or update a existing one
     Similar to django's own create_or_update() but:
 
      * Use update_fields and save only changed fields
      * return the information about changed field names.
+     * validate before save
     """
     assert isinstance(lookup, dict)
     instance = ModelClass.objects.filter(**lookup).first()
     if not instance:
-        instance = ModelClass.objects.create(**lookup, **values)
+        instance = ModelClass(**lookup, **values)
+        instance.full_clean(validate_unique=False)  # Don't create non-valid instances
+        instance.save()
         return instance, True, None
 
     updated_fields = []
     for key, value in values.items():
         if getattr(instance, key) != value:
             setattr(instance, key, value)
             updated_fields.append(key)
 
     if updated_fields:
+        instance.full_clean(validate_unique=False)  # Don't save new non-valid values
         instance.save(update_fields=updated_fields)
 
     return instance, False, updated_fields
```

### Comparing `bx_py_utils-8/bx_py_utils/models/timetracking.py` & `bx_py_utils-9/bx_py_utils/models/timetracking.py`

 * *Files identical despite different names*

### Comparing `bx_py_utils-8/bx_py_utils/test_utils/datetime.py` & `bx_py_utils-9/bx_py_utils/test_utils/datetime.py`

 * *Files identical despite different names*

### Comparing `bx_py_utils-8/bx_py_utils/test_utils/model_clean_assert.py` & `bx_py_utils-9/bx_py_utils/test_utils/model_clean_assert.py`

 * *Files identical despite different names*

### Comparing `bx_py_utils-8/pyproject.toml` & `bx_py_utils-9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'bx_py_utils'
-version = "8"
+version = "9"
 description = 'Various Python / Django utility functions'
 authors = [
     'Jens Diemer <jens.diemer@boxine.de>',
     'Philipp Hagemeister <phihag@phihag.de>'
 ]
 classifiers = [
     'Development Status :: 3 - Alpha',
```

### Comparing `bx_py_utils-8/setup.py` & `bx_py_utils-9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 entry_points = \
 {'console_scripts': ['publish = '
                      'bx_py_utils_tests.test_project.publish:publish']}
 
 setup_kwargs = {
     'name': 'bx-py-utils',
-    'version': '8',
+    'version': '9',
     'description': 'Various Python / Django utility functions',
     'long_description': '# Boxine - bx_py_utils\n\nVarious Python / Django utility functions\n\n## Quickstart\n\n```bash\n~$ git clone https://github.com/boxine/bx_py_utils.git\n~$ cd bx_py_utils\n~/bx_py_utils$ make\nhelp                 List all commands\ninstall-poetry       install or update poetry\ninstall              install via poetry\nupdate               Update the dependencies as according to the pyproject.toml file\nlint                 Run code formatters and linter\nfix-code-style       Fix code formatting\ntox-listenvs         List all tox test environments\ntox                  Run pytest via tox with all environments\ntox-py36             Run pytest via tox with *python v3.6*\ntox-py37             Run pytest via tox with *python v3.7*\ntox-py38             Run pytest via tox with *python v3.8*\ntox-py39             Run pytest via tox with *python v3.9*\npytest               Run pytest\npytest-ci            Run pytest with CI settings\npublish              Release new version to PyPi\nmakemessages         Make and compile locales message files\n```\n\n## License\n\n[MIT](LICENSE). Patches welcome!\n',
     'author': 'Jens Diemer',
     'author_email': 'jens.diemer@boxine.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `bx_py_utils-8/PKG-INFO` & `bx_py_utils-9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bx-py-utils
-Version: 8
+Version: 9
 Summary: Various Python / Django utility functions
 License: MIT
 Keywords: django,utilities
 Author: Jens Diemer
 Author-email: jens.diemer@boxine.de
 Requires-Python: >=3.6,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

