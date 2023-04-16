# Comparing `tmp/django_upload_to-0.3.2.tar.gz` & `tmp/django_upload_to-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_upload_to-0.3.2.tar", max compression
+gzip compressed data, was "django_upload_to-0.3.3.tar", max compression
```

## Comparing `django_upload_to-0.3.2.tar` & `django_upload_to-0.3.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-04-16 03:55:31.942087 django_upload_to-0.3.2/LICENSE
--rw-r--r--   0        0        0     3173 2023-04-16 03:55:31.942087 django_upload_to-0.3.2/README.md
--rw-r--r--   0        0        0     2116 2023-04-16 03:55:31.942087 django_upload_to-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4502 2023-04-16 03:55:31.946087 django_upload_to-0.3.2/upload_to/__init__.py
--rw-r--r--   0        0        0     4001 1970-01-01 00:00:00.000000 django_upload_to-0.3.2/setup.py
--rw-r--r--   0        0        0     5014 1970-01-01 00:00:00.000000 django_upload_to-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-16 22:46:22.322270 django_upload_to-0.3.3/LICENSE
+-rw-r--r--   0        0        0     3173 2023-04-16 22:46:22.322270 django_upload_to-0.3.3/README.md
+-rw-r--r--   0        0        0     2056 2023-04-16 22:46:22.322270 django_upload_to-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4502 2023-04-16 22:46:22.322270 django_upload_to-0.3.3/upload_to/__init__.py
+-rw-r--r--   0        0        0     4001 1970-01-01 00:00:00.000000 django_upload_to-0.3.3/setup.py
+-rw-r--r--   0        0        0     4946 1970-01-01 00:00:00.000000 django_upload_to-0.3.3/PKG-INFO
```

### Comparing `django_upload_to-0.3.2/LICENSE` & `django_upload_to-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_upload_to-0.3.2/README.md` & `django_upload_to-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `django_upload_to-0.3.2/pyproject.toml` & `django_upload_to-0.3.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-upload-to"
-version = "0.3.2"
+version = "0.3.3"
 description = "It generates dynamically a directory path and a file name for Django FileField"
 authors = ["Valberto Carneiro <valbertovc@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/valbertovc/django-upload-to"
 classifiers=[
     "Development Status :: 4 - Beta",
     "Framework :: Django :: 2",
@@ -35,15 +35,14 @@
 ]
 include = [
 "LICENSE",
 ]
 
 [tool.poetry.urls]
 "Homepage" = "https://valbertovc.github.io/django-upload-to/"
-"Source" = "https://github.com/valbertovc/django-upload-to"
 "Bug Tracker" = "https://github.com/valbertovc/django-upload-to/issues"
 "Changelog" = "https://github.com/valbertovc/django-upload-to/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 Django = ">=2.2.0,>=3.0.0,>=4.0.0"
```

### Comparing `django_upload_to-0.3.2/upload_to/__init__.py` & `django_upload_to-0.3.3/upload_to/__init__.py`

 * *Files identical despite different names*

