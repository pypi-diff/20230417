# Comparing `tmp/flask-whooshee-0.8.2.tar.gz` & `tmp/flask-whooshee-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-whooshee-0.8.2.tar", last modified: Sun Jan 23 04:43:16 2022, max compression
+gzip compressed data, was "flask-whooshee-0.9.0.tar", last modified: Mon Apr 17 11:34:54 2023, max compression
```

## Comparing `flask-whooshee-0.8.2.tar` & `flask-whooshee-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2022-01-23 04:43:16.362766 flask-whooshee-0.8.2/
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1528 2022-01-13 01:22:25.000000 flask-whooshee-0.8.2/LICENSE
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       75 2022-01-13 01:22:25.000000 flask-whooshee-0.8.2/MANIFEST.in
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1898 2022-01-23 04:43:16.362766 flask-whooshee-0.8.2/PKG-INFO
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1885 2022-01-13 01:22:25.000000 flask-whooshee-0.8.2/README.md
-drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2022-01-23 04:43:16.362766 flask-whooshee-0.8.2/flask_whooshee.egg-info/
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     1898 2022-01-23 04:43:16.000000 flask-whooshee-0.8.2/flask_whooshee.egg-info/PKG-INFO
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      317 2022-01-23 04:43:16.000000 flask-whooshee-0.8.2/flask_whooshee.egg-info/SOURCES.txt
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)        1 2022-01-23 04:43:16.000000 flask-whooshee-0.8.2/flask_whooshee.egg-info/dependency_links.txt
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)        1 2022-01-23 04:43:16.000000 flask-whooshee-0.8.2/flask_whooshee.egg-info/not-zip-safe
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       32 2022-01-23 04:43:16.000000 flask-whooshee-0.8.2/flask_whooshee.egg-info/requires.txt
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       15 2022-01-23 04:43:16.000000 flask-whooshee-0.8.2/flask_whooshee.egg-info/top_level.txt
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)    20760 2022-01-13 01:22:25.000000 flask-whooshee-0.8.2/flask_whooshee.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       52 2022-01-13 01:22:25.000000 flask-whooshee-0.8.2/requirements.txt
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       67 2022-01-23 04:43:16.363766 flask-whooshee-0.8.2/setup.cfg
--rwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)     2279 2022-01-13 01:26:13.000000 flask-whooshee-0.8.2/setup.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)    32704 2022-01-13 01:22:25.000000 flask-whooshee-0.8.2/test.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-17 11:34:54.849385 flask-whooshee-0.9.0/
+-rw-r--r--   0 twine    (17125) twine    (17125)     1528 2021-07-16 08:14:01.000000 flask-whooshee-0.9.0/LICENSE
+-rw-r--r--   0 twine    (17125) twine    (17125)       75 2021-07-16 08:14:01.000000 flask-whooshee-0.9.0/MANIFEST.in
+-rw-r--r--   0 twine    (17125) twine    (17125)     1905 2023-04-17 11:34:54.849385 flask-whooshee-0.9.0/PKG-INFO
+-rw-r--r--   0 twine    (17125) twine    (17125)     1885 2021-07-16 08:14:01.000000 flask-whooshee-0.9.0/README.md
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-17 11:34:54.849385 flask-whooshee-0.9.0/flask_whooshee.egg-info/
+-rw-r--r--   0 twine    (17125) twine    (17125)     1905 2023-04-17 11:34:54.000000 flask-whooshee-0.9.0/flask_whooshee.egg-info/PKG-INFO
+-rw-r--r--   0 twine    (17125) twine    (17125)      332 2023-04-17 11:34:54.000000 flask-whooshee-0.9.0/flask_whooshee.egg-info/SOURCES.txt
+-rw-r--r--   0 twine    (17125) twine    (17125)        1 2023-04-17 11:34:54.000000 flask-whooshee-0.9.0/flask_whooshee.egg-info/dependency_links.txt
+-rw-r--r--   0 twine    (17125) twine    (17125)        1 2021-07-16 08:14:12.000000 flask-whooshee-0.9.0/flask_whooshee.egg-info/not-zip-safe
+-rw-r--r--   0 twine    (17125) twine    (17125)       32 2023-04-17 11:34:54.000000 flask-whooshee-0.9.0/flask_whooshee.egg-info/requires.txt
+-rw-r--r--   0 twine    (17125) twine    (17125)       15 2023-04-17 11:34:54.000000 flask-whooshee-0.9.0/flask_whooshee.egg-info/top_level.txt
+-rw-r--r--   0 twine    (17125) twine    (17125)    20762 2023-04-17 11:34:49.000000 flask-whooshee-0.9.0/flask_whooshee.py
+-rw-r--r--   0 twine    (17125) twine    (17125)       71 2023-04-17 11:34:49.000000 flask-whooshee-0.9.0/pyproject.toml
+-rw-r--r--   0 twine    (17125) twine    (17125)       69 2023-04-17 11:34:49.000000 flask-whooshee-0.9.0/requirements.txt
+-rw-r--r--   0 twine    (17125) twine    (17125)       67 2023-04-17 11:34:54.849385 flask-whooshee-0.9.0/setup.cfg
+-rwxr-xr-x   0 twine    (17125) twine    (17125)     2332 2023-04-17 11:34:49.000000 flask-whooshee-0.9.0/setup.py
+-rw-r--r--   0 twine    (17125) twine    (17125)    32980 2023-04-17 11:34:49.000000 flask-whooshee-0.9.0/test.py
```

### Comparing `flask-whooshee-0.8.2/LICENSE` & `flask-whooshee-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-whooshee-0.8.2/PKG-INFO` & `flask-whooshee-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: flask-whooshee
-Version: 0.8.2
+Version: 0.9.0
 Summary: Flask-SQLAlchemy - Whoosh Integration
 Home-page: https://github.com/bkabrda/flask-whooshee
 Author: Bohuslav "Slavek" Kabrda
 Author-email: bkabrda@redhat.com
