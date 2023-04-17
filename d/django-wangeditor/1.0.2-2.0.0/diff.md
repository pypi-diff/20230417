# Comparing `tmp/django-wangeditor-1.0.2.tar.gz` & `tmp/django-wangeditor-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-wangeditor-1.0.2.tar", last modified: Sun Mar 19 11:41:51 2023, max compression
+gzip compressed data, was "django-wangeditor-2.0.0.tar", last modified: Mon Apr 17 09:39:40 2023, max compression
```

## Comparing `django-wangeditor-1.0.2.tar` & `django-wangeditor-2.0.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/
--rw-r--r--   0 hubery     (501) staff       (20)     3774 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/PKG-INFO
--rw-r--r--   0 hubery     (501) staff       (20)     1504 2023-03-19 11:10:52.000000 django-wangeditor-1.0.2/LICENSE
--rw-r--r--   0 hubery     (501) staff       (20)      139 2023-03-19 11:10:52.000000 django-wangeditor-1.0.2/MANIFEST.in
-drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/docs/
--rw-r--r--   0 hubery     (501) staff       (20)       26 2023-03-19 11:10:52.000000 django-wangeditor-1.0.2/docs/README.md
--rw-r--r--   0 hubery     (501) staff       (20)      204 2023-03-19 11:10:52.000000 django-wangeditor-1.0.2/setup.py
-drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/django_wangeditor.egg-info/
--rw-r--r--   0 hubery     (501) staff       (20)     3774 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/django_wangeditor.egg-info/PKG-INFO
--rw-r--r--   0 hubery     (501) staff       (20)        1 2023-03-19 11:26:43.000000 django-wangeditor-1.0.2/django_wangeditor.egg-info/not-zip-safe
--rw-r--r--   0 hubery     (501) staff       (20)      714 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/django_wangeditor.egg-info/SOURCES.txt
--rw-r--r--   0 hubery     (501) staff       (20)       23 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/django_wangeditor.egg-info/requires.txt
--rw-r--r--   0 hubery     (501) staff       (20)       11 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/django_wangeditor.egg-info/top_level.txt
--rw-r--r--   0 hubery     (501) staff       (20)        1 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/django_wangeditor.egg-info/dependency_links.txt
--rw-r--r--   0 hubery     (501) staff       (20)     1230 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/setup.cfg
--rw-r--r--   0 hubery     (501) staff       (20)     2878 2023-03-19 11:41:34.000000 django-wangeditor-1.0.2/README.rst
-drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/wangeditor/
--rw-r--r--   0 hubery     (501) staff       (20)      735 2023-03-19 11:10:52.000000 django-wangeditor-1.0.2/wangeditor/configs.py
--rw-r--r--   0 hubery     (501) staff       (20)      858 2023-03-19 11:10:52.000000 django-wangeditor-1.0.2/wangeditor/fields.py
-drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/wangeditor/backends/
--rw-r--r--   0 hubery     (501) staff       (20)      600 2023-03-19 11:10:52.000000 django-wangeditor-1.0.2/wangeditor/backends/__init__.py
--rw-r--r--   0 hubery     (501) staff       (20)      506 2023-03-19 11:10:52.000000 django-wangeditor-1.0.2/wangeditor/backends/dummy_backend.py
--rw-r--r--   0 hubery     (501) staff       (20)      441 2023-03-19 11:16:23.000000 django-wangeditor-1.0.2/wangeditor/__init__.py
--rw-r--r--   0 hubery     (501) staff       (20)     3910 2023-03-19 11:12:31.000000 django-wangeditor-1.0.2/wangeditor/widgets.py
--rw-r--r--   0 hubery     (501) staff       (20)     1460 2023-03-19 11:10:52.000000 django-wangeditor-1.0.2/wangeditor/utils.py
-drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/wangeditor/static/
-drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/wangeditor/static/wangeditor/
--rw-r--r--   0 hubery     (501) staff       (20)     3467 2023-03-19 11:10:52.000000 django-wangeditor-1.0.2/wangeditor/static/wangeditor/wangeditor-init.js
--rwxr-xr-x   0 hubery     (501) staff       (20)    66009 2023-03-19 11:10:52.000000 django-wangeditor-1.0.2/wangeditor/static/wangeditor/wangEditor.min.js
--rw-r--r--   0 hubery     (501) staff       (20)   220242 2023-03-19 11:10:52.000000 django-wangeditor-1.0.2/wangeditor/static/wangeditor/wangEditor.min.js.map
-drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/wangeditor/templates/
-drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-03-19 11:41:51.000000 django-wangeditor-1.0.2/wangeditor/templates/wangeditor/
--rw-r--r--   0 hubery     (501) staff       (20)      719 2023-03-19 11:10:52.000000 django-wangeditor-1.0.2/wangeditor/templates/wangeditor/widget.html
--rw-r--r--   0 hubery     (501) staff       (20)      882 2023-03-19 11:12:18.000000 django-wangeditor-1.0.2/wangeditor/urls.py
--rw-r--r--   0 hubery     (501) staff       (20)     2580 2023-03-19 11:10:52.000000 django-wangeditor-1.0.2/wangeditor/views.py
+drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-04-17 09:39:40.124184 django-wangeditor-2.0.0/
+-rw-r--r--   0 hubery     (501) staff       (20)     1504 2023-03-19 11:10:52.000000 django-wangeditor-2.0.0/LICENSE
+-rw-r--r--   0 hubery     (501) staff       (20)      139 2023-03-19 11:10:52.000000 django-wangeditor-2.0.0/MANIFEST.in
+-rw-r--r--   0 hubery     (501) staff       (20)     3601 2023-04-17 09:39:40.124399 django-wangeditor-2.0.0/PKG-INFO
+-rw-r--r--   0 hubery     (501) staff       (20)     2573 2023-04-17 09:39:21.000000 django-wangeditor-2.0.0/README.rst
+drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-04-17 09:39:40.084914 django-wangeditor-2.0.0/django_wangeditor.egg-info/
+-rw-r--r--   0 hubery     (501) staff       (20)     3601 2023-04-17 09:39:39.000000 django-wangeditor-2.0.0/django_wangeditor.egg-info/PKG-INFO
+-rw-r--r--   0 hubery     (501) staff       (20)      755 2023-04-17 09:39:40.000000 django-wangeditor-2.0.0/django_wangeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 hubery     (501) staff       (20)        1 2023-04-17 09:39:40.000000 django-wangeditor-2.0.0/django_wangeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 hubery     (501) staff       (20)        1 2023-04-17 09:19:25.000000 django-wangeditor-2.0.0/django_wangeditor.egg-info/not-zip-safe
+-rw-r--r--   0 hubery     (501) staff       (20)       23 2023-04-17 09:39:40.000000 django-wangeditor-2.0.0/django_wangeditor.egg-info/requires.txt
+-rw-r--r--   0 hubery     (501) staff       (20)       11 2023-04-17 09:39:40.000000 django-wangeditor-2.0.0/django_wangeditor.egg-info/top_level.txt
+drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-04-17 09:39:40.085481 django-wangeditor-2.0.0/docs/
+-rw-r--r--   0 hubery     (501) staff       (20)       26 2023-03-19 11:10:52.000000 django-wangeditor-2.0.0/docs/README.md
+-rw-r--r--   0 hubery     (501) staff       (20)     1349 2023-04-17 09:39:40.125480 django-wangeditor-2.0.0/setup.cfg
+-rw-r--r--   0 hubery     (501) staff       (20)      570 2023-04-17 09:13:57.000000 django-wangeditor-2.0.0/setup.py
+drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-04-17 09:39:40.092166 django-wangeditor-2.0.0/wangeditor/
+-rw-r--r--   0 hubery     (501) staff       (20)      441 2023-04-17 09:08:56.000000 django-wangeditor-2.0.0/wangeditor/__init__.py
+drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-04-17 09:39:40.093865 django-wangeditor-2.0.0/wangeditor/backends/
+-rw-r--r--   0 hubery     (501) staff       (20)      598 2023-04-17 07:09:49.000000 django-wangeditor-2.0.0/wangeditor/backends/__init__.py
+-rw-r--r--   0 hubery     (501) staff       (20)      622 2023-04-17 07:13:31.000000 django-wangeditor-2.0.0/wangeditor/backends/dummy_backend.py
+-rw-r--r--   0 hubery     (501) staff       (20)     3641 2023-04-17 07:14:36.000000 django-wangeditor-2.0.0/wangeditor/configs.py
+-rw-r--r--   0 hubery     (501) staff       (20)      858 2023-04-14 09:33:56.000000 django-wangeditor-2.0.0/wangeditor/fields.py
+drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-04-17 09:39:40.076748 django-wangeditor-2.0.0/wangeditor/static/
+drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-04-17 09:39:40.121863 django-wangeditor-2.0.0/wangeditor/static/wangeditor/
+drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-04-17 09:39:40.122630 django-wangeditor-2.0.0/wangeditor/static/wangeditor/css/
+-rw-r--r--   0 hubery     (501) staff       (20)    14906 2023-04-14 09:40:17.000000 django-wangeditor-2.0.0/wangeditor/static/wangeditor/css/style.css
+-rw-r--r--   0 hubery     (501) staff       (20)  1335072 2023-04-14 09:40:02.000000 django-wangeditor-2.0.0/wangeditor/static/wangeditor/wangEditor-v5.js
+-rw-r--r--   0 hubery     (501) staff       (20)  2596073 2023-04-14 09:40:53.000000 django-wangeditor-2.0.0/wangeditor/static/wangeditor/wangEditor-v5.js.map
+-rw-r--r--   0 hubery     (501) staff       (20)     4881 2023-04-17 07:58:04.000000 django-wangeditor-2.0.0/wangeditor/static/wangeditor/wangeditor-init.js
+drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-04-17 09:39:40.077316 django-wangeditor-2.0.0/wangeditor/templates/
+drwxr-xr-x   0 hubery     (501) staff       (20)        0 2023-04-17 09:39:40.123400 django-wangeditor-2.0.0/wangeditor/templates/wangeditor/
+-rw-r--r--   0 hubery     (501) staff       (20)     2286 2023-04-17 09:06:54.000000 django-wangeditor-2.0.0/wangeditor/templates/wangeditor/widget.html
+-rw-r--r--   0 hubery     (501) staff       (20)     1098 2023-04-17 07:14:36.000000 django-wangeditor-2.0.0/wangeditor/urls.py
+-rw-r--r--   0 hubery     (501) staff       (20)     1689 2023-04-17 07:13:31.000000 django-wangeditor-2.0.0/wangeditor/utils.py
+-rw-r--r--   0 hubery     (501) staff       (20)     3534 2023-04-17 07:59:14.000000 django-wangeditor-2.0.0/wangeditor/views.py
+-rw-r--r--   0 hubery     (501) staff       (20)     3999 2023-04-17 06:27:13.000000 django-wangeditor-2.0.0/wangeditor/widgets.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-wangeditor-1.0.2/PKG-INFO` & `django-wangeditor-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: django-wangeditor
-Version: 1.0.2
+Version: 2.0.0
 Summary: A Django app to use wangeditor.
 Home-page: https://github.com/pangxiaobin/django-wangeditor
 Author: Hubery
 Author-email: panglaibin2013@163.com
 License: BSD-3-Clause
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 License-File: LICENSE
 
 
 =================
 django-wangeditor
