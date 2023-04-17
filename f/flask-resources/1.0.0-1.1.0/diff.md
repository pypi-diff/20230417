# Comparing `tmp/flask-resources-1.0.0.tar.gz` & `tmp/flask-resources-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flask-resources-1.0.0.tar", last modified: Wed Mar  8 15:49:22 2023, max compression
+gzip compressed data, was "dist/flask-resources-1.1.0.tar", last modified: Mon Apr 17 14:16:05 2023, max compression
```

## Comparing `flask-resources-1.0.0.tar` & `flask-resources-1.1.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:49:22.000000 flask-resources-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-08 15:49:13.000000 flask-resources-1.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-08 15:49:13.000000 flask-resources-1.0.0/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-08 15:49:13.000000 flask-resources-1.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-08 15:49:13.000000 flask-resources-1.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-03-08 15:49:13.000000 flask-resources-1.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-08 15:49:13.000000 flask-resources-1.0.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-08 15:49:13.000000 flask-resources-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-08 15:49:13.000000 flask-resources-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-03-08 15:49:22.000000 flask-resources-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-03-08 15:49:13.000000 flask-resources-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-08 15:49:13.000000 flask-resources-1.0.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:49:22.000000 flask-resources-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-03-08 15:49:13.000000 flask-resources-1.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-08 15:49:13.000000 flask-resources-1.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-08 15:49:13.000000 flask-resources-1.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-08 15:49:13.000000 flask-resources-1.0.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10198 2023-03-08 15:49:13.000000 flask-resources-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-08 15:49:13.000000 flask-resources-1.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-08 15:49:13.000000 flask-resources-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-08 15:49:13.000000 flask-resources-1.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-08 15:49:13.000000 flask-resources-1.0.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-03-08 15:49:13.000000 flask-resources-1.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-08 15:49:13.000000 flask-resources-1.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-08 15:49:13.000000 flask-resources-1.0.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:49:22.000000 flask-resources-1.0.0/flask_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/content_negotiation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:49:22.000000 flask-resources-1.0.0/flask_resources/deserializers/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/deserializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/deserializers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/deserializers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:49:22.000000 flask-resources-1.0.0/flask_resources/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/parsers/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/parsers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/parsers/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:49:22.000000 flask-resources-1.0.0/flask_resources/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-08 15:49:13.000000 flask-resources-1.0.0/flask_resources/serializers/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:49:22.000000 flask-resources-1.0.0/flask_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-03-08 15:49:21.000000 flask-resources-1.0.0/flask_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-08 15:49:22.000000 flask-resources-1.0.0/flask_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 15:49:21.000000 flask-resources-1.0.0/flask_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 15:49:21.000000 flask-resources-1.0.0/flask_resources.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-08 15:49:21.000000 flask-resources-1.0.0/flask_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-08 15:49:21.000000 flask-resources-1.0.0/flask_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-08 15:49:13.000000 flask-resources-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-08 15:49:13.000000 flask-resources-1.0.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      491 2023-03-08 15:49:13.000000 flask-resources-1.0.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-08 15:49:22.000000 flask-resources-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-08 15:49:13.000000 flask-resources-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:49:22.000000 flask-resources-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-08 15:49:13.000000 flask-resources-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-03-08 15:49:13.000000 flask-resources-1.0.0/tests/test_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-08 15:49:13.000000 flask-resources-1.0.0/tests/test_body_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-08 15:49:13.000000 flask-resources-1.0.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-03-08 15:49:13.000000 flask-resources-1.0.0/tests/test_content_negotiation.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-08 15:49:13.000000 flask-resources-1.0.0/tests/test_deserializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-08 15:49:13.000000 flask-resources-1.0.0/tests/test_resources_docexample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-03-08 15:49:13.000000 flask-resources-1.0.0/tests/test_resources_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-03-08 15:49:13.000000 flask-resources-1.0.0/tests/test_response_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-03-08 15:49:13.000000 flask-resources-1.0.0/tests/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:16:05.000000 flask-resources-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-17 14:15:57.000000 flask-resources-1.1.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 14:15:57.000000 flask-resources-1.1.0/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-17 14:15:57.000000 flask-resources-1.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-17 14:15:57.000000 flask-resources-1.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-17 14:15:57.000000 flask-resources-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-17 14:15:57.000000 flask-resources-1.1.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-17 14:15:57.000000 flask-resources-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-17 14:15:57.000000 flask-resources-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-17 14:16:05.000000 flask-resources-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-17 14:15:57.000000 flask-resources-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-17 14:15:57.000000 flask-resources-1.1.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:16:05.000000 flask-resources-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-04-17 14:15:57.000000 flask-resources-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-17 14:15:57.000000 flask-resources-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-17 14:15:57.000000 flask-resources-1.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-17 14:15:57.000000 flask-resources-1.1.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10198 2023-04-17 14:15:57.000000 flask-resources-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-17 14:15:57.000000 flask-resources-1.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-17 14:15:57.000000 flask-resources-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-17 14:15:57.000000 flask-resources-1.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-17 14:15:57.000000 flask-resources-1.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-04-17 14:15:57.000000 flask-resources-1.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 14:15:57.000000 flask-resources-1.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-17 14:15:57.000000 flask-resources-1.1.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:16:05.000000 flask-resources-1.1.0/flask_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/content_negotiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:16:05.000000 flask-resources-1.1.0/flask_resources/deserializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/deserializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/deserializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/deserializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:16:05.000000 flask-resources-1.1.0/flask_resources/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/parsers/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/parsers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/parsers/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:16:05.000000 flask-resources-1.1.0/flask_resources/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-17 14:15:57.000000 flask-resources-1.1.0/flask_resources/serializers/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:16:05.000000 flask-resources-1.1.0/flask_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-17 14:16:05.000000 flask-resources-1.1.0/flask_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-17 14:16:05.000000 flask-resources-1.1.0/flask_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:16:05.000000 flask-resources-1.1.0/flask_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:16:05.000000 flask-resources-1.1.0/flask_resources.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-17 14:16:05.000000 flask-resources-1.1.0/flask_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 14:16:05.000000 flask-resources-1.1.0/flask_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 14:15:57.000000 flask-resources-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-17 14:15:57.000000 flask-resources-1.1.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      491 2023-04-17 14:15:57.000000 flask-resources-1.1.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-17 14:16:05.000000 flask-resources-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-17 14:15:57.000000 flask-resources-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:16:05.000000 flask-resources-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-17 14:15:57.000000 flask-resources-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-17 14:15:57.000000 flask-resources-1.1.0/tests/test_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-17 14:15:57.000000 flask-resources-1.1.0/tests/test_body_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-17 14:15:57.000000 flask-resources-1.1.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-04-17 14:15:57.000000 flask-resources-1.1.0/tests/test_content_negotiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-17 14:15:57.000000 flask-resources-1.1.0/tests/test_deserializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-17 14:15:57.000000 flask-resources-1.1.0/tests/test_resources_docexample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-17 14:15:57.000000 flask-resources-1.1.0/tests/test_resources_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-17 14:15:57.000000 flask-resources-1.1.0/tests/test_response_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-17 14:15:57.000000 flask-resources-1.1.0/tests/test_serializers.py
```

### Comparing `flask-resources-1.0.0/.editorconfig` & `flask-resources-1.1.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/CHANGES.rst` & `flask-resources-1.1.0/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,19 @@
     Flask-Resources is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 1.0.0. (released 2023-03-09)
