# Comparing `tmp/adapter-client-1.0.1.tar.gz` & `tmp/adapter-client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapter-client-1.0.1.tar", last modified: Wed Aug 10 13:21:39 2022, max compression
+gzip compressed data, was "adapter-client-1.1.0.tar", last modified: Mon Apr 17 05:19:00 2023, max compression
```

## Comparing `adapter-client-1.0.1.tar` & `adapter-client-1.1.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 13:21:39.854065 adapter-client-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      290 2022-07-22 09:13:24.000000 adapter-client-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4146 2022-08-10 13:21:39.854065 adapter-client-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3243 2022-07-22 09:13:24.000000 adapter-client-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 13:21:39.835065 adapter-client-1.0.1/requirements/
--rw-r--r--   0 root         (0) root         (0)      112 2022-07-22 09:13:24.000000 adapter-client-1.0.1/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-22 09:13:24.000000 adapter-client-1.0.1/requirements/prod.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-10 13:21:39.854065 adapter-client-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2431 2022-07-22 09:13:24.000000 adapter-client-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 13:21:39.833065 adapter-client-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 13:21:39.838065 adapter-client-1.0.1/src/adapter_client/
--rw-r--r--   0 root         (0) root         (0)       70 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 13:21:39.840065 adapter-client-1.0.1/src/adapter_client/adapters/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/adapters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3709 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/adapters/base.py
--rw-r--r--   0 root         (0) root         (0)     9914 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/adapters/db.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 13:21:39.841065 adapter-client-1.0.1/src/adapter_client/adapters/smev/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/adapters/smev/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8489 2022-08-10 13:21:26.000000 adapter-client-1.0.1/src/adapter_client/adapters/smev/adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 13:21:39.843065 adapter-client-1.0.1/src/adapter_client/adapters/smev/interfaces/
--rw-r--r--   0 root         (0) root         (0)       95 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/adapters/smev/interfaces/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1621 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/adapters/smev/interfaces/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 13:21:39.844065 adapter-client-1.0.1/src/adapter_client/adapters/smev/interfaces/soap/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/adapters/smev/interfaces/soap/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12607 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/adapters/smev/interfaces/soap/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 13:21:39.847065 adapter-client-1.0.1/src/adapter_client/adapters/smev/interfaces/soap/schema/
--rw-r--r--   0 root         (0) root         (0)     8513 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl
--rw-r--r--   0 root         (0) root         (0)     4627 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd
--rw-r--r--   0 root         (0) root         (0)    56967 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 13:21:39.850065 adapter-client-1.0.1/src/adapter_client/adapters/smev/services/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/adapters/smev/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)      301 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/adapters/smev/services/base.py
--rw-r--r--   0 root         (0) root         (0)     1501 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/adapters/smev/services/registry.py
--rw-r--r--   0 root         (0) root         (0)     3606 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/apps.py
--rw-r--r--   0 root         (0) root         (0)      961 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 13:21:39.850065 adapter-client-1.0.1/src/adapter_client/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 13:21:39.851065 adapter-client-1.0.1/src/adapter_client/core/domain/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/core/domain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7973 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/core/domain/model.py
--rw-r--r--   0 root         (0) root         (0)      286 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/core/services.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 13:21:39.853065 adapter-client-1.0.1/src/adapter_client/migrations/
--rw-r--r--   0 root         (0) root         (0)     7165 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6523 2022-07-22 09:13:24.000000 adapter-client-1.0.1/src/adapter_client/models.py
--rw-r--r--   0 root         (0) root         (0)     4895 2022-08-10 13:21:26.000000 adapter-client-1.0.1/src/adapter_client/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 13:21:39.839065 adapter-client-1.0.1/src/adapter_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4146 2022-08-10 13:21:39.000000 adapter-client-1.0.1/src/adapter_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1515 2022-08-10 13:21:39.000000 adapter-client-1.0.1/src/adapter_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-08-10 13:21:39.000000 adapter-client-1.0.1/src/adapter_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2022-08-10 13:21:39.000000 adapter-client-1.0.1/src/adapter_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-08-10 13:21:39.000000 adapter-client-1.0.1/src/adapter_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      450 2022-08-10 13:21:39.000000 adapter-client-1.0.1/version.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.784935 adapter-client-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      290 2022-07-22 09:13:24.000000 adapter-client-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4146 2023-04-17 05:19:00.784935 adapter-client-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3243 2022-07-22 09:13:24.000000 adapter-client-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.761935 adapter-client-1.1.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)      112 2023-04-17 05:18:46.000000 adapter-client-1.1.0/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-07-22 09:13:24.000000 adapter-client-1.1.0/requirements/prod.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 05:19:00.784935 adapter-client-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2431 2022-07-22 09:13:24.000000 adapter-client-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.758935 adapter-client-1.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.764935 adapter-client-1.1.0/src/adapter_client/
+-rw-r--r--   0 root         (0) root         (0)       70 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.766935 adapter-client-1.1.0/src/adapter_client/adapters/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/base.py
+-rw-r--r--   0 root         (0) root         (0)     9914 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/db.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.768935 adapter-client-1.1.0/src/adapter_client/adapters/smev/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8563 2023-04-17 05:18:46.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.770935 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/
+-rw-r--r--   0 root         (0) root         (0)       95 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.771935 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12607 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.774935 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/schema/
+-rw-r--r--   0 root         (0) root         (0)     8513 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl
+-rw-r--r--   0 root         (0) root         (0)     4627 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd
+-rw-r--r--   0 root         (0) root         (0)    56967 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.777935 adapter-client-1.1.0/src/adapter_client/adapters/smev/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      301 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/services/base.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/services/registry.py
+-rw-r--r--   0 root         (0) root         (0)     3606 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/apps.py
+-rw-r--r--   0 root         (0) root         (0)      961 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.781935 adapter-client-1.1.0/src/adapter_client/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.781935 adapter-client-1.1.0/src/adapter_client/core/domain/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/core/domain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7973 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/core/domain/model.py
+-rw-r--r--   0 root         (0) root         (0)      286 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/core/services.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.783935 adapter-client-1.1.0/src/adapter_client/migrations/
+-rw-r--r--   0 root         (0) root         (0)     7165 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6597 2023-04-17 05:18:46.000000 adapter-client-1.1.0/src/adapter_client/models.py
+-rw-r--r--   0 root         (0) root         (0)     4899 2023-04-17 05:18:46.000000 adapter-client-1.1.0/src/adapter_client/tasks.py
+-rw-r--r--   0 root         (0) root         (0)      574 2023-04-17 05:18:46.000000 adapter-client-1.1.0/src/adapter_client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.765935 adapter-client-1.1.0/src/adapter_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4146 2023-04-17 05:19:00.000000 adapter-client-1.1.0/src/adapter_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-04-17 05:19:00.000000 adapter-client-1.1.0/src/adapter_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-17 05:19:00.000000 adapter-client-1.1.0/src/adapter_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-04-17 05:19:00.000000 adapter-client-1.1.0/src/adapter_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-17 05:19:00.000000 adapter-client-1.1.0/src/adapter_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      450 2023-04-17 05:19:00.000000 adapter-client-1.1.0/version.conf
```

### Comparing `adapter-client-1.0.1/PKG-INFO` & `adapter-client-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapter-client
-Version: 1.0.1
+Version: 1.1.0
 Summary: Клиент для взаимодействия со СМЭВ3 посредством Адаптера
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
```

### Comparing `adapter-client-1.0.1/README.md` & `adapter-client-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `adapter-client-1.0.1/setup.py` & `adapter-client-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.0.1/src/adapter_client/adapters/base.py` & `adapter-client-1.1.0/src/adapter_client/adapters/base.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.0.1/src/adapter_client/adapters/db.py` & `adapter-client-1.1.0/src/adapter_client/adapters/db.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.0.1/src/adapter_client/adapters/smev/adapter.py` & `adapter-client-1.1.0/src/adapter_client/adapters/smev/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from django.utils.module_loading import import_string
 
 from adapter_client.adapters.smev.interfaces.base import ExchangeResult
 from adapter_client.adapters.smev.services.base import AbstractService
 from adapter_client.adapters.smev.services.registry import ServiceRegistry
 from adapter_client.core.domain import model
+from adapter_client.utils import close_connections
 
 from ..base import AbstractIncomingMessageRepository
 from ..base import AbstractJournal
 from ..base import AbstractOutgoingMessageRepository
 from ..db import config_repository
 from .interfaces.base import AbstractInterface
 
@@ -149,14 +150,15 @@
     def _enqueue_message(self, message: model.Message):
         """Добавление исходящего сообщения в очередь"""
         assert message.id is None
         self._outgoing_message_repository.add(
             model.OutgoingMessage(message=message)
         )
 
+    @close_connections
     def _process_exchange_result(
         self,
         exchange_result: ExchangeResult
     ) -> ExchangeResult:
         """
         Добавление и попытка обработки входящего сообщения из ExchangeResult.
         """
```

