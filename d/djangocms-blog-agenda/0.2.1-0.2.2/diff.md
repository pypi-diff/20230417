# Comparing `tmp/djangocms-blog-agenda-0.2.1.tar.gz` & `tmp/djangocms-blog-agenda-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-blog-agenda-0.2.1.tar", last modified: Tue Apr  4 09:39:29 2023, max compression
+gzip compressed data, was "djangocms-blog-agenda-0.2.2.tar", last modified: Mon Apr 17 14:06:16 2023, max compression
```

## Comparing `djangocms-blog-agenda-0.2.1.tar` & `djangocms-blog-agenda-0.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-04 09:39:29.979495 djangocms-blog-agenda-0.2.1/
--rw-r--r--   0 kapt       (501)       20       45 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.1/AUTHORS.md
--rw-r--r--   0 kapt       (501)       20     1318 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.1/CONTRIBUTING.md
--rw-r--r--   0 kapt       (501)       20    35149 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.1/LICENSE
--rw-r--r--   0 kapt       (501)       20      159 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.1/MANIFEST.in
--rw-r--r--   0 kapt       (501)       20     3435 2023-04-04 09:39:29.979495 djangocms-blog-agenda-0.2.1/PKG-INFO
--rw-r--r--   0 kapt       (501)       20     2682 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.1/README.md
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-04 09:39:29.972495 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/
--rw-r--r--   0 kapt       (501)       20        0 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/__init__.py
--rw-r--r--   0 kapt       (501)       20     1972 2023-04-04 09:28:02.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/admin.py
--rw-r--r--   0 kapt       (501)       20     1746 2023-03-31 09:10:44.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/apps.py
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-04 09:39:29.967495 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/locale/
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-04 09:39:29.967495 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/locale/fr/
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-04 09:39:29.976495 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/locale/fr/LC_MESSAGES/
--rw-r--r--   0 kapt       (501)       20     1325 2023-03-30 12:04:15.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 kapt       (501)       20     2841 2023-03-30 12:04:02.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-04 09:39:29.977495 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/migrations/
--rw-r--r--   0 kapt       (501)       20     1076 2023-03-30 10:38:48.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/migrations/0001_initial.py
--rw-r--r--   0 kapt       (501)       20     1139 2023-03-30 14:50:16.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py
--rw-r--r--   0 kapt       (501)       20        0 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/migrations/__init__.py
--rw-r--r--   0 kapt       (501)       20      765 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/misc.py
--rw-r--r--   0 kapt       (501)       20      700 2023-03-31 09:16:37.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/models.py
--rw-r--r--   0 kapt       (501)       20     1115 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/patched_urls.py
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-04 09:39:29.967495 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/templates/
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-04 09:39:29.979495 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/
--rw-r--r--   0 kapt       (501)       20     1341 2023-03-30 10:37:22.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html
--rw-r--r--   0 kapt       (501)       20     1742 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html
--rw-r--r--   0 kapt       (501)       20     1361 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html
--rw-r--r--   0 kapt       (501)       20     1889 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html
--rw-r--r--   0 kapt       (501)       20     1284 2023-04-04 09:27:19.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/views.py
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-04 09:39:29.975495 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda.egg-info/
--rw-r--r--   0 kapt       (501)       20     3435 2023-04-04 09:39:29.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda.egg-info/PKG-INFO
--rw-r--r--   0 kapt       (501)       20     1065 2023-04-04 09:39:29.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda.egg-info/SOURCES.txt
--rw-r--r--   0 kapt       (501)       20        1 2023-04-04 09:39:29.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda.egg-info/dependency_links.txt
--rw-r--r--   0 kapt       (501)       20       15 2023-04-04 09:39:29.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda.egg-info/requires.txt
--rw-r--r--   0 kapt       (501)       20       22 2023-04-04 09:39:29.000000 djangocms-blog-agenda-0.2.1/djangocms_blog_agenda.egg-info/top_level.txt
--rw-r--r--   0 kapt       (501)       20      786 2023-04-04 09:39:29.980495 djangocms-blog-agenda-0.2.1/setup.cfg
--rw-r--r--   0 kapt       (501)       20       53 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.1/setup.py
+drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 14:06:16.856130 djangocms-blog-agenda-0.2.2/
+-rw-r--r--   0 kapt       (501)       20       45 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.2/AUTHORS.md
+-rw-r--r--   0 kapt       (501)       20     1318 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.2/CONTRIBUTING.md
+-rw-r--r--   0 kapt       (501)       20    35149 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.2/LICENSE
+-rw-r--r--   0 kapt       (501)       20      159 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.2/MANIFEST.in
+-rw-r--r--   0 kapt       (501)       20     3435 2023-04-17 14:06:16.856130 djangocms-blog-agenda-0.2.2/PKG-INFO
+-rw-r--r--   0 kapt       (501)       20     2682 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.2/README.md
+drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 14:06:16.853130 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/
+-rw-r--r--   0 kapt       (501)       20        0 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/__init__.py
+-rw-r--r--   0 kapt       (501)       20     1972 2023-04-04 09:28:02.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/admin.py
+-rw-r--r--   0 kapt       (501)       20     1746 2023-03-31 09:10:44.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/apps.py
+drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 14:06:16.850130 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/locale/
+drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 14:06:16.851130 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/locale/fr/
+drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 14:06:16.854130 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 kapt       (501)       20     1345 2023-04-17 13:58:32.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 kapt       (501)       20     2940 2023-04-17 13:58:32.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 14:06:16.855130 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/migrations/
+-rw-r--r--   0 kapt       (501)       20     1076 2023-03-30 10:38:48.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/migrations/0001_initial.py
+-rw-r--r--   0 kapt       (501)       20     1139 2023-03-30 14:50:16.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py
+-rw-r--r--   0 kapt       (501)       20        0 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/migrations/__init__.py
+-rw-r--r--   0 kapt       (501)       20      765 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/misc.py
+-rw-r--r--   0 kapt       (501)       20      700 2023-03-31 09:16:37.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/models.py
+-rw-r--r--   0 kapt       (501)       20      672 2023-04-17 13:58:19.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/patched_urls.py
+drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 14:06:16.851130 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/templates/
+drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 14:06:16.855130 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/
+-rw-r--r--   0 kapt       (501)       20     1341 2023-03-30 10:37:22.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html
+-rw-r--r--   0 kapt       (501)       20     1742 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html
+-rw-r--r--   0 kapt       (501)       20     1361 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html
+-rw-r--r--   0 kapt       (501)       20     1889 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html
+-rw-r--r--   0 kapt       (501)       20     1284 2023-04-04 09:27:19.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/views.py
+drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 14:06:16.854130 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda.egg-info/
+-rw-r--r--   0 kapt       (501)       20     3435 2023-04-17 14:06:16.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda.egg-info/PKG-INFO
+-rw-r--r--   0 kapt       (501)       20     1065 2023-04-17 14:06:16.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda.egg-info/SOURCES.txt
+-rw-r--r--   0 kapt       (501)       20        1 2023-04-17 14:06:16.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda.egg-info/dependency_links.txt
+-rw-r--r--   0 kapt       (501)       20       15 2023-04-17 14:06:16.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda.egg-info/requires.txt
+-rw-r--r--   0 kapt       (501)       20       22 2023-04-17 14:06:16.000000 djangocms-blog-agenda-0.2.2/djangocms_blog_agenda.egg-info/top_level.txt
+-rw-r--r--   0 kapt       (501)       20      786 2023-04-17 14:06:16.857130 djangocms-blog-agenda-0.2.2/setup.cfg
+-rw-r--r--   0 kapt       (501)       20       53 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.2.2/setup.py
```

### Comparing `djangocms-blog-agenda-0.2.1/CONTRIBUTING.md` & `djangocms-blog-agenda-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.2.1/LICENSE` & `djangocms-blog-agenda-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.2.1/PKG-INFO` & `djangocms-blog-agenda-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-blog-agenda
-Version: 0.2.1
+Version: 0.2.2
 Summary: Create an agenda on top of djangocms-blog!
 Home-page: https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 Author: Corentin Bettiol
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django CMS
```

### Comparing `djangocms-blog-agenda-0.2.1/README.md` & `djangocms-blog-agenda-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/admin.py` & `djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/apps.py` & `djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/apps.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo` & `djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo`

 * *Files 17% similar despite different names*

#### msgunfmt {}

```diff
@@ -52,24 +52,25 @@
 
 msgid "SEO"
 msgstr "SEO"
 
 msgid "Tag"
 msgstr "Tag"
 