### Comparing `django_upload_to-0.3.2/setup.py` & `django_upload_to-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Django>=4.0.0']
 
 setup_kwargs = {
     'name': 'django-upload-to',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'It generates dynamically a directory path and a file name for Django FileField',
     'long_description': '# django-upload-to\n\n[![codecov](https://codecov.io/github/valbertovc/django-upload-to/branch/main/graph/badge.svg?token=2R5S5GTS0X)](https://codecov.io/github/valbertovc/django-upload-to)\n\nIt generates dynamically a directory path and a secure file name for Django FileField.\n\nMain options:\n- Ready to use generators.\n- Generate secure file name without especial characters.\n- Generate file name using a uuid value.\n- Dynamically generate paths from the model instance.\n- Generate paths using Python datetime formats.\n\n## Get started\nInstall the django-upload-to in your virtual environment\n```bash\n$ pip install django-upload-to\n```\nImport it in your models file and add it as a `upload_to` argument in the `FileField` \n```python\n# my_app/models.py\nfrom upload_to import UploadTo\nfrom django.db import models\n\n\nclass MyModel(models.Model):\n    attachment = models.FileField(upload_to=UploadTo("attachments"))\n```\nThe path and file name generated will be like this:\n```text\n"attachments/the-file-name-uploaded.pdf"\n```\n\n## How to use the ready-to-use classes\n\nConsider the scenario below:\n```python\nimport upload_to\nfrom django.db import models\n\n\nclass MyUser(models.Model):\n    username = models.CharField(...)\n    avatar = models.FileField(upload_to=<generator>)\n\ninstance = MyUser(username=\'user@email.com\')\n```\nReplace the `<generator>` fragment by the generators as showed below:\n#### File in root folder\n```python\n>>> generator = upload_to.UploadTo()\n>>> generator(instance, "file.pdf")\n"file.pdf"\n\n```\n#### Define a folder structure\n```python\n>>> generator = upload_to.UploadTo(prefix=["files", "documents"])\n>>> generator(instance, "file.pdf")\n"files/documents/file.pdf"\n```\n#### Generate a folder name using datetime formats from Python\n```python\n>>> generator = upload_to.UploadTo(prefix=["pictures", "%Y"])\n>>> generator(instance, "file.png")\n"pictures/2023/file.png"\n```\n#### Replace the file name by an hexadecimal uuid value\n```python\n# 4. replace file name by a uuid value\n>>> generator = upload_to.UuidUploadTo()\n>>> generator(instance, "file.pdf")\n"b189dfdf25e640b2ba5c497472c20962.pdf"\n```\n#### Generate the folder path using the instance\'s attributes\n```python\n>>> generator = upload_to.AttrUploadTo(attrs=["username"])\n>>> generator(instance, "file.pdf")\n"useremailcom/file.pdf"\n```\n#### Generate the folder path using the app_label and the model_name from the instance\'s meta options\n```python\n>>> generator = upload_to.ModelUploadTo()\n>>> generator(instance, "file.pdf")\n"my_app/user/file.pdf"\n```\n\n## Customize your upload paths\n\n```python\n# my_app/models.py\nimport upload_to\nfrom django.db import models\n\n\ndef my_upload_generator(instance, filename):\n    filename = upload_to.uuid_filename(filename)\n    path = upload_to.options_from_instance(instance)\n    return upload_to.upload_to(path, filename)\n\nclass MyProfile(models.Model):\n    user = models.OneToOneField(...)\n    avatar = models.FileField(upload_to=my_upload_generator)\n```\n\n## Useful links\n\n1. [Documentation](https://valbertovc.github.io/django-upload-to/)\n2. [Changelog](https://github.com/valbertovc/django-upload-to/releases)\n3. [PyPi Page](https://pypi.org/project/django-upload-to/)',
     'author': 'Valberto Carneiro',
     'author_email': 'valbertovc@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/valbertovc/django-upload-to',
```

### Comparing `django_upload_to-0.3.2/PKG-INFO` & `django_upload_to-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-upload-to
-Version: 0.3.2
+Version: 0.3.3
 Summary: It generates dynamically a directory path and a file name for Django FileField
 Home-page: https://github.com/valbertovc/django-upload-to
 Keywords: django,file,media,upload
 Author: Valberto Carneiro
 Author-email: valbertovc@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 4 - Beta
@@ -31,15 +31,14 @@
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: Django (>=4.0.0)
 Project-URL: Bug Tracker, https://github.com/valbertovc/django-upload-to/issues
 Project-URL: Changelog, https://github.com/valbertovc/django-upload-to/releases
 Project-URL: Homepage, https://valbertovc.github.io/django-upload-to/
 Project-URL: Repository, https://github.com/valbertovc/django-upload-to
-Project-URL: Source, https://github.com/valbertovc/django-upload-to
 Description-Content-Type: text/markdown
 
 # django-upload-to
 
 [![codecov](https://codecov.io/github/valbertovc/django-upload-to/branch/main/graph/badge.svg?token=2R5S5GTS0X)](https://codecov.io/github/valbertovc/django-upload-to)
 
 It generates dynamically a directory path and a secure file name for Django FileField.
```

