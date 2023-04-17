# Comparing `tmp/django-snowflake-4.2a1.tar.gz` & `tmp/django-snowflake-4.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-snowflake-4.2a1.tar", last modified: Sat Mar 18 14:45:40 2023, max compression
+gzip compressed data, was "django-snowflake-4.2b1.tar", last modified: Wed Apr 12 00:41:54 2023, max compression
```

## Comparing `django-snowflake-4.2a1.tar` & `django-snowflake-4.2b1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-03-18 14:45:40.676679 django-snowflake-4.2a1/
--rw-rw-r--   0 tim       (1000) tim       (1000)       76 2023-03-18 14:41:51.000000 django-snowflake-4.2a1/CHANGELOG.md
--rw-rw-r--   0 tim       (1000) tim       (1000)     1045 2021-12-02 00:53:37.000000 django-snowflake-4.2a1/LICENSE
--rw-rw-r--   0 tim       (1000) tim       (1000)       21 2022-03-02 21:04:16.000000 django-snowflake-4.2a1/MANIFEST.in
--rw-rw-r--   0 tim       (1000) tim       (1000)     4576 2023-03-18 14:45:40.676679 django-snowflake-4.2a1/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     3581 2023-03-18 14:41:51.000000 django-snowflake-4.2a1/README.md
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-03-18 14:45:40.672679 django-snowflake-4.2a1/django_snowflake/
--rw-rw-r--   0 tim       (1000) tim       (1000)      284 2023-03-18 14:41:51.000000 django-snowflake-4.2a1/django_snowflake/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6509 2022-03-07 00:47:16.000000 django-snowflake-4.2a1/django_snowflake/base.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2495 2022-03-07 00:47:16.000000 django-snowflake-4.2a1/django_snowflake/client.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2150 2022-03-02 21:04:16.000000 django-snowflake-4.2a1/django_snowflake/creation.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    17119 2023-03-18 14:41:51.000000 django-snowflake-4.2a1/django_snowflake/features.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1891 2022-03-02 21:04:16.000000 django-snowflake-4.2a1/django_snowflake/functions.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     8528 2023-03-18 14:41:51.000000 django-snowflake-4.2a1/django_snowflake/introspection.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     8013 2023-03-14 01:22:31.000000 django-snowflake-4.2a1/django_snowflake/operations.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6881 2023-03-18 14:41:51.000000 django-snowflake-4.2a1/django_snowflake/schema.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      766 2021-11-12 23:38:40.000000 django-snowflake-4.2a1/django_snowflake/utils.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-03-18 14:45:40.676679 django-snowflake-4.2a1/django_snowflake.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)     4576 2023-03-18 14:45:40.000000 django-snowflake-4.2a1/django_snowflake.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)      547 2023-03-18 14:45:40.000000 django-snowflake-4.2a1/django_snowflake.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-03-18 14:45:40.000000 django-snowflake-4.2a1/django_snowflake.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       34 2023-03-18 14:45:40.000000 django-snowflake-4.2a1/django_snowflake.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       17 2023-03-18 14:45:40.000000 django-snowflake-4.2a1/django_snowflake.egg-info/top_level.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)     1194 2023-03-18 14:45:40.676679 django-snowflake-4.2a1/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2022-03-02 21:04:16.000000 django-snowflake-4.2a1/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-12 00:41:54.811958 django-snowflake-4.2b1/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      138 2023-04-12 00:40:12.000000 django-snowflake-4.2b1/CHANGELOG.md
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1058 2023-04-12 00:28:15.000000 django-snowflake-4.2b1/LICENSE
+-rw-rw-r--   0 tim       (1000) tim       (1000)       21 2023-04-10 00:45:59.000000 django-snowflake-4.2b1/MANIFEST.in
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5746 2023-04-12 00:41:54.811958 django-snowflake-4.2b1/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4740 2023-04-12 00:28:25.000000 django-snowflake-4.2b1/README.md
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-12 00:41:54.811958 django-snowflake-4.2b1/django_snowflake/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      349 2023-04-12 00:39:59.000000 django-snowflake-4.2b1/django_snowflake/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6751 2023-04-10 00:45:58.000000 django-snowflake-4.2b1/django_snowflake/base.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2495 2023-04-10 00:45:58.000000 django-snowflake-4.2b1/django_snowflake/client.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4232 2023-04-10 00:45:58.000000 django-snowflake-4.2b1/django_snowflake/compiler.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2150 2023-04-10 00:45:58.000000 django-snowflake-4.2b1/django_snowflake/creation.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    20557 2023-04-12 00:39:59.000000 django-snowflake-4.2b1/django_snowflake/features.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1891 2023-04-10 00:45:58.000000 django-snowflake-4.2b1/django_snowflake/functions.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     8564 2023-04-12 00:28:15.000000 django-snowflake-4.2b1/django_snowflake/introspection.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3040 2023-04-10 00:45:58.000000 django-snowflake-4.2b1/django_snowflake/lookups.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     8063 2023-04-11 02:39:33.000000 django-snowflake-4.2b1/django_snowflake/operations.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6956 2023-04-10 00:45:59.000000 django-snowflake-4.2b1/django_snowflake/schema.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      766 2023-04-10 00:45:58.000000 django-snowflake-4.2b1/django_snowflake/utils.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-12 00:41:54.811958 django-snowflake-4.2b1/django_snowflake.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5746 2023-04-12 00:41:54.000000 django-snowflake-4.2b1/django_snowflake.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)      604 2023-04-12 00:41:54.000000 django-snowflake-4.2b1/django_snowflake.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-04-12 00:41:54.000000 django-snowflake-4.2b1/django_snowflake.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       34 2023-04-12 00:41:54.000000 django-snowflake-4.2b1/django_snowflake.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       17 2023-04-12 00:41:54.000000 django-snowflake-4.2b1/django_snowflake.egg-info/top_level.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1205 2023-04-12 00:41:54.811958 django-snowflake-4.2b1/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-04-10 00:45:59.000000 django-snowflake-4.2b1/setup.py
```

### Comparing `django-snowflake-4.2a1/LICENSE` & `django-snowflake-4.2b1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2021 Cedar
+Copyright (c) 2023 Snowflake Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `django-snowflake-4.2a1/PKG-INFO` & `django-snowflake-4.2b1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,44 @@
-Metadata-Version: 2.1
-Name: django-snowflake
-Version: 4.2a1
-Summary: Django backend for Snowflake
-Home-page: https://github.com/cedar-team/django-snowflake
-Maintainer: Tim Graham
-Maintainer-email: timograham@gmail.com
-License: MIT License
-Project-URL: Source, https://github.com/cedar-team/django-snowflake
-Project-URL: Tracker, https://github.com/cedar-team/django-snowflake/issues
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.2
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Snowflake backend for Django
 
 ## Install and usage
 
 Use the version of django-snowflake that corresponds to your version of
 Django. For example, to get the latest compatible release for Django 4.2.x:
 
 `pip install django-snowflake==4.2.*`
 
 The minor release number of Django doesn't correspond to the minor release
 number of django-snowflake. Use the latest minor release of each.
 
+If a release series of django-snowflake only has pre-releases (alphas or
+betas), you'll see an error with a list of the available versions. In that
+case, include `--pre` to allow `pip` to install the latest pre-release.
+
+For example, if django-snowflake 4.2 alpha 1 is the latest available version
+of the 4.2 release series:
+
+```
+$ pip install django-snowflake==4.2.*
+ERROR: Could not find a version that satisfies the requirement
+django-snowflake==4.2.* (from versions: ..., 4.2a1)
+
+$ pip install --pre django-snowflake==4.2.*
+...
+Successfully installed ... django-snowflake-4.2a1 ...
+```
+
 Configure the Django `DATABASES` setting similar to this:
 
 ```python
 DATABASES = {
     'default': {
         'ENGINE': 'django_snowflake',
         'NAME': 'MY_DATABASE',
-        'SCHEMA': 'MY_SCHEME',
+        'SCHEMA': 'MY_SCHEMA',
         'WAREHOUSE': 'MY_WAREHOUSE',
         'USER': 'my_user',
         'PASSWORD': 'my_password',
         'ACCOUNT': 'my_account',
         # Include 'OPTIONS' if you need to specify any other
         # snowflake.connector.connect() parameters.
         # https://docs.snowflake.com/en/user-guide/python-connector-api.html#connect
@@ -65,16 +56,14 @@
 - Snowflake supports defining foreign key and unique constraints, however, it
   doesn't enforce them. Thus, Django manages these constraints and `inspectdb`
   detects them, but Django won't raise `IntegrityError` if they're violated.
 
 - Snowflake doesn't support indexes. Thus, Django ignores any indexes defined
   on models or fields.
 
-- `JSONField` is [not supported](https://github.com/cedar-team/django-snowflake/issues/23).
-
 - Snowflake doesn't support check constraints, so the various
   `PositiveIntegerField` model fields allow negative values (though validation
   at the form level still works).
 
 ## Notes on Django QuerySets
 
 * Snowflake has
@@ -83,15 +72,15 @@
 * Valid values for `QuerySet.explain()`'s `format` parameter are `'json'`,
   `'tabular'`, and `'text'`. The default is `'tabular'`.
 
 ## Known issues and limitations
 
 This list isn't exhaustive. If you run into a problem, consult
 `django_snowflake/features.py` to see if a similar test is skipped. Please
-[create an issue on GitHub](https://github.com/cedar-team/django-snowflake/issues/new)
+[create an issue on GitHub](https://github.com/Snowflake-Labs/django-snowflake/issues/new)
 if you encounter an issue worth documenting.
 
 * Snowflake doesn't support `last_insert_id` to retrieve the ID of a newly
   created object. Instead, this backend issues the query
   `SELECT MAX(pk_name) FROM table_name` to retrieve the ID. This is subject
   to race conditions if objects are created concurrently. This makes this
   backend inappropriate for use in web app use cases where multiple clients
@@ -100,14 +89,26 @@
 
 * Snowflake only supports single layer transactions, but Django's `TestCase`
   requires that the database supports nested transactions. Therefore, Django's
   `TestCase` operates like `TransactionTestCase`, without the benefit of
   transactions to speed it up. A future version of Django (5.0 at the earliest)
   may leverage Snowflake's single layer transactions to give some speed up.
 
-* Interval math where the interval is a column
-  [is not supported](https://github.com/cedar-team/django-snowflake/issues/27).
+* Due to snowflake-connector-python's [lack of VARIANT support](https://github.com/snowflakedb/snowflake-connector-python/issues/244),
+  some `JSONField` queries with complex JSON parameters [don't work](https://github.com/Snowflake-Labs/django-snowflake/issues/58).
 
-* Interval math with a null interval
-  [crashes](https://github.com/cedar-team/django-snowflake/issues/26).
+  For example, if `value` is a `JSONField`, this won't work:
+  ```python
+  >>> JSONModel.objects.filter(value__k={"l": "m"})
+  ```
+  A workaround is:
+  ```python
+  >>> from django.db.models.expressions import RawSQL
+  >>> JSONModel.objects.filter(value__k=RawSQL("PARSE_JSON(%s)", ('{"l": "m"}',)))
+  ```
+  In addition, ``QuerySet.bulk_update()`` isn't supported for `JSONField`.
 
+* Interval math where the interval is a column
+  [is not supported](https://github.com/Snowflake-Labs/django-snowflake/issues/27).
 
+* Interval math with a null interval
+  [crashes](https://github.com/Snowflake-Labs/django-snowflake/issues/26).
```

### Comparing `django-snowflake-4.2a1/django_snowflake/base.py` & `django-snowflake-4.2b1/django_snowflake/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import os
+
 from django.core.exceptions import ImproperlyConfigured
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.utils.asyncio import async_unsafe
 
 try:
     import snowflake.connector as Database
 except ImportError as e:
     raise ImproperlyConfigured("Error loading snowflake connector module: %s" % e)
 
 # Some of these import snowflake connector, so import them after checking if it's installed.
+from . import __version__                                   # NOQA isort:skip
 from .client import DatabaseClient                          # NOQA isort:skip
 from .creation import DatabaseCreation                      # NOQA isort:skip
 from .features import DatabaseFeatures                      # NOQA isort:skip
 from .introspection import DatabaseIntrospection            # NOQA isort:skip
 from .operations import DatabaseOperations                  # NOQA isort:skip
 from .schema import DatabaseSchemaEditor                    # NOQA isort:skip
 
@@ -91,14 +94,16 @@
 
     def get_connection_params(self):
         settings_dict = self.settings_dict
         conn_params = {
             'interpolate_empty_sequences':  True,
             **settings_dict['OPTIONS'],
         }
+        if os.environ.get('RUNNING_DJANGOS_TEST_SUITE') != 'true':
+            conn_params['application'] = 'Django_SnowflakeConnector_%s' % __version__
 
         if settings_dict['NAME']:
             conn_params['database'] = self.ops.quote_name(settings_dict['NAME'])
 
         if settings_dict['USER']:
             conn_params['user'] = settings_dict['USER']
         else:
```

### Comparing `django-snowflake-4.2a1/django_snowflake/client.py` & `django-snowflake-4.2b1/django_snowflake/client.py`

 * *Files identical despite different names*

### Comparing `django-snowflake-4.2a1/django_snowflake/creation.py` & `django-snowflake-4.2b1/django_snowflake/creation.py`

 * *Files identical despite different names*

### Comparing `django-snowflake-4.2a1/django_snowflake/features.py` & `django-snowflake-4.2b1/django_snowflake/features.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 from django.db import InterfaceError
 from django.db.backends.base.features import BaseDatabaseFeatures
 from django.utils.functional import cached_property
 
 
 class DatabaseFeatures(BaseDatabaseFeatures):
     can_clone_databases = True
-    can_introspect_json_field = False
     closed_cursor_error_class = InterfaceError
+    create_test_procedure_without_params_sql = """
+        CREATE PROCEDURE test_procedure() RETURNS varchar LANGUAGE JAVASCRIPT AS $$
+           var i = 1;
+    $$"""
+    create_test_procedure_with_int_param_sql = """
+        CREATE OR REPLACE PROCEDURE test_procedure(value integer) RETURNS varchar LANGUAGE PYTHON
+            HANDLER = 'run'
+            RUNTIME_VERSION = '3.8'
+            PACKAGES = ('snowflake-snowpark-python')
+        AS
+        $$def run(session, value): pass
+    $$"""
     # This feature is specific to the Django fork used for testing.
     enforces_foreign_key_constraints = False
     # This feature is specific to the Django fork used for testing.
     enforces_unique_constraints = False
     allows_multiple_constraints_on_same_fields = False
     has_json_object_function = False
     indexes_foreign_keys = False
@@ -21,16 +32,15 @@
     supports_column_check_constraints = False
     supports_table_check_constraints = False
     supports_expression_indexes = False
     supports_ignore_conflicts = False
     # This feature is specific to the Django fork used for testing.
     supports_indexes = False
     supports_index_column_ordering = False
-    # Not yet implemented in this backend.
-    supports_json_field = False
+    supports_json_field_contains = False
     supports_over_clause = True
     supports_partial_indexes = False
     # https://docs.snowflake.com/en/sql-reference/functions-regexp.html#backreferences
     supports_regex_backreferencing = False
     supports_sequence_reset = False
     supports_slicing_ordering_in_compound = True
     supports_subqueries_in_group_by = False
@@ -73,23 +83,66 @@
         'expressions.tests.FTimeDeltaTests.test_delta_update',
         # Altering Integer PK to AutoField not supported.
         'migrations.test_operations.OperationTests.test_alter_field_pk',
         'schema.tests.SchemaTests.test_alter_int_pk_to_autofield_pk',
         'schema.tests.SchemaTests.test_alter_int_pk_to_bigautofield_pk',
         'schema.tests.SchemaTests.test_alter_smallint_pk_to_smallautofield_pk',
         # Interval math with NULL crashes:
-        # https://github.com/cedar-team/django-snowflake/issues/26
+        # https://github.com/Snowflake-Labs/django-snowflake/issues/26
         'expressions.tests.FTimeDeltaTests.test_date_subtraction',
         'expressions.tests.FTimeDeltaTests.test_datetime_subtraction',
         'expressions.tests.FTimeDeltaTests.test_time_subtraction',
         # Invalid expression [(SELECT (MAX(U0.NUM_EMPLOYEES)) + 1 AS
         # "NEW_NUM_EMPLOYEES" FROM EXPRESSIONS_COMPANY AS U0 GROUP BY U0.ID,
         # ...  ORDER BY U0.NUM_EMPLOYEES DESC NULLS FIRST LIMIT 1 OFFSET 0)]
         # in VALUES clause.
         'expressions.tests.BasicExpressionsTests.test_object_create_with_f_expression_in_subquery',
+        # JSONField queries with complex JSON parameters don't work:
+        # https://github.com/Snowflake-Labs/django-snowflake/issues/58
+        # Query:
+        #   WHERE "MODEL_FIELDS_NULLABLEJSONMODEL"."VALUE" = 'null'
+        # needs to operate as:
+        #   WHERE "MODEL_FIELDS_NULLABLEJSONMODEL"."VALUE" = PARSE_JSON('null')
+        'model_fields.test_jsonfield.TestSaveLoad.test_json_null_different_from_sql_null',
+        # Query:
+        #   WHERE TO_JSON("MODEL_FIELDS_NULLABLEJSONMODEL"."VALUE":k) = '{"l": "m"}'
+        # needs to operate as:
+        #   WHERE TO_JSON("MODEL_FIELDS_NULLABLEJSONMODEL"."VALUE":k) = PARSE_JSON('{"l": "m"}')
+        'model_fields.test_jsonfield.TestQuerying.test_shallow_lookup_obj_target',
+        # Query:
+        #   WHERE "MODEL_FIELDS_NULLABLEJSONMODEL"."VALUE" = '{"a": "b", "c": 14}'
+        # needs to operate as:
+        #   WHERE "MODEL_FIELDS_NULLABLEJSONMODEL"."VALUE" = PARSE_JSON('{"a": "b", "c": 14}')
+        'model_fields.test_jsonfield.TestQuerying.test_exact_complex',
+        # Three cases:
+        #     lookup='value__bar__in', value=[['foo', 'bar']]
+        #     lookup='value__bar__in', value=[['foo', 'bar'], ['a']]
+        #     lookup='value__bax__in', value=[{'foo': 'bar'}, {'a': 'b'}]
+        # Query:
+        #   WHERE TO_JSON("MODEL_FIELDS_NULLABLEJSONMODEL"."VALUE":bar) IN ('["foo", "bar"]')
+        # needs to operate as:
+        #   WHERE TO_JSON("MODEL_FIELDS_NULLABLEJSONMODEL"."VALUE":bar) IN (PARSE_JSON('["foo", "bar"]'))
+        'model_fields.test_jsonfield.TestQuerying.test_key_in',
+        # QuerySet.bulk_update() not supported for JSONField:
+        # Expression type does not match column data type, expecting VARIANT
+        # but got VARCHAR(16777216) for column JSON_FIELD
+        'queries.test_bulk_update.BulkUpdateTests.test_json_field',
+        # Server-side bug?
+        # CAST(TO_JSON("MODEL_FIELDS_NULLABLEJSONMODEL"."VALUE":d) AS VARIANT)
+        # gives '"[\\"e\\",{\\"f\\":\\"g\\"}]"' and appending [0] gives None.
+        # The expected result ('"e"') is given by:
+        # PARSE_JSON(TO_JSON("MODEL_FIELDS_NULLABLEJSONMODEL"."VALUE":d))[0]
+        # Possibly this backend could rewrite CAST(... AS VARIANT) to PARSE_JSON(...)?
+        'model_fields.test_jsonfield.TestQuerying.test_key_transform_annotation_expression',
+        'model_fields.test_jsonfield.TestQuerying.test_key_transform_expression',
+        'model_fields.test_jsonfield.TestQuerying.test_nested_key_transform_annotation_expression',
+        'model_fields.test_jsonfield.TestQuerying.test_nested_key_transform_expression',
+        # Fixed if TO_JSON is removed from the ORDER BY clause (or may be fine
+        # as is as some databases give the ordering that Snowflake does.)
+        'model_fields.test_jsonfield.TestQuerying.test_ordering_by_transform',
     }
 
     django_test_skips = {
         'Snowflake does not enforce FOREIGN KEY constraints.': {
             'backends.tests.FkConstraintsTests',
             'model_fields.test_uuid.TestAsPrimaryKeyTransactionTests.test_unsaved_fk',
         },
@@ -157,14 +210,16 @@
             'expressions.tests.BasicExpressionsTests.test_subquery_filter_by_lazy',
             'expressions.tests.BasicExpressionsTests.test_subquery_in_filter',
             'expressions.tests.FTimeDeltaTests.test_date_subquery_subtraction',
             'expressions.tests.FTimeDeltaTests.test_datetime_subquery_subtraction',
             'expressions_window.tests.WindowFunctionTests.test_subquery_row_range_rank',
             'lookup.tests.LookupQueryingTests.test_filter_subquery_lhs',
             'lookup.tests.LookupTests.test_nested_outerref_lhs',
+            'model_fields.test_jsonfield.TestQuerying.test_nested_key_transform_on_subquery',
+            'model_fields.test_jsonfield.TestQuerying.test_obj_subquery_lookup',
             'queries.test_qs_combinators.QuerySetSetOperationTests.test_union_in_subquery',
             'queries.test_qs_combinators.QuerySetSetOperationTests.test_union_in_subquery_related_outerref',
             'queries.test_qs_combinators.QuerySetSetOperationTests.test_union_with_values_list_on_annotated_and_unannotated',  # noqa
             'queries.tests.ExcludeTest17600.test_exclude_plain',
             'queries.tests.ExcludeTest17600.test_exclude_plain_distinct',
             'queries.tests.ExcludeTest17600.test_exclude_with_q_is_equal_to_plain_exclude',
             'queries.tests.ExcludeTest17600.test_exclude_with_q_is_equal_to_plain_exclude_variation',
```

### Comparing `django-snowflake-4.2a1/django_snowflake/functions.py` & `django-snowflake-4.2b1/django_snowflake/functions.py`

 * *Files identical despite different names*

### Comparing `django-snowflake-4.2a1/django_snowflake/introspection.py` & `django-snowflake-4.2b1/django_snowflake/introspection.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         'BOOLEAN': 'BooleanField',
         'DATE': 'DateField',
         'FLOAT': 'FloatField',
         'NUMBER': 'BigIntegerField',
         'TIME': 'TimeField',
         'TIMESTAMP_LTZ': 'DateTimeField',
         'VARCHAR': 'CharField',
+        'VARIANT': 'JSONField',
     }
 
     def get_constraints(self, cursor, table_name):
         table_name = self.connection.ops.quote_name(table_name)
         constraints = {}
         # Foreign keys
         cursor.execute(f'SHOW IMPORTED KEYS IN TABLE {table_name}')
@@ -173,15 +174,15 @@
         # Add quotes around Snowflake generated constraint names like
         # SYS_CONSTRAINT_e8775210-b2d4-4947-b382-c57cecc6bb6d to preserve
         # casing.
         if name.startswith("SYS_CONSTRAINT_"):
             return f'"{name}"'
         # TODO: If the identifier field isn't uppercase, then it needs to be
         # quoted to preserve its case.
-        # https://github.com/cedar-team/django-snowflake/issues/43
+        # https://github.com/Snowflake-Labs/django-snowflake/issues/43
         # This may require some changes in Django itself to work properly. This
         # would replace the special handling of SYS_CONSTRAINT_ above.
         # if name != name.upper():
         #    return f'"{name}"'
         # Otherwise, the identifier name can be lowercased for use as a model
         # field name, for example. DatabaseOperations.quote_name() reverses
         # this transformation by uppercasing the name.
```

### Comparing `django-snowflake-4.2a1/django_snowflake/operations.py` & `django-snowflake-4.2b1/django_snowflake/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 class DatabaseOperations(BaseDatabaseOperations):
     cast_char_field_without_max_length = 'varchar'
     cast_data_types = {
         'AutoField': 'NUMBER',
         'BigAutoField': 'NUMBER',
         'SmallAutoField': 'NUMBER',
     }
+    compiler_module = 'django_snowflake.compiler'
     explain_prefix = 'EXPLAIN USING'
 
     def bulk_insert_sql(self, fields, placeholder_rows):
         placeholder_rows_sql = (', '.join(row) for row in placeholder_rows)
         values_sql = ', '.join('(%s)' % sql for sql in placeholder_rows_sql)
         return 'VALUES ' + values_sql
```

### Comparing `django-snowflake-4.2a1/django_snowflake/schema.py` & `django-snowflake-4.2b1/django_snowflake/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 
 
 class DatabaseSchemaEditor(BaseDatabaseSchemaEditor):
     sql_create_column_inline_fk = (
         'CONSTRAINT %(name)s FOREIGN KEY REFERENCES %(to_table)s(%(to_column)s)'
     )
+    sql_delete_procedure = 'DROP PROCEDURE %(procedure)s(%(param_types)s)'
 
     def _create_index_sql(self, model, fields=None, **kwargs):
         # Snowflake doesn't use indexes.
         return ''
 
     def _model_indexes_sql(self, model):
         return []
```

### Comparing `django-snowflake-4.2a1/django_snowflake/utils.py` & `django-snowflake-4.2b1/django_snowflake/utils.py`

 * *Files identical despite different names*

### Comparing `django-snowflake-4.2a1/django_snowflake.egg-info/SOURCES.txt` & `django-snowflake-4.2b1/django_snowflake.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 django_snowflake/__init__.py
 django_snowflake/base.py
 django_snowflake/client.py
+django_snowflake/compiler.py
 django_snowflake/creation.py
 django_snowflake/features.py
 django_snowflake/functions.py
 django_snowflake/introspection.py
+django_snowflake/lookups.py
 django_snowflake/operations.py
 django_snowflake/schema.py
 django_snowflake/utils.py
 django_snowflake.egg-info/PKG-INFO
 django_snowflake.egg-info/SOURCES.txt
 django_snowflake.egg-info/dependency_links.txt
 django_snowflake.egg-info/requires.txt
```

### Comparing `django-snowflake-4.2a1/setup.cfg` & `django-snowflake-4.2b1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [metadata]
 name = django-snowflake
 version = attr: django_snowflake.__version__
-url = https://github.com/cedar-team/django-snowflake
+url = https://github.com/Snowflake-Labs/django-snowflake
 maintainer = Tim Graham
 maintainer_email = timograham@gmail.com
 license = MIT License
 description = Django backend for Snowflake
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	Framework :: Django
 	Framework :: Django :: 4.2
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 project_urls = 
-	Source = https://github.com/cedar-team/django-snowflake
-	Tracker = https://github.com/cedar-team/django-snowflake/issues
+	Source = https://github.com/Snowflake-Labs/django-snowflake
+	Tracker = https://github.com/Snowflake-Labs/django-snowflake/issues
 
 [options]
 python_requires = >=3.8
 packages = find:
 install_requires = 
 	snowflake-connector-python >= 2.7.4
```

