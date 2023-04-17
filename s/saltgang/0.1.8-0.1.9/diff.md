# Comparing `tmp/saltgang-0.1.8.tar.gz` & `tmp/saltgang-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saltgang-0.1.8.tar", last modified: Sun Apr 17 02:10:02 2022, max compression
+gzip compressed data, was "saltgang-0.1.9.tar", last modified: Sun Apr 17 03:00:23 2022, max compression
```

## Comparing `saltgang-0.1.8.tar` & `saltgang-0.1.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 02:10:02.380900 saltgang-0.1.8/
--rw-r--r--   0 mtm        (501) staff       (20)     7294 2022-04-06 02:28:40.000000 saltgang-0.1.8/.cirrus.yml
--rw-r--r--   0 mtm        (501) staff       (20)      591 2022-04-06 02:28:40.000000 saltgang-0.1.8/.coveragerc
--rw-r--r--   0 mtm        (501) staff       (20)      550 2022-04-06 02:28:40.000000 saltgang-0.1.8/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       56 2022-04-06 02:28:40.000000 saltgang-0.1.8/.isort.cfg
--rw-r--r--   0 mtm        (501) staff       (20)     1330 2022-04-06 02:28:40.000000 saltgang-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 mtm        (501) staff       (20)      490 2022-04-06 02:28:40.000000 saltgang-0.1.8/.readthedocs.yml
--rw-r--r--   0 mtm        (501) staff       (20)       87 2022-04-06 02:28:40.000000 saltgang-0.1.8/AUTHORS.rst
--rw-r--r--   0 mtm        (501) staff       (20)      128 2022-04-06 02:28:40.000000 saltgang-0.1.8/CHANGELOG.rst
--rw-r--r--   0 mtm        (501) staff       (20)    13836 2022-04-06 02:28:40.000000 saltgang-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 mtm        (501) staff       (20)    15922 2022-04-06 02:28:40.000000 saltgang-0.1.8/LICENSE.txt
--rw-r--r--   0 mtm        (501) staff       (20)     2552 2022-04-17 02:10:02.381311 saltgang-0.1.8/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)     2069 2022-04-06 02:28:40.000000 saltgang-0.1.8/README.rst
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 02:10:02.320814 saltgang-0.1.8/docs/
--rw-r--r--   0 mtm        (501) staff       (20)     1154 2022-04-06 02:28:40.000000 saltgang-0.1.8/docs/Makefile
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 02:10:02.321461 saltgang-0.1.8/docs/_static/
--rw-r--r--   0 mtm        (501) staff       (20)       18 2022-04-06 02:28:40.000000 saltgang-0.1.8/docs/_static/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       41 2022-04-06 02:28:40.000000 saltgang-0.1.8/docs/authors.rst
--rw-r--r--   0 mtm        (501) staff       (20)       43 2022-04-06 02:28:40.000000 saltgang-0.1.8/docs/changelog.rst
--rw-r--r--   0 mtm        (501) staff       (20)     9737 2022-04-06 02:28:40.000000 saltgang-0.1.8/docs/conf.py
--rw-r--r--   0 mtm        (501) staff       (20)       33 2022-04-06 02:28:40.000000 saltgang-0.1.8/docs/contributing.rst
--rw-r--r--   0 mtm        (501) staff       (20)     2317 2022-04-06 02:28:40.000000 saltgang-0.1.8/docs/index.rst
--rw-r--r--   0 mtm        (501) staff       (20)       67 2022-04-06 02:28:40.000000 saltgang-0.1.8/docs/license.rst
--rw-r--r--   0 mtm        (501) staff       (20)       39 2022-04-06 02:28:40.000000 saltgang-0.1.8/docs/readme.rst
--rw-r--r--   0 mtm        (501) staff       (20)      233 2022-04-06 02:28:40.000000 saltgang-0.1.8/docs/requirements.txt
--rw-r--r--   0 mtm        (501) staff       (20)      355 2022-04-06 02:28:40.000000 saltgang-0.1.8/pyproject.toml
--rw-r--r--   0 mtm        (501) staff       (20)     1462 2022-04-17 02:10:02.383257 saltgang-0.1.8/setup.cfg
--rw-r--r--   0 mtm        (501) staff       (20)      705 2022-04-06 02:28:40.000000 saltgang-0.1.8/setup.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 02:10:02.291013 saltgang-0.1.8/src/
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 02:10:02.332826 saltgang-0.1.8/src/saltgang/
--rw-r--r--   0 mtm        (501) staff       (20)      577 2022-04-06 02:28:40.000000 saltgang-0.1.8/src/saltgang/__init__.py
--rw-r--r--   0 mtm        (501) staff       (20)     1225 2022-04-10 15:55:25.000000 saltgang-0.1.8/src/saltgang/args.py
--rw-r--r--   0 mtm        (501) staff       (20)      459 2022-04-11 14:08:23.000000 saltgang-0.1.8/src/saltgang/common.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 02:10:02.341983 saltgang-0.1.8/src/saltgang/conf/
--rw-r--r--   0 mtm        (501) staff       (20)      758 2022-04-17 00:45:31.000000 saltgang-0.1.8/src/saltgang/conf/config.yml
--rw-r--r--   0 mtm        (501) staff       (20)     1729 2022-04-17 02:03:09.000000 saltgang-0.1.8/src/saltgang/conf.py
--rw-r--r--   0 mtm        (501) staff       (20)     2588 2022-04-17 02:07:09.000000 saltgang-0.1.8/src/saltgang/encassist.py
--rw-r--r--   0 mtm        (501) staff       (20)     4232 2022-04-10 16:09:55.000000 saltgang-0.1.8/src/saltgang/fetch.py
--rw-r--r--   0 mtm        (501) staff       (20)      249 2022-04-11 15:22:53.000000 saltgang-0.1.8/src/saltgang/logger.py
--rw-r--r--   0 mtm        (501) staff       (20)     1467 2022-04-17 01:34:16.000000 saltgang-0.1.8/src/saltgang/main.py
--rw-r--r--   0 mtm        (501) staff       (20)     2433 2022-04-11 14:09:29.000000 saltgang-0.1.8/src/saltgang/meta.py
--rw-r--r--   0 mtm        (501) staff       (20)     7126 2022-04-11 14:09:29.000000 saltgang-0.1.8/src/saltgang/panel.py
--rw-r--r--   0 mtm        (501) staff       (20)      322 2022-04-06 02:28:40.000000 saltgang-0.1.8/src/saltgang/project.py
--rw-r--r--   0 mtm        (501) staff       (20)     6910 2022-04-11 14:09:29.000000 saltgang-0.1.8/src/saltgang/quickstart.py
--rw-r--r--   0 mtm        (501) staff       (20)     2978 2022-04-11 14:09:29.000000 saltgang-0.1.8/src/saltgang/settings.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 02:10:02.378444 saltgang-0.1.8/src/saltgang/templates/
--rw-r--r--   0 mtm        (501) staff       (20)      535 2022-04-06 02:28:40.000000 saltgang-0.1.8/src/saltgang/templates/c.tmpl
--rw-r--r--   0 mtm        (501) staff       (20)     1478 2022-04-06 02:28:40.000000 saltgang-0.1.8/src/saltgang/templates/go.tmpl
--rw-r--r--   0 mtm        (501) staff       (20)      344 2022-04-06 02:28:40.000000 saltgang-0.1.8/src/saltgang/templates/ini.tmpl
--rw-r--r--   0 mtm        (501) staff       (20)      356 2022-04-06 02:28:40.000000 saltgang-0.1.8/src/saltgang/templates/ini2.tmpl
--rw-r--r--   0 mtm        (501) staff       (20)      630 2022-04-06 02:28:40.000000 saltgang-0.1.8/src/saltgang/templates/ini_check.tmpl
--rw-r--r--   0 mtm        (501) staff       (20)      142 2022-04-06 02:28:40.000000 saltgang-0.1.8/src/saltgang/templates/view4.tmpl
--rw-r--r--   0 mtm        (501) staff       (20)      153 2022-04-06 02:28:40.000000 saltgang-0.1.8/src/saltgang/templates/view5.tmpl
--rw-r--r--   0 mtm        (501) staff       (20)      209 2022-04-06 02:28:40.000000 saltgang-0.1.8/src/saltgang/templates/view7.tmpl
--rw-r--r--   0 mtm        (501) staff       (20)     2347 2022-04-17 01:34:01.000000 saltgang-0.1.8/src/saltgang/ytt.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 02:10:02.338951 saltgang-0.1.8/src/saltgang.egg-info/
--rw-r--r--   0 mtm        (501) staff       (20)     2552 2022-04-17 02:10:01.000000 saltgang-0.1.8/src/saltgang.egg-info/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)     1283 2022-04-17 02:10:02.000000 saltgang-0.1.8/src/saltgang.egg-info/SOURCES.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2022-04-17 02:10:01.000000 saltgang-0.1.8/src/saltgang.egg-info/dependency_links.txt
--rw-r--r--   0 mtm        (501) staff       (20)       47 2022-04-17 02:10:01.000000 saltgang-0.1.8/src/saltgang.egg-info/entry_points.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2022-02-12 21:04:41.000000 saltgang-0.1.8/src/saltgang.egg-info/not-zip-safe
--rw-r--r--   0 mtm        (501) staff       (20)      285 2022-04-17 02:10:02.000000 saltgang-0.1.8/src/saltgang.egg-info/requires.txt
--rw-r--r--   0 mtm        (501) staff       (20)        9 2022-04-17 02:10:02.000000 saltgang-0.1.8/src/saltgang.egg-info/top_level.txt
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 02:10:02.380207 saltgang-0.1.8/tests/
--rw-r--r--   0 mtm        (501) staff       (20)      276 2022-04-06 02:28:40.000000 saltgang-0.1.8/tests/conftest.py
--rw-r--r--   0 mtm        (501) staff       (20)      596 2022-04-06 02:28:40.000000 saltgang-0.1.8/tests/test_skeleton.py
--rw-r--r--   0 mtm        (501) staff       (20)     2007 2022-04-06 02:28:40.000000 saltgang-0.1.8/tox.ini
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 03:00:23.525036 saltgang-0.1.9/
+-rw-r--r--   0 mtm        (501) staff       (20)     7294 2022-04-06 02:28:40.000000 saltgang-0.1.9/.cirrus.yml
+-rw-r--r--   0 mtm        (501) staff       (20)      591 2022-04-06 02:28:40.000000 saltgang-0.1.9/.coveragerc
+-rw-r--r--   0 mtm        (501) staff       (20)      550 2022-04-06 02:28:40.000000 saltgang-0.1.9/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       56 2022-04-06 02:28:40.000000 saltgang-0.1.9/.isort.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)     1330 2022-04-06 02:28:40.000000 saltgang-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 mtm        (501) staff       (20)      490 2022-04-06 02:28:40.000000 saltgang-0.1.9/.readthedocs.yml
+-rw-r--r--   0 mtm        (501) staff       (20)       87 2022-04-06 02:28:40.000000 saltgang-0.1.9/AUTHORS.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      128 2022-04-06 02:28:40.000000 saltgang-0.1.9/CHANGELOG.rst
+-rw-r--r--   0 mtm        (501) staff       (20)    13836 2022-04-06 02:28:40.000000 saltgang-0.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 mtm        (501) staff       (20)    15922 2022-04-06 02:28:40.000000 saltgang-0.1.9/LICENSE.txt
+-rw-r--r--   0 mtm        (501) staff       (20)     2552 2022-04-17 03:00:23.525275 saltgang-0.1.9/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)     2069 2022-04-06 02:28:40.000000 saltgang-0.1.9/README.rst
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 03:00:23.508925 saltgang-0.1.9/docs/
+-rw-r--r--   0 mtm        (501) staff       (20)     1154 2022-04-06 02:28:40.000000 saltgang-0.1.9/docs/Makefile
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 03:00:23.509476 saltgang-0.1.9/docs/_static/
+-rw-r--r--   0 mtm        (501) staff       (20)       18 2022-04-06 02:28:40.000000 saltgang-0.1.9/docs/_static/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       41 2022-04-06 02:28:40.000000 saltgang-0.1.9/docs/authors.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       43 2022-04-06 02:28:40.000000 saltgang-0.1.9/docs/changelog.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     9737 2022-04-06 02:28:40.000000 saltgang-0.1.9/docs/conf.py
+-rw-r--r--   0 mtm        (501) staff       (20)       33 2022-04-06 02:28:40.000000 saltgang-0.1.9/docs/contributing.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     2317 2022-04-06 02:28:40.000000 saltgang-0.1.9/docs/index.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       67 2022-04-06 02:28:40.000000 saltgang-0.1.9/docs/license.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       39 2022-04-06 02:28:40.000000 saltgang-0.1.9/docs/readme.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      233 2022-04-06 02:28:40.000000 saltgang-0.1.9/docs/requirements.txt
+-rw-r--r--   0 mtm        (501) staff       (20)      355 2022-04-06 02:28:40.000000 saltgang-0.1.9/pyproject.toml
+-rw-r--r--   0 mtm        (501) staff       (20)     1462 2022-04-17 03:00:23.526377 saltgang-0.1.9/setup.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)      705 2022-04-06 02:28:40.000000 saltgang-0.1.9/setup.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 03:00:23.496068 saltgang-0.1.9/src/
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 03:00:23.514627 saltgang-0.1.9/src/saltgang/
+-rw-r--r--   0 mtm        (501) staff       (20)      577 2022-04-06 02:28:40.000000 saltgang-0.1.9/src/saltgang/__init__.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1225 2022-04-10 15:55:25.000000 saltgang-0.1.9/src/saltgang/args.py
+-rw-r--r--   0 mtm        (501) staff       (20)      459 2022-04-11 14:08:23.000000 saltgang-0.1.9/src/saltgang/common.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 03:00:23.518794 saltgang-0.1.9/src/saltgang/conf/
+-rw-r--r--   0 mtm        (501) staff       (20)      758 2022-04-17 02:40:10.000000 saltgang-0.1.9/src/saltgang/conf/config.yml
+-rw-r--r--   0 mtm        (501) staff       (20)     1691 2022-04-17 02:29:35.000000 saltgang-0.1.9/src/saltgang/conf.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2688 2022-04-17 02:54:08.000000 saltgang-0.1.9/src/saltgang/encassist.py
+-rw-r--r--   0 mtm        (501) staff       (20)     4232 2022-04-10 16:09:55.000000 saltgang-0.1.9/src/saltgang/fetch.py
+-rw-r--r--   0 mtm        (501) staff       (20)      249 2022-04-11 15:22:53.000000 saltgang-0.1.9/src/saltgang/logger.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1467 2022-04-17 01:34:16.000000 saltgang-0.1.9/src/saltgang/main.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2433 2022-04-11 14:09:29.000000 saltgang-0.1.9/src/saltgang/meta.py
+-rw-r--r--   0 mtm        (501) staff       (20)     7126 2022-04-11 14:09:29.000000 saltgang-0.1.9/src/saltgang/panel.py
+-rw-r--r--   0 mtm        (501) staff       (20)      322 2022-04-06 02:28:40.000000 saltgang-0.1.9/src/saltgang/project.py
+-rw-r--r--   0 mtm        (501) staff       (20)     6910 2022-04-11 14:09:29.000000 saltgang-0.1.9/src/saltgang/quickstart.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2978 2022-04-11 14:09:29.000000 saltgang-0.1.9/src/saltgang/settings.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 03:00:23.523793 saltgang-0.1.9/src/saltgang/templates/
+-rw-r--r--   0 mtm        (501) staff       (20)      535 2022-04-06 02:28:40.000000 saltgang-0.1.9/src/saltgang/templates/c.tmpl
+-rw-r--r--   0 mtm        (501) staff       (20)     1478 2022-04-06 02:28:40.000000 saltgang-0.1.9/src/saltgang/templates/go.tmpl
+-rw-r--r--   0 mtm        (501) staff       (20)      344 2022-04-06 02:28:40.000000 saltgang-0.1.9/src/saltgang/templates/ini.tmpl
+-rw-r--r--   0 mtm        (501) staff       (20)      356 2022-04-06 02:28:40.000000 saltgang-0.1.9/src/saltgang/templates/ini2.tmpl
+-rw-r--r--   0 mtm        (501) staff       (20)      630 2022-04-06 02:28:40.000000 saltgang-0.1.9/src/saltgang/templates/ini_check.tmpl
+-rw-r--r--   0 mtm        (501) staff       (20)      142 2022-04-06 02:28:40.000000 saltgang-0.1.9/src/saltgang/templates/view4.tmpl
+-rw-r--r--   0 mtm        (501) staff       (20)      153 2022-04-06 02:28:40.000000 saltgang-0.1.9/src/saltgang/templates/view5.tmpl
+-rw-r--r--   0 mtm        (501) staff       (20)      209 2022-04-06 02:28:40.000000 saltgang-0.1.9/src/saltgang/templates/view7.tmpl
+-rw-r--r--   0 mtm        (501) staff       (20)     2347 2022-04-17 02:56:03.000000 saltgang-0.1.9/src/saltgang/ytt.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 03:00:23.517939 saltgang-0.1.9/src/saltgang.egg-info/
+-rw-r--r--   0 mtm        (501) staff       (20)     2552 2022-04-17 03:00:22.000000 saltgang-0.1.9/src/saltgang.egg-info/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)     1283 2022-04-17 03:00:23.000000 saltgang-0.1.9/src/saltgang.egg-info/SOURCES.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2022-04-17 03:00:22.000000 saltgang-0.1.9/src/saltgang.egg-info/dependency_links.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       47 2022-04-17 03:00:23.000000 saltgang-0.1.9/src/saltgang.egg-info/entry_points.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2022-02-12 21:04:41.000000 saltgang-0.1.9/src/saltgang.egg-info/not-zip-safe
+-rw-r--r--   0 mtm        (501) staff       (20)      285 2022-04-17 03:00:23.000000 saltgang-0.1.9/src/saltgang.egg-info/requires.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        9 2022-04-17 03:00:23.000000 saltgang-0.1.9/src/saltgang.egg-info/top_level.txt
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2022-04-17 03:00:23.524740 saltgang-0.1.9/tests/
+-rw-r--r--   0 mtm        (501) staff       (20)      276 2022-04-06 02:28:40.000000 saltgang-0.1.9/tests/conftest.py
+-rw-r--r--   0 mtm        (501) staff       (20)      596 2022-04-06 02:28:40.000000 saltgang-0.1.9/tests/test_skeleton.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2007 2022-04-06 02:28:40.000000 saltgang-0.1.9/tox.ini
```

### Comparing `saltgang-0.1.8/.cirrus.yml` & `saltgang-0.1.9/.cirrus.yml`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/.coveragerc` & `saltgang-0.1.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/.gitignore` & `saltgang-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/.pre-commit-config.yaml` & `saltgang-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/CONTRIBUTING.rst` & `saltgang-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/LICENSE.txt` & `saltgang-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/PKG-INFO` & `saltgang-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saltgang
-Version: 0.1.8
+Version: 0.1.9
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MPL-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `saltgang-0.1.8/README.rst` & `saltgang-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/docs/Makefile` & `saltgang-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/docs/conf.py` & `saltgang-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/docs/index.rst` & `saltgang-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/setup.cfg` & `saltgang-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/setup.py` & `saltgang-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/src/saltgang/__init__.py` & `saltgang-0.1.9/src/saltgang/__init__.py`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/src/saltgang/args.py` & `saltgang-0.1.9/src/saltgang/args.py`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/src/saltgang/conf/config.yml` & `saltgang-0.1.9/src/saltgang/conf/config.yml`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/src/saltgang/conf.py` & `saltgang-0.1.9/src/saltgang/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,18 +31,16 @@
         _logger.debug(f"{path} has digest {digest}")
         return digest
 
     return doit(conf1) != doit(conf2)
 
 
 def get_deployed_conf():
-    p1 = platformdirs.user_data_dir(appname, appauthor)
-    basedir = pathlib.Path(p1)
-    conf = basedir / get_package_conf().name
-    return conf
+    dd = platformdirs.user_data_dir(appname, appauthor)
+    return pathlib.Path(dd) / get_package_conf().name
 
 
 def get_package_conf():
     PACKAGE_CONF_DIR = pathlib.Path(pkg_resources.resource_filename(package, "conf/"))
     conf_fname = "config.yml"
     return PACKAGE_CONF_DIR / conf_fname
```

