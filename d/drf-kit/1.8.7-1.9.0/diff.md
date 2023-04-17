# Comparing `tmp/drf-kit-1.8.7.tar.gz` & `tmp/drf-kit-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-kit-1.8.7.tar", max compression
+gzip compressed data, was "drf-kit-1.9.0.tar", max compression
```

## Comparing `drf-kit-1.8.7.tar` & `drf-kit-1.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      322 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/__init__.py
--rw-r--r--   0        0        0     3074 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/cache.py
--rw-r--r--   0        0        0     3694 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/exceptions.py
--rw-r--r--   0        0        0      579 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/fields.py
--rw-r--r--   0        0        0     2554 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/filters.py
--rw-r--r--   0        0        0     1265 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/managers.py
--rw-r--r--   0        0        0     6533 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/models.py
--rw-r--r--   0        0        0     3105 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/pagination.py
--rw-r--r--   0        0        0     2475 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/serializers.py
--rw-r--r--   0        0        0     1053 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/signals.py
--rw-r--r--   0        0        0      994 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/storage.py
--rw-r--r--   0        0        0    11909 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/tests.py
--rw-r--r--   0        0        0     1324 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/views/__init__.py
--rw-r--r--   0        0        0     3731 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/views/nested_viewsets.py
--rw-r--r--   0        0        0     3464 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/views/single_nested_viewsets.py
--rw-r--r--   0        0        0     1145 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/views/stats_views.py
--rw-r--r--   0        0        0     8073 2022-01-04 19:40:41.853929 drf-kit-1.8.7/drf_kit/views/viewsets.py
--rw-r--r--   0        0        0      940 2022-01-04 19:40:41.853929 drf-kit-1.8.7/pyproject.toml
--rw-r--r--   0        0        0      698 2022-01-04 19:40:53.305524 drf-kit-1.8.7/setup.py
--rw-r--r--   0        0        0      485 2022-01-04 19:40:53.305805 drf-kit-1.8.7/PKG-INFO
+-rw-r--r--   0        0        0      322 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/__init__.py
+-rw-r--r--   0        0        0     3074 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/cache.py
+-rw-r--r--   0        0        0     3694 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/exceptions.py
+-rw-r--r--   0        0        0      579 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/fields.py
+-rw-r--r--   0        0        0     2554 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/filters.py
+-rw-r--r--   0        0        0     1265 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/managers.py
+-rw-r--r--   0        0        0     6865 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/models.py
+-rw-r--r--   0        0        0     3105 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/pagination.py
+-rw-r--r--   0        0        0     2475 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/serializers.py
+-rw-r--r--   0        0        0     1053 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/signals.py
+-rw-r--r--   0        0        0      994 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/storage.py
+-rw-r--r--   0        0        0    11909 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/tests.py
+-rw-r--r--   0        0        0     1324 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/views/__init__.py
+-rw-r--r--   0        0        0     3731 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/views/nested_viewsets.py
+-rw-r--r--   0        0        0     3464 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/views/single_nested_viewsets.py
+-rw-r--r--   0        0        0     1145 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/views/stats_views.py
+-rw-r--r--   0        0        0     8073 2022-01-07 16:14:58.641308 drf-kit-1.9.0/drf_kit/views/viewsets.py
+-rw-r--r--   0        0        0      940 2022-01-07 16:14:58.641308 drf-kit-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      698 2022-01-07 16:15:11.420714 drf-kit-1.9.0/setup.py
+-rw-r--r--   0        0        0      485 2022-01-07 16:15:11.421014 drf-kit-1.9.0/PKG-INFO
```

### Comparing `drf-kit-1.8.7/drf_kit/cache.py` & `drf-kit-1.9.0/drf_kit/cache.py`

 * *Files identical despite different names*

### Comparing `drf-kit-1.8.7/drf_kit/exceptions.py` & `drf-kit-1.9.0/drf_kit/exceptions.py`

 * *Files identical despite different names*

### Comparing `drf-kit-1.8.7/drf_kit/fields.py` & `drf-kit-1.9.0/drf_kit/fields.py`

 * *Files identical despite different names*

### Comparing `drf-kit-1.8.7/drf_kit/filters.py` & `drf-kit-1.9.0/drf_kit/filters.py`

 * *Files identical despite different names*

### Comparing `drf-kit-1.8.7/drf_kit/managers.py` & `drf-kit-1.9.0/drf_kit/managers.py`

 * *Files identical despite different names*

### Comparing `drf-kit-1.8.7/drf_kit/models.py` & `drf-kit-1.9.0/drf_kit/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 from pathlib import Path
 
 from django.db import models
-from django.db.models import Max
 from django.forms.models import model_to_dict
 from django.urls import reverse
 from django.utils.timezone import now
 from django.utils.translation import ugettext as _
 from ordered_model.models import OrderedModelBase as _OrderedModelBase
 
 from drf_kit import exceptions, managers, signals
