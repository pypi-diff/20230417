# Comparing `tmp/axdd-person-client-1.1.0.tar.gz` & `tmp/axdd-person-client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axdd-person-client-1.1.0.tar", last modified: Wed Jan  4 20:47:36 2023, max compression
+gzip compressed data, was "axdd-person-client-1.1.1.tar", last modified: Mon Apr 17 17:17:07 2023, max compression
```

## Comparing `axdd-person-client-1.1.0.tar` & `axdd-person-client-1.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-04 20:47:36.928136 axdd-person-client-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-01-04 20:47:36.928136 axdd-person-client-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-04 20:47:36.924136 axdd-person-client-1.1.0/axdd_person_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-01-04 20:47:36.000000 axdd-person-client-1.1.0/axdd_person_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-01-04 20:47:36.000000 axdd-person-client-1.1.0/axdd_person_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-04 20:47:36.000000 axdd-person-client-1.1.0/axdd_person_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-01-04 20:47:36.000000 axdd-person-client-1.1.0/axdd_person_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-01-04 20:47:36.000000 axdd-person-client-1.1.0/axdd_person_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-04 20:47:36.924136 axdd-person-client-1.1.0/conf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/conf/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-04 20:47:36.928136 axdd-person-client-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-04 20:47:36.924136 axdd-person-client-1.1.0/uw_person_client/
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/uw_person_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-04 20:47:36.924136 axdd-person-client-1.1.0/uw_person_client/clients/
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/uw_person_client/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24861 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/uw_person_client/clients/core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/uw_person_client/clients/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/uw_person_client/components.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-04 20:47:36.924136 axdd-person-client-1.1.0/uw_person_client/databases/
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/uw_person_client/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/uw_person_client/databases/postgres.py
--rw-r--r--   0 runner    (1001) docker     (122)     6164 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/uw_person_client/databases/uwpds.py
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/uw_person_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/uw_person_client/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-04 20:47:36.928136 axdd-person-client-1.1.0/uw_person_client/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/uw_person_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/uw_person_client/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (122)    33872 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/uw_person_client/tests/test_core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-01-04 20:47:29.000000 axdd-person-client-1.1.0/uw_person_client/tests/test_mock_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 17:17:07.461833 axdd-person-client-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-04-17 17:17:07.461833 axdd-person-client-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 17:17:07.453833 axdd-person-client-1.1.1/axdd_person_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-04-17 17:17:07.000000 axdd-person-client-1.1.1/axdd_person_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-04-17 17:17:07.000000 axdd-person-client-1.1.1/axdd_person_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 17:17:07.000000 axdd-person-client-1.1.1/axdd_person_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-04-17 17:17:07.000000 axdd-person-client-1.1.1/axdd_person_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-17 17:17:07.000000 axdd-person-client-1.1.1/axdd_person_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 17:17:07.457833 axdd-person-client-1.1.1/conf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/conf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-17 17:17:07.461833 axdd-person-client-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 17:17:07.457833 axdd-person-client-1.1.1/uw_person_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/uw_person_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 17:17:07.457833 axdd-person-client-1.1.1/uw_person_client/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/uw_person_client/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24666 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/uw_person_client/clients/core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/uw_person_client/clients/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/uw_person_client/components.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 17:17:07.457833 axdd-person-client-1.1.1/uw_person_client/databases/
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/uw_person_client/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/uw_person_client/databases/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5633 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/uw_person_client/databases/uwpds.py
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/uw_person_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/uw_person_client/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 17:17:07.457833 axdd-person-client-1.1.1/uw_person_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/uw_person_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/uw_person_client/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33684 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/uw_person_client/tests/test_core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-04-17 17:16:54.000000 axdd-person-client-1.1.1/uw_person_client/tests/test_mock_client.py
```

### Comparing `axdd-person-client-1.1.0/LICENSE` & `axdd-person-client-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.0/PKG-INFO` & `axdd-person-client-1.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.0
+Version: 1.1.1
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.0/README.md` & `axdd-person-client-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.0/axdd_person_client.egg-info/PKG-INFO` & `axdd-person-client-1.1.1/axdd_person_client.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.0
+Version: 1.1.1
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.0/axdd_person_client.egg-info/SOURCES.txt` & `axdd-person-client-1.1.1/axdd_person_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.0/conf/settings.py` & `axdd-person-client-1.1.1/conf/settings.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.0/setup.py` & `axdd-person-client-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.0/uw_person_client/clients/__init__.py` & `axdd-person-client-1.1.1/uw_person_client/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.0/uw_person_client/clients/core_client.py` & `axdd-person-client-1.1.1/uw_person_client/clients/core_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright 2023 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
 