-License: BSD
+License: BSD-3-Clause
 Keywords: flask,sqlalchemy,whoosh
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -67,9 +67,7 @@
 
 Links
 `````
 
 * `Documentation <https://flask-whooshee.readthedocs.io>`_
 * `Source Code <https://github.com/bkabrda/flask-whooshee>`_
 * `Issues <https://github.com/bkabrda/flask-whooshee/issues>`_
-
-
```

### Comparing `flask-whooshee-0.8.2/README.md` & `flask-whooshee-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `flask-whooshee-0.8.2/flask_whooshee.egg-info/PKG-INFO` & `flask-whooshee-0.9.0/flask_whooshee.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: flask-whooshee
-Version: 0.8.2
+Version: 0.9.0
 Summary: Flask-SQLAlchemy - Whoosh Integration
 Home-page: https://github.com/bkabrda/flask-whooshee
 Author: Bohuslav "Slavek" Kabrda
 Author-email: bkabrda@redhat.com
-License: BSD
+License: BSD-3-Clause
 Keywords: flask,sqlalchemy,whoosh
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -67,9 +67,7 @@
 
 Links
 `````
 
 * `Documentation <https://flask-whooshee.readthedocs.io>`_
 * `Source Code <https://github.com/bkabrda/flask-whooshee>`_
 * `Issues <https://github.com/bkabrda/flask-whooshee/issues>`_
-
-
```

### Comparing `flask-whooshee-0.8.2/flask_whooshee.py` & `flask-whooshee-0.9.0/flask_whooshee.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from sqlalchemy.sql.annotation import AnnotatedTable, AnnotatedAlias
 
 INSERT_KWD = 'insert'
 UPDATE_KWD = 'update'
 DELETE_KWD = 'delete'
 
 
-__version__ = '0.7.0'
+__version__ = '0.9.0'
 
 
 def _get_app(obj):
     return (getattr(obj, 'app', None) or current_app)
 
 def _get_config(obj):
     return _get_app(obj).extensions['whooshee']
@@ -122,19 +122,19 @@
                 if m.__name__.lower() == uniq.split('_')[0]:
                     attr = getattr(m, uniq.split('_')[1])
 
         search_query = self.filter(attr.in_(res))
 
         if order_by_relevance < 0: # we want all returned rows ordered
             search_query = search_query.order_by(sqlalchemy.sql.expression.case(
-                [(attr == uniq_val, index) for index, uniq_val in enumerate(res)],
+                *[(attr == uniq_val, index) for index, uniq_val in enumerate(res)],
             ))
         elif order_by_relevance > 0: # we want only number of specified rows ordered
             search_query = search_query.order_by(sqlalchemy.sql.expression.case(
-                [(attr == uniq_val, index) for index, uniq_val in enumerate(res) if index < order_by_relevance],
+                *[(attr == uniq_val, index) for index, uniq_val in enumerate(res) if index < order_by_relevance],
                 else_=order_by_relevance
             ))
         else: # no ordering
             pass
 
         return search_query