### Comparing `saltgang-0.1.8/src/saltgang/encassist.py` & `saltgang-0.1.9/src/saltgang/encassist.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,16 +22,16 @@
         ),
     )
     parser.add_argument(
         "--conf",
         help="path to config.yml",
     )
     parser.add_argument(
-        "--yaml-path",
-        help="provide the path to encassist yaml file",
+        "--outpath",
+        help="provide the path to where to write the resulting encassist yaml file",
     )
 
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument("--macos", action="store_true")
     group.add_argument("--linux", action="store_true")
     group.add_argument("--win-avid", action="store_true")
     group.add_argument("--win-universal", action="store_true")
@@ -70,23 +70,25 @@
     if not conf_path.exists():
         confmod.main(args)
 
     _logger.info(f"reading {conf_path}")
     conf = OmegaConf.load(conf_path)
 
     values = conf.sku[sku].value_paths
-    outpath = conf.sku[sku].outpath
+
+    o = args.outpath if args.outpath else conf.sku[sku].outpath
+    conf.sku[sku].outpath = o
 
     b = args.config_basedir if args.config_basedir else conf.common.configdir
     conf.common.configdir = b
 
     ytt_params = yttmod.YttParams(
         main=conf.common.main,
         values=values,
-        outpath=outpath,
+        outpath=conf.sku[sku].outpath,
     )
 
     _logger.debug(ytt_params)
     ytt = yttmod.Ytt(ytt_params)
 
     if not yttmod.Ytt.check_installed():
         _logger.fatal("Can't find ytt")