+Version 1.1.0 (released 2023-04-17)
+
+- Serializers: add marshmallow schema processors
+
+Version 1.0.0 (released 2023-03-09)
 
 - Remove MarshmallowJSONSerializer (deprecated).
 - Remove XMLSerializer in favor of SimpleSerializer with encoder function.
 - Remove SerializerMixin in favor of BaseSerializer interface.
 - Replace flask.JSONEncoder by json.JSONEncoder.
 
 Version 0.9.1 (released 2023-02-24)
```

### Comparing `flask-resources-1.0.0/CONTRIBUTING.rst` & `flask-resources-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/LICENSE` & `flask-resources-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/MANIFEST.in` & `flask-resources-1.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/PKG-INFO` & `flask-resources-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-resources
-Version: 1.0.0
+Version: 1.1.0
 Summary: "Flask Resources module to create REST APIs."
 Home-page: https://github.com/inveniosoftware/flask-resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -43,15 +43,19 @@
             Flask-Resources is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
-        Version 1.0.0. (released 2023-03-09)
+        Version 1.1.0 (released 2023-04-17)
+        
+        - Serializers: add marshmallow schema processors
+        
+        Version 1.0.0 (released 2023-03-09)
         
         - Remove MarshmallowJSONSerializer (deprecated).
         - Remove XMLSerializer in favor of SimpleSerializer with encoder function.
         - Remove SerializerMixin in favor of BaseSerializer interface.
         - Replace flask.JSONEncoder by json.JSONEncoder.
         
         Version 0.9.1 (released 2023-02-24)