@@ -33,15 +35,15 @@
 1.Install or add django-wangeditor to your python path.::
 
     pip install django-wangeditor
 
 2.Add "wangeditor" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
-        ... 
+        ...
         'wangeditor',
     ]
 
 3.Run the collectstatic management command: `$ ./manage.py collectstatic.` This will copy static CKEditor required media resources into the directory given by the STATIC_ROOT setting. See Django's documentation on managing static files for more info.
 
 
 -----
@@ -68,55 +70,52 @@
  MEDIA_ROOT = os.path.join(BASE_DIR, 'media')
 
  WANGEDITOR_UPLOAD_PATH = "uploads/"
 
 
 2.Include the wangeditor URLconf in your project urls.py like this::
 
+  from django.conf.urls.static import static
+  from django.conf import settings
   # django >= 2.0
   path('wangeditor/', include('wangeditor.urls'))
   # django < 2.0
   url(r'wangeditor/', include('wangeditor.urls'))
+  if settings.DEBUG:
+      urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
 
-  urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
 
-3.Opens the configuration for uploading images::
-
-  WANGEDITOR_CONFIGS = {
-      'default':{
-          'uploadImgServer': '/wangeditor/upload/'
-      }
-  }
 
 -------
 config
 -------
-Optional - customizing wangEditor editor
-Add a WANGEDITOR_CONFIGS setting to the project's settings.py file.::
+Optional - customizing wangEditor editor Add a WANGEDITOR_CONFIGS setting to the project's settings.py file.::
 
