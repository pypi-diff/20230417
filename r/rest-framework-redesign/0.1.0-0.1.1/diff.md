# Comparing `tmp/rest_framework_redesign-0.1.0.tar.gz` & `tmp/rest_framework_redesign-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_framework_redesign-0.1.0.tar", max compression
+gzip compressed data, was "rest_framework_redesign-0.1.1.tar", max compression
```

## Comparing `rest_framework_redesign-0.1.0.tar` & `rest_framework_redesign-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.0/LICENSE
--rw-r--r--   0        0        0      620 2023-04-17 08:30:43.625510 rest_framework_redesign-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       85 2023-04-17 08:21:25.011142 rest_framework_redesign-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.0/rest_framework_redesign/__init__.py
--rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.0/rest_framework_redesign/admin.py
--rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.0/rest_framework_redesign/apps.py
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.0/rest_framework_redesign/migrations/__init__.py
--rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.0/rest_framework_redesign/models.py
--rw-r--r--   0        0        0    20040 2023-04-17 08:17:55.060391 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/api.html
--rw-r--r--   0        0        0      707 2023-04-15 12:47:58.113148 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      714 2023-04-15 12:46:54.902747 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      521 2023-04-16 12:17:54.556801 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0      835 2023-04-17 06:09:51.030141 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1536 2023-04-17 06:10:08.352256 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1096 2023-04-17 06:10:16.889823 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1448 2023-04-17 06:10:38.062218 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1205 2023-04-17 06:11:00.824317 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1239 2023-04-17 06:12:33.906413 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      813 2023-04-17 06:12:09.013201 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     4358 2023-04-17 06:11:41.318982 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      321 2023-04-15 06:53:33.457951 rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.0/rest_framework_redesign/tests.py
--rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.0/rest_framework_redesign/views.py
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.1/LICENSE
+-rw-r--r--   0        0        0      620 2023-04-17 10:46:17.091546 rest_framework_redesign-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      874 2023-04-17 10:54:06.143589 rest_framework_redesign-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.1/rest_framework_redesign/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.1/rest_framework_redesign/admin.py
+-rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.1/rest_framework_redesign/apps.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.1/rest_framework_redesign/migrations/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.1/rest_framework_redesign/models.py
+-rw-r--r--   0        0        0    20074 2023-04-17 10:42:53.173824 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/api.html
+-rw-r--r--   0        0        0      707 2023-04-15 12:47:58.113148 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      714 2023-04-15 12:46:54.902747 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      521 2023-04-16 12:17:54.556801 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0      835 2023-04-17 06:09:51.030141 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1536 2023-04-17 06:10:08.352256 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1096 2023-04-17 06:10:16.889823 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1448 2023-04-17 06:10:38.062218 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1205 2023-04-17 06:11:00.824317 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1239 2023-04-17 06:12:33.906413 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      813 2023-04-17 06:12:09.013201 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     4358 2023-04-17 06:11:41.318982 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      302 2023-04-17 10:44:35.187066 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.1/rest_framework_redesign/tests.py
+-rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.1/rest_framework_redesign/views.py
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.1/PKG-INFO
```

### Comparing `rest_framework_redesign-0.1.0/LICENSE` & `rest_framework_redesign-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.0/pyproject.toml` & `rest_framework_redesign-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rest-framework-redesign"
-version = "0.1.0"
+version = "0.1.1"
 description = "Redesign of the browsable api of Django REST Framework"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rest_framework_redesign"}]
 homepage = "https://github.com/youzarsiph/rest-framework-redesign/"
 repository = "https://github.com/youzarsiph/rest-framework-redesign/"
```

### Comparing `rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/api.html` & `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/api.html`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         <nav style="float: right">
           {% get_pagination_html paginator %}
         </nav>
       {% endif %}
     </section>
 
     {% block request_forms %}
-      <section class="d-flex align-items-center justify-content-end gap-4 mb-4" aria-label="{% translate 'Request form' %}">
+      <section class="d-grid d-md-flex align-items-lg-center justify-content-lg-end gap-4 mb-4" aria-label="{% translate 'Request form' %}">
         {% if 'GET' in allowed_methods %}
           <form id="get-form">
             <fieldset>
               {% if api_settings.URL_FORMAT_OVERRIDE %}
                 <div class="btn-group" role="group">
                   <a class="btn btn-lg btn-primary" href="{{ request.get_full_path }}" rel="nofollow"
                     title="Make a GET request on the {{ name }} resource">
@@ -175,24 +175,24 @@
               {% endif %}
             </fieldset>
           </form>
         {% endif %}
 
         {% if options_form %}
           <form class="button-form" action="{{ request.get_full_path }}" data-method="OPTIONS">
-            <button type="submit" class="btn btn-lg btn-secondary" title="Make an OPTIONS request on the {{ name }} resource">
+            <button type="submit" class="btn btn-lg btn-secondary w-100" title="Make an OPTIONS request on the {{ name }} resource">
               <strong>
                 {% translate "OPTIONS" %}
               </strong>
             </button>
           </form>
         {% endif %}
 
         {% if delete_form %}
-          <button type="button" class="btn btn-lg btn-danger" data-bs-toggle="modal" data-bs-target="#deleteModal"
+          <button type="button" class="btn btn-lg btn-danger w-100" data-bs-toggle="modal" data-bs-target="#deleteModal"
             title="Make a DELETE request on the {{ name }} resource">
             <strong>
               {% translate "DELETE" %}
             </strong>
           </button>
 
           <div class="modal fade" id="deleteModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
@@ -226,15 +226,15 @@
               </div>
             </div>
           </div>
         {% endif %}
 
         {% if extra_actions %}
           <div class="dropdown" style="float: right; margin-right: 10px">
-            <button class="btn btn-lg btn-info" id="extra-actions-menu" data-bs-toggle="dropdown" aria-haspopup="true"
+            <button class="btn btn-lg btn-info w-100" id="extra-actions-menu" data-bs-toggle="dropdown" aria-haspopup="true"
               aria-expanded="true">
               <strong>
                 {% translate "Extra Actions" %}
               </strong>
               <span class="caret"></span>
             </button>
             <ul class="dropdown-menu" aria-labelledby="extra-actions-menu">
```

### Comparing `rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/filters/base.html` & `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/filters/base.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/filters/ordering.html` & `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/filters/search.html` & `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html` & `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html` & `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/input.html` & `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/radio.html` & `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/select.html` & `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html` & `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html` & `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/login.html` & `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/login.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/pagination/numbers.html` & `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.0/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html` & `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