+msgctxt "agenda_view_url"
+msgid "archives/"
+msgstr "archives/"
+
 msgid "by"
 msgstr "par"
 
 msgid "next"
 msgstr "suivant"
 
 msgid "of"
 msgstr "sur"
 
-msgid "past/"
-msgstr "archives/"
-
 msgid "previous"
 msgstr "précédent"
 
 msgid "read more"
 msgstr "lire la suite"
```

### Comparing `djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po` & `djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -4,59 +4,60 @@
 # DEV KAPT <dev@kapt.mobi>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-30 14:01+0200\n"
+"POT-Creation-Date: 2023-04-17 15:56+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: djangocms_blog_agenda/admin.py:22 djangocms_blog_agenda/admin.py:23
-#: djangocms_blog_agenda/models.py:14 djangocms_blog_agenda/models.py:18
+#: djangocms_blog_agenda/models.py:17 djangocms_blog_agenda/models.py:21
 msgid "Event infos"
 msgstr "Informations sur l'événement"
 
-#: djangocms_blog_agenda/admin.py:39
+#: djangocms_blog_agenda/admin.py:41
 msgid "Info"
 msgstr "Information"
 
-#: djangocms_blog_agenda/admin.py:50
+#: djangocms_blog_agenda/admin.py:52
 msgid "Images"
 msgstr "Images"
 
