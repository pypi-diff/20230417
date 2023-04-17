# Comparing `tmp/django-pictures-1.0rc4.tar.gz` & `tmp/django-pictures-1.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pictures-1.0rc4.tar", last modified: Thu Sep 29 16:12:49 2022, max compression
+gzip compressed data, was "django-pictures-1.0rc5.tar", last modified: Thu Oct 27 08:43:18 2022, max compression
```

## Comparing `django-pictures-1.0rc4.tar` & `django-pictures-1.0rc5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1324 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/LICENSE
--rw-r--r--   0        0        0     6705 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/README.md
--rw-r--r--   0        0        0      171 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/__init__.py
--rw-r--r--   0        0        0      174 2022-09-29 16:12:49.935465 django-pictures-1.0rc4/pictures/_version.py
--rw-r--r--   0        0        0      155 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/apps.py
--rw-r--r--   0        0        0     1012 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/checks.py
--rw-r--r--   0        0        0      624 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/conf.py
--rw-r--r--   0        0        0        0 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/contrib/__init__.py
--rw-r--r--   0        0        0      544 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/contrib/rest_framework.py
--rw-r--r--   0        0        0      857 2022-09-29 16:12:35.127437 django-pictures-1.0rc4/pictures/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1179 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3195 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/migrations.py
--rw-r--r--   0        0        0     8040 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/models.py
--rw-r--r--   0        0        0     3726 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/tasks.py
--rw-r--r--   0        0        0      165 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/templates/pictures/attrs.html
--rw-r--r--   0        0        0      537 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/templates/pictures/picture.html
--rw-r--r--   0        0        0        0 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/templatetags/__init__.py
--rw-r--r--   0        0        0     1996 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/templatetags/pictures.py
--rw-r--r--   0        0        0      214 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/urls.py
--rw-r--r--   0        0        0     3695 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/utils.py
--rw-r--r--   0        0        0     1907 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/validators.py
--rw-r--r--   0        0        0      725 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pictures/views.py
--rw-r--r--   0        0        0     2073 2022-09-29 16:12:17.491409 django-pictures-1.0rc4/pyproject.toml
--rw-r--r--   0        0        0     8518 1970-01-01 00:00:00.000000 django-pictures-1.0rc4/PKG-INFO
+-rw-r--r--   0        0        0     1324 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/LICENSE
+-rw-r--r--   0        0        0     8619 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/README.md
+-rw-r--r--   0        0        0      171 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/__init__.py
+-rw-r--r--   0        0        0      174 2022-10-27 08:43:17.999077 django-pictures-1.0rc5/pictures/_version.py
+-rw-r--r--   0        0        0      155 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/apps.py
+-rw-r--r--   0        0        0     1012 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/checks.py
+-rw-r--r--   0        0        0      624 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/conf.py
+-rw-r--r--   0        0        0        0 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/contrib/__init__.py
+-rw-r--r--   0        0        0     2050 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/contrib/rest_framework.py
+-rw-r--r--   0        0        0      857 2022-10-27 08:43:02.170796 django-pictures-1.0rc5/pictures/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1179 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3195 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/migrations.py
+-rw-r--r--   0        0        0     8040 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/models.py
+-rw-r--r--   0        0        0     3726 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/tasks.py
+-rw-r--r--   0        0        0      165 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/templates/pictures/attrs.html
+-rw-r--r--   0        0        0      537 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/templates/pictures/picture.html
+-rw-r--r--   0        0        0        0 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/templatetags/__init__.py
+-rw-r--r--   0        0        0     2001 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/templatetags/pictures.py
+-rw-r--r--   0        0        0      214 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/urls.py
+-rw-r--r--   0        0        0     3695 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/utils.py
+-rw-r--r--   0        0        0     1907 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/validators.py
+-rw-r--r--   0        0        0      725 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/views.py
+-rw-r--r--   0        0        0     2278 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pyproject.toml
+-rw-r--r--   0        0        0    10667 1970-01-01 00:00:00.000000 django-pictures-1.0rc5/PKG-INFO
```

### Comparing `django-pictures-1.0rc4/LICENSE` & `django-pictures-1.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc4/README.md` & `django-pictures-1.0rc5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-# django-pictures
+![Django Pictures Logo](https://repository-images.githubusercontent.com/455480246/daaa7870-d28c-4fce-8296-d3e3af487a64)
+
+# Django Pictures
 
 Responsive cross-browser image library using modern codes like AVIF & WebP.
 
 * responsive web images using the [picture](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/picture) tag
 * native grid system support
 * serve files with or without a CDN
 * placeholders for local development
 * migration support
-* async image processing for Celery or Dramatiq
+* async image processing for [Celery] or [Dramatiq]
+* [DRF] support
 
 [![PyPi Version](https://img.shields.io/pypi/v/django-pictures.svg)](https://pypi.python.org/pypi/django-pictures/)
 [![Test Coverage](https://codecov.io/gh/codingjoe/django-pictures/branch/main/graph/badge.svg)](https://codecov.io/gh/codingjoe/django-pictures)
 [![GitHub License](https://img.shields.io/github/license/codingjoe/django-pictures)](https://raw.githubusercontent.com/codingjoe/django-pictures/master/LICENSE)
 
 ## Usage
 
@@ -101,14 +104,33 @@
 
 if get_settings().USE_PLACEHOLDERS:
     urlpatterns += [
         path("_pictures/", include("pictures.urls")),
     ]
 ```
 
+### Legacy use-cases (email)
+
+Although the `picture`-tag is [adequate for most use-cases][caniuse-picture],
+some remain, where a single `img` tag is necessary. Notably in email, where
+[most clients do support WebP][caniemail-webp] but not [srcset][caniemail-srcset].
+The template tag `img_url` returns a single size image URL.
+In addition to the ratio you will need to define the `file_type`
+as well as the `width` (absolute width in pixels).
+
+
+```html
+{% load pictures %}
+<img src="{% img_url profile.picture ratio="3/2" file_type="webp" width=800 %}" alt="profile picture">
+```
+
+[caniuse-picture]: https://caniuse.com/picture
+[caniemail-webp]: https://www.caniemail.com/features/image-webp/
+[caniemail-srcset]: https://www.caniemail.com/features/html-srcset/
+
 ## Config
 
 ### Aspect ratios
 
 You can specify the aspect ratios of your images. Images will be cropped to the
 specified aspect ratio. Aspect ratios are specified as a string with a slash
 between the width and height. For example, `16/9` will crop the image to 16:9.
@@ -190,24 +212,61 @@
 You can follow [the example][migration] in our test app, to see how it works.
 
 [migration]: tests/testapp/migrations/0002_alter_profile_picture.py
 
 
 ## Contrib
 
-### Django Rest Framework (DRF)
+### Django Rest Framework ([DRF])
 
 We do ship with a read-only `PictureField` that can be used to include all
 available picture sizes in a DRF serializer.
 
 ```python
 from rest_framework import serializers
 from pictures.contrib.rest_framework import PictureField
 
 class PictureSerializer(serializers.Serializer):
     picture = PictureField()
 ```
 
+You may provide optional GET parameters to the serializer, to specify the aspect
+ratio and breakpoints you want to include in the response. The parameters are
+prefixed with the `fieldname_` to avoid conflicts with other fields.
+
+```bash
+curl http://localhost:8000/api/path/?picture_ratio=16%2F9&picture_m=6&picture_l=4
+# %2F is the url encoded slash
+```
+
+```json
+{
+  "other_fields": "…",
+  "picture": {
+    "url": "/path/to/image.jpg",
+    "width": 800,
+    "height": 800,
+    "ratios": {
+      "1/1": {
+        "sources": {
+          "image/webp": {
+            "100": "/path/to/image/1/100w.webp",
+            "200": "…"
+          }
+        },
+        "media": "(min-width: 0px) and (max-width: 991px) 100vw, (min-width: 992px) and (max-width: 1199px) 33vw, 25vw"
+      }
+    }
+  }
+}
+```
+
+Note that the `media` keys are only included, if you have specified breakpoints.
+
 ### Django Cleanup
 
 `PictureField` is compatible with [Django Cleanup](https://github.com/un1t/django-cleanup),
 which automatically deletes its file and corresponding `SimplePicture` files.
+
+[drf]: https://www.django-rest-framework.org/
+[celery]: https://docs.celeryproject.org/en/stable/
+[dramatiq]: https://dramatiq.io/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-pictures-1.0rc4/pictures/checks.py` & `django-pictures-1.0rc5/pictures/checks.py`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc4/pictures/conf.py` & `django-pictures-1.0rc5/pictures/conf.py`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc4/pictures/locale/de/LC_MESSAGES/django.mo` & `django-pictures-1.0rc5/pictures/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc4/pictures/locale/de/LC_MESSAGES/django.po` & `django-pictures-1.0rc5/pictures/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc4/pictures/migrations.py` & `django-pictures-1.0rc5/pictures/migrations.py`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc4/pictures/models.py` & `django-pictures-1.0rc5/pictures/models.py`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc4/pictures/tasks.py` & `django-pictures-1.0rc5/pictures/tasks.py`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc4/pictures/templates/pictures/picture.html` & `django-pictures-1.0rc5/pictures/templates/pictures/picture.html`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc4/pictures/templatetags/pictures.py` & `django-pictures-1.0rc5/pictures/templatetags/pictures.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,10 +55,10 @@
         sizes = file_types[file_type.upper()]
     except KeyError as e:
         raise ValueError(
             f"Invalid file type: {file_type}. Choices are: {', '.join(file_types.keys())}"
         ) from e
     for w, img in sorted(sizes.items()):
         url = img.url
-        if w >= width:
+        if w >= int(width):
             break
     return url
```

### Comparing `django-pictures-1.0rc4/pictures/utils.py` & `django-pictures-1.0rc5/pictures/utils.py`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc4/pictures/validators.py` & `django-pictures-1.0rc5/pictures/validators.py`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc4/pictures/views.py` & `django-pictures-1.0rc5/pictures/views.py`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc4/PKG-INFO` & `django-pictures-1.0rc5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pictures
-Version: 1.0rc4
+Version: 1.0rc5
 Summary: Responsive cross-browser image library using modern codes like AVIF & WebP.
 Keywords: pillow,Django,image,pictures,WebP,AVIF
 Author-email: Johannes Maron <johannes@maron.family>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -31,31 +31,37 @@
 Requires-Dist: django-dramatiq ; extra == "dramatiq"
 Requires-Dist: djangorestframework ; extra == "drf"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-django ; extra == "test"
 Requires-Dist: redis ; extra == "test"
 Project-URL: Changelog, https://github.com/codingjoe/django-pictures/releases
+Project-URL: Documentation, https://github.com/codingjoe/django-pictures#django-pictures
+Project-URL: Issue-Tracker, https://github.com/codingjoe/django-pictures/issues
 Project-URL: Project-URL, https://github.com/codingjoe/django-pictures
+Project-URL: Source, https://github.com/codingjoe/django-pictures
 Provides-Extra: celery
 Provides-Extra: cleanup
 Provides-Extra: dramatiq
 Provides-Extra: drf
 Provides-Extra: test
 
-# django-pictures
+![Django Pictures Logo](https://repository-images.githubusercontent.com/455480246/daaa7870-d28c-4fce-8296-d3e3af487a64)
+
+# Django Pictures
 
 Responsive cross-browser image library using modern codes like AVIF & WebP.
 
 * responsive web images using the [picture](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/picture) tag
 * native grid system support
 * serve files with or without a CDN
 * placeholders for local development
 * migration support
-* async image processing for Celery or Dramatiq
+* async image processing for [Celery] or [Dramatiq]
+* [DRF] support
 
 [![PyPi Version](https://img.shields.io/pypi/v/django-pictures.svg)](https://pypi.python.org/pypi/django-pictures/)
 [![Test Coverage](https://codecov.io/gh/codingjoe/django-pictures/branch/main/graph/badge.svg)](https://codecov.io/gh/codingjoe/django-pictures)
 [![GitHub License](https://img.shields.io/github/license/codingjoe/django-pictures)](https://raw.githubusercontent.com/codingjoe/django-pictures/master/LICENSE)
 
 ## Usage
 
@@ -145,14 +151,33 @@
 
 if get_settings().USE_PLACEHOLDERS:
     urlpatterns += [
         path("_pictures/", include("pictures.urls")),
     ]
 ```
 
+### Legacy use-cases (email)
+
+Although the `picture`-tag is [adequate for most use-cases][caniuse-picture],
+some remain, where a single `img` tag is necessary. Notably in email, where
+[most clients do support WebP][caniemail-webp] but not [srcset][caniemail-srcset].
+The template tag `img_url` returns a single size image URL.
+In addition to the ratio you will need to define the `file_type`
+as well as the `width` (absolute width in pixels).
+
+
+```html
+{% load pictures %}
+<img src="{% img_url profile.picture ratio="3/2" file_type="webp" width=800 %}" alt="profile picture">
+```
+
+[caniuse-picture]: https://caniuse.com/picture
+[caniemail-webp]: https://www.caniemail.com/features/image-webp/
+[caniemail-srcset]: https://www.caniemail.com/features/html-srcset/
+
 ## Config
 
 ### Aspect ratios
 
 You can specify the aspect ratios of your images. Images will be cropped to the
 specified aspect ratio. Aspect ratios are specified as a string with a slash
 between the width and height. For example, `16/9` will crop the image to 16:9.
@@ -234,25 +259,62 @@
 You can follow [the example][migration] in our test app, to see how it works.
 
 [migration]: tests/testapp/migrations/0002_alter_profile_picture.py
 
 
 ## Contrib
 
-### Django Rest Framework (DRF)
+### Django Rest Framework ([DRF])
 
 We do ship with a read-only `PictureField` that can be used to include all
 available picture sizes in a DRF serializer.
 
 ```python
 from rest_framework import serializers
 from pictures.contrib.rest_framework import PictureField
 
 class PictureSerializer(serializers.Serializer):
     picture = PictureField()
 ```
 
+You may provide optional GET parameters to the serializer, to specify the aspect
+ratio and breakpoints you want to include in the response. The parameters are
+prefixed with the `fieldname_` to avoid conflicts with other fields.
+
+```bash
+curl http://localhost:8000/api/path/?picture_ratio=16%2F9&picture_m=6&picture_l=4
+# %2F is the url encoded slash
+```
+
+```json
+{
+  "other_fields": "…",
+  "picture": {
+    "url": "/path/to/image.jpg",
+    "width": 800,
+    "height": 800,
+    "ratios": {
+      "1/1": {
+        "sources": {
+          "image/webp": {
+            "100": "/path/to/image/1/100w.webp",
+            "200": "…"
+          }
+        },
+        "media": "(min-width: 0px) and (max-width: 991px) 100vw, (min-width: 992px) and (max-width: 1199px) 33vw, 25vw"
+      }
+    }
+  }
+}
+```
+
+Note that the `media` keys are only included, if you have specified breakpoints.
+
 ### Django Cleanup
 
 `PictureField` is compatible with [Django Cleanup](https://github.com/un1t/django-cleanup),
 which automatically deletes its file and corresponding `SimplePicture` files.
 
+[drf]: https://www.django-rest-framework.org/
+[celery]: https://docs.celeryproject.org/en/stable/
+[dramatiq]: https://dramatiq.io/
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