```

### Comparing `saltgang-0.1.8/src/saltgang/fetch.py` & `saltgang-0.1.9/src/saltgang/fetch.py`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/src/saltgang/main.py` & `saltgang-0.1.9/src/saltgang/main.py`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/src/saltgang/meta.py` & `saltgang-0.1.9/src/saltgang/meta.py`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/src/saltgang/panel.py` & `saltgang-0.1.9/src/saltgang/panel.py`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/src/saltgang/quickstart.py` & `saltgang-0.1.9/src/saltgang/quickstart.py`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/src/saltgang/settings.py` & `saltgang-0.1.9/src/saltgang/settings.py`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/src/saltgang/templates/c.tmpl` & `saltgang-0.1.9/src/saltgang/templates/c.tmpl`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/src/saltgang/templates/go.tmpl` & `saltgang-0.1.9/src/saltgang/templates/go.tmpl`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/src/saltgang/templates/ini_check.tmpl` & `saltgang-0.1.9/src/saltgang/templates/ini_check.tmpl`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/src/saltgang/ytt.py` & `saltgang-0.1.9/src/saltgang/ytt.py`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/src/saltgang.egg-info/PKG-INFO` & `saltgang-0.1.9/src/saltgang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saltgang
-Version: 0.1.8
+Version: 0.1.9
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MPL-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `saltgang-0.1.8/src/saltgang.egg-info/SOURCES.txt` & `saltgang-0.1.9/src/saltgang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/tests/test_skeleton.py` & `saltgang-0.1.9/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `saltgang-0.1.8/tox.ini` & `saltgang-0.1.9/tox.ini`

 * *Files identical despite different names*