@@ -124,32 +123,41 @@
         null=True,
         blank=True,
         verbose_name=_("order"),
     )
     order_field_name = "order"
 
     def save(self, *args, **kwargs):
-        if getattr(self, self.order_field_name) is None:
-            highest_order = (
-                self.get_ordering_queryset().aggregate(Max(self.order_field_name)).get(self.order_field_name + "__max")
-            )
-            new_order = 0 if highest_order is None else highest_order + 1
-            setattr(self, self.order_field_name, new_order)
-        super().save(*args, **kwargs)
+        if kwargs.pop("ignore_order_validation", False):
+            return super().save(*args, **kwargs)
 
-        new_order = getattr(self, self.order_field_name, None)
-        if not new_order:
-            return
-
-        clash = self.get_ordering_queryset().filter(**{self.order_field_name: new_order}).exclude(pk=self.pk).first()
-        if not clash:
-            return
+        # How to prevent the order indexes from becoming sparse:
+        # 1. Fetch the list of objects of that grouping, except the current item
+        # 2. Insert the current item in the desired index
+        #    a. if the current item does not have a specified index, add to the end
+        #    b. if it does, add to that index
+        # 3. Traverse the list and update each item whose index has changed
+
+        order = getattr(self, self.order_field_name)
+
+        group = list(self.get_ordering_queryset().exclude(id=self.pk))
+
+        if order is not None:  # when updating
+            group.insert(max(0, order), self)
+        else:  # when creating
+            group.append(self)
+
+        for index, obj in enumerate(group):
+            if obj.pk == self.pk:
+                setattr(self, self.order_field_name, index)
+            elif obj.order != index:
+                obj.order = index
+                obj.save(ignore_order_validation=True)
 
-        setattr(clash, self.order_field_name, new_order + 1)
-        clash.save()
+        return super().save(*args, **kwargs)
 
     class Meta:
         abstract = True
         ordering = ("order", "-updated_at")
 
 
 class BaseOrderedModel(OrderedModelMixin, BaseModel):
```

### Comparing `drf-kit-1.8.7/drf_kit/pagination.py` & `drf-kit-1.9.0/drf_kit/pagination.py`

 * *Files identical despite different names*

### Comparing `drf-kit-1.8.7/drf_kit/serializers.py` & `drf-kit-1.9.0/drf_kit/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-kit-1.8.7/drf_kit/signals.py` & `drf-kit-1.9.0/drf_kit/signals.py`

 * *Files identical despite different names*

### Comparing `drf-kit-1.8.7/drf_kit/storage.py` & `drf-kit-1.9.0/drf_kit/storage.py`

 * *Files identical despite different names*

### Comparing `drf-kit-1.8.7/drf_kit/tests.py` & `drf-kit-1.9.0/drf_kit/tests.py`

 * *Files identical despite different names*

### Comparing `drf-kit-1.8.7/drf_kit/views/__init__.py` & `drf-kit-1.9.0/drf_kit/views/__init__.py`

 * *Files identical despite different names*

### Comparing `drf-kit-1.8.7/drf_kit/views/nested_viewsets.py` & `drf-kit-1.9.0/drf_kit/views/nested_viewsets.py`

 * *Files identical despite different names*

### Comparing `drf-kit-1.8.7/drf_kit/views/single_nested_viewsets.py` & `drf-kit-1.9.0/drf_kit/views/single_nested_viewsets.py`

 * *Files identical despite different names*

### Comparing `drf-kit-1.8.7/drf_kit/views/stats_views.py` & `drf-kit-1.9.0/drf_kit/views/stats_views.py`

 * *Files identical despite different names*

### Comparing `drf-kit-1.8.7/drf_kit/views/viewsets.py` & `drf-kit-1.9.0/drf_kit/views/viewsets.py`

 * *Files identical despite different names*

### Comparing `drf-kit-1.8.7/pyproject.toml` & `drf-kit-1.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-kit"
-version = "1.8.7"
+version = "1.9.0"
 description = "DRF Toolkit"
 authors = ["eduK <pd@eduk.com>"]
 packages = [
     { include = "drf_kit" },
 ]
```

### Comparing `drf-kit-1.8.7/setup.py` & `drf-kit-1.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'django-filter>=2,<3',
  'django-ordered-model>=3,<4',
  'djangorestframework>=3,<4',
  'drf-extensions>=0,<1']
 
 setup_kwargs = {
     'name': 'drf-kit',
-    'version': '1.8.7',
+    'version': '1.9.0',
     'description': 'DRF Toolkit',
     'long_description': None,
     'author': 'eduK',
     'author_email': 'pd@eduk.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