### Comparing `adapter-client-1.0.1/src/adapter_client/adapters/smev/interfaces/base.py` & `adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.0.1/src/adapter_client/adapters/smev/interfaces/soap/interface.py` & `adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/interface.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.0.1/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl` & `adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl`

 * *Files identical despite different names*

### Comparing `adapter-client-1.0.1/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd` & `adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd`

 * *Files identical despite different names*

### Comparing `adapter-client-1.0.1/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd` & `adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd`

 * *Files identical despite different names*

### Comparing `adapter-client-1.0.1/src/adapter_client/adapters/smev/services/registry.py` & `adapter-client-1.1.0/src/adapter_client/adapters/smev/services/registry.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.0.1/src/adapter_client/apps.py` & `adapter-client-1.1.0/src/adapter_client/apps.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.0.1/src/adapter_client/config.py` & `adapter-client-1.1.0/src/adapter_client/config.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.0.1/src/adapter_client/core/domain/model.py` & `adapter-client-1.1.0/src/adapter_client/core/domain/model.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.0.1/src/adapter_client/migrations/0001_initial.py` & `adapter-client-1.1.0/src/adapter_client/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.0.1/src/adapter_client/models.py` & `adapter-client-1.1.0/src/adapter_client/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # coding: utf-8
-from django.contrib.postgres.fields import JSONField
+
+try:
+    from django.db.models import JSONField
+except ImportError:
+    from django.contrib.postgres.fields import JSONField
+
 from django.core.validators import MaxValueValidator
 from django.core.validators import MinValueValidator
 from django.db import models
 from django.db.models.signals import post_save
 from django.dispatch.dispatcher import receiver
 
 from adapter_client.core.domain import model