-    WANGEDITOR_CONFIGS = {
-    'default': {
-        'menus': ['head', 'bold', 'fontSize', 'fontName', 'italic', 'underline', 'strikeThrough', 'foreColor',
-                  'backColor',
-                  'link', 'list', 'justify', 'quote', 'emoticon', 'image', 'table', 'video', 'code', 'undo', 'redo'],
-        'pasteFilterStyle': True,  # Whether to turn off paste style filtering
-        'pasteIgnoreImg': False,  # Whether to ignore images in the pasted content
-        'colors': [
-            '#000000',
-            '#eeece0',
-            '#1c487f',
-            '#4d80bf',
-        ],  # Custom configuration color (font color, background color) can add more color number
-        'showLinkImg': False,  # Hide the inserted network image
+ WANGEDITOR_CONFIGS = {
+  "default": {
+    "toolbar_config":{
+      "modalAppendToBody": False,
     }
+    "menu_conf": {
+       "uploadImage": {
+          "server": "/wangeditor/img_upload/",
+        },
+        "uploadVideo": {
+          "server": "/wangeditor/video_upload/"
+        }
     }
+ }
+ # toobar_config and menu_conf cong please see https://www.wangeditor.com/v5/toolbar-config.html and https://www.wangeditor.com/v5/menu-config.html
 
 -----------
 Update Log
 -----------
+version-2.0.0
+
+1、update wangeditor to wangeditor-v5;
+
 version-1.0.2
+
 1、Resolve compatibility issues with django 4.0
 
 
 Refer to the configuration for more information, please see `https://www.kancloud.cn/wangfupeng/wangeditor3/332599`
-
-
```

### Comparing `django-wangeditor-1.0.2/LICENSE` & `django-wangeditor-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-wangeditor-1.0.2/django_wangeditor.egg-info/PKG-INFO` & `django-wangeditor-2.0.0/django_wangeditor.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: django-wangeditor
-Version: 1.0.2
+Version: 2.0.0
 Summary: A Django app to use wangeditor.
 Home-page: https://github.com/pangxiaobin/django-wangeditor
 Author: Hubery
 Author-email: panglaibin2013@163.com
 License: BSD-3-Clause
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 License-File: LICENSE
 
 
 =================
 django-wangeditor
@@ -33,15 +35,15 @@
 1.Install or add django-wangeditor to your python path.::
 
     pip install django-wangeditor
 
 2.Add "wangeditor" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
-        ... 
+        ...
         'wangeditor',
     ]
 
 3.Run the collectstatic management command: `$ ./manage.py collectstatic.` This will copy static CKEditor required media resources into the directory given by the STATIC_ROOT setting. See Django's documentation on managing static files for more info.
 
 
 -----
@@ -68,55 +70,52 @@
  MEDIA_ROOT = os.path.join(BASE_DIR, 'media')
 
  WANGEDITOR_UPLOAD_PATH = "uploads/"
 
 
 2.Include the wangeditor URLconf in your project urls.py like this::
 
+  from django.conf.urls.static import static
+  from django.conf import settings
   # django >= 2.0
   path('wangeditor/', include('wangeditor.urls'))
   # django < 2.0
   url(r'wangeditor/', include('wangeditor.urls'))
+  if settings.DEBUG:
+      urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
 
-  urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
 
-3.Opens the configuration for uploading images::
-
-  WANGEDITOR_CONFIGS = {
-      'default':{
-          'uploadImgServer': '/wangeditor/upload/'
-      }
-  }
 
 -------
 config
 -------
-Optional - customizing wangEditor editor
-Add a WANGEDITOR_CONFIGS setting to the project's settings.py file.::
+Optional - customizing wangEditor editor Add a WANGEDITOR_CONFIGS setting to the project's settings.py file.::
 
-    WANGEDITOR_CONFIGS = {
-    'default': {
-        'menus': ['head', 'bold', 'fontSize', 'fontName', 'italic', 'underline', 'strikeThrough', 'foreColor',
-                  'backColor',
-                  'link', 'list', 'justify', 'quote', 'emoticon', 'image', 'table', 'video', 'code', 'undo', 'redo'],
-        'pasteFilterStyle': True,  # Whether to turn off paste style filtering
-        'pasteIgnoreImg': False,  # Whether to ignore images in the pasted content
-        'colors': [
-            '#000000',
-            '#eeece0',
-            '#1c487f',
-            '#4d80bf',
-        ],  # Custom configuration color (font color, background color) can add more color number
-        'showLinkImg': False,  # Hide the inserted network image
+ WANGEDITOR_CONFIGS = {
+  "default": {
+    "toolbar_config":{
+      "modalAppendToBody": False,
     }
+    "menu_conf": {
+       "uploadImage": {
+          "server": "/wangeditor/img_upload/",
+        },
+        "uploadVideo": {
+          "server": "/wangeditor/video_upload/"
+        }
     }
+ }
+ # toobar_config and menu_conf cong please see https://www.wangeditor.com/v5/toolbar-config.html and https://www.wangeditor.com/v5/menu-config.html
 
 -----------
 Update Log
 -----------
+version-2.0.0
+
+1、update wangeditor to wangeditor-v5;
+
 version-1.0.2
+
 1、Resolve compatibility issues with django 4.0
 
 
 Refer to the configuration for more information, please see `https://www.kancloud.cn/wangfupeng/wangeditor3/332599`
-
-
```

### Comparing `django-wangeditor-1.0.2/django_wangeditor.egg-info/SOURCES.txt` & `django-wangeditor-2.0.0/django_wangeditor.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 wangeditor/fields.py
 wangeditor/urls.py
 wangeditor/utils.py
 wangeditor/views.py
 wangeditor/widgets.py
 wangeditor/backends/__init__.py
 wangeditor/backends/dummy_backend.py
-wangeditor/static/wangeditor/wangEditor.min.js
-wangeditor/static/wangeditor/wangEditor.min.js.map
+wangeditor/static/wangeditor/wangEditor-v5.js
+wangeditor/static/wangeditor/wangEditor-v5.js.map
 wangeditor/static/wangeditor/wangeditor-init.js
+wangeditor/static/wangeditor/css/style.css
 wangeditor/templates/wangeditor/widget.html
```

### Comparing `django-wangeditor-1.0.2/README.rst` & `django-wangeditor-2.0.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 1.Install or add django-wangeditor to your python path.::
 
     pip install django-wangeditor
 
 2.Add "wangeditor" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
-        ... 
+        ...
         'wangeditor',
     ]
 
 3.Run the collectstatic management command: `$ ./manage.py collectstatic.` This will copy static CKEditor required media resources into the directory given by the STATIC_ROOT setting. See Django's documentation on managing static files for more info.
 
 
 -----
@@ -44,53 +44,52 @@
  MEDIA_ROOT = os.path.join(BASE_DIR, 'media')
 
  WANGEDITOR_UPLOAD_PATH = "uploads/"
 
 
 2.Include the wangeditor URLconf in your project urls.py like this::
 
+  from django.conf.urls.static import static
+  from django.conf import settings
   # django >= 2.0
   path('wangeditor/', include('wangeditor.urls'))
   # django < 2.0
   url(r'wangeditor/', include('wangeditor.urls'))
+  if settings.DEBUG:
+      urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
 
-  urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
 
-3.Opens the configuration for uploading images::
-
-  WANGEDITOR_CONFIGS = {
-      'default':{
-          'uploadImgServer': '/wangeditor/upload/'
-      }
-  }
 
 -------
 config
 -------
-Optional - customizing wangEditor editor
-Add a WANGEDITOR_CONFIGS setting to the project's settings.py file.::
+Optional - customizing wangEditor editor Add a WANGEDITOR_CONFIGS setting to the project's settings.py file.::
 
-    WANGEDITOR_CONFIGS = {
-    'default': {
-        'menus': ['head', 'bold', 'fontSize', 'fontName', 'italic', 'underline', 'strikeThrough', 'foreColor',
-                  'backColor',
-                  'link', 'list', 'justify', 'quote', 'emoticon', 'image', 'table', 'video', 'code', 'undo', 'redo'],
-        'pasteFilterStyle': True,  # Whether to turn off paste style filtering
-        'pasteIgnoreImg': False,  # Whether to ignore images in the pasted content
-        'colors': [
-            '#000000',
-            '#eeece0',
-            '#1c487f',
-            '#4d80bf',
-        ],  # Custom configuration color (font color, background color) can add more color number
-        'showLinkImg': False,  # Hide the inserted network image
+ WANGEDITOR_CONFIGS = {
+  "default": {
+    "toolbar_config":{
+      "modalAppendToBody": False,
     }
+    "menu_conf": {
+       "uploadImage": {
+          "server": "/wangeditor/img_upload/",
+        },
+        "uploadVideo": {
+          "server": "/wangeditor/video_upload/"
+        }
     }
+ }
+ # toobar_config and menu_conf cong please see https://www.wangeditor.com/v5/toolbar-config.html and https://www.wangeditor.com/v5/menu-config.html
 
 -----------
 Update Log
 -----------
+version-2.0.0
+
+1、update wangeditor to wangeditor-v5;
+
 version-1.0.2
+
 1、Resolve compatibility issues with django 4.0
 
 
 Refer to the configuration for more information, please see `https://www.kancloud.cn/wangfupeng/wangeditor3/332599`
```

### Comparing `django-wangeditor-1.0.2/wangeditor/fields.py` & `django-wangeditor-2.0.0/wangeditor/fields.py`

 * *Files identical despite different names*

### Comparing `django-wangeditor-1.0.2/wangeditor/backends/__init__.py` & `django-wangeditor-2.0.0/wangeditor/backends/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,9 +16,7 @@
         backend_id = getattr(settings, "WANGEDITOR_IMAGE_BACKEND", None)
         if backend_id is None:
             return DummyBackend
         return self._registry[backend_id]
 
 
 registry = BackendRegistry()
-
-
```

### Comparing `django-wangeditor-1.0.2/wangeditor/widgets.py` & `django-wangeditor-2.0.0/wangeditor/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 class WangEditorWidget(forms.Textarea):
     class Media:
         # js
         js = (
             JS('wangeditor/wangeditor-init.js', {
                 'id': 'wangeditor-init-script',
             }),
-            'wangeditor/wangEditor.min.js',
+            'wangeditor/wangEditor-v5.js',
         )
 
     def __init__(self, config_name='default', *args, **kwargs):
         super(WangEditorWidget, self).__init__(*args, **kwargs)
         # Setup config from defaults.
         self.config = WANG_DEFAULT_CONFIG.copy()
 
@@ -99,15 +99,16 @@
             renderer = get_default_renderer()
         if value is None:
             value = ''
         final_attrs = self.build_attrs(self.attrs, attrs, name=name)
         return mark_safe(renderer.render('wangeditor/widget.html', {
             'final_attrs': flatatt(final_attrs),  # flatatt  设置html 的属性, 形式key=value
             'value': force_text(value),
-            'config': json_encode(self.config),
+            'toolbar_config': json_encode(self.config['toolbar_config']),
+            'menu_conf': json_encode(self.config['menu_conf']),
             'id': final_attrs['id'],
         }))
 
     def build_attrs(self, base_attrs, extra_attrs=None, **kwargs):
         """
         Helper function for building an attribute dictionary.
         This is combination of the same method from Django<=1.10 and Django1.11+
```

### Comparing `django-wangeditor-1.0.2/wangeditor/utils.py` & `django-wangeditor-2.0.0/wangeditor/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import string
 
 from django.conf import settings
 from django.template.defaultfilters import slugify
 from django.utils.module_loading import import_string
 
 IMAGE_EXTENSIONS = {'jpg', 'jpeg', 'png', 'gif'}
+VIDEO_EXTENSIONS = {'mp4', 'webm', 'ogg', '3gpp', 'mpeg-4'}
 
 
 # Allow for a custom storage backend defined in settings.
 # https://docs.djangoproject.com/en/3.0/ref/files/storage/
 def get_storage_class():
 
     return import_string(getattr(settings, 'WANGEDITOR_STORAGE_BACKEND', 'django.core.files.storage.DefaultStorage'))()
@@ -49,8 +50,13 @@
     Determine system file's media URL.
     """
     return storage.url(path)
 
 
 def is_valid_image_extension(file_name):
     """验证是否为图片"""
-    return file_name.split('.')[-1] in IMAGE_EXTENSIONS if file_name else False
+    return file_name.split('.')[-1].lower() in IMAGE_EXTENSIONS if file_name else False
+
+
+def is_valid_video_extension(file_name):
+    """验证是否为video"""
+    return file_name.split('.')[-1].lower() in VIDEO_EXTENSIONS if file_name else False
```

### Comparing `django-wangeditor-1.0.2/wangeditor/static/wangeditor/wangeditor-init.js` & `django-wangeditor-2.0.0/wangeditor/static/wangeditor/wangeditor-init.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -37,40 +37,72 @@
     } else {
         document.addEventListener('DOMContentLoaded', runInitialisers);
     }
 
     function initialiseWangEditor() {
         var divs = Array.prototype.slice.call(document.querySelectorAll('div[data-type=wangeditortype]'));
         var textareas = Array.prototype.slice.call(document.querySelectorAll('textarea[data-type=wangtextareas]'));
+        var wangeditortype_toolbars = Array.prototype.slice.call(document.querySelectorAll('div[data-type=wangeditorToolbar]'));
+        var wangeditortype_container = Array.prototype.slice.call(document.querySelectorAll('div[data-type=wangeditorContainer]'));
         for (var i = 0; i < divs.length; ++i) {
             var d = divs[i];
             var t = textareas[i];
+            var tool = wangeditortype_toolbars[i]
+            var container = wangeditortype_container[i]
             if (d.getAttribute('data-processed') === '0' && d.id.indexOf('__prefix__') === -1) {
                 d.setAttribute('data-processed', '1');
-                var E = window.wangEditor;
-                var editor = new E(document.getElementById(d.id));
-                const textarea = document.getElementById(t.id);
-                editor.customConfig = JSON.parse(d.getAttribute('data-config'));
-                editor.customConfig.onchange = function(html) {
-                    // 监控变化，同步更新到 textarea
-                    textarea.innerHTML = html;
-                };
-                editor.customConfig.uploadImgHooks = {
-                    fail: function(xhr, editor, result) {
-                        // 图片上传并返回结果，但图片插入错误时触发
-                        // xhr 是 XMLHttpRequst 对象，editor 是编辑器对象，result 是服务器端返回的结果
-                        if (result['errno'] !== 0) {
-                            alert(result['msg'])
-                        }
+                const {
+                    createEditor,
+                    createToolbar
+                } = window.wangEditor
+                const menutCong = JSON.parse(d.getAttribute('data-menu-conf'));
+
+                const editorConfig = {
+                    onChange(editor) {
+                        textarea.innerHTML = editor.getHtml();
                     },
-                };
-                editor.create();
-                if (textarea.innerHTML.length !== 0) {
-                    editor.txt.html(textarea.innerText);
+                    MENU_CONF: menutCong
+                }
+                editorConfig.MENU_CONF['uploadVideo']['onFailed'] = function(file, res) {
+                    alert(`${file.name} 上传失败`, res['msg'])
+                }
+                editorConfig.MENU_CONF['uploadImage']['onFailed'] = function(file, res) {
+                    alert(`${file.name} 上传失败`, res['msg'])
+                }
+                const editor = createEditor({
+                    selector: '#' + container.id,
+                    html: '',
+                    config: editorConfig,
+                    mode: 'default', // or 'simple'
+                })
+
+                editor.on('fullScreen', () => {
+                    const stickyElements = document.querySelectorAll('.sticky');
+                    stickyElements.forEach(element => {
+                        element.style.display = 'none';
+                    });
+                })
+                editor.on('unFullScreen', () => {
+                    const stickyElements = document.querySelectorAll('.sticky');
+                    stickyElements.forEach(element => {
+                        element.style.display = '';
+                    });
+                })
+                const toolbarConfig = JSON.parse(d.getAttribute('data-toolbar-config'));
+                const toolbar = createToolbar({
+                    editor,
+                    selector: '#' + tool.id,
+                    config: toolbarConfig,
+                    mode: 'default', // or 'simple'
+                })
+                const textarea = document.getElementById(t.id);
+                // const toolbarConfig = JSON.parse(d.getAttribute('data-config'))
 
+                if (textarea.innerHTML.length !== 0) {
+                    editor.setHtml(textarea.innerText);
                 }
             }
         }
     }
 
     function initialiseWangEditorInInlinedForms() {
         // 监听首页增加和修改按钮
```

### Comparing `django-wangeditor-1.0.2/wangeditor/urls.py` & `django-wangeditor-2.0.0/wangeditor/urls.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from __future__ import absolute_import
 
 from django.contrib.admin.views.decorators import staff_member_required  # 验证用户是否已登录
 from . import views
 try:
     from django.conf.urls import url
     urlpatterns = [
-        url(r'^upload/$', staff_member_required(views.upload), name='upload')
+        url(r'^img_upload/$', staff_member_required(views.img_upload), name='img_upload'),
+        url(r'^video_upload/$', staff_member_required(views.video_upload), name='video_upload')
     ]
 except ImportError:
     from django.urls import path
     urlpatterns = [
-        path('upload/', staff_member_required(views.upload), name='upload')
+        path('img_upload/', staff_member_required(views.img_upload), name='img_upload'),
+        path('video_upload/', staff_member_required(views.video_upload), name='video_upload')
     ]
```