-#: djangocms_blog_agenda/admin.py:57
+#: djangocms_blog_agenda/admin.py:59
 msgid "SEO"
 msgstr "SEO"
 
 #: djangocms_blog_agenda/models.py:8
 msgid "Event start"
 msgstr "Début de l’événement"
 
 #: djangocms_blog_agenda/models.py:10
 msgid "Event end"
 msgstr "Fin de l’événement"
 
-#: djangocms_blog_agenda/models.py:10
+#: djangocms_blog_agenda/models.py:13
 msgid "If the event is held over several days"
 msgstr "Si l’événement se tient sur plusieurs jours"
 
-#: djangocms_blog_agenda/models.py:15
+#: djangocms_blog_agenda/models.py:18
 msgid "Events infos"
 msgstr "Informations sur les événements"
 
-#: djangocms_blog_agenda/patched_urls.py:27
-msgid "past/"
+#: djangocms_blog_agenda/patched_urls.py:13
+msgctxt "agenda_view_url"
+msgid "archives/"
 msgstr "archives/"
 
 #: djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html:6
 msgid "by"
 msgstr "par"
 
 #: djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html:32
@@ -98,7 +99,11 @@
 #: djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html:32
 msgid "of"
 msgstr "sur"
 
 #: djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html:35
 msgid "next"
 msgstr "suivant"
+
+#~ msgctxt "agenda_view_url"
+#~ msgid "past/"
+#~ msgstr "archives/"
```

### Comparing `djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/migrations/0001_initial.py` & `djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py` & `djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/misc.py` & `djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/misc.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/models.py` & `djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html` & `djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html` & `djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html` & `djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html` & `djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.2.1/djangocms_blog_agenda/views.py` & `djangocms-blog-agenda-0.2.2/djangocms_blog_agenda/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.2.1/djangocms_blog_agenda.egg-info/PKG-INFO` & `djangocms-blog-agenda-0.2.2/djangocms_blog_agenda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-blog-agenda
-Version: 0.2.1
+Version: 0.2.2
 Summary: Create an agenda on top of djangocms-blog!
 Home-page: https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 Author: Corentin Bettiol
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django CMS
```

### Comparing `djangocms-blog-agenda-0.2.1/djangocms_blog_agenda.egg-info/SOURCES.txt` & `djangocms-blog-agenda-0.2.2/djangocms_blog_agenda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.2.1/setup.cfg` & `djangocms-blog-agenda-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangocms-blog-agenda
-version = 0.2.1
+version = 0.2.2
 description = Create an agenda on top of djangocms-blog!
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 author = Corentin Bettiol
 author_email = dev@kapt.mobi
 classifiers =
```