```

### Comparing `adapter-client-1.0.1/src/adapter_client/tasks.py` & `adapter-client-1.1.0/src/adapter_client/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,14 @@
         (ProcessTask, config.find_request_retry_time),
     ):
         schedule, _ = IntervalSchedule.objects.get_or_create(
             every=retry_time,
             period=IntervalSchedule.SECONDS,
         )
         task_name = get_full_qualname(task_cls)
-        task = PeriodicTask.objects.update_or_create(
+        task, *_ = PeriodicTask.objects.update_or_create(
             task=task_name, name=task_name,
             defaults={'interval': schedule}
         )
         PeriodicTasks.changed(task)
 
     logger.info('Periodic tasks configured')
```

### Comparing `adapter-client-1.0.1/src/adapter_client.egg-info/PKG-INFO` & `adapter-client-1.1.0/src/adapter_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapter-client
-Version: 1.0.1
+Version: 1.1.0
 Summary: Клиент для взаимодействия со СМЭВ3 посредством Адаптера
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
```

### Comparing `adapter-client-1.0.1/src/adapter_client.egg-info/SOURCES.txt` & `adapter-client-1.1.0/src/adapter_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 requirements/base.txt
 requirements/prod.txt
 src/adapter_client/__init__.py
 src/adapter_client/apps.py
 src/adapter_client/config.py
 src/adapter_client/models.py
 src/adapter_client/tasks.py
+src/adapter_client/utils.py
 src/adapter_client.egg-info/PKG-INFO
 src/adapter_client.egg-info/SOURCES.txt
 src/adapter_client.egg-info/dependency_links.txt
 src/adapter_client.egg-info/requires.txt
 src/adapter_client.egg-info/top_level.txt
 src/adapter_client/adapters/__init__.py
 src/adapter_client/adapters/base.py
```