```

### Comparing `flask-whooshee-0.8.2/setup.py` & `flask-whooshee-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,25 +51,27 @@
 `````
 
 * `Documentation <https://flask-whooshee.readthedocs.io>`_
 * `Source Code <https://github.com/bkabrda/flask-whooshee>`_
 * `Issues <https://github.com/bkabrda/flask-whooshee/issues>`_
 """
 from setuptools import setup
+from flask_whooshee import __version__
+
 
 setup(
     name='flask-whooshee',
-    version='0.8.2',
+    version=__version__,
     description='Flask-SQLAlchemy - Whoosh Integration',
     long_description=__doc__,
     keywords='flask, sqlalchemy, whoosh',
     author='Bohuslav "Slavek" Kabrda',
     author_email='bkabrda@redhat.com',
     url='https://github.com/bkabrda/flask-whooshee',
-    license='BSD',
+    license='BSD-3-Clause',
     py_modules=['flask_whooshee'],
     test_suite='test',
     zip_safe=False,
     platforms='any',
     install_requires=[
         'blinker',
         'Flask-Sqlalchemy',
```

### Comparing `flask-whooshee-0.8.2/test.py` & `flask-whooshee-0.9.0/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from flexmock import flexmock
 import whoosh
 from whoosh.filedb.filestore import RamStorage
 from flask import Flask
 from flask_sqlalchemy import SQLAlchemy, BaseQuery
 from sqlalchemy.orm import Query as SQLAQuery
+from sqlalchemy.sql import text
 from flask_whooshee import AbstractWhoosheer, Whooshee, WhoosheeQuery
 
 
 class BaseTestCases(object):
 
     class BaseTest(TestCase):
 
@@ -27,14 +28,17 @@
             self.app.config['TESTING'] = True
             self.app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
 
             self.db = SQLAlchemy(self.app)
 
         def setUp(self):
 
+            self.ctx = self.app.app_context()
+            self.ctx.push()
+
             class User(self.db.Model):
                 id = self.db.Column(self.db.Integer, primary_key=True)
                 name = self.db.Column(self.db.String)
 
             # separate index for just entry
             @self.wh.register_model('title', 'content')
             class Entry(self.db.Model):
@@ -115,14 +119,15 @@
 
             self.all_inst = [self.u1, self.u2, self.u3, self.e1, self.e2, self.e3, self.e4, self.n1]
 
         def tearDown(self):
             shutil.rmtree(self.app.config['WHOOSHEE_DIR'], ignore_errors=True)
             Whooshee.whoosheers = []
             self.db.drop_all()
+            self.ctx.pop()
 
         # tests testing model whoosheers should have mw in their name, for custom whoosheers it's cw
         # ideally, there should be a separate class for model whoosheer and custom whoosheer
         # but we also want to test how they coexist
 
         def test_nothing_found(self):
             found = self.Entry.query.whooshee_search('not there!').all()
@@ -259,15 +264,15 @@
 
         def test_reindex(self):
             self.db.session.add_all(self.all_inst)
             self.db.session.commit()
             # generall reindex
             self.wh.reindex()
             # put stallone directly in db and find him only after reindex
-            result = self.db.session.execute("INSERT INTO entry VALUES (100, 'rambo', 'pack of one two and three', {0})".format(self.u3.id))
+            result = self.db.session.execute(text("INSERT INTO entry VALUES (100, 'rambo', 'pack of one two and three', {0})".format(self.u3.id)))
             self.db.session.commit()
             found = self.Entry.query.join(self.User).whooshee_search('rambo').all()
             self.assertEqual(len(found), 0)
             self.wh.reindex()
             found = self.Entry.query.join(self.User).whooshee_search('rambo').all()
             self.assertEqual(len(found), 1)
 
@@ -408,35 +413,31 @@
         self.wh = Whooshee()
 
         super(TestsWithInitApp, self).setUp()
         # we intentionally call `init_app` after creating whoosheers, to test that lazy app
         # intialization is possible
         self.wh.init_app(self.app)
 
-        self.ctx = self.app.app_context()
-        self.ctx.push()
-
-    def tearDown(self):
-        super(TestsWithInitApp, self).tearDown()
-        self.ctx.pop()
-
 
 class TestsAppWithMemoryStorage(TestCase):
 
     def setUp(self):
         self.app = Flask(__name__)
 
         self.app.config['WHOOSHEE_MEMORY_STORAGE'] = True
         self.app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite://'
         self.app.config['TESTING'] = True
         self.app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
 
         self.db = SQLAlchemy(self.app)
         self.wh = Whooshee(self.app)
 
+        self.ctx = self.app.app_context()
+        self.ctx.push()
+
         class User(self.db.Model):
             id = self.db.Column(self.db.Integer, primary_key=True)
             name = self.db.Column(self.db.String)
 
         # separate index for just entry
         @self.wh.register_model('title', 'content')
         class Entry(self.db.Model):
@@ -492,15 +493,15 @@
             def delete_entry(cls, writer, entry):
                 writer.delete_by_term('entry_id', entry.id)
 
         self.User = User
         self.Entry = Entry
         self.EntryUserWhoosheer = EntryUserWhoosheer
 
-        self.db.create_all(app=self.app)
+        self.db.create_all()
 
         self.u1 = User(name=u'chuck')
         self.u2 = User(name=u'arnold')
         self.u3 = User(name=u'silvester')
 
         self.e1 = Entry(title=u'chuck nr. 1 article', content=u'blah blah blah', user=self.u1)
         self.e2 = Entry(title=u'norris nr. 2 article', content=u'spam spam spam', user=self.u1)
@@ -508,34 +509,39 @@
         self.e4 = Entry(title=u'the less dangerous', content=u'chuck is better', user=self.u3)
 
         self.all_inst = [self.u1, self.u2, self.u3, self.e1, self.e2, self.e3, self.e4]
         self.db.session.add_all(self.all_inst)
         self.db.session.commit()
 
     def tearDown(self):
-        self.db.drop_all(app=self.app)
+        self.db.drop_all()
+        self.ctx.pop()
 
     def test_memory_storage(self):
         indexes = self.app.extensions['whooshee']['whoosheers_indexes']
         self.assertTrue(isinstance(indexes[self.EntryUserWhoosheer].storage, RamStorage))
 
 
 class TestBigInteger(TestCase):
+    # pylint: disable=too-many-instance-attributes
 
     def setUp(self):
         self.app = Flask(__name__)
 
         self.app.config['WHOOSHEE_MEMORY_STORAGE'] = True
         self.app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite://'
         self.app.config['TESTING'] = True
         self.app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
 
         self.db = SQLAlchemy(self.app)
         self.wh = Whooshee(self.app)
 
+        self.ctx = self.app.app_context()
+        self.ctx.push()
+
         class User(self.db.Model):
             id = self.db.Column(self.db.Integer, primary_key=True)
             name = self.db.Column(self.db.String)
 
         # Need to make sure BigInteger PK's can be created
         @self.wh.register_model('title', 'content')
         class Entry(self.db.Model):
@@ -544,23 +550,24 @@
             content = self.db.Column(self.db.Text)
             user = self.db.relationship(User, backref = self.db.backref('entries'))
             user_id = self.db.Column(self.db.Integer, self.db.ForeignKey('user.id'))
 
         self.User = User
         self.Entry = Entry
 
-        self.db.create_all(app=self.app)
+        self.db.create_all()
 
         self.u1 = User(name=u'chuck')
         self.e1 = Entry(id=1000000000000, title=u'chuck nr. 1 article', content=u'blah blah blah', user=self.u1)
 
         self.db.session.commit()
 
     def tearDown(self):
-        self.db.drop_all(app=self.app)
+        self.db.drop_all()
+        self.ctx.pop()
 
     def test_add(self):
             # test that the add operation works for Big Integer PK
             found = self.Entry.query.whooshee_search('blah blah blah').all()
             self.assertEqual(len(found), 0)
 
             self.db.session.add(self.e1)
@@ -642,16 +649,19 @@
             def delete_entry(cls, writer, entry):
                 writer.delete_by_term('entry_id', entry.id)
 
         self.User = User
         self.Entry = Entry
         self.EntryUserWhoosheer = EntryUserWhoosheer
 
-        self.db.create_all(app=self.app1)
-        self.db.create_all(app=self.app2)
+        with self.app1.app_context():
+            self.db.create_all()
+
+        with self.app2.app_context():
+            self.db.create_all()
 
         self.u1 = User(name=u'chuck')
         self.u2 = User(name=u'arnold')
         self.u3 = User(name=u'silvester')
 
         self.e1 = Entry(title=u'chuck nr. 1 article', content=u'blah blah blah', user=self.u1)
         self.e2 = Entry(title=u'norris nr. 2 article', content=u'spam spam spam', user=self.u1)
@@ -659,16 +669,18 @@
         self.e4 = Entry(title=u'the less dangerous', content=u'chuck is better', user=self.u3)
 
         self.all_inst = [self.u1, self.u2, self.u3, self.e1, self.e2, self.e3, self.e4]
 
     def tearDown(self):
         shutil.rmtree(self.app1.config['WHOOSHEE_DIR'], ignore_errors=True)
         shutil.rmtree(self.app2.config['WHOOSHEE_DIR'], ignore_errors=True)
-        self.db.drop_all(app=self.app1)
-        self.db.drop_all(app=self.app2)
+        with self.app1.app_context():
+            self.db.drop_all()
+        with self.app2.app_context():
+            self.db.drop_all()
 
     def test_multiple_apps(self):
         # IIUC, you can't add the same model instance under multiple apps with flask-sqlalchemy
         #  this pretty much reduces the testing to "make sure we used the right app to do
         #  the search"
         with self.app1.test_request_context():
             self.db.session.add_all([self.u2, self.u3, self.e3, self.e4])
```