+from sqlalchemy import or_
 from sqlalchemy.orm.exc import NoResultFound
 from uw_person_client.clients import AbstractUWPersonClient
 from uw_person_client.databases.uwpds import UWPDS
 from uw_person_client.exceptions import (
     PersonNotFoundException, AdviserNotFoundException)
 from uw_person_client.components import (
     Person, Student, Employee, Transcript, Major, Sport, Adviser, Term,
@@ -18,23 +19,27 @@
     Public methods
     """
 
     def __init__(self):
         self.DB = UWPDS()
 
     def get_person_by_uwnetid(self, uwnetid, **kwargs):
-        sqla_person = self.DB.session.query(self.DB.HistoricalPerson).filter(
-            self.DB.HistoricalPerson.prior_uwnetid == uwnetid).first()
+        sqla_person = self.DB.session.query(self.DB.Person).filter(
+            or_(self.DB.Person.uwnetid == uwnetid,
+                self.DB.Person.prior_uwnetids.any(uwnetid))
+        ).one_or_none()
         if sqla_person is None:
             raise PersonNotFoundException()
         return self._map_person(sqla_person, **kwargs)
 
     def get_person_by_uwregid(self, uwregid, **kwargs):
-        sqla_person = self.DB.session.query(self.DB.HistoricalPerson).filter(
-            self.DB.HistoricalPerson.prior_uwregid == uwregid).first()
+        sqla_person = self.DB.session.query(self.DB.Person).filter(
+            or_(self.DB.Person.uwregid == uwregid,
+                self.DB.Person.prior_uwregids.any(uwregid))
+        ).one_or_none()
         if sqla_person is None:
             raise PersonNotFoundException()
         return self._map_person(sqla_person, **kwargs)
 
     def get_person_by_student_number(self, student_number, **kwargs):
         sqla_person = self.DB.session.query(self.DB.Person).join(
             self.DB.Student).filter(
@@ -123,28 +128,23 @@
                     include_student_sports=True,
                     include_student_advisers=True,
                     include_student_majors=True,
                     include_student_pending_majors=True):
         person = Person()
         person.uwnetid = sqla_person.uwnetid
         person.uwregid = sqla_person.uwregid
-        prior_uwnetids = self.DB.session.query(self.DB.PriorUWNetID).filter(
-            self.DB.PriorUWNetID.person_id == sqla_person.id).all()
-        person.prior_uwnetids = [pni.uwnetid for pni in prior_uwnetids]
-        prior_uwregids = self.DB.session.query(self.DB.PriorUWRegID).filter(
-            self.DB.PriorUWRegID.person_id == sqla_person.id).all()
-        person.prior_uwregids = [pri.uwregid for pri in prior_uwregids]
+        person.prior_uwnetids = sqla_person.prior_uwnetids
+        person.prior_uwregids = sqla_person.prior_uwregids
         person.pronouns = sqla_person.pronouns
         person.full_name = sqla_person.full_name
         person.display_name = sqla_person.display_name
         person.first_name = sqla_person.first_name
         person.surname = sqla_person.surname
         person.preferred_first_name = sqla_person.preferred_first_name
-        person.preferred_middle_name = \
-            sqla_person.preferred_middle_name
+        person.preferred_middle_name = sqla_person.preferred_middle_name
         person.preferred_surname = sqla_person.preferred_surname
         person.whitepages_publish = sqla_person.whitepages_publish
         person.active_student = sqla_person._is_active_student
         person.active_employee = sqla_person._is_active_employee
 
         if include_student:
             try:
```

### Comparing `axdd-person-client-1.1.0/uw_person_client/clients/mock_client.py` & `axdd-person-client-1.1.1/uw_person_client/clients/mock_client.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.0/uw_person_client/components.py` & `axdd-person-client-1.1.1/uw_person_client/components.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.0/uw_person_client/databases/__init__.py` & `axdd-person-client-1.1.1/uw_person_client/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.0/uw_person_client/databases/postgres.py` & `axdd-person-client-1.1.1/uw_person_client/databases/postgres.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.0/uw_person_client/databases/uwpds.py` & `axdd-person-client-1.1.1/uw_person_client/databases/uwpds.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,17 +15,14 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # only map the database once
         if len(UWPDS.Base.classes) == 0:
             self.initialize_relationships()
         # person classes
         self.Person = UWPDS.Base.classes.person
-        self.HistoricalPerson = UWPDS.Base.classes.historical_person
-        self.PriorUWNetID = UWPDS.Base.classes.prior_uwnetids
-        self.PriorUWRegID = UWPDS.Base.classes.prior_uwregids
         # employee classes
         self.Employee = UWPDS.Base.classes.employee
         self.Adviser = UWPDS.Base.classes.adviser
         # student classes
         self.Student = UWPDS.Base.classes.student
         self.Major = UWPDS.Base.classes.major
         self.Sport = UWPDS.Base.classes.sport
@@ -46,24 +43,14 @@
         student_to_adviser = Table(
             'student_to_adviser',
             UWPDS.Base.metadata,
             autoload=True,
             autoload_with=self.engine
         )
 
-        Table(
-            'historical_person',
-            UWPDS.Base.metadata,
-            Column('prior_uwnetid', TEXT(), primary_key=True),
-            Column('prior_uwregid', TEXT(), primary_key=True),
-            Column('id', Integer(), primary_key=True),
-            autoload=True,
-            autoload_with=self.engine
-        )
-
         class Student(UWPDS.Base):
             __tablename__ = "student"
             __table_args__ = {'extend_existing': True}
             sport = relationship("sport",
                                  secondary=student_to_sport,
                                  viewonly=True)
             adviser = relationship("adviser",
```

### Comparing `axdd-person-client-1.1.0/uw_person_client/tests/test_core_client.py` & `axdd-person-client-1.1.1/uw_person_client/tests/test_core_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,61 +18,57 @@
     @patch('uw_person_client.clients.core_client.UWPDS')
     def get_mock_person_client(self, mock_uwpds):
         client = UWPersonClient()
         client.DB = mock_uwpds.return_value
         return client
 
     @patch('uw_person_client.clients.core_client.UWPersonClient._map_person')
-    def test_get_person_by_uwnetid(self, mock_map_person):
+    @patch('uw_person_client.clients.core_client.or_')
+    def test_get_person_by_uwnetid(self, mock_or, mock_map_person):
         client = self.get_mock_person_client()
         # person exists
         mock_person = MagicMock()
-        mock_netid = 'test',
+        mock_netid = 'test'
         client.DB.session.query.return_value.filter.return_value.first = \
             MagicMock(return_value=mock_person)
 
         return_value = client.get_person_by_uwnetid(mock_netid, arg1='arg1')
         # assertions
-        client.DB.session.query.assert_called_once_with(
-            client.DB.HistoricalPerson)
-        client.DB.session.query.return_value.filter.assert_called_once_with(
-            client.DB.HistoricalPerson.prior_uwnetid == mock_netid)
-        client.DB.session.query.return_value.filter.return_value.first.\
+        client.DB.session.query.assert_called_once_with(client.DB.Person)
+        client.DB.session.query.return_value.filter.return_value.one_or_none.\
             assert_called_once()
         self.assertEqual(
             return_value, mock_map_person(mock_person, arg1='arg1'))
 
         # no person found
-        client.DB.session.query.return_value.filter.return_value.first = \
+        client.DB.session.query.return_value.filter.return_value.one_or_none =\
             MagicMock(return_value=None)
         with self.assertRaises(PersonNotFoundException):
             client.get_person_by_uwnetid(mock_netid)
 
     @patch('uw_person_client.clients.core_client.UWPersonClient._map_person')
-    def test_get_person_by_uwregid(self, mock_map_person):
+    @patch('uw_person_client.clients.core_client.or_')
+    def test_get_person_by_uwregid(self, mock_or, mock_map_person):
         client = self.get_mock_person_client()
         # person exists
         mock_person = MagicMock()
-        mock_regid = 'test',
+        mock_regid = 'test'
         client.DB.session.query.return_value.filter.return_value.first = \
             MagicMock(return_value=mock_person)
 
         return_value = client.get_person_by_uwregid(mock_regid, arg1='arg1')
         # assertions
-        client.DB.session.query.assert_called_once_with(
-            client.DB.HistoricalPerson)
-        client.DB.session.query.return_value.filter.assert_called_once_with(
-            client.DB.HistoricalPerson.prior_uwregid == mock_regid)
-        client.DB.session.query.return_value.filter.return_value.first.\
+        client.DB.session.query.assert_called_once_with(client.DB.Person)
+        client.DB.session.query.return_value.filter.return_value.one_or_none.\
             assert_called_once()
         self.assertEqual(
             return_value, mock_map_person(mock_person, arg1='arg1'))
 
         # no person found
-        client.DB.session.query.return_value.filter.return_value.first = \
+        client.DB.session.query.return_value.filter.return_value.one_or_none =\
             MagicMock(return_value=None)
         with self.assertRaises(PersonNotFoundException):
             client.get_person_by_uwregid(mock_regid)
 
     @patch('uw_person_client.clients.core_client.UWPersonClient._map_person')
     def test_get_person_by_student_number(self, mock_map_person):
         client = self.get_mock_person_client()
```

### Comparing `axdd-person-client-1.1.0/uw_person_client/tests/test_mock_client.py` & `axdd-person-client-1.1.1/uw_person_client/tests/test_mock_client.py`

 * *Files identical despite different names*