```

### Comparing `flask-resources-1.0.0/README.rst` & `flask-resources-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/babel.ini` & `flask-resources-1.1.0/babel.ini`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/docs/Makefile` & `flask-resources-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/docs/api.rst` & `flask-resources-1.1.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/docs/conf.py` & `flask-resources-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/docs/index.rst` & `flask-resources-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/docs/make.bat` & `flask-resources-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/flask_resources/__init__.py` & `flask-resources-1.1.0/flask_resources/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     request_body_parser,
     request_parser,
 )
 from .resources import Resource, ResourceConfig, route
 from .responses import ResponseHandler, response_handler
 from .serializers import JSONSerializer, MarshmallowSerializer
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 __all__ = (
     "__version__",
     "create_error_handler",
     "from_conf",
     "HTTPJSONException",
     "JSONDeserializer",
```

### Comparing `flask-resources-1.0.0/flask_resources/config.py` & `flask-resources-1.1.0/flask_resources/config.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/flask_resources/content_negotiation.py` & `flask-resources-1.1.0/flask_resources/content_negotiation.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/flask_resources/context.py` & `flask-resources-1.1.0/flask_resources/context.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/flask_resources/deserializers/json.py` & `flask-resources-1.1.0/flask_resources/deserializers/json.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/flask_resources/errors.py` & `flask-resources-1.1.0/flask_resources/errors.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/flask_resources/parsers/__init__.py` & `flask-resources-1.1.0/flask_resources/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/flask_resources/parsers/base.py` & `flask-resources-1.1.0/flask_resources/parsers/base.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/flask_resources/parsers/body.py` & `flask-resources-1.1.0/flask_resources/parsers/body.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/flask_resources/parsers/decorators.py` & `flask-resources-1.1.0/flask_resources/parsers/decorators.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/flask_resources/parsers/schema.py` & `flask-resources-1.1.0/flask_resources/parsers/schema.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/flask_resources/resources.py` & `flask-resources-1.1.0/flask_resources/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 def route(
     method,
     rule,
     view_meth,
     endpoint=None,
-    rule_options={},
+    rule_options=None,
     apply_decorators=True,
 ):
     """Create a route.
 
     Use this method in ``create_url_rules()`` to build your list of rules.
 
     The ``view_method`` parameter should be a bound method (e.g.
@@ -67,15 +67,15 @@
     view.__name__ = view_name
 
     return {
         "rule": resolve_from_conf(rule, config),
         "methods": [method],
         "view_func": view,
         "endpoint": endpoint,
-        **rule_options,
+        **(rule_options or {}),
     }
 
 
 class ResourceConfig:
     """Configuration for a resource.
 
     This object is used for dependency injection in a resource.
```

### Comparing `flask-resources-1.0.0/flask_resources/responses.py` & `flask-resources-1.1.0/flask_resources/responses.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/flask_resources/serializers/json.py` & `flask-resources-1.1.0/flask_resources/serializers/json.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/flask_resources/serializers/simple.py` & `flask-resources-1.1.0/flask_resources/serializers/simple.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/flask_resources.egg-info/PKG-INFO` & `flask-resources-1.1.0/flask_resources.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-resources
-Version: 1.0.0
+Version: 1.1.0
 Summary: "Flask Resources module to create REST APIs."
 Home-page: https://github.com/inveniosoftware/flask-resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -43,15 +43,19 @@
             Flask-Resources is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
-        Version 1.0.0. (released 2023-03-09)
+        Version 1.1.0 (released 2023-04-17)
+        
+        - Serializers: add marshmallow schema processors
+        
+        Version 1.0.0 (released 2023-03-09)
         
         - Remove MarshmallowJSONSerializer (deprecated).
         - Remove XMLSerializer in favor of SimpleSerializer with encoder function.
         - Remove SerializerMixin in favor of BaseSerializer interface.
         - Replace flask.JSONEncoder by json.JSONEncoder.
         
         Version 0.9.1 (released 2023-02-24)
```

### Comparing `flask-resources-1.0.0/flask_resources.egg-info/SOURCES.txt` & `flask-resources-1.1.0/flask_resources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/setup.cfg` & `flask-resources-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/tests/conftest.py` & `flask-resources-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/tests/test_args_parser.py` & `flask-resources-1.1.0/tests/test_args_parser.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/tests/test_body_parser.py` & `flask-resources-1.1.0/tests/test_body_parser.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/tests/test_config.py` & `flask-resources-1.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/tests/test_content_negotiation.py` & `flask-resources-1.1.0/tests/test_content_negotiation.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/tests/test_deserializers.py` & `flask-resources-1.1.0/tests/test_deserializers.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/tests/test_resources_docexample.py` & `flask-resources-1.1.0/tests/test_resources_docexample.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/tests/test_resources_errors.py` & `flask-resources-1.1.0/tests/test_resources_errors.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/tests/test_response_handlers.py` & `flask-resources-1.1.0/tests/test_response_handlers.py`

 * *Files identical despite different names*

### Comparing `flask-resources-1.0.0/tests/test_serializers.py` & `flask-resources-1.1.0/tests/test_serializers.py`

 * *Files identical despite different names*

