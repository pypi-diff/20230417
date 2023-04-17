# Comparing `tmp/cf-units-3.1.1.tar.gz` & `tmp/cf-units-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf-units-3.1.1.tar", last modified: Tue Jul 12 15:19:54 2022, max compression
+gzip compressed data, was "cf-units-3.2.0.tar", last modified: Mon Apr 17 15:11:33 2023, max compression
```

## Comparing `cf-units-3.1.1.tar` & `cf-units-3.2.0.tar`

### file list

```diff
@@ -1,89 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:54.535653 cf-units-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-07-12 15:19:36.000000 cf-units-3.1.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-07-12 15:19:36.000000 cf-units-3.1.1/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-07-12 15:19:36.000000 cf-units-3.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-07-12 15:19:36.000000 cf-units-3.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-07-12 15:19:36.000000 cf-units-3.1.1/CHANGES
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-07-12 15:19:36.000000 cf-units-3.1.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-07-12 15:19:36.000000 cf-units-3.1.1/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-07-12 15:19:36.000000 cf-units-3.1.1/INSTALL
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-07-12 15:19:36.000000 cf-units-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5663 2022-07-12 15:19:54.535653 cf-units-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4455 2022-07-12 15:19:36.000000 cf-units-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:54.531653 cf-units-3.1.1/cf_units/
--rw-r--r--   0 runner    (1001) docker     (121)    62021 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   754501 2022-07-12 15:19:53.000000 cf-units-3.1.1/cf_units/_udunits2.c
--rw-r--r--   0 runner    (1001) docker     (121)     2571 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/_udunits2.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     8554 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/_udunits2.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:54.531653 cf-units-3.1.1/cf_units/_udunits2_parser/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/_udunits2_parser/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/_udunits2_parser/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     7226 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/_udunits2_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2464 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/_udunits2_parser/compile.py
--rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/_udunits2_parser/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:54.531653 cf-units-3.1.1/cf_units/_udunits2_parser/parser/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/_udunits2_parser/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26495 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/_udunits2_parser/parser/udunits2Lexer.py
--rw-r--r--   0 runner    (1001) docker     (121)    37254 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/_udunits2_parser/parser/udunits2Parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2152 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/_udunits2_parser/parser/udunits2ParserVisitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3618 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/_udunits2_parser/udunits2Lexer.g4.jinja
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/_udunits2_parser/udunits2Parser.g4
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-07-12 15:19:54.000000 cf-units-3.1.1/cf_units/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:54.531653 cf-units-3.1.1/cf_units/etc/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/etc/site.cfg.template
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:54.531653 cf-units-3.1.1/cf_units/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:54.531653 cf-units-3.1.1/cf_units/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:54.531653 cf-units-3.1.1/cf_units/tests/integration/parse/
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/integration/parse/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     7640 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/integration/parse/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (121)    11502 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/integration/test__num2date_to_nearest_second.py
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/integration/test_date2num.py
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/integration/test_num2date.py
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/integration/test_num2pydate.py
--rw-r--r--   0 runner    (1001) docker     (121)     4515 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/test_coding_standards.py
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/test_tex.py
--rw-r--r--   0 runner    (1001) docker     (121)    30615 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/test_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:54.531653 cf-units-3.1.1/cf_units/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3787 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/unit/test__discard_microsecond.py
--rw-r--r--   0 runner    (1001) docker     (121)     8770 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/unit/test__udunits2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:54.531653 cf-units-3.1.1/cf_units/tests/unit/unit/
--rw-r--r--   0 runner    (1001) docker     (121)    11083 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/unit/unit/test_Unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tests/unit/unit/test_as_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/tex.py
--rw-r--r--   0 runner    (1001) docker     (121)     3265 2022-07-12 15:19:36.000000 cf-units-3.1.1/cf_units/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:54.531653 cf-units-3.1.1/cf_units.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5663 2022-07-12 15:19:54.000000 cf-units-3.1.1/cf_units.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-07-12 15:19:54.000000 cf-units-3.1.1/cf_units.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-12 15:19:54.000000 cf-units-3.1.1/cf_units.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-12 15:19:53.000000 cf-units-3.1.1/cf_units.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-12 15:19:54.000000 cf-units-3.1.1/cf_units.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-07-12 15:19:54.000000 cf-units-3.1.1/cf_units.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-07-12 15:19:36.000000 cf-units-3.1.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:54.535653 cf-units-3.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6779 2022-07-12 15:19:36.000000 cf-units-3.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     6714 2022-07-12 15:19:36.000000 cf-units-3.1.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:54.535653 cf-units-3.1.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-07-12 15:19:36.000000 cf-units-3.1.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-07-12 15:19:36.000000 cf-units-3.1.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-07-12 15:19:36.000000 cf-units-3.1.1/docs/source/unit.rst
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-07-12 15:19:36.000000 cf-units-3.1.1/docs/source/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-07-12 15:19:36.000000 cf-units-3.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:54.535653 cf-units-3.1.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-07-12 15:19:36.000000 cf-units-3.1.1/requirements/cf-units.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:19:54.535653 cf-units-3.1.1/requirements/locks/
--rw-r--r--   0 runner    (1001) docker     (121)    11312 2022-07-12 15:19:36.000000 cf-units-3.1.1/requirements/locks/py310-lock-linux-64.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10506 2022-07-12 15:19:36.000000 cf-units-3.1.1/requirements/locks/py310-lock-osx-64.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10500 2022-07-12 15:19:36.000000 cf-units-3.1.1/requirements/locks/py310-lock-win-64.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11179 2022-07-12 15:19:36.000000 cf-units-3.1.1/requirements/locks/py38-lock-linux-64.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10373 2022-07-12 15:19:36.000000 cf-units-3.1.1/requirements/locks/py38-lock-osx-64.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10366 2022-07-12 15:19:36.000000 cf-units-3.1.1/requirements/locks/py38-lock-win-64.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11290 2022-07-12 15:19:36.000000 cf-units-3.1.1/requirements/locks/py39-lock-linux-64.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10484 2022-07-12 15:19:36.000000 cf-units-3.1.1/requirements/locks/py39-lock-osx-64.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10477 2022-07-12 15:19:36.000000 cf-units-3.1.1/requirements/locks/py39-lock-win-64.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1685 2022-07-12 15:19:54.535653 cf-units-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4988 2022-07-12 15:19:36.000000 cf-units-3.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-07-12 15:19:36.000000 cf-units-3.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:33.591631 cf-units-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 15:11:11.000000 cf-units-3.2.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 15:11:11.000000 cf-units-3.2.0/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-17 15:11:11.000000 cf-units-3.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 15:11:11.000000 cf-units-3.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-17 15:11:11.000000 cf-units-3.2.0/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-17 15:11:11.000000 cf-units-3.2.0/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-17 15:11:11.000000 cf-units-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-17 15:11:11.000000 cf-units-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-17 15:11:33.591631 cf-units-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-17 15:11:11.000000 cf-units-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:33.579631 cf-units-3.2.0/cf_units/
+-rw-r--r--   0 runner    (1001) docker     (123)    61997 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   677050 2023-04-17 15:11:32.000000 cf-units-3.2.0/cf_units/_udunits2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/_udunits2.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/_udunits2.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:33.583631 cf-units-3.2.0/cf_units/_udunits2_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/_udunits2_parser/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/_udunits2_parser/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/_udunits2_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/_udunits2_parser/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/_udunits2_parser/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:33.583631 cf-units-3.2.0/cf_units/_udunits2_parser/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/_udunits2_parser/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26494 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/_udunits2_parser/parser/udunits2Lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37244 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/_udunits2_parser/parser/udunits2Parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/_udunits2_parser/parser/udunits2ParserVisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/_udunits2_parser/udunits2Lexer.g4.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/_udunits2_parser/udunits2Parser.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 15:11:33.000000 cf-units-3.2.0/cf_units/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:33.583631 cf-units-3.2.0/cf_units/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/etc/site.cfg.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:33.587631 cf-units-3.2.0/cf_units/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:33.587631 cf-units-3.2.0/cf_units/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:33.587631 cf-units-3.2.0/cf_units/tests/integration/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/integration/parse/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/integration/parse/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/integration/test__num2date_to_nearest_second.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/integration/test_date2num.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/integration/test_num2date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/integration/test_num2pydate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/test_coding_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/test_tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30593 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:33.587631 cf-units-3.2.0/cf_units/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/unit/test__discard_microsecond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/unit/test__udunits2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:33.587631 cf-units-3.2.0/cf_units/tests/unit/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/unit/unit/test_Unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tests/unit/unit/test_as_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-17 15:11:11.000000 cf-units-3.2.0/cf_units/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:33.583631 cf-units-3.2.0/cf_units.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-17 15:11:33.000000 cf-units-3.2.0/cf_units.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-17 15:11:33.000000 cf-units-3.2.0/cf_units.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:11:33.000000 cf-units-3.2.0/cf_units.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:11:32.000000 cf-units-3.2.0/cf_units.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-17 15:11:33.000000 cf-units-3.2.0/cf_units.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 15:11:33.000000 cf-units-3.2.0/cf_units.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-17 15:11:11.000000 cf-units-3.2.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:33.587631 cf-units-3.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-17 15:11:11.000000 cf-units-3.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-17 15:11:11.000000 cf-units-3.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:33.591631 cf-units-3.2.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-17 15:11:11.000000 cf-units-3.2.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-17 15:11:11.000000 cf-units-3.2.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-17 15:11:11.000000 cf-units-3.2.0/docs/source/unit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-17 15:11:11.000000 cf-units-3.2.0/docs/source/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-17 15:11:11.000000 cf-units-3.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:33.591631 cf-units-3.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-17 15:11:11.000000 cf-units-3.2.0/requirements/cf-units.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:11:33.591631 cf-units-3.2.0/requirements/locks/
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-04-17 15:11:11.000000 cf-units-3.2.0/requirements/locks/py310-lock-linux-64.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-17 15:11:11.000000 cf-units-3.2.0/requirements/locks/py310-lock-osx-64.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-04-17 15:11:11.000000 cf-units-3.2.0/requirements/locks/py310-lock-win-64.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-04-17 15:11:11.000000 cf-units-3.2.0/requirements/locks/py38-lock-linux-64.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-04-17 15:11:11.000000 cf-units-3.2.0/requirements/locks/py38-lock-osx-64.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-04-17 15:11:11.000000 cf-units-3.2.0/requirements/locks/py38-lock-win-64.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-04-17 15:11:11.000000 cf-units-3.2.0/requirements/locks/py39-lock-linux-64.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-04-17 15:11:11.000000 cf-units-3.2.0/requirements/locks/py39-lock-osx-64.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-04-17 15:11:11.000000 cf-units-3.2.0/requirements/locks/py39-lock-win-64.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-17 15:11:33.591631 cf-units-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-04-17 15:11:11.000000 cf-units-3.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-17 15:11:11.000000 cf-units-3.2.0/tox.ini
```

### Comparing `cf-units-3.1.1/.pre-commit-config.yaml` & `cf-units-3.2.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
         # Prevent giant files from being committed.
     -   id: check-added-large-files
         # Check whether files parse as valid Python.
     -   id: check-ast
         # Check for file name conflicts on case-insensitive filesytems.
     -   id: check-case-conflict
@@ -15,29 +15,29 @@
     -   id: check-merge-conflict
         # Check for debugger imports and py37+ `breakpoint()` calls in Python source.
     -   id: debug-statements
         # Don't commit to main branch.
     -   id: no-commit-to-branch
 
 -   repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
     -   id: black
         types: [file, python]
         args: [--config=./pyproject.toml]
 
 -   repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
+    rev: 6.0.0
     hooks:
     -   id: flake8
         types: [file, python]
         args: [--config=./setup.cfg]
 
 -   repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
     -   id: isort
         types: [file, python]
         args: [--filter-files]
 
 -   repo: https://github.com/aio-libs/sort-all
     rev: v1.2.0
```

### Comparing `cf-units-3.1.1/.readthedocs.yml` & `cf-units-3.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `cf-units-3.1.1/CHANGES` & `cf-units-3.2.0/CHANGES`

 * *Files identical despite different names*

### Comparing `cf-units-3.1.1/INSTALL` & `cf-units-3.2.0/INSTALL`

 * *Files identical despite different names*

### Comparing `cf-units-3.1.1/PKG-INFO` & `cf-units-3.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: cf-units
-Version: 3.1.1
+Version: 3.2.0
 Summary: Units of measure as required by the Climate and Forecast (CF) metadata conventions
 Home-page: https://github.com/SciTools/cf-units
 Download-URL: https://github.com/SciTools/cf-units
 Author: SciTools Developers
-License: LGPL-3.0-or-later
+License: BSD
 Project-URL: Code, https://github.com/SciTools/cf-units
 Project-URL: Discussions, https://github.com/SciTools/cf-units/discussions
 Project-URL: Issues, https://github.com/SciTools/cf-units/issues
 Keywords: units,cf,netcdf,science,oceanography,meteorology,climate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: all
-License-File: COPYING
+License-File: LICENSE
 
 # [cf-units](https://cf-units.readthedocs.io/en/latest/)
 
 #### Units of measure as defined by the Climate and Forecast (CF) Metadata Conventions.
 
 [comment]: # (https://shields.io/ is a good source of these)
 [![ci-tests](https://github.com/SciTools/cf-units/actions/workflows/ci-tests.yml/badge.svg?branch=main)](https://github.com/SciTools/cf-units/actions/workflows/ci-tests.yml)
@@ -43,15 +43,15 @@
 [![Latest version](https://img.shields.io/github/tag/SciTools/cf-units)](https://github.com/SciTools/cf-units/releases)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3723086.svg)](https://doi.org/10.5281/zenodo.3723086)
 \
 [![Black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)
 [![Flake8](https://img.shields.io/badge/lint-flake8-lightgrey)](https://github.com/PyCQA/flake8)
 [![isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 \
-[![Licence](https://img.shields.io/github/license/SciTools/cf-units)](COPYING)
+[![Licence](https://img.shields.io/badge/license-BSD--3-orange)](LICENSE)
 [![Contributors](https://img.shields.io/github/contributors/SciTools/cf-units)](https://github.com/SciTools/cf-units/graphs/contributors)
 [![Commits since last release](https://img.shields.io/github/commits-since/SciTools/cf-units/latest.svg)](https://github.com/SciTools/cf-units/commits/main)
 
 ## Table of Contents
 
 [comment]: # (NOTE: toc auto-generated with
   https://github.com/jonschlinkert/markdown-toc
@@ -100,13 +100,13 @@
 A full list of code contributors ("cf-units contributors") can be found at
 https://github.com/SciTools/cf-units/graphs/contributors.
 
 Code is just one of many ways of positively contributing to cf-units, please
 see our [contributing guide](.github/CONTRIBUTING.md) for more details on how
 you can get involved.
 
-cf-units is released under a LGPL license with a shared copyright model.
-See [COPYING](COPYING) and [COPYING.LESSER](COPYING.LESSER) for full terms.
+cf-units is released under a BSD-3 license. See [LICENSE](LICENSE) for full
+terms.
 
 The [Met Office](https://metoffice.gov.uk) has made a significant
 contribution to the development, maintenance and support of this library.
 All Met Office contributions are copyright on behalf of the British Crown.
```

### Comparing `cf-units-3.1.1/README.md` & `cf-units-3.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [![Latest version](https://img.shields.io/github/tag/SciTools/cf-units)](https://github.com/SciTools/cf-units/releases)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3723086.svg)](https://doi.org/10.5281/zenodo.3723086)
 \
 [![Black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)
 [![Flake8](https://img.shields.io/badge/lint-flake8-lightgrey)](https://github.com/PyCQA/flake8)
 [![isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 \
-[![Licence](https://img.shields.io/github/license/SciTools/cf-units)](COPYING)
+[![Licence](https://img.shields.io/badge/license-BSD--3-orange)](LICENSE)
 [![Contributors](https://img.shields.io/github/contributors/SciTools/cf-units)](https://github.com/SciTools/cf-units/graphs/contributors)
 [![Commits since last release](https://img.shields.io/github/commits-since/SciTools/cf-units/latest.svg)](https://github.com/SciTools/cf-units/commits/main)
 
 ## Table of Contents
 
 [comment]: # (NOTE: toc auto-generated with
   https://github.com/jonschlinkert/markdown-toc
@@ -72,13 +72,13 @@
 A full list of code contributors ("cf-units contributors") can be found at
 https://github.com/SciTools/cf-units/graphs/contributors.
 
 Code is just one of many ways of positively contributing to cf-units, please
 see our [contributing guide](.github/CONTRIBUTING.md) for more details on how
 you can get involved.
 
-cf-units is released under a LGPL license with a shared copyright model.
-See [COPYING](COPYING) and [COPYING.LESSER](COPYING.LESSER) for full terms.
+cf-units is released under a BSD-3 license. See [LICENSE](LICENSE) for full
+terms.
 
 The [Met Office](https://metoffice.gov.uk) has made a significant
 contribution to the development, maintenance and support of this library.
 All Met Office contributions are copyright on behalf of the British Crown.
```

### Comparing `cf-units-3.1.1/cf_units/__init__.py` & `cf-units-3.2.0/cf_units/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """
 Units of measure.
 
 Provision of a wrapper class to support Unidata/UCAR UDUNITS-2, and the
 cftime calendar functionality.
 
 See also: `UDUNITS-2
 <http://www.unidata.ucar.edu/software/udunits>`_.
 
 """
 
 import copy
+import math
 from contextlib import contextmanager
 
 import cftime
 import numpy as np
 
 from cf_units import _udunits2 as _ud
 from cf_units._udunits2 import (
@@ -28,15 +28,15 @@
     UT_LATIN1,
     UT_NAMES,
     UT_UTF8,
 )
 
 from . import config
 from ._version import version as __version__  # noqa: F401
-from .util import _OrderedHashable, approx_equal
+from .util import _OrderedHashable
 
 __all__ = [
     "CALENDARS",
     "CALENDAR_360_DAY",
     "CALENDAR_365_DAY",
     "CALENDAR_366_DAY",
     "CALENDAR_ALIASES",
@@ -1659,23 +1659,23 @@
             # 1 ** N -> 1
             result = self
         else:
             # UDUNITS-2 does not support floating point raise/root.
             # But if the power is of the form 1/N, where N is an integer
             # (within a certain acceptable accuracy) then we can find the Nth
             # root.
-            if not approx_equal(power, 0.0) and abs(power) < 1:
-                if not approx_equal(1 / power, round(1 / power)):
+            if not math.isclose(power, 0.0) and abs(power) < 1:
+                if not math.isclose(1 / power, round(1 / power)):
                     raise ValueError("Cannot raise a unit by a decimal.")
                 root = int(round(1 / power))
                 result = self.root(root)
             else:
                 # Failing that, check for powers which are (very nearly) simple
                 # integer values.
-                if not approx_equal(power, round(power)):
+                if not math.isclose(power, round(power)):
                     msg = "Cannot raise a unit by a decimal (got %s)." % power
                     raise ValueError(msg)
                 power = int(round(power))
 
                 try:
                     ut_unit = _ud.raise_(self.ut_unit, power)
                 except _ud.UdunitsError as exception:
```

### Comparing `cf-units-3.1.1/cf_units/_udunits2.c` & `cf-units-3.2.0/cf_units/_udunits2.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-/* Generated by Cython 0.29.30 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "include_dirs": [
             "/usr/include"
         ],
         "libraries": [
             "udunits2"
         ],
         "library_dirs": [
-            "/usr/lib"
+            "/usr/lib/x86_64-linux-gnu"
         ],
         "name": "cf_units._udunits2",
         "runtime_library_dirs": [
-            "/usr/lib"
+            "/usr/lib/x86_64-linux-gnu"
         ],
         "sources": [
             "cf_units/_udunits2.pyx"
         ]
     },
     "module_name": "cf_units._udunits2"
 }
@@ -30,16 +30,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_30"
-#define CYTHON_HEX_VERSION 0x001D1EF0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -70,14 +70,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -107,20 +108,21 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -153,18 +155,64 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -176,15 +224,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -215,15 +263,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -525,35 +573,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -718,15 +766,21 @@
 #define __PYX_HAVE__cf_units___udunits2
 #define __PYX_HAVE_API__cf_units___udunits2
 /* Early includes */
 #include "udunits2.h"
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
+#include "numpy/ndarrayobject.h"
+#include "numpy/ndarraytypes.h"
+#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
+
+    /* NumPy API declarations from "numpy/__init__.pxd" */
+    
 #include <errno.h>
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
@@ -993,195 +1047,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":775
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":776
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":777
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":778
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":782
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":783
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":784
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":785
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":789
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":790
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":799
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":800
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":801
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":803
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":804
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":805
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":807
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":808
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":810
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":811
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":812
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1212,91 +1266,91 @@
 
 /*--- Type declarations ---*/
 struct __pyx_obj_8cf_units_9_udunits2_System;
 struct __pyx_obj_8cf_units_9_udunits2_Unit;
 struct __pyx_obj_8cf_units_9_udunits2_Converter;
 struct __pyx_obj_8cf_units_9_udunits2_ErrorMessageHandler;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":814
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":815
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":816
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":818
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
 
-/* "cf_units/_udunits2.pyx":42
+/* "cf_units/_udunits2.pyx":41
  * ##### Wrapper classes #####
  * 
  * cdef class System:             # <<<<<<<<<<<<<<
  *     """
  *     Wrapper class for UDUNITS-2 ut_system. Calls ut_free_system() on
  */
 struct __pyx_obj_8cf_units_9_udunits2_System {
   PyObject_HEAD
   ut_system *csystem;
 };
 
 
-/* "cf_units/_udunits2.pyx":57
+/* "cf_units/_udunits2.pyx":56
  * 
  * 
  * cdef class Unit:             # <<<<<<<<<<<<<<
  *     """
  *     Wrapper class for UDUNITS-2 ut_unit. Calls ut_free() on
  */
 struct __pyx_obj_8cf_units_9_udunits2_Unit {
   PyObject_HEAD
   ut_unit *cunit;
   struct __pyx_obj_8cf_units_9_udunits2_System *system;
 };
 
 
-/* "cf_units/_udunits2.pyx":74
+/* "cf_units/_udunits2.pyx":73
  * 
  * 
  * cdef class Converter:             # <<<<<<<<<<<<<<
  *     """
  *     Wrapper class for UDUNITS-2 cv_converter. Calls cv_free() on
  */
 struct __pyx_obj_8cf_units_9_udunits2_Converter {
   PyObject_HEAD
   cv_converter *cconverter;
 };
 
 
-/* "cf_units/_udunits2.pyx":89
+/* "cf_units/_udunits2.pyx":88
  * 
  * 
  * cdef class ErrorMessageHandler:             # <<<<<<<<<<<<<<
  *     """
  *     Wrapper class for UDUNITS-2 ut_error_message_handler typedef.
  */
 struct __pyx_obj_8cf_units_9_udunits2_ErrorMessageHandler {
@@ -1456,26 +1510,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1615,37 +1669,14 @@
 static int  __Pyx__GetBufferAndValidate(Py_buffer* buf, PyObject* obj,
     __Pyx_TypeInfo* dtype, int flags, int nd, int cast, __Pyx_BufFmt_StackElem* stack);
 static void __Pyx_ZeroBuffer(Py_buffer* buf);
 static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info);
 static Py_ssize_t __Pyx_minusones[] = { -1, -1, -1, -1, -1, -1, -1, -1 };
 static Py_ssize_t __Pyx_zeros[] = { 0, 0, 0, 0, 0, 0, 0, 0 };
 
-/* DictGetItem.proto */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
-#define __Pyx_PyObject_Dict_GetItem(obj, name)\
-    (likely(PyDict_CheckExact(obj)) ?\
-     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
-#else
-#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
-#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
-#endif
-
-/* RaiseTooManyValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
-
-/* RaiseNeedMoreValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
-
-/* RaiseNoneIterError.proto */
-static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
-
-/* ExtTypeTest.proto */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
-
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -1693,20 +1724,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
@@ -1961,17 +2000,14 @@
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value);
-
-/* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
@@ -2015,16 +2051,25 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
+static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
+static PyTypeObject *__pyx_ptype_5numpy_number = 0;
+static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
+static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
+static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
+static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
-static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *, char *, char *, int *); /*proto*/
 
 /* Module declarations from 'libc' */
 
 /* Module declarations from 'libc.errno' */
 
 /* Module declarations from 'cf_units._udunits2' */
 static PyTypeObject *__pyx_ptype_8cf_units_9_udunits2_System = 0;
@@ -2041,17 +2086,14 @@
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t = { "float64_t", NULL, sizeof(__pyx_t_5numpy_float64_t), { 0 }, 0, 'R', 0, 0 };
 #define __Pyx_MODULE_NAME "cf_units._udunits2"
 extern int __pyx_module_is_main_cf_units___udunits2;
 int __pyx_module_is_main_cf_units___udunits2 = 0;
 
 /* Implementation of 'cf_units._udunits2' */
 static PyObject *__pyx_builtin_TypeError;
-static PyObject *__pyx_builtin_ValueError;
-static PyObject *__pyx_builtin_range;
-static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_ImportError;
 static const char __pyx_k_n[] = "n";
 static const char __pyx_k__9[] = "";
 static const char __pyx_k_fr[] = "fr";
 static const char __pyx_k_in[] = "in_";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_to[] = "to";
@@ -2084,15 +2126,14 @@
 static const char __pyx_k_hours[] = "hours";
 static const char __pyx_k_month[] = "month";
 static const char __pyx_k_numer[] = "numer";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_parse[] = "parse";
 static const char __pyx_k_power[] = "power";
 static const char __pyx_k_raise[] = "raise_";
-static const char __pyx_k_range[] = "range";
 static const char __pyx_k_scale[] = "scale";
 static const char __pyx_k_unit1[] = "unit1";
 static const char __pyx_k_unit2[] = "unit2";
 static const char __pyx_k_value[] = "value";
 static const char __pyx_k_System[] = "System";
 static const char __pyx_k_divide[] = "divide";
 static const char __pyx_k_errnum[] = "errnum";
@@ -2141,26 +2182,24 @@
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_reference[] = "reference";
 static const char __pyx_k_UT_BAD_ARG[] = "UT_BAD_ARG";
 static const char __pyx_k_UT_NO_UNIT[] = "UT_NO_UNIT";
 static const char __pyx_k_UT_SUCCESS[] = "UT_SUCCESS";
 static const char __pyx_k_UT_UNKNOWN[] = "UT_UNKNOWN";
-static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_cconverter[] = "cconverter";
 static const char __pyx_k_resolution[] = "resolution";
 static const char __pyx_k_status_msg[] = "status_msg";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_UT_OPEN_ARG[] = "UT_OPEN_ARG";
 static const char __pyx_k_UT_OPEN_ENV[] = "UT_OPEN_ENV";
 static const char __pyx_k_decode_time[] = "decode_time";
 static const char __pyx_k_encode_date[] = "encode_date";
 static const char __pyx_k_encode_time[] = "encode_time";
 static const char __pyx_k_raise_error[] = "_raise_error";
-static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_UT_NO_SECOND[] = "UT_NO_SECOND";
 static const char __pyx_k_UdunitsError[] = "UdunitsError";
 static const char __pyx_k_encode_clock[] = "encode_clock";
 static const char __pyx_k_UT_DEFINITION[] = "UT_DEFINITION";
 static const char __pyx_k_UT_ISO_8859_1[] = "UT_ISO_8859_1";
 static const char __pyx_k_convert_float[] = "convert_float";
 static const char __pyx_k_get_converter[] = "get_converter";
@@ -2183,33 +2222,23 @@
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_ErrorMessageHandler[] = "ErrorMessageHandler";
 static const char __pyx_k_UdunitsError___init[] = "UdunitsError.__init__";
 static const char __pyx_k_UdunitsError_error_msg[] = "UdunitsError.error_msg";
 static const char __pyx_k_cf_units__udunits2_pyx[] = "cf_units/_udunits2.pyx";
 static const char __pyx_k_UdunitsError_status_msg[] = "UdunitsError.status_msg";
 static const char __pyx_k_set_error_message_handler[] = "set_error_message_handler";
-static const char __pyx_k_ndarray_is_not_C_contiguous[] = "ndarray is not C contiguous";
 static const char __pyx_k_UDUNITS_2_call_resulted_in_an_e[] = "\n    UDUNITS-2 call resulted in an error.\n\n    Attributes:\n\n    * status:\n        The UDUNITS-2 ut_status value which resulted from the error.\n    * errnum:\n        The errno value which resulted from the error.\n\n    ";
 static const char __pyx_k_Units_of_measure_Wrapper_for_Un[] = "\nUnits of measure.\n\nWrapper for Unidata/UCAR UDUNITS-2.\n\nSee also: `UDUNITS-2\n<http://www.unidata.ucar.edu/software/udunits/udunits-2/udunits2.html>`_.\n\n";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
-static const char __pyx_k_unknown_dtype_code_in_numpy_pxd[] = "unknown dtype code in numpy.pxd (%d)";
-static const char __pyx_k_Format_string_allocated_too_shor[] = "Format string allocated too short, see comment in numpy.pxd";
-static const char __pyx_k_Non_native_byte_order_not_suppor[] = "Non-native byte order not supported";
-static const char __pyx_k_ndarray_is_not_Fortran_contiguou[] = "ndarray is not Fortran contiguous";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
-static const char __pyx_k_Format_string_allocated_too_shor_2[] = "Format string allocated too short.";
 static PyObject *__pyx_n_s_Converter;
 static PyObject *__pyx_n_s_ErrorMessageHandler;
-static PyObject *__pyx_kp_u_Format_string_allocated_too_shor;
-static PyObject *__pyx_kp_u_Format_string_allocated_too_shor_2;
 static PyObject *__pyx_n_s_ImportError;
 static PyObject *__pyx_n_s_NULL_UNIT;
-static PyObject *__pyx_kp_u_Non_native_byte_order_not_suppor;
-static PyObject *__pyx_n_s_RuntimeError;
 static PyObject *__pyx_n_s_System;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_UDUNITS_2_call_resulted_in_an_e;
 static PyObject *__pyx_n_s_UNKNOWN;
 static PyObject *__pyx_n_s_UT_ASCII;
 static PyObject *__pyx_n_s_UT_BAD_ARG;
 static PyObject *__pyx_n_s_UT_CANT_FORMAT;
@@ -2234,15 +2263,14 @@
 static PyObject *__pyx_n_s_UT_VISIT_ERROR;
 static PyObject *__pyx_n_s_UdunitsError;
 static PyObject *__pyx_n_s_UdunitsError___init;
 static PyObject *__pyx_n_s_UdunitsError___str;
 static PyObject *__pyx_n_s_UdunitsError_error_msg;
 static PyObject *__pyx_n_s_UdunitsError_status_msg;
 static PyObject *__pyx_n_s_Unit;
-static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_kp_s__10;
 static PyObject *__pyx_kp_s__11;
 static PyObject *__pyx_kp_s__9;
 static PyObject *__pyx_n_s_are_convertible;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_buf;
 static PyObject *__pyx_n_s_cconverter;
@@ -2291,16 +2319,14 @@
 static PyObject *__pyx_n_s_minutes;
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_month;
 static PyObject *__pyx_n_s_multiply;
 static PyObject *__pyx_n_s_n;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
-static PyObject *__pyx_kp_u_ndarray_is_not_C_contiguous;
-static PyObject *__pyx_kp_u_ndarray_is_not_Fortran_contiguou;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numer;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_s_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_s_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_offset;
@@ -2311,15 +2337,14 @@
 static PyObject *__pyx_n_s_parse;
 static PyObject *__pyx_n_s_path;
 static PyObject *__pyx_n_s_power;
 static PyObject *__pyx_n_s_prepare;
 static PyObject *__pyx_n_s_qualname;
 static PyObject *__pyx_n_s_raise;
 static PyObject *__pyx_n_s_raise_error;
-static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_read_xml;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_reference;
 static PyObject *__pyx_n_s_resolution;
 static PyObject *__pyx_n_s_result;
@@ -2339,15 +2364,14 @@
 static PyObject *__pyx_n_s_string;
 static PyObject *__pyx_n_s_system;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_to;
 static PyObject *__pyx_n_s_unit;
 static PyObject *__pyx_n_s_unit1;
 static PyObject *__pyx_n_s_unit2;
-static PyObject *__pyx_kp_u_unknown_dtype_code_in_numpy_pxd;
 static PyObject *__pyx_n_s_value;
 static PyObject *__pyx_n_s_year;
 static int __pyx_pf_8cf_units_9_udunits2_6System___cinit__(struct __pyx_obj_8cf_units_9_udunits2_System *__pyx_v_self); /* proto */
 static void __pyx_pf_8cf_units_9_udunits2_6System_2__dealloc__(struct __pyx_obj_8cf_units_9_udunits2_System *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8cf_units_9_udunits2_6System_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_8cf_units_9_udunits2_System *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8cf_units_9_udunits2_6System_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_8cf_units_9_udunits2_System *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_8cf_units_9_udunits2_4Unit___cinit__(struct __pyx_obj_8cf_units_9_udunits2_Unit *__pyx_v_self); /* proto */
@@ -2389,16 +2413,14 @@
 static PyObject *__pyx_pf_8cf_units_9_udunits2_42encode_time(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_year, int __pyx_v_month, int __pyx_v_day, int __pyx_v_hour, int __pyx_v_minute, double __pyx_v_second); /* proto */
 static PyObject *__pyx_pf_8cf_units_9_udunits2_44decode_time(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_value); /* proto */
 static PyObject *__pyx_pf_8cf_units_9_udunits2_46set_error_message_handler(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_8cf_units_9_udunits2_ErrorMessageHandler *__pyx_v_handler); /* proto */
 static PyObject *__pyx_pf_8cf_units_9_udunits2_48convert_float(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_8cf_units_9_udunits2_Converter *__pyx_v_converter, float __pyx_v_value); /* proto */
 static PyObject *__pyx_pf_8cf_units_9_udunits2_50convert_floats(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_8cf_units_9_udunits2_Converter *__pyx_v_converter, PyArrayObject *__pyx_v_in_, PyArrayObject *__pyx_v_out); /* proto */
 static PyObject *__pyx_pf_8cf_units_9_udunits2_52convert_double(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_8cf_units_9_udunits2_Converter *__pyx_v_converter, double __pyx_v_value); /* proto */
 static PyObject *__pyx_pf_8cf_units_9_udunits2_54convert_doubles(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_8cf_units_9_udunits2_Converter *__pyx_v_converter, PyArrayObject *__pyx_v_in_, PyArrayObject *__pyx_v_out); /* proto */
-static int __pyx_pf_5numpy_7ndarray___getbuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
-static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info); /* proto */
 static PyObject *__pyx_tp_new_8cf_units_9_udunits2_System(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_8cf_units_9_udunits2_Unit(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_8cf_units_9_udunits2_Converter(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_8cf_units_9_udunits2_ErrorMessageHandler(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_2;
@@ -2412,85 +2434,80 @@
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__14;
-static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
-static PyObject *__pyx_tuple__19;
-static PyObject *__pyx_tuple__21;
-static PyObject *__pyx_tuple__23;
-static PyObject *__pyx_tuple__25;
-static PyObject *__pyx_tuple__27;
-static PyObject *__pyx_tuple__29;
-static PyObject *__pyx_tuple__31;
-static PyObject *__pyx_tuple__33;
-static PyObject *__pyx_tuple__35;
-static PyObject *__pyx_tuple__37;
-static PyObject *__pyx_tuple__39;
-static PyObject *__pyx_tuple__41;
-static PyObject *__pyx_tuple__43;
-static PyObject *__pyx_tuple__45;
-static PyObject *__pyx_tuple__47;
-static PyObject *__pyx_tuple__49;
-static PyObject *__pyx_tuple__51;
-static PyObject *__pyx_tuple__53;
-static PyObject *__pyx_tuple__55;
-static PyObject *__pyx_tuple__57;
-static PyObject *__pyx_tuple__59;
-static PyObject *__pyx_tuple__61;
-static PyObject *__pyx_tuple__63;
-static PyObject *__pyx_tuple__65;
-static PyObject *__pyx_tuple__67;
-static PyObject *__pyx_tuple__69;
-static PyObject *__pyx_tuple__71;
-static PyObject *__pyx_tuple__73;
-static PyObject *__pyx_tuple__75;
-static PyObject *__pyx_tuple__77;
-static PyObject *__pyx_tuple__79;
-static PyObject *__pyx_tuple__81;
-static PyObject *__pyx_codeobj__20;
-static PyObject *__pyx_codeobj__22;
-static PyObject *__pyx_codeobj__24;
-static PyObject *__pyx_codeobj__26;
-static PyObject *__pyx_codeobj__28;
-static PyObject *__pyx_codeobj__30;
-static PyObject *__pyx_codeobj__32;
-static PyObject *__pyx_codeobj__34;
-static PyObject *__pyx_codeobj__36;
-static PyObject *__pyx_codeobj__38;
-static PyObject *__pyx_codeobj__40;
-static PyObject *__pyx_codeobj__42;
-static PyObject *__pyx_codeobj__44;
-static PyObject *__pyx_codeobj__46;
-static PyObject *__pyx_codeobj__48;
-static PyObject *__pyx_codeobj__50;
-static PyObject *__pyx_codeobj__52;
-static PyObject *__pyx_codeobj__54;
-static PyObject *__pyx_codeobj__56;
-static PyObject *__pyx_codeobj__58;
-static PyObject *__pyx_codeobj__60;
-static PyObject *__pyx_codeobj__62;
-static PyObject *__pyx_codeobj__64;
-static PyObject *__pyx_codeobj__66;
-static PyObject *__pyx_codeobj__68;
-static PyObject *__pyx_codeobj__70;
-static PyObject *__pyx_codeobj__72;
-static PyObject *__pyx_codeobj__74;
-static PyObject *__pyx_codeobj__76;
-static PyObject *__pyx_codeobj__78;
-static PyObject *__pyx_codeobj__80;
-static PyObject *__pyx_codeobj__82;
+static PyObject *__pyx_tuple__20;
+static PyObject *__pyx_tuple__22;
+static PyObject *__pyx_tuple__24;
+static PyObject *__pyx_tuple__26;
+static PyObject *__pyx_tuple__28;
+static PyObject *__pyx_tuple__30;
+static PyObject *__pyx_tuple__32;
+static PyObject *__pyx_tuple__34;
+static PyObject *__pyx_tuple__36;
+static PyObject *__pyx_tuple__38;
+static PyObject *__pyx_tuple__40;
+static PyObject *__pyx_tuple__42;
+static PyObject *__pyx_tuple__44;
+static PyObject *__pyx_tuple__46;
+static PyObject *__pyx_tuple__48;
+static PyObject *__pyx_tuple__50;
+static PyObject *__pyx_tuple__52;
+static PyObject *__pyx_tuple__54;
+static PyObject *__pyx_tuple__56;
+static PyObject *__pyx_tuple__58;
+static PyObject *__pyx_tuple__60;
+static PyObject *__pyx_tuple__62;
+static PyObject *__pyx_tuple__64;
+static PyObject *__pyx_tuple__66;
+static PyObject *__pyx_tuple__68;
+static PyObject *__pyx_tuple__70;
+static PyObject *__pyx_tuple__72;
+static PyObject *__pyx_tuple__74;
+static PyObject *__pyx_tuple__76;
+static PyObject *__pyx_codeobj__15;
+static PyObject *__pyx_codeobj__17;
+static PyObject *__pyx_codeobj__19;
+static PyObject *__pyx_codeobj__21;
+static PyObject *__pyx_codeobj__23;
+static PyObject *__pyx_codeobj__25;
+static PyObject *__pyx_codeobj__27;
+static PyObject *__pyx_codeobj__29;
+static PyObject *__pyx_codeobj__31;
+static PyObject *__pyx_codeobj__33;
+static PyObject *__pyx_codeobj__35;
+static PyObject *__pyx_codeobj__37;
+static PyObject *__pyx_codeobj__39;
+static PyObject *__pyx_codeobj__41;
+static PyObject *__pyx_codeobj__43;
+static PyObject *__pyx_codeobj__45;
+static PyObject *__pyx_codeobj__47;
+static PyObject *__pyx_codeobj__49;
+static PyObject *__pyx_codeobj__51;
+static PyObject *__pyx_codeobj__53;
+static PyObject *__pyx_codeobj__55;
+static PyObject *__pyx_codeobj__57;
+static PyObject *__pyx_codeobj__59;
+static PyObject *__pyx_codeobj__61;
+static PyObject *__pyx_codeobj__63;
+static PyObject *__pyx_codeobj__65;
+static PyObject *__pyx_codeobj__67;
+static PyObject *__pyx_codeobj__69;
+static PyObject *__pyx_codeobj__71;
+static PyObject *__pyx_codeobj__73;
+static PyObject *__pyx_codeobj__75;
+static PyObject *__pyx_codeobj__77;
 /* Late includes */
 
-/* "cf_units/_udunits2.pyx":50
+/* "cf_units/_udunits2.pyx":49
  *     cdef ut_system *csystem
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.csystem = NULL
  * 
  */
 
@@ -2511,38 +2528,38 @@
 }
 
 static int __pyx_pf_8cf_units_9_udunits2_6System___cinit__(struct __pyx_obj_8cf_units_9_udunits2_System *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "cf_units/_udunits2.pyx":51
+  /* "cf_units/_udunits2.pyx":50
  * 
  *     def __cinit__(self):
  *         self.csystem = NULL             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
   __pyx_v_self->csystem = NULL;
 
-  /* "cf_units/_udunits2.pyx":50
+  /* "cf_units/_udunits2.pyx":49
  *     cdef ut_system *csystem
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.csystem = NULL
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":53
+/* "cf_units/_udunits2.pyx":52
  *         self.csystem = NULL
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         ut_free_system(self.csystem)
  * 
  */
 
@@ -2557,24 +2574,24 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8cf_units_9_udunits2_6System_2__dealloc__(struct __pyx_obj_8cf_units_9_udunits2_System *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "cf_units/_udunits2.pyx":54
+  /* "cf_units/_udunits2.pyx":53
  * 
  *     def __dealloc__(self):
  *         ut_free_system(self.csystem)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   ut_free_system(__pyx_v_self->csystem);
 
-  /* "cf_units/_udunits2.pyx":53
+  /* "cf_units/_udunits2.pyx":52
  *         self.csystem = NULL
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         ut_free_system(self.csystem)
  * 
  */
 
@@ -2691,15 +2708,15 @@
   __Pyx_AddTraceback("cf_units._udunits2.System.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":66
+/* "cf_units/_udunits2.pyx":65
  *     cdef System system
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.cunit = NULL
  *         self.system = None
  */
 
@@ -2720,51 +2737,51 @@
 }
 
 static int __pyx_pf_8cf_units_9_udunits2_4Unit___cinit__(struct __pyx_obj_8cf_units_9_udunits2_Unit *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "cf_units/_udunits2.pyx":67
+  /* "cf_units/_udunits2.pyx":66
  * 
  *     def __cinit__(self):
  *         self.cunit = NULL             # <<<<<<<<<<<<<<
  *         self.system = None
  * 
  */
   __pyx_v_self->cunit = NULL;
 
-  /* "cf_units/_udunits2.pyx":68
+  /* "cf_units/_udunits2.pyx":67
  *     def __cinit__(self):
  *         self.cunit = NULL
  *         self.system = None             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->system);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->system));
   __pyx_v_self->system = ((struct __pyx_obj_8cf_units_9_udunits2_System *)Py_None);
 
-  /* "cf_units/_udunits2.pyx":66
+  /* "cf_units/_udunits2.pyx":65
  *     cdef System system
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.cunit = NULL
  *         self.system = None
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":70
+/* "cf_units/_udunits2.pyx":69
  *         self.system = None
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         ut_free(self.cunit)
  * 
  */
 
@@ -2779,24 +2796,24 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8cf_units_9_udunits2_4Unit_2__dealloc__(struct __pyx_obj_8cf_units_9_udunits2_Unit *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "cf_units/_udunits2.pyx":71
+  /* "cf_units/_udunits2.pyx":70
  * 
  *     def __dealloc__(self):
  *         ut_free(self.cunit)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   ut_free(__pyx_v_self->cunit);
 
-  /* "cf_units/_udunits2.pyx":70
+  /* "cf_units/_udunits2.pyx":69
  *         self.system = None
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         ut_free(self.cunit)
  * 
  */
 
@@ -2913,15 +2930,15 @@
   __Pyx_AddTraceback("cf_units._udunits2.Unit.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":82
+/* "cf_units/_udunits2.pyx":81
  *     cdef cv_converter *cconverter
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.cconverter = NULL
  * 
  */
 
@@ -2942,38 +2959,38 @@
 }
 
 static int __pyx_pf_8cf_units_9_udunits2_9Converter___cinit__(struct __pyx_obj_8cf_units_9_udunits2_Converter *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "cf_units/_udunits2.pyx":83
+  /* "cf_units/_udunits2.pyx":82
  * 
  *     def __cinit__(self):
  *         self.cconverter = NULL             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
   __pyx_v_self->cconverter = NULL;
 
-  /* "cf_units/_udunits2.pyx":82
+  /* "cf_units/_udunits2.pyx":81
  *     cdef cv_converter *cconverter
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.cconverter = NULL
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":85
+/* "cf_units/_udunits2.pyx":84
  *         self.cconverter = NULL
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         cv_free(self.cconverter)
  * 
  */
 
@@ -2988,24 +3005,24 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8cf_units_9_udunits2_9Converter_2__dealloc__(struct __pyx_obj_8cf_units_9_udunits2_Converter *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "cf_units/_udunits2.pyx":86
+  /* "cf_units/_udunits2.pyx":85
  * 
  *     def __dealloc__(self):
  *         cv_free(self.cconverter)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   cv_free(__pyx_v_self->cconverter);
 
-  /* "cf_units/_udunits2.pyx":85
+  /* "cf_units/_udunits2.pyx":84
  *         self.cconverter = NULL
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         cv_free(self.cconverter)
  * 
  */
 
@@ -3122,15 +3139,15 @@
   __Pyx_AddTraceback("cf_units._udunits2.Converter.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":96
+/* "cf_units/_udunits2.pyx":95
  *     cdef ut_error_message_handler chandler
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.chandler = NULL
  * 
  */
 
@@ -3151,24 +3168,24 @@
 }
 
 static int __pyx_pf_8cf_units_9_udunits2_19ErrorMessageHandler___cinit__(struct __pyx_obj_8cf_units_9_udunits2_ErrorMessageHandler *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "cf_units/_udunits2.pyx":97
+  /* "cf_units/_udunits2.pyx":96
  * 
  *     def __cinit__(self):
  *         self.chandler = NULL             # <<<<<<<<<<<<<<
  * 
  * # The following wrap_* functions should be called directly after the api call
  */
   __pyx_v_self->chandler = NULL;
 
-  /* "cf_units/_udunits2.pyx":96
+  /* "cf_units/_udunits2.pyx":95
  *     cdef ut_error_message_handler chandler
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.chandler = NULL
  * 
  */
 
@@ -3287,15 +3304,15 @@
   __Pyx_AddTraceback("cf_units._udunits2.ErrorMessageHandler.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":103
+/* "cf_units/_udunits2.pyx":102
  * # correct ut_status and errno values are retreived by _raise_error()
  * 
  * cdef System wrap_system(ut_system* csystem):             # <<<<<<<<<<<<<<
  *     if csystem is NULL:
  *         _raise_error()
  */
 
@@ -3308,93 +3325,93 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("wrap_system", 0);
 
-  /* "cf_units/_udunits2.pyx":104
+  /* "cf_units/_udunits2.pyx":103
  * 
  * cdef System wrap_system(ut_system* csystem):
  *     if csystem is NULL:             # <<<<<<<<<<<<<<
  *         _raise_error()
  *     cdef System sytem = System()
  */
   __pyx_t_1 = ((__pyx_v_csystem == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "cf_units/_udunits2.pyx":105
+    /* "cf_units/_udunits2.pyx":104
  * cdef System wrap_system(ut_system* csystem):
  *     if csystem is NULL:
  *         _raise_error()             # <<<<<<<<<<<<<<
  *     cdef System sytem = System()
  *     sytem.csystem = csystem
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_raise_error); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 105, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_raise_error); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 104, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 105, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 104, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "cf_units/_udunits2.pyx":104
+    /* "cf_units/_udunits2.pyx":103
  * 
  * cdef System wrap_system(ut_system* csystem):
  *     if csystem is NULL:             # <<<<<<<<<<<<<<
  *         _raise_error()
  *     cdef System sytem = System()
  */
   }
 
-  /* "cf_units/_udunits2.pyx":106
+  /* "cf_units/_udunits2.pyx":105
  *     if csystem is NULL:
  *         _raise_error()
  *     cdef System sytem = System()             # <<<<<<<<<<<<<<
  *     sytem.csystem = csystem
  *     return sytem
  */
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8cf_units_9_udunits2_System)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 106, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8cf_units_9_udunits2_System)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_sytem = ((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "cf_units/_udunits2.pyx":107
+  /* "cf_units/_udunits2.pyx":106
  *         _raise_error()
  *     cdef System sytem = System()
  *     sytem.csystem = csystem             # <<<<<<<<<<<<<<
  *     return sytem
  * 
  */
   __pyx_v_sytem->csystem = __pyx_v_csystem;
 
-  /* "cf_units/_udunits2.pyx":108
+  /* "cf_units/_udunits2.pyx":107
  *     cdef System sytem = System()
  *     sytem.csystem = csystem
  *     return sytem             # <<<<<<<<<<<<<<
  * 
  * cdef Unit wrap_unit(System system, ut_unit* cunit):
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_sytem));
   __pyx_r = __pyx_v_sytem;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":103
+  /* "cf_units/_udunits2.pyx":102
  * # correct ut_status and errno values are retreived by _raise_error()
  * 
  * cdef System wrap_system(ut_system* csystem):             # <<<<<<<<<<<<<<
  *     if csystem is NULL:
  *         _raise_error()
  */
 
@@ -3408,15 +3425,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_sytem);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":110
+/* "cf_units/_udunits2.pyx":109
  *     return sytem
  * 
  * cdef Unit wrap_unit(System system, ut_unit* cunit):             # <<<<<<<<<<<<<<
  *     if cunit is NULL:
  *         _raise_error()
  */
 
@@ -3429,106 +3446,106 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("wrap_unit", 0);
 
-  /* "cf_units/_udunits2.pyx":111
+  /* "cf_units/_udunits2.pyx":110
  * 
  * cdef Unit wrap_unit(System system, ut_unit* cunit):
  *     if cunit is NULL:             # <<<<<<<<<<<<<<
  *         _raise_error()
  *     cdef Unit unit = Unit()
  */
   __pyx_t_1 = ((__pyx_v_cunit == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "cf_units/_udunits2.pyx":112
+    /* "cf_units/_udunits2.pyx":111
  * cdef Unit wrap_unit(System system, ut_unit* cunit):
  *     if cunit is NULL:
  *         _raise_error()             # <<<<<<<<<<<<<<
  *     cdef Unit unit = Unit()
  *     unit.cunit = cunit
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_raise_error); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 112, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_raise_error); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 112, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "cf_units/_udunits2.pyx":111
+    /* "cf_units/_udunits2.pyx":110
  * 
  * cdef Unit wrap_unit(System system, ut_unit* cunit):
  *     if cunit is NULL:             # <<<<<<<<<<<<<<
  *         _raise_error()
  *     cdef Unit unit = Unit()
  */
   }
 
-  /* "cf_units/_udunits2.pyx":113
+  /* "cf_units/_udunits2.pyx":112
  *     if cunit is NULL:
  *         _raise_error()
  *     cdef Unit unit = Unit()             # <<<<<<<<<<<<<<
  *     unit.cunit = cunit
  *     unit.system = system
  */
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8cf_units_9_udunits2_Unit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 113, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8cf_units_9_udunits2_Unit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_unit = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "cf_units/_udunits2.pyx":114
+  /* "cf_units/_udunits2.pyx":113
  *         _raise_error()
  *     cdef Unit unit = Unit()
  *     unit.cunit = cunit             # <<<<<<<<<<<<<<
  *     unit.system = system
  *     return unit
  */
   __pyx_v_unit->cunit = __pyx_v_cunit;
 
-  /* "cf_units/_udunits2.pyx":115
+  /* "cf_units/_udunits2.pyx":114
  *     cdef Unit unit = Unit()
  *     unit.cunit = cunit
  *     unit.system = system             # <<<<<<<<<<<<<<
  *     return unit
  * 
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_system));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_system));
   __Pyx_GOTREF(__pyx_v_unit->system);
   __Pyx_DECREF(((PyObject *)__pyx_v_unit->system));
   __pyx_v_unit->system = __pyx_v_system;
 
-  /* "cf_units/_udunits2.pyx":116
+  /* "cf_units/_udunits2.pyx":115
  *     unit.cunit = cunit
  *     unit.system = system
  *     return unit             # <<<<<<<<<<<<<<
  * 
  * cdef Converter wrap_converter(cv_converter* cconverter):
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_unit));
   __pyx_r = __pyx_v_unit;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":110
+  /* "cf_units/_udunits2.pyx":109
  *     return sytem
  * 
  * cdef Unit wrap_unit(System system, ut_unit* cunit):             # <<<<<<<<<<<<<<
  *     if cunit is NULL:
  *         _raise_error()
  */
 
@@ -3542,15 +3559,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_unit);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":118
+/* "cf_units/_udunits2.pyx":117
  *     return unit
  * 
  * cdef Converter wrap_converter(cv_converter* cconverter):             # <<<<<<<<<<<<<<
  *     if cconverter is NULL:
  *         _raise_error()
  */
 
@@ -3563,93 +3580,93 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("wrap_converter", 0);
 
-  /* "cf_units/_udunits2.pyx":119
+  /* "cf_units/_udunits2.pyx":118
  * 
  * cdef Converter wrap_converter(cv_converter* cconverter):
  *     if cconverter is NULL:             # <<<<<<<<<<<<<<
  *         _raise_error()
  *     cdef Converter converter = Converter()
  */
   __pyx_t_1 = ((__pyx_v_cconverter == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "cf_units/_udunits2.pyx":120
+    /* "cf_units/_udunits2.pyx":119
  * cdef Converter wrap_converter(cv_converter* cconverter):
  *     if cconverter is NULL:
  *         _raise_error()             # <<<<<<<<<<<<<<
  *     cdef Converter converter = Converter()
  *     converter.cconverter = cconverter
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_raise_error); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 120, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_raise_error); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 119, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 120, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 119, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "cf_units/_udunits2.pyx":119
+    /* "cf_units/_udunits2.pyx":118
  * 
  * cdef Converter wrap_converter(cv_converter* cconverter):
  *     if cconverter is NULL:             # <<<<<<<<<<<<<<
  *         _raise_error()
  *     cdef Converter converter = Converter()
  */
   }
 
-  /* "cf_units/_udunits2.pyx":121
+  /* "cf_units/_udunits2.pyx":120
  *     if cconverter is NULL:
  *         _raise_error()
  *     cdef Converter converter = Converter()             # <<<<<<<<<<<<<<
  *     converter.cconverter = cconverter
  *     return converter
  */
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8cf_units_9_udunits2_Converter)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 121, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8cf_units_9_udunits2_Converter)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_converter = ((struct __pyx_obj_8cf_units_9_udunits2_Converter *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "cf_units/_udunits2.pyx":122
+  /* "cf_units/_udunits2.pyx":121
  *         _raise_error()
  *     cdef Converter converter = Converter()
  *     converter.cconverter = cconverter             # <<<<<<<<<<<<<<
  *     return converter
  * 
  */
   __pyx_v_converter->cconverter = __pyx_v_cconverter;
 
-  /* "cf_units/_udunits2.pyx":123
+  /* "cf_units/_udunits2.pyx":122
  *     cdef Converter converter = Converter()
  *     converter.cconverter = cconverter
  *     return converter             # <<<<<<<<<<<<<<
  * 
  * cdef ErrorMessageHandler _ignore = ErrorMessageHandler()
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_converter));
   __pyx_r = __pyx_v_converter;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":118
+  /* "cf_units/_udunits2.pyx":117
  *     return unit
  * 
  * cdef Converter wrap_converter(cv_converter* cconverter):             # <<<<<<<<<<<<<<
  *     if cconverter is NULL:
  *         _raise_error()
  */
 
@@ -3663,15 +3680,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_converter);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":148
+/* "cf_units/_udunits2.pyx":147
  * 
  *     """
  *     def __init__(self, ut_status status, int errnum):             # <<<<<<<<<<<<<<
  *         self.status = status
  *         self.errnum = errnum
  */
 
@@ -3709,40 +3726,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_status)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(1, 148, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(1, 147, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_errnum)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(1, 148, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(1, 147, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(1, 148, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(1, 147, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
-    __pyx_v_status = ((ut_status)__Pyx_PyInt_As_ut_status(values[1])); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 148, __pyx_L3_error)
-    __pyx_v_errnum = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_errnum == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 148, __pyx_L3_error)
+    __pyx_v_status = ((ut_status)__Pyx_PyInt_As_ut_status(values[1])); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 147, __pyx_L3_error)
+    __pyx_v_errnum = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_errnum == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 147, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 148, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 147, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.UdunitsError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_12UdunitsError___init__(__pyx_self, __pyx_v_self, __pyx_v_status, __pyx_v_errnum);
 
@@ -3756,39 +3773,39 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "cf_units/_udunits2.pyx":149
+  /* "cf_units/_udunits2.pyx":148
  *     """
  *     def __init__(self, ut_status status, int errnum):
  *         self.status = status             # <<<<<<<<<<<<<<
  *         self.errnum = errnum
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_ut_status(__pyx_v_status); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 149, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_ut_status(__pyx_v_status); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_status, __pyx_t_1) < 0) __PYX_ERR(1, 149, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_status, __pyx_t_1) < 0) __PYX_ERR(1, 148, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":150
+  /* "cf_units/_udunits2.pyx":149
  *     def __init__(self, ut_status status, int errnum):
  *         self.status = status
  *         self.errnum = errnum             # <<<<<<<<<<<<<<
  * 
  *     def status_msg(self):
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_errnum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 150, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_errnum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_errnum, __pyx_t_1) < 0) __PYX_ERR(1, 150, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_errnum, __pyx_t_1) < 0) __PYX_ERR(1, 149, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":148
+  /* "cf_units/_udunits2.pyx":147
  * 
  *     """
  *     def __init__(self, ut_status status, int errnum):             # <<<<<<<<<<<<<<
  *         self.status = status
  *         self.errnum = errnum
  */
 
@@ -3801,15 +3818,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":152
+/* "cf_units/_udunits2.pyx":151
  *         self.errnum = errnum
  * 
  *     def status_msg(self):             # <<<<<<<<<<<<<<
  *         """
  *         String representation of the UDUNITS-2 ut_status value which resulted
  */
 
@@ -3837,89 +3854,89 @@
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("status_msg", 0);
 
-  /* "cf_units/_udunits2.pyx":158
+  /* "cf_units/_udunits2.pyx":157
  * 
  *         """
  *         if 0 <= self.status < len(_UT_STATUS):             # <<<<<<<<<<<<<<
  *             return _UT_STATUS[self.status]
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_status); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 158, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_status); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 157, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_int_0, __pyx_t_1, Py_LE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 158, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_int_0, __pyx_t_1, Py_LE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 157, __pyx_L1_error)
   if (__Pyx_PyObject_IsTrue(__pyx_t_2)) {
     __Pyx_DECREF(__pyx_t_2);
     __pyx_t_3 = __pyx_v_8cf_units_9_udunits2__UT_STATUS;
     __Pyx_INCREF(__pyx_t_3);
     if (unlikely(__pyx_t_3 == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(1, 158, __pyx_L1_error)
+      __PYX_ERR(1, 157, __pyx_L1_error)
     }
-    __pyx_t_4 = PyList_GET_SIZE(__pyx_t_3); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 158, __pyx_L1_error)
+    __pyx_t_4 = PyList_GET_SIZE(__pyx_t_3); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 157, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 158, __pyx_L1_error)
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 157, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 158, __pyx_L1_error)
+    __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 157, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(1, 158, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(1, 157, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_5) {
 
-    /* "cf_units/_udunits2.pyx":159
+    /* "cf_units/_udunits2.pyx":158
  *         """
  *         if 0 <= self.status < len(_UT_STATUS):
  *             return _UT_STATUS[self.status]             # <<<<<<<<<<<<<<
  *         else:
  *             return 'UNKNOWN'
  */
     __Pyx_XDECREF(__pyx_r);
     if (unlikely(__pyx_v_8cf_units_9_udunits2__UT_STATUS == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 159, __pyx_L1_error)
+      __PYX_ERR(1, 158, __pyx_L1_error)
     }
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_status); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 159, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_status); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_8cf_units_9_udunits2__UT_STATUS, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 159, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_8cf_units_9_udunits2__UT_STATUS, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "cf_units/_udunits2.pyx":158
+    /* "cf_units/_udunits2.pyx":157
  * 
  *         """
  *         if 0 <= self.status < len(_UT_STATUS):             # <<<<<<<<<<<<<<
  *             return _UT_STATUS[self.status]
  *         else:
  */
   }
 
-  /* "cf_units/_udunits2.pyx":161
+  /* "cf_units/_udunits2.pyx":160
  *             return _UT_STATUS[self.status]
  *         else:
  *             return 'UNKNOWN'             # <<<<<<<<<<<<<<
  * 
  *     def error_msg(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_n_s_UNKNOWN);
     __pyx_r = __pyx_n_s_UNKNOWN;
     goto __pyx_L0;
   }
 
-  /* "cf_units/_udunits2.pyx":152
+  /* "cf_units/_udunits2.pyx":151
  *         self.errnum = errnum
  * 
  *     def status_msg(self):             # <<<<<<<<<<<<<<
  *         """
  *         String representation of the UDUNITS-2 ut_status value which resulted
  */
 
@@ -3932,15 +3949,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":163
+/* "cf_units/_udunits2.pyx":162
  *             return 'UNKNOWN'
  * 
  *     def error_msg(self):             # <<<<<<<<<<<<<<
  *         """
  *         The message string associated with the errno value which resulted from
  */
 
@@ -3967,44 +3984,44 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("error_msg", 0);
 
-  /* "cf_units/_udunits2.pyx":169
+  /* "cf_units/_udunits2.pyx":168
  * 
  *         """
  *         return string.strerror(self.errnum) if self.errnum else ''             # <<<<<<<<<<<<<<
  * 
  *     def __str__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_errnum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 169, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_errnum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(1, 169, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(1, 168, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_3) {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_errnum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 169, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_errnum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 168, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 169, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 168, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyBytes_FromString(strerror(__pyx_t_4)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 169, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_FromString(strerror(__pyx_t_4)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 168, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_s__9);
     __pyx_t_1 = __pyx_kp_s__9;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":163
+  /* "cf_units/_udunits2.pyx":162
  *             return 'UNKNOWN'
  * 
  *     def error_msg(self):             # <<<<<<<<<<<<<<
  *         """
  *         The message string associated with the errno value which resulted from
  */
 
@@ -4016,15 +4033,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":171
+/* "cf_units/_udunits2.pyx":170
  *         return string.strerror(self.errnum) if self.errnum else ''
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         str_err = ': {}'.format(string.strerror(self.errnum)) \
  *                   if self.errnum else ''
  */
 
@@ -4054,92 +4071,92 @@
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "cf_units/_udunits2.pyx":173
+  /* "cf_units/_udunits2.pyx":172
  *     def __str__(self):
  *         str_err = ': {}'.format(string.strerror(self.errnum)) \
  *                   if self.errnum else ''             # <<<<<<<<<<<<<<
  *         return '{}{}'.format(self.status_msg(), str_err)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_errnum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 173, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_errnum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(1, 173, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(1, 172, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_3) {
 
-    /* "cf_units/_udunits2.pyx":172
+    /* "cf_units/_udunits2.pyx":171
  * 
  *     def __str__(self):
  *         str_err = ': {}'.format(string.strerror(self.errnum)) \             # <<<<<<<<<<<<<<
  *                   if self.errnum else ''
  *         return '{}{}'.format(self.status_msg(), str_err)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__10, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 172, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__10, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 171, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_errnum); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 172, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_errnum); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 171, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_5); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 172, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_5); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 171, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyBytes_FromString(strerror(__pyx_t_6)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 172, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBytes_FromString(strerror(__pyx_t_6)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 171, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_7, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 172, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 171, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_s__9);
     __pyx_t_1 = __pyx_kp_s__9;
   }
   __pyx_v_str_err = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":174
+  /* "cf_units/_udunits2.pyx":173
  *         str_err = ': {}'.format(string.strerror(self.errnum)) \
  *                   if self.errnum else ''
  *         return '{}{}'.format(self.status_msg(), str_err)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__11, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 174, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s__11, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_status_msg); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 174, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_status_msg); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 174, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
@@ -4149,51 +4166,51 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_4, __pyx_v_str_err};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 174, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 173, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_4, __pyx_v_str_err};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 174, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 173, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 174, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 173, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_t_4);
     __Pyx_INCREF(__pyx_v_str_err);
     __Pyx_GIVEREF(__pyx_v_str_err);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_v_str_err);
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 174, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 173, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":171
+  /* "cf_units/_udunits2.pyx":170
  *         return string.strerror(self.errnum) if self.errnum else ''
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         str_err = ': {}'.format(string.strerror(self.errnum)) \
  *                   if self.errnum else ''
  */
 
@@ -4209,15 +4226,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_str_err);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":177
+/* "cf_units/_udunits2.pyx":176
  * 
  * 
  * def _raise_error():             # <<<<<<<<<<<<<<
  *     """
  *     Raise a UdunitsError with the current value of errno and ut_status
  */
 
@@ -4249,53 +4266,53 @@
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_raise_error", 0);
 
-  /* "cf_units/_udunits2.pyx":182
+  /* "cf_units/_udunits2.pyx":181
  * 
  *     """
  *     errnum = errno.errno             # <<<<<<<<<<<<<<
  *     errno.errno = 0
  *     status = ut_get_status()
  */
   __pyx_v_errnum = errno;
 
-  /* "cf_units/_udunits2.pyx":183
+  /* "cf_units/_udunits2.pyx":182
  *     """
  *     errnum = errno.errno
  *     errno.errno = 0             # <<<<<<<<<<<<<<
  *     status = ut_get_status()
  *     raise UdunitsError(status, errnum)
  */
   errno = 0;
 
-  /* "cf_units/_udunits2.pyx":184
+  /* "cf_units/_udunits2.pyx":183
  *     errnum = errno.errno
  *     errno.errno = 0
  *     status = ut_get_status()             # <<<<<<<<<<<<<<
  *     raise UdunitsError(status, errnum)
  * 
  */
   __pyx_v_status = ut_get_status();
 
-  /* "cf_units/_udunits2.pyx":185
+  /* "cf_units/_udunits2.pyx":184
  *     errno.errno = 0
  *     status = ut_get_status()
  *     raise UdunitsError(status, errnum)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_UdunitsError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 185, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_UdunitsError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 184, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_ut_status(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 185, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_ut_status(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 184, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_errnum); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 185, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_errnum); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 184, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -4304,53 +4321,53 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_3, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 185, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 184, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_3, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 185, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 184, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 185, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 184, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 185, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 184, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(1, 185, __pyx_L1_error)
+  __PYX_ERR(1, 184, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":177
+  /* "cf_units/_udunits2.pyx":176
  * 
  * 
  * def _raise_error():             # <<<<<<<<<<<<<<
  *     """
  *     Raise a UdunitsError with the current value of errno and ut_status
  */
 
@@ -4365,15 +4382,15 @@
   __Pyx_AddTraceback("cf_units._udunits2._raise_error", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":193
+/* "cf_units/_udunits2.pyx":192
  * # See the UDUNITS-2 documentation for details.
  * 
  * def read_xml(char* path=NULL):             # <<<<<<<<<<<<<<
  *     cdef ut_system* csystem = ut_read_xml(path)
  *     return wrap_system(csystem)
  */
 
@@ -4405,33 +4422,33 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_path);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_xml") < 0)) __PYX_ERR(1, 193, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_xml") < 0)) __PYX_ERR(1, 192, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_path = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_path) && PyErr_Occurred())) __PYX_ERR(1, 193, __pyx_L3_error)
+      __pyx_v_path = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_path) && PyErr_Occurred())) __PYX_ERR(1, 192, __pyx_L3_error)
     } else {
       __pyx_v_path = ((char *)NULL);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("read_xml", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 193, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("read_xml", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 192, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.read_xml", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_2read_xml(__pyx_self, __pyx_v_path);
 
@@ -4446,38 +4463,38 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_xml", 0);
 
-  /* "cf_units/_udunits2.pyx":194
+  /* "cf_units/_udunits2.pyx":193
  * 
  * def read_xml(char* path=NULL):
  *     cdef ut_system* csystem = ut_read_xml(path)             # <<<<<<<<<<<<<<
  *     return wrap_system(csystem)
  * 
  */
   __pyx_v_csystem = ut_read_xml(__pyx_v_path);
 
-  /* "cf_units/_udunits2.pyx":195
+  /* "cf_units/_udunits2.pyx":194
  * def read_xml(char* path=NULL):
  *     cdef ut_system* csystem = ut_read_xml(path)
  *     return wrap_system(csystem)             # <<<<<<<<<<<<<<
  * 
  * def get_unit_by_name(System system, char* name):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_system(__pyx_v_csystem)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 195, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_system(__pyx_v_csystem)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":193
+  /* "cf_units/_udunits2.pyx":192
  * # See the UDUNITS-2 documentation for details.
  * 
  * def read_xml(char* path=NULL):             # <<<<<<<<<<<<<<
  *     cdef ut_system* csystem = ut_read_xml(path)
  *     return wrap_system(csystem)
  */
 
@@ -4488,15 +4505,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":197
+/* "cf_units/_udunits2.pyx":196
  *     return wrap_system(csystem)
  * 
  * def get_unit_by_name(System system, char* name):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_get_unit_by_name(system.csystem, name)
  *     return wrap_unit(system, cunit)
  */
 
@@ -4531,38 +4548,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_system)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_unit_by_name", 1, 2, 2, 1); __PYX_ERR(1, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_unit_by_name", 1, 2, 2, 1); __PYX_ERR(1, 196, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_unit_by_name") < 0)) __PYX_ERR(1, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_unit_by_name") < 0)) __PYX_ERR(1, 196, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_system = ((struct __pyx_obj_8cf_units_9_udunits2_System *)values[0]);
-    __pyx_v_name = __Pyx_PyObject_AsWritableString(values[1]); if (unlikely((!__pyx_v_name) && PyErr_Occurred())) __PYX_ERR(1, 197, __pyx_L3_error)
+    __pyx_v_name = __Pyx_PyObject_AsWritableString(values[1]); if (unlikely((!__pyx_v_name) && PyErr_Occurred())) __PYX_ERR(1, 196, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_unit_by_name", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_unit_by_name", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 196, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.get_unit_by_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_system), __pyx_ptype_8cf_units_9_udunits2_System, 1, "system", 0))) __PYX_ERR(1, 197, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_system), __pyx_ptype_8cf_units_9_udunits2_System, 1, "system", 0))) __PYX_ERR(1, 196, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_4get_unit_by_name(__pyx_self, __pyx_v_system, __pyx_v_name);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4576,38 +4593,38 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_unit_by_name", 0);
 
-  /* "cf_units/_udunits2.pyx":198
+  /* "cf_units/_udunits2.pyx":197
  * 
  * def get_unit_by_name(System system, char* name):
  *     cdef ut_unit* cunit = ut_get_unit_by_name(system.csystem, name)             # <<<<<<<<<<<<<<
  *     return wrap_unit(system, cunit)
  * 
  */
   __pyx_v_cunit = ut_get_unit_by_name(__pyx_v_system->csystem, __pyx_v_name);
 
-  /* "cf_units/_udunits2.pyx":199
+  /* "cf_units/_udunits2.pyx":198
  * def get_unit_by_name(System system, char* name):
  *     cdef ut_unit* cunit = ut_get_unit_by_name(system.csystem, name)
  *     return wrap_unit(system, cunit)             # <<<<<<<<<<<<<<
  * 
  * def clone(Unit unit):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(__pyx_v_system, __pyx_v_cunit)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(__pyx_v_system, __pyx_v_cunit)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":197
+  /* "cf_units/_udunits2.pyx":196
  *     return wrap_system(csystem)
  * 
  * def get_unit_by_name(System system, char* name):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_get_unit_by_name(system.csystem, name)
  *     return wrap_unit(system, cunit)
  */
 
@@ -4618,15 +4635,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":201
+/* "cf_units/_udunits2.pyx":200
  *     return wrap_unit(system, cunit)
  * 
  * def clone(Unit unit):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_clone(unit.cunit)
  *     return wrap_unit(unit.system, cunit)
  */
 
@@ -4636,15 +4653,15 @@
 static PyObject *__pyx_pw_8cf_units_9_udunits2_7clone(PyObject *__pyx_self, PyObject *__pyx_v_unit) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("clone (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 201, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 200, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_6clone(__pyx_self, ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)__pyx_v_unit));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4659,41 +4676,41 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clone", 0);
 
-  /* "cf_units/_udunits2.pyx":202
+  /* "cf_units/_udunits2.pyx":201
  * 
  * def clone(Unit unit):
  *     cdef ut_unit* cunit = ut_clone(unit.cunit)             # <<<<<<<<<<<<<<
  *     return wrap_unit(unit.system, cunit)
  * 
  */
   __pyx_v_cunit = ut_clone(__pyx_v_unit->cunit);
 
-  /* "cf_units/_udunits2.pyx":203
+  /* "cf_units/_udunits2.pyx":202
  * def clone(Unit unit):
  *     cdef ut_unit* cunit = ut_clone(unit.cunit)
  *     return wrap_unit(unit.system, cunit)             # <<<<<<<<<<<<<<
  * 
  * def is_dimensionless(Unit unit):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = ((PyObject *)__pyx_v_unit->system);
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 203, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":201
+  /* "cf_units/_udunits2.pyx":200
  *     return wrap_unit(system, cunit)
  * 
  * def clone(Unit unit):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_clone(unit.cunit)
  *     return wrap_unit(unit.system, cunit)
  */
 
@@ -4705,15 +4722,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":205
+/* "cf_units/_udunits2.pyx":204
  *     return wrap_unit(unit.system, cunit)
  * 
  * def is_dimensionless(Unit unit):             # <<<<<<<<<<<<<<
  *     return <bint>ut_is_dimensionless(unit.cunit)
  * 
  */
 
@@ -4723,15 +4740,15 @@
 static PyObject *__pyx_pw_8cf_units_9_udunits2_9is_dimensionless(PyObject *__pyx_self, PyObject *__pyx_v_unit) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_dimensionless (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 205, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 204, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_8is_dimensionless(__pyx_self, ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)__pyx_v_unit));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4744,29 +4761,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_dimensionless", 0);
 
-  /* "cf_units/_udunits2.pyx":206
+  /* "cf_units/_udunits2.pyx":205
  * 
  * def is_dimensionless(Unit unit):
  *     return <bint>ut_is_dimensionless(unit.cunit)             # <<<<<<<<<<<<<<
  * 
  * def compare(Unit unit1, Unit unit2):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong((ut_is_dimensionless(__pyx_v_unit->cunit) != 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 206, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((ut_is_dimensionless(__pyx_v_unit->cunit) != 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":205
+  /* "cf_units/_udunits2.pyx":204
  *     return wrap_unit(unit.system, cunit)
  * 
  * def is_dimensionless(Unit unit):             # <<<<<<<<<<<<<<
  *     return <bint>ut_is_dimensionless(unit.cunit)
  * 
  */
 
@@ -4777,15 +4794,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":208
+/* "cf_units/_udunits2.pyx":207
  *     return <bint>ut_is_dimensionless(unit.cunit)
  * 
  * def compare(Unit unit1, Unit unit2):             # <<<<<<<<<<<<<<
  *     return ut_compare(unit1.cunit, unit2.cunit)
  * 
  */
 
@@ -4820,39 +4837,39 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_unit1)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_unit2)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("compare", 1, 2, 2, 1); __PYX_ERR(1, 208, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("compare", 1, 2, 2, 1); __PYX_ERR(1, 207, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "compare") < 0)) __PYX_ERR(1, 208, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "compare") < 0)) __PYX_ERR(1, 207, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_unit1 = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[0]);
     __pyx_v_unit2 = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("compare", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 208, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("compare", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 207, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.compare", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit1), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit1", 0))) __PYX_ERR(1, 208, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit2), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit2", 0))) __PYX_ERR(1, 208, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit1), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit1", 0))) __PYX_ERR(1, 207, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit2), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit2", 0))) __PYX_ERR(1, 207, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_10compare(__pyx_self, __pyx_v_unit1, __pyx_v_unit2);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4865,29 +4882,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compare", 0);
 
-  /* "cf_units/_udunits2.pyx":209
+  /* "cf_units/_udunits2.pyx":208
  * 
  * def compare(Unit unit1, Unit unit2):
  *     return ut_compare(unit1.cunit, unit2.cunit)             # <<<<<<<<<<<<<<
  * 
  * def are_convertible(Unit unit1, Unit unit2):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(ut_compare(__pyx_v_unit1->cunit, __pyx_v_unit2->cunit)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 209, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(ut_compare(__pyx_v_unit1->cunit, __pyx_v_unit2->cunit)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":208
+  /* "cf_units/_udunits2.pyx":207
  *     return <bint>ut_is_dimensionless(unit.cunit)
  * 
  * def compare(Unit unit1, Unit unit2):             # <<<<<<<<<<<<<<
  *     return ut_compare(unit1.cunit, unit2.cunit)
  * 
  */
 
@@ -4898,15 +4915,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":211
+/* "cf_units/_udunits2.pyx":210
  *     return ut_compare(unit1.cunit, unit2.cunit)
  * 
  * def are_convertible(Unit unit1, Unit unit2):             # <<<<<<<<<<<<<<
  *     return <bint>ut_are_convertible(unit1.cunit, unit2.cunit)
  * 
  */
 
@@ -4941,39 +4958,39 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_unit1)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_unit2)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("are_convertible", 1, 2, 2, 1); __PYX_ERR(1, 211, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("are_convertible", 1, 2, 2, 1); __PYX_ERR(1, 210, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "are_convertible") < 0)) __PYX_ERR(1, 211, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "are_convertible") < 0)) __PYX_ERR(1, 210, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_unit1 = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[0]);
     __pyx_v_unit2 = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("are_convertible", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 211, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("are_convertible", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 210, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.are_convertible", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit1), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit1", 0))) __PYX_ERR(1, 211, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit2), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit2", 0))) __PYX_ERR(1, 211, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit1), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit1", 0))) __PYX_ERR(1, 210, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit2), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit2", 0))) __PYX_ERR(1, 210, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_12are_convertible(__pyx_self, __pyx_v_unit1, __pyx_v_unit2);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4986,29 +5003,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("are_convertible", 0);
 
-  /* "cf_units/_udunits2.pyx":212
+  /* "cf_units/_udunits2.pyx":211
  * 
  * def are_convertible(Unit unit1, Unit unit2):
  *     return <bint>ut_are_convertible(unit1.cunit, unit2.cunit)             # <<<<<<<<<<<<<<
  * 
  * def get_converter(Unit fr, Unit to):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong((ut_are_convertible(__pyx_v_unit1->cunit, __pyx_v_unit2->cunit) != 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 212, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((ut_are_convertible(__pyx_v_unit1->cunit, __pyx_v_unit2->cunit) != 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":211
+  /* "cf_units/_udunits2.pyx":210
  *     return ut_compare(unit1.cunit, unit2.cunit)
  * 
  * def are_convertible(Unit unit1, Unit unit2):             # <<<<<<<<<<<<<<
  *     return <bint>ut_are_convertible(unit1.cunit, unit2.cunit)
  * 
  */
 
@@ -5019,15 +5036,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":214
+/* "cf_units/_udunits2.pyx":213
  *     return <bint>ut_are_convertible(unit1.cunit, unit2.cunit)
  * 
  * def get_converter(Unit fr, Unit to):             # <<<<<<<<<<<<<<
  *     cdef cv_converter* cconverter = ut_get_converter(fr.cunit, to.cunit)
  *     return wrap_converter(cconverter)
  */
 
@@ -5062,39 +5079,39 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fr)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_to)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_converter", 1, 2, 2, 1); __PYX_ERR(1, 214, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_converter", 1, 2, 2, 1); __PYX_ERR(1, 213, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_converter") < 0)) __PYX_ERR(1, 214, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_converter") < 0)) __PYX_ERR(1, 213, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_fr = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[0]);
     __pyx_v_to = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_converter", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 214, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_converter", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 213, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.get_converter", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fr), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "fr", 0))) __PYX_ERR(1, 214, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_to), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "to", 0))) __PYX_ERR(1, 214, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fr), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "fr", 0))) __PYX_ERR(1, 213, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_to), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "to", 0))) __PYX_ERR(1, 213, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_14get_converter(__pyx_self, __pyx_v_fr, __pyx_v_to);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5108,38 +5125,38 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_converter", 0);
 
-  /* "cf_units/_udunits2.pyx":215
+  /* "cf_units/_udunits2.pyx":214
  * 
  * def get_converter(Unit fr, Unit to):
  *     cdef cv_converter* cconverter = ut_get_converter(fr.cunit, to.cunit)             # <<<<<<<<<<<<<<
  *     return wrap_converter(cconverter)
  * 
  */
   __pyx_v_cconverter = ut_get_converter(__pyx_v_fr->cunit, __pyx_v_to->cunit);
 
-  /* "cf_units/_udunits2.pyx":216
+  /* "cf_units/_udunits2.pyx":215
  * def get_converter(Unit fr, Unit to):
  *     cdef cv_converter* cconverter = ut_get_converter(fr.cunit, to.cunit)
  *     return wrap_converter(cconverter)             # <<<<<<<<<<<<<<
  * 
  * def scale(double factor, Unit unit):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_converter(__pyx_v_cconverter)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 216, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_converter(__pyx_v_cconverter)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":214
+  /* "cf_units/_udunits2.pyx":213
  *     return <bint>ut_are_convertible(unit1.cunit, unit2.cunit)
  * 
  * def get_converter(Unit fr, Unit to):             # <<<<<<<<<<<<<<
  *     cdef cv_converter* cconverter = ut_get_converter(fr.cunit, to.cunit)
  *     return wrap_converter(cconverter)
  */
 
@@ -5150,15 +5167,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":218
+/* "cf_units/_udunits2.pyx":217
  *     return wrap_converter(cconverter)
  * 
  * def scale(double factor, Unit unit):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_scale(factor, unit.cunit)
  *     return wrap_unit(unit.system, cunit)
  */
 
@@ -5193,38 +5210,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_factor)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_unit)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("scale", 1, 2, 2, 1); __PYX_ERR(1, 218, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("scale", 1, 2, 2, 1); __PYX_ERR(1, 217, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "scale") < 0)) __PYX_ERR(1, 218, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "scale") < 0)) __PYX_ERR(1, 217, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_factor = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_factor == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 218, __pyx_L3_error)
+    __pyx_v_factor = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_factor == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 217, __pyx_L3_error)
     __pyx_v_unit = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("scale", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 218, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("scale", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 217, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.scale", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 218, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 217, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_16scale(__pyx_self, __pyx_v_factor, __pyx_v_unit);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5239,41 +5256,41 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("scale", 0);
 
-  /* "cf_units/_udunits2.pyx":219
+  /* "cf_units/_udunits2.pyx":218
  * 
  * def scale(double factor, Unit unit):
  *     cdef ut_unit* cunit = ut_scale(factor, unit.cunit)             # <<<<<<<<<<<<<<
  *     return wrap_unit(unit.system, cunit)
  * 
  */
   __pyx_v_cunit = ut_scale(__pyx_v_factor, __pyx_v_unit->cunit);
 
-  /* "cf_units/_udunits2.pyx":220
+  /* "cf_units/_udunits2.pyx":219
  * def scale(double factor, Unit unit):
  *     cdef ut_unit* cunit = ut_scale(factor, unit.cunit)
  *     return wrap_unit(unit.system, cunit)             # <<<<<<<<<<<<<<
  * 
  * def offset(Unit unit, double offset):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = ((PyObject *)__pyx_v_unit->system);
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 220, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":218
+  /* "cf_units/_udunits2.pyx":217
  *     return wrap_converter(cconverter)
  * 
  * def scale(double factor, Unit unit):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_scale(factor, unit.cunit)
  *     return wrap_unit(unit.system, cunit)
  */
 
@@ -5285,15 +5302,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":222
+/* "cf_units/_udunits2.pyx":221
  *     return wrap_unit(unit.system, cunit)
  * 
  * def offset(Unit unit, double offset):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_offset(unit.cunit, offset)
  *     return wrap_unit(unit.system, cunit)
  */
 
@@ -5328,38 +5345,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_unit)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_offset)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("offset", 1, 2, 2, 1); __PYX_ERR(1, 222, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("offset", 1, 2, 2, 1); __PYX_ERR(1, 221, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "offset") < 0)) __PYX_ERR(1, 222, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "offset") < 0)) __PYX_ERR(1, 221, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_unit = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[0]);
-    __pyx_v_offset = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_offset == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 222, __pyx_L3_error)
+    __pyx_v_offset = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_offset == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 221, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("offset", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 222, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("offset", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 221, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.offset", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 222, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 221, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_18offset(__pyx_self, __pyx_v_unit, __pyx_v_offset);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5374,41 +5391,41 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("offset", 0);
 
-  /* "cf_units/_udunits2.pyx":223
+  /* "cf_units/_udunits2.pyx":222
  * 
  * def offset(Unit unit, double offset):
  *     cdef ut_unit* cunit = ut_offset(unit.cunit, offset)             # <<<<<<<<<<<<<<
  *     return wrap_unit(unit.system, cunit)
  * 
  */
   __pyx_v_cunit = ut_offset(__pyx_v_unit->cunit, __pyx_v_offset);
 
-  /* "cf_units/_udunits2.pyx":224
+  /* "cf_units/_udunits2.pyx":223
  * def offset(Unit unit, double offset):
  *     cdef ut_unit* cunit = ut_offset(unit.cunit, offset)
  *     return wrap_unit(unit.system, cunit)             # <<<<<<<<<<<<<<
  * 
  * def offset_by_time(Unit unit, double origin):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = ((PyObject *)__pyx_v_unit->system);
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 224, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":222
+  /* "cf_units/_udunits2.pyx":221
  *     return wrap_unit(unit.system, cunit)
  * 
  * def offset(Unit unit, double offset):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_offset(unit.cunit, offset)
  *     return wrap_unit(unit.system, cunit)
  */
 
@@ -5420,15 +5437,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":226
+/* "cf_units/_udunits2.pyx":225
  *     return wrap_unit(unit.system, cunit)
  * 
  * def offset_by_time(Unit unit, double origin):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_offset_by_time(unit.cunit, origin)
  *     return wrap_unit(unit.system, cunit)
  */
 
@@ -5463,38 +5480,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_unit)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_origin)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("offset_by_time", 1, 2, 2, 1); __PYX_ERR(1, 226, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("offset_by_time", 1, 2, 2, 1); __PYX_ERR(1, 225, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "offset_by_time") < 0)) __PYX_ERR(1, 226, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "offset_by_time") < 0)) __PYX_ERR(1, 225, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_unit = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[0]);
-    __pyx_v_origin = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_origin == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 226, __pyx_L3_error)
+    __pyx_v_origin = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_origin == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 225, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("offset_by_time", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 226, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("offset_by_time", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 225, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.offset_by_time", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 226, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 225, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_20offset_by_time(__pyx_self, __pyx_v_unit, __pyx_v_origin);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5509,41 +5526,41 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("offset_by_time", 0);
 
-  /* "cf_units/_udunits2.pyx":227
+  /* "cf_units/_udunits2.pyx":226
  * 
  * def offset_by_time(Unit unit, double origin):
  *     cdef ut_unit* cunit = ut_offset_by_time(unit.cunit, origin)             # <<<<<<<<<<<<<<
  *     return wrap_unit(unit.system, cunit)
  * 
  */
   __pyx_v_cunit = ut_offset_by_time(__pyx_v_unit->cunit, __pyx_v_origin);
 
-  /* "cf_units/_udunits2.pyx":228
+  /* "cf_units/_udunits2.pyx":227
  * def offset_by_time(Unit unit, double origin):
  *     cdef ut_unit* cunit = ut_offset_by_time(unit.cunit, origin)
  *     return wrap_unit(unit.system, cunit)             # <<<<<<<<<<<<<<
  * 
  * def multiply(Unit unit1, Unit unit2):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = ((PyObject *)__pyx_v_unit->system);
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 228, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":226
+  /* "cf_units/_udunits2.pyx":225
  *     return wrap_unit(unit.system, cunit)
  * 
  * def offset_by_time(Unit unit, double origin):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_offset_by_time(unit.cunit, origin)
  *     return wrap_unit(unit.system, cunit)
  */
 
@@ -5555,15 +5572,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":230
+/* "cf_units/_udunits2.pyx":229
  *     return wrap_unit(unit.system, cunit)
  * 
  * def multiply(Unit unit1, Unit unit2):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_multiply(unit1.cunit, unit2.cunit)
  *     return wrap_unit(unit1.system, cunit)
  */
 
@@ -5598,39 +5615,39 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_unit1)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_unit2)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("multiply", 1, 2, 2, 1); __PYX_ERR(1, 230, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("multiply", 1, 2, 2, 1); __PYX_ERR(1, 229, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "multiply") < 0)) __PYX_ERR(1, 230, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "multiply") < 0)) __PYX_ERR(1, 229, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_unit1 = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[0]);
     __pyx_v_unit2 = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("multiply", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 230, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("multiply", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 229, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.multiply", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit1), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit1", 0))) __PYX_ERR(1, 230, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit2), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit2", 0))) __PYX_ERR(1, 230, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit1), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit1", 0))) __PYX_ERR(1, 229, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit2), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit2", 0))) __PYX_ERR(1, 229, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_22multiply(__pyx_self, __pyx_v_unit1, __pyx_v_unit2);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5645,41 +5662,41 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("multiply", 0);
 
-  /* "cf_units/_udunits2.pyx":231
+  /* "cf_units/_udunits2.pyx":230
  * 
  * def multiply(Unit unit1, Unit unit2):
  *     cdef ut_unit* cunit = ut_multiply(unit1.cunit, unit2.cunit)             # <<<<<<<<<<<<<<
  *     return wrap_unit(unit1.system, cunit)
  * 
  */
   __pyx_v_cunit = ut_multiply(__pyx_v_unit1->cunit, __pyx_v_unit2->cunit);
 
-  /* "cf_units/_udunits2.pyx":232
+  /* "cf_units/_udunits2.pyx":231
  * def multiply(Unit unit1, Unit unit2):
  *     cdef ut_unit* cunit = ut_multiply(unit1.cunit, unit2.cunit)
  *     return wrap_unit(unit1.system, cunit)             # <<<<<<<<<<<<<<
  * 
  * def invert(Unit unit):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = ((PyObject *)__pyx_v_unit1->system);
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 232, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":230
+  /* "cf_units/_udunits2.pyx":229
  *     return wrap_unit(unit.system, cunit)
  * 
  * def multiply(Unit unit1, Unit unit2):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_multiply(unit1.cunit, unit2.cunit)
  *     return wrap_unit(unit1.system, cunit)
  */
 
@@ -5691,15 +5708,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":234
+/* "cf_units/_udunits2.pyx":233
  *     return wrap_unit(unit1.system, cunit)
  * 
  * def invert(Unit unit):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit =  ut_invert(unit.cunit)
  *     return wrap_unit(unit.system, cunit)
  */
 
@@ -5709,15 +5726,15 @@
 static PyObject *__pyx_pw_8cf_units_9_udunits2_25invert(PyObject *__pyx_self, PyObject *__pyx_v_unit) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("invert (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 234, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 233, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_24invert(__pyx_self, ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)__pyx_v_unit));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5732,41 +5749,41 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("invert", 0);
 
-  /* "cf_units/_udunits2.pyx":235
+  /* "cf_units/_udunits2.pyx":234
  * 
  * def invert(Unit unit):
  *     cdef ut_unit* cunit =  ut_invert(unit.cunit)             # <<<<<<<<<<<<<<
  *     return wrap_unit(unit.system, cunit)
  * 
  */
   __pyx_v_cunit = ut_invert(__pyx_v_unit->cunit);
 
-  /* "cf_units/_udunits2.pyx":236
+  /* "cf_units/_udunits2.pyx":235
  * def invert(Unit unit):
  *     cdef ut_unit* cunit =  ut_invert(unit.cunit)
  *     return wrap_unit(unit.system, cunit)             # <<<<<<<<<<<<<<
  * 
  * def divide(Unit numer, Unit denom):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = ((PyObject *)__pyx_v_unit->system);
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 236, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 235, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":234
+  /* "cf_units/_udunits2.pyx":233
  *     return wrap_unit(unit1.system, cunit)
  * 
  * def invert(Unit unit):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit =  ut_invert(unit.cunit)
  *     return wrap_unit(unit.system, cunit)
  */
 
@@ -5778,15 +5795,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":238
+/* "cf_units/_udunits2.pyx":237
  *     return wrap_unit(unit.system, cunit)
  * 
  * def divide(Unit numer, Unit denom):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_divide(numer.cunit, denom.cunit)
  *     return wrap_unit(numer.system, cunit)
  */
 
@@ -5821,39 +5838,39 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_numer)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_denom)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("divide", 1, 2, 2, 1); __PYX_ERR(1, 238, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("divide", 1, 2, 2, 1); __PYX_ERR(1, 237, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "divide") < 0)) __PYX_ERR(1, 238, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "divide") < 0)) __PYX_ERR(1, 237, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_numer = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[0]);
     __pyx_v_denom = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("divide", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 238, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("divide", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 237, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.divide", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_numer), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "numer", 0))) __PYX_ERR(1, 238, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_denom), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "denom", 0))) __PYX_ERR(1, 238, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_numer), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "numer", 0))) __PYX_ERR(1, 237, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_denom), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "denom", 0))) __PYX_ERR(1, 237, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_26divide(__pyx_self, __pyx_v_numer, __pyx_v_denom);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5868,41 +5885,41 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("divide", 0);
 
-  /* "cf_units/_udunits2.pyx":239
+  /* "cf_units/_udunits2.pyx":238
  * 
  * def divide(Unit numer, Unit denom):
  *     cdef ut_unit* cunit = ut_divide(numer.cunit, denom.cunit)             # <<<<<<<<<<<<<<
  *     return wrap_unit(numer.system, cunit)
  * 
  */
   __pyx_v_cunit = ut_divide(__pyx_v_numer->cunit, __pyx_v_denom->cunit);
 
-  /* "cf_units/_udunits2.pyx":240
+  /* "cf_units/_udunits2.pyx":239
  * def divide(Unit numer, Unit denom):
  *     cdef ut_unit* cunit = ut_divide(numer.cunit, denom.cunit)
  *     return wrap_unit(numer.system, cunit)             # <<<<<<<<<<<<<<
  * 
  * def raise_(Unit unit, int power):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = ((PyObject *)__pyx_v_numer->system);
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 240, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 239, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":238
+  /* "cf_units/_udunits2.pyx":237
  *     return wrap_unit(unit.system, cunit)
  * 
  * def divide(Unit numer, Unit denom):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_divide(numer.cunit, denom.cunit)
  *     return wrap_unit(numer.system, cunit)
  */
 
@@ -5914,15 +5931,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":242
+/* "cf_units/_udunits2.pyx":241
  *     return wrap_unit(numer.system, cunit)
  * 
  * def raise_(Unit unit, int power):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_raise(unit.cunit, power)
  *     return wrap_unit(unit.system, cunit)
  */
 
@@ -5957,38 +5974,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_unit)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_power)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("raise_", 1, 2, 2, 1); __PYX_ERR(1, 242, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("raise_", 1, 2, 2, 1); __PYX_ERR(1, 241, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "raise_") < 0)) __PYX_ERR(1, 242, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "raise_") < 0)) __PYX_ERR(1, 241, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_unit = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[0]);
-    __pyx_v_power = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_power == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 242, __pyx_L3_error)
+    __pyx_v_power = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_power == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 241, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("raise_", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 242, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("raise_", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 241, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.raise_", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 242, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 241, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_28raise_(__pyx_self, __pyx_v_unit, __pyx_v_power);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -6003,41 +6020,41 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("raise_", 0);
 
-  /* "cf_units/_udunits2.pyx":243
+  /* "cf_units/_udunits2.pyx":242
  * 
  * def raise_(Unit unit, int power):
  *     cdef ut_unit* cunit = ut_raise(unit.cunit, power)             # <<<<<<<<<<<<<<
  *     return wrap_unit(unit.system, cunit)
  * 
  */
   __pyx_v_cunit = ut_raise(__pyx_v_unit->cunit, __pyx_v_power);
 
-  /* "cf_units/_udunits2.pyx":244
+  /* "cf_units/_udunits2.pyx":243
  * def raise_(Unit unit, int power):
  *     cdef ut_unit* cunit = ut_raise(unit.cunit, power)
  *     return wrap_unit(unit.system, cunit)             # <<<<<<<<<<<<<<
  * 
  * def root(Unit unit, int root):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = ((PyObject *)__pyx_v_unit->system);
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 244, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":242
+  /* "cf_units/_udunits2.pyx":241
  *     return wrap_unit(numer.system, cunit)
  * 
  * def raise_(Unit unit, int power):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_raise(unit.cunit, power)
  *     return wrap_unit(unit.system, cunit)
  */
 
@@ -6049,15 +6066,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":246
+/* "cf_units/_udunits2.pyx":245
  *     return wrap_unit(unit.system, cunit)
  * 
  * def root(Unit unit, int root):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_root(unit.cunit, root)
  *     return wrap_unit(unit.system, cunit)
  */
 
@@ -6092,38 +6109,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_unit)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_root)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("root", 1, 2, 2, 1); __PYX_ERR(1, 246, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("root", 1, 2, 2, 1); __PYX_ERR(1, 245, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "root") < 0)) __PYX_ERR(1, 246, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "root") < 0)) __PYX_ERR(1, 245, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_unit = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[0]);
-    __pyx_v_root = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_root == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 246, __pyx_L3_error)
+    __pyx_v_root = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_root == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 245, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("root", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 246, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("root", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 245, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.root", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 246, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 245, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_30root(__pyx_self, __pyx_v_unit, __pyx_v_root);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -6138,41 +6155,41 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("root", 0);
 
-  /* "cf_units/_udunits2.pyx":247
+  /* "cf_units/_udunits2.pyx":246
  * 
  * def root(Unit unit, int root):
  *     cdef ut_unit* cunit = ut_root(unit.cunit, root)             # <<<<<<<<<<<<<<
  *     return wrap_unit(unit.system, cunit)
  * 
  */
   __pyx_v_cunit = ut_root(__pyx_v_unit->cunit, __pyx_v_root);
 
-  /* "cf_units/_udunits2.pyx":248
+  /* "cf_units/_udunits2.pyx":247
  * def root(Unit unit, int root):
  *     cdef ut_unit* cunit = ut_root(unit.cunit, root)
  *     return wrap_unit(unit.system, cunit)             # <<<<<<<<<<<<<<
  * 
  * def log(double base, Unit reference):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = ((PyObject *)__pyx_v_unit->system);
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 248, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":246
+  /* "cf_units/_udunits2.pyx":245
  *     return wrap_unit(unit.system, cunit)
  * 
  * def root(Unit unit, int root):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_root(unit.cunit, root)
  *     return wrap_unit(unit.system, cunit)
  */
 
@@ -6184,15 +6201,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":250
+/* "cf_units/_udunits2.pyx":249
  *     return wrap_unit(unit.system, cunit)
  * 
  * def log(double base, Unit reference):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_log(base, reference.cunit)
  *     return wrap_unit(reference.system, cunit)
  */
 
@@ -6227,38 +6244,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_base)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reference)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("log", 1, 2, 2, 1); __PYX_ERR(1, 250, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("log", 1, 2, 2, 1); __PYX_ERR(1, 249, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "log") < 0)) __PYX_ERR(1, 250, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "log") < 0)) __PYX_ERR(1, 249, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_base = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_base == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 250, __pyx_L3_error)
+    __pyx_v_base = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_base == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 249, __pyx_L3_error)
     __pyx_v_reference = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("log", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 250, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("log", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 249, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.log", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_reference), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "reference", 0))) __PYX_ERR(1, 250, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_reference), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "reference", 0))) __PYX_ERR(1, 249, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_32log(__pyx_self, __pyx_v_base, __pyx_v_reference);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -6273,41 +6290,41 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("log", 0);
 
-  /* "cf_units/_udunits2.pyx":251
+  /* "cf_units/_udunits2.pyx":250
  * 
  * def log(double base, Unit reference):
  *     cdef ut_unit* cunit = ut_log(base, reference.cunit)             # <<<<<<<<<<<<<<
  *     return wrap_unit(reference.system, cunit)
  * 
  */
   __pyx_v_cunit = ut_log(__pyx_v_base, __pyx_v_reference->cunit);
 
-  /* "cf_units/_udunits2.pyx":252
+  /* "cf_units/_udunits2.pyx":251
  * def log(double base, Unit reference):
  *     cdef ut_unit* cunit = ut_log(base, reference.cunit)
  *     return wrap_unit(reference.system, cunit)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = ((PyObject *)__pyx_v_reference->system);
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 252, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(((struct __pyx_obj_8cf_units_9_udunits2_System *)__pyx_t_1), __pyx_v_cunit)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":250
+  /* "cf_units/_udunits2.pyx":249
  *     return wrap_unit(unit.system, cunit)
  * 
  * def log(double base, Unit reference):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_log(base, reference.cunit)
  *     return wrap_unit(reference.system, cunit)
  */
 
@@ -6319,15 +6336,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":255
+/* "cf_units/_udunits2.pyx":254
  * 
  * 
  * def parse(System system, char* string, ut_encoding encoding):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_parse(system.csystem, string, encoding)
  *     return wrap_unit(system, cunit)
  */
 
@@ -6365,46 +6382,46 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_system)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_string)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("parse", 1, 3, 3, 1); __PYX_ERR(1, 255, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("parse", 1, 3, 3, 1); __PYX_ERR(1, 254, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_encoding)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("parse", 1, 3, 3, 2); __PYX_ERR(1, 255, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("parse", 1, 3, 3, 2); __PYX_ERR(1, 254, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "parse") < 0)) __PYX_ERR(1, 255, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "parse") < 0)) __PYX_ERR(1, 254, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_system = ((struct __pyx_obj_8cf_units_9_udunits2_System *)values[0]);
-    __pyx_v_string = __Pyx_PyObject_AsWritableString(values[1]); if (unlikely((!__pyx_v_string) && PyErr_Occurred())) __PYX_ERR(1, 255, __pyx_L3_error)
-    __pyx_v_encoding = ((ut_encoding)__Pyx_PyInt_As_ut_encoding(values[2])); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 255, __pyx_L3_error)
+    __pyx_v_string = __Pyx_PyObject_AsWritableString(values[1]); if (unlikely((!__pyx_v_string) && PyErr_Occurred())) __PYX_ERR(1, 254, __pyx_L3_error)
+    __pyx_v_encoding = ((ut_encoding)__Pyx_PyInt_As_ut_encoding(values[2])); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 254, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("parse", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 255, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("parse", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 254, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.parse", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_system), __pyx_ptype_8cf_units_9_udunits2_System, 1, "system", 0))) __PYX_ERR(1, 255, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_system), __pyx_ptype_8cf_units_9_udunits2_System, 1, "system", 0))) __PYX_ERR(1, 254, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_34parse(__pyx_self, __pyx_v_system, __pyx_v_string, __pyx_v_encoding);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -6418,38 +6435,38 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parse", 0);
 
-  /* "cf_units/_udunits2.pyx":256
+  /* "cf_units/_udunits2.pyx":255
  * 
  * def parse(System system, char* string, ut_encoding encoding):
  *     cdef ut_unit* cunit = ut_parse(system.csystem, string, encoding)             # <<<<<<<<<<<<<<
  *     return wrap_unit(system, cunit)
  * 
  */
   __pyx_v_cunit = ut_parse(__pyx_v_system->csystem, __pyx_v_string, __pyx_v_encoding);
 
-  /* "cf_units/_udunits2.pyx":257
+  /* "cf_units/_udunits2.pyx":256
  * def parse(System system, char* string, ut_encoding encoding):
  *     cdef ut_unit* cunit = ut_parse(system.csystem, string, encoding)
  *     return wrap_unit(system, cunit)             # <<<<<<<<<<<<<<
  * 
  * def format(Unit unit, unsigned opts=0):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(__pyx_v_system, __pyx_v_cunit)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 257, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_8cf_units_9_udunits2_wrap_unit(__pyx_v_system, __pyx_v_cunit)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":255
+  /* "cf_units/_udunits2.pyx":254
  * 
  * 
  * def parse(System system, char* string, ut_encoding encoding):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_parse(system.csystem, string, encoding)
  *     return wrap_unit(system, cunit)
  */
 
@@ -6460,15 +6477,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":259
+/* "cf_units/_udunits2.pyx":258
  *     return wrap_unit(system, cunit)
  * 
  * def format(Unit unit, unsigned opts=0):             # <<<<<<<<<<<<<<
  *     cdef bytearray buf = bytearray(_STRING_BUFFER_DEPTH)
  *     n = ut_format(unit.cunit, buf, len(buf), opts)
  */
 
@@ -6507,41 +6524,41 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_opts);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "format") < 0)) __PYX_ERR(1, 259, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "format") < 0)) __PYX_ERR(1, 258, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_unit = ((struct __pyx_obj_8cf_units_9_udunits2_Unit *)values[0]);
     if (values[1]) {
-      __pyx_v_opts = __Pyx_PyInt_As_unsigned_int(values[1]); if (unlikely((__pyx_v_opts == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 259, __pyx_L3_error)
+      __pyx_v_opts = __Pyx_PyInt_As_unsigned_int(values[1]); if (unlikely((__pyx_v_opts == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 258, __pyx_L3_error)
     } else {
       __pyx_v_opts = ((unsigned int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("format", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 259, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("format", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 258, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.format", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 259, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_unit), __pyx_ptype_8cf_units_9_udunits2_Unit, 1, "unit", 0))) __PYX_ERR(1, 258, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_36format(__pyx_self, __pyx_v_unit, __pyx_v_opts);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -6562,172 +6579,172 @@
   PyObject *__pyx_t_6 = NULL;
   Py_ssize_t __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("format", 0);
 
-  /* "cf_units/_udunits2.pyx":260
+  /* "cf_units/_udunits2.pyx":259
  * 
  * def format(Unit unit, unsigned opts=0):
  *     cdef bytearray buf = bytearray(_STRING_BUFFER_DEPTH)             # <<<<<<<<<<<<<<
  *     n = ut_format(unit.cunit, buf, len(buf), opts)
  *     if n >= _STRING_BUFFER_DEPTH:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_8cf_units_9_udunits2__STRING_BUFFER_DEPTH); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 260, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_8cf_units_9_udunits2__STRING_BUFFER_DEPTH); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 260, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_buf = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "cf_units/_udunits2.pyx":261
+  /* "cf_units/_udunits2.pyx":260
  * def format(Unit unit, unsigned opts=0):
  *     cdef bytearray buf = bytearray(_STRING_BUFFER_DEPTH)
  *     n = ut_format(unit.cunit, buf, len(buf), opts)             # <<<<<<<<<<<<<<
  *     if n >= _STRING_BUFFER_DEPTH:
  *         buf = bytearray(n + 1)
  */
-  __pyx_t_3 = __Pyx_PyObject_AsWritableString(__pyx_v_buf); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(1, 261, __pyx_L1_error)
-  __pyx_t_4 = PyByteArray_GET_SIZE(__pyx_v_buf); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 261, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(ut_format(__pyx_v_unit->cunit, __pyx_t_3, __pyx_t_4, __pyx_v_opts)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 261, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_AsWritableString(__pyx_v_buf); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(1, 260, __pyx_L1_error)
+  __pyx_t_4 = PyByteArray_GET_SIZE(__pyx_v_buf); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 260, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(ut_format(__pyx_v_unit->cunit, __pyx_t_3, __pyx_t_4, __pyx_v_opts)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_n = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "cf_units/_udunits2.pyx":262
+  /* "cf_units/_udunits2.pyx":261
  *     cdef bytearray buf = bytearray(_STRING_BUFFER_DEPTH)
  *     n = ut_format(unit.cunit, buf, len(buf), opts)
  *     if n >= _STRING_BUFFER_DEPTH:             # <<<<<<<<<<<<<<
  *         buf = bytearray(n + 1)
  *         n = ut_format(unit.cunit, buf, len(buf), opts)
  */
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_8cf_units_9_udunits2__STRING_BUFFER_DEPTH); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 262, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_8cf_units_9_udunits2__STRING_BUFFER_DEPTH); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 261, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_n, __pyx_t_2, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 262, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_n, __pyx_t_2, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 261, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(1, 262, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(1, 261, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_5) {
 
-    /* "cf_units/_udunits2.pyx":263
+    /* "cf_units/_udunits2.pyx":262
  *     n = ut_format(unit.cunit, buf, len(buf), opts)
  *     if n >= _STRING_BUFFER_DEPTH:
  *         buf = bytearray(n + 1)             # <<<<<<<<<<<<<<
  *         n = ut_format(unit.cunit, buf, len(buf), opts)
  *     if n == -1:
  */
-    __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_n, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 263, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_n, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 262, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 263, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 262, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_buf, ((PyObject*)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "cf_units/_udunits2.pyx":264
+    /* "cf_units/_udunits2.pyx":263
  *     if n >= _STRING_BUFFER_DEPTH:
  *         buf = bytearray(n + 1)
  *         n = ut_format(unit.cunit, buf, len(buf), opts)             # <<<<<<<<<<<<<<
  *     if n == -1:
  *         _raise_error()
  */
-    __pyx_t_3 = __Pyx_PyObject_AsWritableString(__pyx_v_buf); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(1, 264, __pyx_L1_error)
-    __pyx_t_4 = PyByteArray_GET_SIZE(__pyx_v_buf); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 264, __pyx_L1_error)
-    __pyx_t_2 = __Pyx_PyInt_From_int(ut_format(__pyx_v_unit->cunit, __pyx_t_3, __pyx_t_4, __pyx_v_opts)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 264, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_AsWritableString(__pyx_v_buf); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(1, 263, __pyx_L1_error)
+    __pyx_t_4 = PyByteArray_GET_SIZE(__pyx_v_buf); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 263, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(ut_format(__pyx_v_unit->cunit, __pyx_t_3, __pyx_t_4, __pyx_v_opts)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_n, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "cf_units/_udunits2.pyx":262
+    /* "cf_units/_udunits2.pyx":261
  *     cdef bytearray buf = bytearray(_STRING_BUFFER_DEPTH)
  *     n = ut_format(unit.cunit, buf, len(buf), opts)
  *     if n >= _STRING_BUFFER_DEPTH:             # <<<<<<<<<<<<<<
  *         buf = bytearray(n + 1)
  *         n = ut_format(unit.cunit, buf, len(buf), opts)
  */
   }
 
-  /* "cf_units/_udunits2.pyx":265
+  /* "cf_units/_udunits2.pyx":264
  *         buf = bytearray(n + 1)
  *         n = ut_format(unit.cunit, buf, len(buf), opts)
  *     if n == -1:             # <<<<<<<<<<<<<<
  *         _raise_error()
  *     return bytes(buf[:n])
  */
-  __pyx_t_2 = __Pyx_PyInt_EqObjC(__pyx_v_n, __pyx_int_neg_1, -1L, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 265, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_EqObjC(__pyx_v_n, __pyx_int_neg_1, -1L, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 264, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(1, 265, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(1, 264, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_5) {
 
-    /* "cf_units/_udunits2.pyx":266
+    /* "cf_units/_udunits2.pyx":265
  *         n = ut_format(unit.cunit, buf, len(buf), opts)
  *     if n == -1:
  *         _raise_error()             # <<<<<<<<<<<<<<
  *     return bytes(buf[:n])
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_raise_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 266, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_raise_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 265, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 266, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 265, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "cf_units/_udunits2.pyx":265
+    /* "cf_units/_udunits2.pyx":264
  *         buf = bytearray(n + 1)
  *         n = ut_format(unit.cunit, buf, len(buf), opts)
  *     if n == -1:             # <<<<<<<<<<<<<<
  *         _raise_error()
  *     return bytes(buf[:n])
  */
   }
 
-  /* "cf_units/_udunits2.pyx":267
+  /* "cf_units/_udunits2.pyx":266
  *     if n == -1:
  *         _raise_error()
  *     return bytes(buf[:n])             # <<<<<<<<<<<<<<
  * 
  * def encode_date(int year, int month, int day):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_n);
   __pyx_t_2 = __pyx_v_n;
   __pyx_t_5 = (__pyx_t_2 == Py_None);
   if (__pyx_t_5) {
     __pyx_t_4 = PY_SSIZE_T_MAX;
   } else {
-    __pyx_t_7 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_7 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 267, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_7 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 266, __pyx_L1_error)
     __pyx_t_4 = __pyx_t_7;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PySequence_GetSlice(__pyx_v_buf, 0, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 267, __pyx_L1_error)
+  __pyx_t_2 = PySequence_GetSlice(__pyx_v_buf, 0, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 266, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 267, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 266, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":259
+  /* "cf_units/_udunits2.pyx":258
  *     return wrap_unit(system, cunit)
  * 
  * def format(Unit unit, unsigned opts=0):             # <<<<<<<<<<<<<<
  *     cdef bytearray buf = bytearray(_STRING_BUFFER_DEPTH)
  *     n = ut_format(unit.cunit, buf, len(buf), opts)
  */
 
@@ -6742,15 +6759,15 @@
   __Pyx_XDECREF(__pyx_v_buf);
   __Pyx_XDECREF(__pyx_v_n);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":269
+/* "cf_units/_udunits2.pyx":268
  *     return bytes(buf[:n])
  * 
  * def encode_date(int year, int month, int day):             # <<<<<<<<<<<<<<
  *     return ut_encode_date(year, month, day)
  * 
  */
 
@@ -6788,40 +6805,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_year)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_month)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("encode_date", 1, 3, 3, 1); __PYX_ERR(1, 269, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("encode_date", 1, 3, 3, 1); __PYX_ERR(1, 268, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_day)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("encode_date", 1, 3, 3, 2); __PYX_ERR(1, 269, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("encode_date", 1, 3, 3, 2); __PYX_ERR(1, 268, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "encode_date") < 0)) __PYX_ERR(1, 269, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "encode_date") < 0)) __PYX_ERR(1, 268, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_year = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_year == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 269, __pyx_L3_error)
-    __pyx_v_month = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_month == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 269, __pyx_L3_error)
-    __pyx_v_day = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_day == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 269, __pyx_L3_error)
+    __pyx_v_year = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_year == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 268, __pyx_L3_error)
+    __pyx_v_month = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_month == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 268, __pyx_L3_error)
+    __pyx_v_day = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_day == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 268, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("encode_date", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 269, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("encode_date", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 268, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.encode_date", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_38encode_date(__pyx_self, __pyx_v_year, __pyx_v_month, __pyx_v_day);
 
@@ -6835,29 +6852,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode_date", 0);
 
-  /* "cf_units/_udunits2.pyx":270
+  /* "cf_units/_udunits2.pyx":269
  * 
  * def encode_date(int year, int month, int day):
  *     return ut_encode_date(year, month, day)             # <<<<<<<<<<<<<<
  * 
  * def encode_clock(int hours, int minutes, double seconds):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(ut_encode_date(__pyx_v_year, __pyx_v_month, __pyx_v_day)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 270, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(ut_encode_date(__pyx_v_year, __pyx_v_month, __pyx_v_day)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":269
+  /* "cf_units/_udunits2.pyx":268
  *     return bytes(buf[:n])
  * 
  * def encode_date(int year, int month, int day):             # <<<<<<<<<<<<<<
  *     return ut_encode_date(year, month, day)
  * 
  */
 
@@ -6868,15 +6885,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":272
+/* "cf_units/_udunits2.pyx":271
  *     return ut_encode_date(year, month, day)
  * 
  * def encode_clock(int hours, int minutes, double seconds):             # <<<<<<<<<<<<<<
  *     return ut_encode_clock(hours, minutes, seconds)
  * 
  */
 
@@ -6914,40 +6931,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_hours)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_minutes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("encode_clock", 1, 3, 3, 1); __PYX_ERR(1, 272, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("encode_clock", 1, 3, 3, 1); __PYX_ERR(1, 271, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_seconds)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("encode_clock", 1, 3, 3, 2); __PYX_ERR(1, 272, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("encode_clock", 1, 3, 3, 2); __PYX_ERR(1, 271, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "encode_clock") < 0)) __PYX_ERR(1, 272, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "encode_clock") < 0)) __PYX_ERR(1, 271, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_hours = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_hours == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 272, __pyx_L3_error)
-    __pyx_v_minutes = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_minutes == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 272, __pyx_L3_error)
-    __pyx_v_seconds = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_seconds == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 272, __pyx_L3_error)
+    __pyx_v_hours = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_hours == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 271, __pyx_L3_error)
+    __pyx_v_minutes = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_minutes == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 271, __pyx_L3_error)
+    __pyx_v_seconds = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_seconds == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 271, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("encode_clock", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 272, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("encode_clock", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 271, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.encode_clock", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_40encode_clock(__pyx_self, __pyx_v_hours, __pyx_v_minutes, __pyx_v_seconds);
 
@@ -6961,29 +6978,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode_clock", 0);
 
-  /* "cf_units/_udunits2.pyx":273
+  /* "cf_units/_udunits2.pyx":272
  * 
  * def encode_clock(int hours, int minutes, double seconds):
  *     return ut_encode_clock(hours, minutes, seconds)             # <<<<<<<<<<<<<<
  * 
  * def encode_time(int year, int month, int day,
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(ut_encode_clock(__pyx_v_hours, __pyx_v_minutes, __pyx_v_seconds)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 273, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(ut_encode_clock(__pyx_v_hours, __pyx_v_minutes, __pyx_v_seconds)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":272
+  /* "cf_units/_udunits2.pyx":271
  *     return ut_encode_date(year, month, day)
  * 
  * def encode_clock(int hours, int minutes, double seconds):             # <<<<<<<<<<<<<<
  *     return ut_encode_clock(hours, minutes, seconds)
  * 
  */
 
@@ -6994,15 +7011,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":275
+/* "cf_units/_udunits2.pyx":274
  *     return ut_encode_clock(hours, minutes, seconds)
  * 
  * def encode_time(int year, int month, int day,             # <<<<<<<<<<<<<<
  *                 int hour, int minute, double second):
  *     return ut_encode_time(year, month, day, hour, minute, second)
  */
 
@@ -7049,64 +7066,64 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_year)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_month)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("encode_time", 1, 6, 6, 1); __PYX_ERR(1, 275, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("encode_time", 1, 6, 6, 1); __PYX_ERR(1, 274, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_day)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("encode_time", 1, 6, 6, 2); __PYX_ERR(1, 275, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("encode_time", 1, 6, 6, 2); __PYX_ERR(1, 274, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_hour)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("encode_time", 1, 6, 6, 3); __PYX_ERR(1, 275, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("encode_time", 1, 6, 6, 3); __PYX_ERR(1, 274, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_minute)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("encode_time", 1, 6, 6, 4); __PYX_ERR(1, 275, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("encode_time", 1, 6, 6, 4); __PYX_ERR(1, 274, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_second)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("encode_time", 1, 6, 6, 5); __PYX_ERR(1, 275, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("encode_time", 1, 6, 6, 5); __PYX_ERR(1, 274, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "encode_time") < 0)) __PYX_ERR(1, 275, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "encode_time") < 0)) __PYX_ERR(1, 274, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 6) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
     }
-    __pyx_v_year = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_year == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 275, __pyx_L3_error)
-    __pyx_v_month = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_month == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 275, __pyx_L3_error)
-    __pyx_v_day = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_day == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 275, __pyx_L3_error)
-    __pyx_v_hour = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_hour == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 276, __pyx_L3_error)
-    __pyx_v_minute = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_minute == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 276, __pyx_L3_error)
-    __pyx_v_second = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_second == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 276, __pyx_L3_error)
+    __pyx_v_year = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_year == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 274, __pyx_L3_error)
+    __pyx_v_month = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_month == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 274, __pyx_L3_error)
+    __pyx_v_day = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_day == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 274, __pyx_L3_error)
+    __pyx_v_hour = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_hour == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 275, __pyx_L3_error)
+    __pyx_v_minute = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_minute == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 275, __pyx_L3_error)
+    __pyx_v_second = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_second == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 275, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("encode_time", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 275, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("encode_time", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 274, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.encode_time", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_42encode_time(__pyx_self, __pyx_v_year, __pyx_v_month, __pyx_v_day, __pyx_v_hour, __pyx_v_minute, __pyx_v_second);
 
@@ -7120,29 +7137,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode_time", 0);
 
-  /* "cf_units/_udunits2.pyx":277
+  /* "cf_units/_udunits2.pyx":276
  * def encode_time(int year, int month, int day,
  *                 int hour, int minute, double second):
  *     return ut_encode_time(year, month, day, hour, minute, second)             # <<<<<<<<<<<<<<
  * 
  * def decode_time(double value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(ut_encode_time(__pyx_v_year, __pyx_v_month, __pyx_v_day, __pyx_v_hour, __pyx_v_minute, __pyx_v_second)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 277, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(ut_encode_time(__pyx_v_year, __pyx_v_month, __pyx_v_day, __pyx_v_hour, __pyx_v_minute, __pyx_v_second)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":275
+  /* "cf_units/_udunits2.pyx":274
  *     return ut_encode_clock(hours, minutes, seconds)
  * 
  * def encode_time(int year, int month, int day,             # <<<<<<<<<<<<<<
  *                 int hour, int minute, double second):
  *     return ut_encode_time(year, month, day, hour, minute, second)
  */
 
@@ -7153,15 +7170,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":279
+/* "cf_units/_udunits2.pyx":278
  *     return ut_encode_time(year, month, day, hour, minute, second)
  * 
  * def decode_time(double value):             # <<<<<<<<<<<<<<
  *     cdef int year, month, day, hour, minute
  *     cdef double second, resolution
  */
 
@@ -7173,15 +7190,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("decode_time (wrapper)", 0);
   assert(__pyx_arg_value); {
-    __pyx_v_value = __pyx_PyFloat_AsDouble(__pyx_arg_value); if (unlikely((__pyx_v_value == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 279, __pyx_L3_error)
+    __pyx_v_value = __pyx_PyFloat_AsDouble(__pyx_arg_value); if (unlikely((__pyx_v_value == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 278, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.decode_time", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -7211,46 +7228,46 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decode_time", 0);
 
-  /* "cf_units/_udunits2.pyx":282
+  /* "cf_units/_udunits2.pyx":281
  *     cdef int year, month, day, hour, minute
  *     cdef double second, resolution
  *     ut_decode_time(value, &year, &month, &day, &hour, &minute, &second,             # <<<<<<<<<<<<<<
  *                    &resolution)
  *     return (year, month, day, hour, minute, second, resolution)
  */
   ut_decode_time(__pyx_v_value, (&__pyx_v_year), (&__pyx_v_month), (&__pyx_v_day), (&__pyx_v_hour), (&__pyx_v_minute), (&__pyx_v_second), (&__pyx_v_resolution));
 
-  /* "cf_units/_udunits2.pyx":284
+  /* "cf_units/_udunits2.pyx":283
  *     ut_decode_time(value, &year, &month, &day, &hour, &minute, &second,
  *                    &resolution)
  *     return (year, month, day, hour, minute, second, resolution)             # <<<<<<<<<<<<<<
  * 
  * def set_error_message_handler(ErrorMessageHandler handler):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_year); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 284, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_year); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_month); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 284, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_month); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_day); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 284, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_day); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_hour); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 284, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_hour); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_minute); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 284, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_minute); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_second); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 284, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_second); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = PyFloat_FromDouble(__pyx_v_resolution); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 284, __pyx_L1_error)
+  __pyx_t_7 = PyFloat_FromDouble(__pyx_v_resolution); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = PyTuple_New(7); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 284, __pyx_L1_error)
+  __pyx_t_8 = PyTuple_New(7); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_3);
@@ -7269,15 +7286,15 @@
   __pyx_t_5 = 0;
   __pyx_t_6 = 0;
   __pyx_t_7 = 0;
   __pyx_r = __pyx_t_8;
   __pyx_t_8 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":279
+  /* "cf_units/_udunits2.pyx":278
  *     return ut_encode_time(year, month, day, hour, minute, second)
  * 
  * def decode_time(double value):             # <<<<<<<<<<<<<<
  *     cdef int year, month, day, hour, minute
  *     cdef double second, resolution
  */
 
@@ -7295,15 +7312,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":286
+/* "cf_units/_udunits2.pyx":285
  *     return (year, month, day, hour, minute, second, resolution)
  * 
  * def set_error_message_handler(ErrorMessageHandler handler):             # <<<<<<<<<<<<<<
  *     cdef ErrorMessageHandler result = ErrorMessageHandler()
  *     result.chandler = ut_set_error_message_handler(handler.chandler)
  */
 
@@ -7313,15 +7330,15 @@
 static PyObject *__pyx_pw_8cf_units_9_udunits2_47set_error_message_handler(PyObject *__pyx_self, PyObject *__pyx_v_handler) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_error_message_handler (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_handler), __pyx_ptype_8cf_units_9_udunits2_ErrorMessageHandler, 1, "handler", 0))) __PYX_ERR(1, 286, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_handler), __pyx_ptype_8cf_units_9_udunits2_ErrorMessageHandler, 1, "handler", 0))) __PYX_ERR(1, 285, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_46set_error_message_handler(__pyx_self, ((struct __pyx_obj_8cf_units_9_udunits2_ErrorMessageHandler *)__pyx_v_handler));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -7335,48 +7352,48 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_error_message_handler", 0);
 
-  /* "cf_units/_udunits2.pyx":287
+  /* "cf_units/_udunits2.pyx":286
  * 
  * def set_error_message_handler(ErrorMessageHandler handler):
  *     cdef ErrorMessageHandler result = ErrorMessageHandler()             # <<<<<<<<<<<<<<
  *     result.chandler = ut_set_error_message_handler(handler.chandler)
  *     return result
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8cf_units_9_udunits2_ErrorMessageHandler)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8cf_units_9_udunits2_ErrorMessageHandler)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_result = ((struct __pyx_obj_8cf_units_9_udunits2_ErrorMessageHandler *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":288
+  /* "cf_units/_udunits2.pyx":287
  * def set_error_message_handler(ErrorMessageHandler handler):
  *     cdef ErrorMessageHandler result = ErrorMessageHandler()
  *     result.chandler = ut_set_error_message_handler(handler.chandler)             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
   __pyx_v_result->chandler = ut_set_error_message_handler(__pyx_v_handler->chandler);
 
-  /* "cf_units/_udunits2.pyx":289
+  /* "cf_units/_udunits2.pyx":288
  *     cdef ErrorMessageHandler result = ErrorMessageHandler()
  *     result.chandler = ut_set_error_message_handler(handler.chandler)
  *     return result             # <<<<<<<<<<<<<<
  * 
  * def convert_float(Converter converter, float value):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":286
+  /* "cf_units/_udunits2.pyx":285
  *     return (year, month, day, hour, minute, second, resolution)
  * 
  * def set_error_message_handler(ErrorMessageHandler handler):             # <<<<<<<<<<<<<<
  *     cdef ErrorMessageHandler result = ErrorMessageHandler()
  *     result.chandler = ut_set_error_message_handler(handler.chandler)
  */
 
@@ -7388,15 +7405,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":291
+/* "cf_units/_udunits2.pyx":290
  *     return result
  * 
  * def convert_float(Converter converter, float value):             # <<<<<<<<<<<<<<
  *     return cv_convert_float(converter.cconverter, value)
  * 
  */
 
@@ -7431,38 +7448,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_converter)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("convert_float", 1, 2, 2, 1); __PYX_ERR(1, 291, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("convert_float", 1, 2, 2, 1); __PYX_ERR(1, 290, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "convert_float") < 0)) __PYX_ERR(1, 291, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "convert_float") < 0)) __PYX_ERR(1, 290, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_converter = ((struct __pyx_obj_8cf_units_9_udunits2_Converter *)values[0]);
-    __pyx_v_value = __pyx_PyFloat_AsFloat(values[1]); if (unlikely((__pyx_v_value == (float)-1) && PyErr_Occurred())) __PYX_ERR(1, 291, __pyx_L3_error)
+    __pyx_v_value = __pyx_PyFloat_AsFloat(values[1]); if (unlikely((__pyx_v_value == (float)-1) && PyErr_Occurred())) __PYX_ERR(1, 290, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("convert_float", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 291, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("convert_float", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 290, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.convert_float", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_converter), __pyx_ptype_8cf_units_9_udunits2_Converter, 1, "converter", 0))) __PYX_ERR(1, 291, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_converter), __pyx_ptype_8cf_units_9_udunits2_Converter, 1, "converter", 0))) __PYX_ERR(1, 290, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_48convert_float(__pyx_self, __pyx_v_converter, __pyx_v_value);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -7475,29 +7492,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert_float", 0);
 
-  /* "cf_units/_udunits2.pyx":292
+  /* "cf_units/_udunits2.pyx":291
  * 
  * def convert_float(Converter converter, float value):
  *     return cv_convert_float(converter.cconverter, value)             # <<<<<<<<<<<<<<
  * 
  * def convert_floats(Converter converter, np.ndarray[np.float32_t] in_, np.ndarray[np.float32_t] out):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(cv_convert_float(__pyx_v_converter->cconverter, __pyx_v_value)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(cv_convert_float(__pyx_v_converter->cconverter, __pyx_v_value)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 291, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":291
+  /* "cf_units/_udunits2.pyx":290
  *     return result
  * 
  * def convert_float(Converter converter, float value):             # <<<<<<<<<<<<<<
  *     return cv_convert_float(converter.cconverter, value)
  * 
  */
 
@@ -7508,15 +7525,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":294
+/* "cf_units/_udunits2.pyx":293
  *     return cv_convert_float(converter.cconverter, value)
  * 
  * def convert_floats(Converter converter, np.ndarray[np.float32_t] in_, np.ndarray[np.float32_t] out):             # <<<<<<<<<<<<<<
  *     cv_convert_floats(converter.cconverter, <float*> in_.data, in_.size, <float*> out.data)
  *     return out
  */
 
@@ -7554,48 +7571,48 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_converter)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_in)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("convert_floats", 1, 3, 3, 1); __PYX_ERR(1, 294, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("convert_floats", 1, 3, 3, 1); __PYX_ERR(1, 293, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_out)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("convert_floats", 1, 3, 3, 2); __PYX_ERR(1, 294, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("convert_floats", 1, 3, 3, 2); __PYX_ERR(1, 293, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "convert_floats") < 0)) __PYX_ERR(1, 294, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "convert_floats") < 0)) __PYX_ERR(1, 293, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_converter = ((struct __pyx_obj_8cf_units_9_udunits2_Converter *)values[0]);
     __pyx_v_in_ = ((PyArrayObject *)values[1]);
     __pyx_v_out = ((PyArrayObject *)values[2]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("convert_floats", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 294, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("convert_floats", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 293, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.convert_floats", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_converter), __pyx_ptype_8cf_units_9_udunits2_Converter, 1, "converter", 0))) __PYX_ERR(1, 294, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_in_), __pyx_ptype_5numpy_ndarray, 1, "in_", 0))) __PYX_ERR(1, 294, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_out), __pyx_ptype_5numpy_ndarray, 1, "out", 0))) __PYX_ERR(1, 294, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_converter), __pyx_ptype_8cf_units_9_udunits2_Converter, 1, "converter", 0))) __PYX_ERR(1, 293, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_in_), __pyx_ptype_5numpy_ndarray, 1, "in_", 0))) __PYX_ERR(1, 293, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_out), __pyx_ptype_5numpy_ndarray, 1, "out", 0))) __PYX_ERR(1, 293, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_50convert_floats(__pyx_self, __pyx_v_converter, __pyx_v_in_, __pyx_v_out);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -7622,49 +7639,49 @@
   __pyx_pybuffernd_in_.rcbuffer = &__pyx_pybuffer_in_;
   __pyx_pybuffer_out.pybuffer.buf = NULL;
   __pyx_pybuffer_out.refcount = 0;
   __pyx_pybuffernd_out.data = NULL;
   __pyx_pybuffernd_out.rcbuffer = &__pyx_pybuffer_out;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_in_.rcbuffer->pybuffer, (PyObject*)__pyx_v_in_, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(1, 294, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_in_.rcbuffer->pybuffer, (PyObject*)__pyx_v_in_, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(1, 293, __pyx_L1_error)
   }
   __pyx_pybuffernd_in_.diminfo[0].strides = __pyx_pybuffernd_in_.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_in_.diminfo[0].shape = __pyx_pybuffernd_in_.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_out.rcbuffer->pybuffer, (PyObject*)__pyx_v_out, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(1, 294, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_out.rcbuffer->pybuffer, (PyObject*)__pyx_v_out, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(1, 293, __pyx_L1_error)
   }
   __pyx_pybuffernd_out.diminfo[0].strides = __pyx_pybuffernd_out.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_out.diminfo[0].shape = __pyx_pybuffernd_out.rcbuffer->pybuffer.shape[0];
 
-  /* "cf_units/_udunits2.pyx":295
+  /* "cf_units/_udunits2.pyx":294
  * 
  * def convert_floats(Converter converter, np.ndarray[np.float32_t] in_, np.ndarray[np.float32_t] out):
  *     cv_convert_floats(converter.cconverter, <float*> in_.data, in_.size, <float*> out.data)             # <<<<<<<<<<<<<<
  *     return out
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_in_), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 295, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_in_), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 294, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_size_t(__pyx_t_1); if (unlikely((__pyx_t_2 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 295, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_size_t(__pyx_t_1); if (unlikely((__pyx_t_2 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 294, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   (void)(cv_convert_floats(__pyx_v_converter->cconverter, ((float *)__pyx_v_in_->data), __pyx_t_2, ((float *)__pyx_v_out->data)));
 
-  /* "cf_units/_udunits2.pyx":296
+  /* "cf_units/_udunits2.pyx":295
  * def convert_floats(Converter converter, np.ndarray[np.float32_t] in_, np.ndarray[np.float32_t] out):
  *     cv_convert_floats(converter.cconverter, <float*> in_.data, in_.size, <float*> out.data)
  *     return out             # <<<<<<<<<<<<<<
  * 
  * def convert_double(Converter converter, double value):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_out));
   __pyx_r = ((PyObject *)__pyx_v_out);
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":294
+  /* "cf_units/_udunits2.pyx":293
  *     return cv_convert_float(converter.cconverter, value)
  * 
  * def convert_floats(Converter converter, np.ndarray[np.float32_t] in_, np.ndarray[np.float32_t] out):             # <<<<<<<<<<<<<<
  *     cv_convert_floats(converter.cconverter, <float*> in_.data, in_.size, <float*> out.data)
  *     return out
  */
 
@@ -7686,15 +7703,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_out.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":298
+/* "cf_units/_udunits2.pyx":297
  *     return out
  * 
  * def convert_double(Converter converter, double value):             # <<<<<<<<<<<<<<
  *     return cv_convert_double(converter.cconverter, value)
  * 
  */
 
@@ -7729,38 +7746,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_converter)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("convert_double", 1, 2, 2, 1); __PYX_ERR(1, 298, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("convert_double", 1, 2, 2, 1); __PYX_ERR(1, 297, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "convert_double") < 0)) __PYX_ERR(1, 298, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "convert_double") < 0)) __PYX_ERR(1, 297, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_converter = ((struct __pyx_obj_8cf_units_9_udunits2_Converter *)values[0]);
-    __pyx_v_value = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_value == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 298, __pyx_L3_error)
+    __pyx_v_value = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_value == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 297, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("convert_double", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 298, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("convert_double", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 297, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.convert_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_converter), __pyx_ptype_8cf_units_9_udunits2_Converter, 1, "converter", 0))) __PYX_ERR(1, 298, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_converter), __pyx_ptype_8cf_units_9_udunits2_Converter, 1, "converter", 0))) __PYX_ERR(1, 297, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_52convert_double(__pyx_self, __pyx_v_converter, __pyx_v_value);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -7773,29 +7790,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert_double", 0);
 
-  /* "cf_units/_udunits2.pyx":299
+  /* "cf_units/_udunits2.pyx":298
  * 
  * def convert_double(Converter converter, double value):
  *     return cv_convert_double(converter.cconverter, value)             # <<<<<<<<<<<<<<
  * 
  * def convert_doubles(Converter converter, np.ndarray[np.float64_t] in_, np.ndarray[np.float64_t] out):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(cv_convert_double(__pyx_v_converter->cconverter, __pyx_v_value)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 299, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(cv_convert_double(__pyx_v_converter->cconverter, __pyx_v_value)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":298
+  /* "cf_units/_udunits2.pyx":297
  *     return out
  * 
  * def convert_double(Converter converter, double value):             # <<<<<<<<<<<<<<
  *     return cv_convert_double(converter.cconverter, value)
  * 
  */
 
@@ -7806,15 +7823,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cf_units/_udunits2.pyx":301
+/* "cf_units/_udunits2.pyx":300
  *     return cv_convert_double(converter.cconverter, value)
  * 
  * def convert_doubles(Converter converter, np.ndarray[np.float64_t] in_, np.ndarray[np.float64_t] out):             # <<<<<<<<<<<<<<
  *     cv_convert_doubles(converter.cconverter, <double*> in_.data, in_.size, <double*> out.data)
  *     return out
  */
 
@@ -7852,48 +7869,48 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_converter)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_in)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("convert_doubles", 1, 3, 3, 1); __PYX_ERR(1, 301, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("convert_doubles", 1, 3, 3, 1); __PYX_ERR(1, 300, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_out)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("convert_doubles", 1, 3, 3, 2); __PYX_ERR(1, 301, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("convert_doubles", 1, 3, 3, 2); __PYX_ERR(1, 300, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "convert_doubles") < 0)) __PYX_ERR(1, 301, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "convert_doubles") < 0)) __PYX_ERR(1, 300, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_converter = ((struct __pyx_obj_8cf_units_9_udunits2_Converter *)values[0]);
     __pyx_v_in_ = ((PyArrayObject *)values[1]);
     __pyx_v_out = ((PyArrayObject *)values[2]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("convert_doubles", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 301, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("convert_doubles", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 300, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cf_units._udunits2.convert_doubles", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_converter), __pyx_ptype_8cf_units_9_udunits2_Converter, 1, "converter", 0))) __PYX_ERR(1, 301, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_in_), __pyx_ptype_5numpy_ndarray, 1, "in_", 0))) __PYX_ERR(1, 301, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_out), __pyx_ptype_5numpy_ndarray, 1, "out", 0))) __PYX_ERR(1, 301, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_converter), __pyx_ptype_8cf_units_9_udunits2_Converter, 1, "converter", 0))) __PYX_ERR(1, 300, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_in_), __pyx_ptype_5numpy_ndarray, 1, "in_", 0))) __PYX_ERR(1, 300, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_out), __pyx_ptype_5numpy_ndarray, 1, "out", 0))) __PYX_ERR(1, 300, __pyx_L1_error)
   __pyx_r = __pyx_pf_8cf_units_9_udunits2_54convert_doubles(__pyx_self, __pyx_v_converter, __pyx_v_in_, __pyx_v_out);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -7920,46 +7937,46 @@
   __pyx_pybuffernd_in_.rcbuffer = &__pyx_pybuffer_in_;
   __pyx_pybuffer_out.pybuffer.buf = NULL;
   __pyx_pybuffer_out.refcount = 0;
   __pyx_pybuffernd_out.data = NULL;
   __pyx_pybuffernd_out.rcbuffer = &__pyx_pybuffer_out;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_in_.rcbuffer->pybuffer, (PyObject*)__pyx_v_in_, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(1, 301, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_in_.rcbuffer->pybuffer, (PyObject*)__pyx_v_in_, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(1, 300, __pyx_L1_error)
   }
   __pyx_pybuffernd_in_.diminfo[0].strides = __pyx_pybuffernd_in_.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_in_.diminfo[0].shape = __pyx_pybuffernd_in_.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_out.rcbuffer->pybuffer, (PyObject*)__pyx_v_out, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(1, 301, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_out.rcbuffer->pybuffer, (PyObject*)__pyx_v_out, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(1, 300, __pyx_L1_error)
   }
   __pyx_pybuffernd_out.diminfo[0].strides = __pyx_pybuffernd_out.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_out.diminfo[0].shape = __pyx_pybuffernd_out.rcbuffer->pybuffer.shape[0];
 
-  /* "cf_units/_udunits2.pyx":302
+  /* "cf_units/_udunits2.pyx":301
  * 
  * def convert_doubles(Converter converter, np.ndarray[np.float64_t] in_, np.ndarray[np.float64_t] out):
  *     cv_convert_doubles(converter.cconverter, <double*> in_.data, in_.size, <double*> out.data)             # <<<<<<<<<<<<<<
  *     return out
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_in_), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 302, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_in_), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 301, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_size_t(__pyx_t_1); if (unlikely((__pyx_t_2 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 302, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_size_t(__pyx_t_1); if (unlikely((__pyx_t_2 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 301, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   (void)(cv_convert_doubles(__pyx_v_converter->cconverter, ((double *)__pyx_v_in_->data), __pyx_t_2, ((double *)__pyx_v_out->data)));
 
-  /* "cf_units/_udunits2.pyx":303
+  /* "cf_units/_udunits2.pyx":302
  * def convert_doubles(Converter converter, np.ndarray[np.float64_t] in_, np.ndarray[np.float64_t] out):
  *     cv_convert_doubles(converter.cconverter, <double*> in_.data, in_.size, <double*> out.data)
  *     return out             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_out));
   __pyx_r = ((PyObject *)__pyx_v_out);
   goto __pyx_L0;
 
-  /* "cf_units/_udunits2.pyx":301
+  /* "cf_units/_udunits2.pyx":300
  *     return cv_convert_double(converter.cconverter, value)
  * 
  * def convert_doubles(Converter converter, np.ndarray[np.float64_t] in_, np.ndarray[np.float64_t] out):             # <<<<<<<<<<<<<<
  *     cv_convert_doubles(converter.cconverter, <double*> in_.data, in_.size, <double*> out.data)
  *     return out
  */
 
@@ -7981,874 +7998,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_out.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
- *         # experimental exception made for __getbuffer__ and __releasebuffer__
- *         # -- the details of this may change.
- *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
- *             # This implementation of getbuffer is geared towards Cython
- *             # requirements, and does not yet fulfill the PEP.
- */
-
-/* Python wrapper */
-static CYTHON_UNUSED int __pyx_pw_5numpy_7ndarray_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
-static CYTHON_UNUSED int __pyx_pw_5numpy_7ndarray_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__getbuffer__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5numpy_7ndarray___getbuffer__(((PyArrayObject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info), ((int)__pyx_v_flags));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_5numpy_7ndarray___getbuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  int __pyx_v_i;
-  int __pyx_v_ndim;
-  int __pyx_v_endian_detector;
-  int __pyx_v_little_endian;
-  int __pyx_v_t;
-  char *__pyx_v_f;
-  PyArray_Descr *__pyx_v_descr = 0;
-  int __pyx_v_offset;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  PyArray_Descr *__pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  char *__pyx_t_9;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  if (__pyx_v_info == NULL) {
-    PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
-    return -1;
-  }
-  __Pyx_RefNannySetupContext("__getbuffer__", 0);
-  __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
-  __Pyx_GIVEREF(__pyx_v_info->obj);
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":265
- * 
- *             cdef int i, ndim
- *             cdef int endian_detector = 1             # <<<<<<<<<<<<<<
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- * 
- */
-  __pyx_v_endian_detector = 1;
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":266
- *             cdef int i, ndim
- *             cdef int endian_detector = 1
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
- * 
- *             ndim = PyArray_NDIM(self)
- */
-  __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":268
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- * 
- *             ndim = PyArray_NDIM(self)             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- */
-  __pyx_v_ndim = PyArray_NDIM(__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  __pyx_t_2 = (((__pyx_v_flags & PyBUF_C_CONTIGUOUS) == PyBUF_C_CONTIGUOUS) != 0);
-  if (__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L4_bool_binop_done;
-  }
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":271
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):             # <<<<<<<<<<<<<<
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- */
-  __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_C_CONTIGUOUS) != 0)) != 0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L4_bool_binop_done:;
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  if (unlikely(__pyx_t_1)) {
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 272, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 272, __pyx_L1_error)
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  }
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  __pyx_t_2 = (((__pyx_v_flags & PyBUF_F_CONTIGUOUS) == PyBUF_F_CONTIGUOUS) != 0);
-  if (__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L7_bool_binop_done;
-  }
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":275
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):             # <<<<<<<<<<<<<<
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- * 
- */
-  __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_F_CONTIGUOUS) != 0)) != 0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L7_bool_binop_done:;
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  if (unlikely(__pyx_t_1)) {
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
- * 
- *             info.buf = PyArray_DATA(self)
- */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 276, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 276, __pyx_L1_error)
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  }
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":278
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- * 
- *             info.buf = PyArray_DATA(self)             # <<<<<<<<<<<<<<
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  __pyx_v_info->buf = PyArray_DATA(__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":279
- * 
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim             # <<<<<<<<<<<<<<
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 # Allocate new buffer for strides and shape info.
- */
-  __pyx_v_info->ndim = __pyx_v_ndim;
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- */
-  __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":283
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)             # <<<<<<<<<<<<<<
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):
- */
-    __pyx_v_info->strides = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * 2) * ((size_t)__pyx_v_ndim))));
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":284
- *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
- *                 info.shape = info.strides + ndim             # <<<<<<<<<<<<<<
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- */
-    __pyx_v_info->shape = (__pyx_v_info->strides + __pyx_v_ndim);
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":285
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):             # <<<<<<<<<<<<<<
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- */
-    __pyx_t_4 = __pyx_v_ndim;
-    __pyx_t_5 = __pyx_t_4;
-    for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
-      __pyx_v_i = __pyx_t_6;
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":286
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]             # <<<<<<<<<<<<<<
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- *             else:
- */
-      (__pyx_v_info->strides[__pyx_v_i]) = (PyArray_STRIDES(__pyx_v_self)[__pyx_v_i]);
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":287
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- *                     info.shape[i] = PyArray_DIMS(self)[i]             # <<<<<<<<<<<<<<
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- */
-      (__pyx_v_info->shape[__pyx_v_i]) = (PyArray_DIMS(__pyx_v_self)[__pyx_v_i]);
-    }
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":280
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- */
-    goto __pyx_L9;
-  }
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":289
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL
- */
-  /*else*/ {
-    __pyx_v_info->strides = ((Py_ssize_t *)PyArray_STRIDES(__pyx_v_self));
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":290
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)             # <<<<<<<<<<<<<<
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)
- */
-    __pyx_v_info->shape = ((Py_ssize_t *)PyArray_DIMS(__pyx_v_self));
-  }
-  __pyx_L9:;
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":291
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
- *             info.itemsize = PyArray_ITEMSIZE(self)
- *             info.readonly = not PyArray_ISWRITEABLE(self)
- */
-  __pyx_v_info->suboffsets = NULL;
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":292
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)             # <<<<<<<<<<<<<<
- *             info.readonly = not PyArray_ISWRITEABLE(self)
- * 
- */
-  __pyx_v_info->itemsize = PyArray_ITEMSIZE(__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":293
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)
- *             info.readonly = not PyArray_ISWRITEABLE(self)             # <<<<<<<<<<<<<<
- * 
- *             cdef int t
- */
-  __pyx_v_info->readonly = (!(PyArray_ISWRITEABLE(__pyx_v_self) != 0));
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":296
- * 
- *             cdef int t
- *             cdef char* f = NULL             # <<<<<<<<<<<<<<
- *             cdef dtype descr = <dtype>PyArray_DESCR(self)
- *             cdef int offset
- */
-  __pyx_v_f = NULL;
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":297
- *             cdef int t
- *             cdef char* f = NULL
- *             cdef dtype descr = <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
- *             cdef int offset
- * 
- */
-  __pyx_t_7 = PyArray_DESCR(__pyx_v_self);
-  __pyx_t_3 = ((PyObject *)__pyx_t_7);
-  __Pyx_INCREF(__pyx_t_3);
-  __pyx_v_descr = ((PyArray_Descr *)__pyx_t_3);
-  __pyx_t_3 = 0;
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":300
- *             cdef int offset
- * 
- *             info.obj = self             # <<<<<<<<<<<<<<
- * 
- *             if not PyDataType_HASFIELDS(descr):
- */
-  __Pyx_INCREF(((PyObject *)__pyx_v_self));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
-  __Pyx_GOTREF(__pyx_v_info->obj);
-  __Pyx_DECREF(__pyx_v_info->obj);
-  __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
- *             info.obj = self
- * 
- *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- */
-  __pyx_t_1 = ((!(PyDataType_HASFIELDS(__pyx_v_descr) != 0)) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":303
- * 
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num             # <<<<<<<<<<<<<<
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- */
-    __pyx_t_4 = __pyx_v_descr->type_num;
-    __pyx_v_t = __pyx_t_4;
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    __pyx_t_2 = ((__pyx_v_descr->byteorder == '>') != 0);
-    if (!__pyx_t_2) {
-      goto __pyx_L15_next_or;
-    } else {
-    }
-    __pyx_t_2 = (__pyx_v_little_endian != 0);
-    if (!__pyx_t_2) {
-    } else {
-      __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L14_bool_binop_done;
-    }
-    __pyx_L15_next_or:;
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":305
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"
- */
-    __pyx_t_2 = ((__pyx_v_descr->byteorder == '<') != 0);
-    if (__pyx_t_2) {
-    } else {
-      __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L14_bool_binop_done;
-    }
-    __pyx_t_2 = ((!(__pyx_v_little_endian != 0)) != 0);
-    __pyx_t_1 = __pyx_t_2;
-    __pyx_L14_bool_binop_done:;
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    if (unlikely(__pyx_t_1)) {
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 306, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(2, 306, __pyx_L1_error)
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    }
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":307
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"
- */
-    switch (__pyx_v_t) {
-      case NPY_BYTE:
-      __pyx_v_f = ((char *)"b");
-      break;
-      case NPY_UBYTE:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":308
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"
- */
-      __pyx_v_f = ((char *)"B");
-      break;
-      case NPY_SHORT:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":309
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"
- */
-      __pyx_v_f = ((char *)"h");
-      break;
-      case NPY_USHORT:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":310
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"
- */
-      __pyx_v_f = ((char *)"H");
-      break;
-      case NPY_INT:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":311
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"
- */
-      __pyx_v_f = ((char *)"i");
-      break;
-      case NPY_UINT:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":312
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"
- */
-      __pyx_v_f = ((char *)"I");
-      break;
-      case NPY_LONG:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":313
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"
- */
-      __pyx_v_f = ((char *)"l");
-      break;
-      case NPY_ULONG:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":314
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- */
-      __pyx_v_f = ((char *)"L");
-      break;
-      case NPY_LONGLONG:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":315
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"
- */
-      __pyx_v_f = ((char *)"q");
-      break;
-      case NPY_ULONGLONG:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":316
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"
- */
-      __pyx_v_f = ((char *)"Q");
-      break;
-      case NPY_FLOAT:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":317
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- */
-      __pyx_v_f = ((char *)"f");
-      break;
-      case NPY_DOUBLE:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":318
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- */
-      __pyx_v_f = ((char *)"d");
-      break;
-      case NPY_LONGDOUBLE:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":319
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- */
-      __pyx_v_f = ((char *)"g");
-      break;
-      case NPY_CFLOAT:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":320
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- */
-      __pyx_v_f = ((char *)"Zf");
-      break;
-      case NPY_CDOUBLE:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":321
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- *                 elif t == NPY_OBJECT:      f = "O"
- */
-      __pyx_v_f = ((char *)"Zd");
-      break;
-      case NPY_CLONGDOUBLE:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":322
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_OBJECT:      f = "O"
- *                 else:
- */
-      __pyx_v_f = ((char *)"Zg");
-      break;
-      case NPY_OBJECT:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":323
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- *                 elif t == NPY_OBJECT:      f = "O"             # <<<<<<<<<<<<<<
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- */
-      __pyx_v_f = ((char *)"O");
-      break;
-      default:
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":325
- *                 elif t == NPY_OBJECT:      f = "O"
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
- *                 info.format = f
- *                 return
- */
-      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = PyUnicode_Format(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(2, 325, __pyx_L1_error)
-      break;
-    }
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":326
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *                 info.format = f             # <<<<<<<<<<<<<<
- *                 return
- *             else:
- */
-    __pyx_v_info->format = __pyx_v_f;
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":327
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *                 info.format = f
- *                 return             # <<<<<<<<<<<<<<
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- */
-    __pyx_r = 0;
-    goto __pyx_L0;
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":302
- *             info.obj = self
- * 
- *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- */
-  }
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":329
- *                 return
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)             # <<<<<<<<<<<<<<
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0
- */
-  /*else*/ {
-    __pyx_v_info->format = ((char *)PyObject_Malloc(0xFF));
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":330
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- *                 info.format[0] = c'^' # Native data types, manual alignment             # <<<<<<<<<<<<<<
- *                 offset = 0
- *                 f = _util_dtypestring(descr, info.format + 1,
- */
-    (__pyx_v_info->format[0]) = '^';
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":331
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0             # <<<<<<<<<<<<<<
- *                 f = _util_dtypestring(descr, info.format + 1,
- *                                       info.format + _buffer_format_string_len,
- */
-    __pyx_v_offset = 0;
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":332
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0
- *                 f = _util_dtypestring(descr, info.format + 1,             # <<<<<<<<<<<<<<
- *                                       info.format + _buffer_format_string_len,
- *                                       &offset)
- */
-    __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_descr, (__pyx_v_info->format + 1), (__pyx_v_info->format + 0xFF), (&__pyx_v_offset)); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(2, 332, __pyx_L1_error)
-    __pyx_v_f = __pyx_t_9;
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":335
- *                                       info.format + _buffer_format_string_len,
- *                                       &offset)
- *                 f[0] = c'\0' # Terminate format string             # <<<<<<<<<<<<<<
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- */
-    (__pyx_v_f[0]) = '\x00';
-  }
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":258
- *         # experimental exception made for __getbuffer__ and __releasebuffer__
- *         # -- the details of this may change.
- *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
- *             # This implementation of getbuffer is geared towards Cython
- *             # requirements, and does not yet fulfill the PEP.
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.ndarray.__getbuffer__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  if (__pyx_v_info->obj != NULL) {
-    __Pyx_GOTREF(__pyx_v_info->obj);
-    __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
-  }
-  goto __pyx_L2;
-  __pyx_L0:;
-  if (__pyx_v_info->obj == Py_None) {
-    __Pyx_GOTREF(__pyx_v_info->obj);
-    __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
-  }
-  __pyx_L2:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_descr);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
- *                 f[0] = c'\0' # Terminate format string
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- */
-
-/* Python wrapper */
-static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info); /*proto*/
-static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__releasebuffer__ (wrapper)", 0);
-  __pyx_pf_5numpy_7ndarray_2__releasebuffer__(((PyArrayObject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("__releasebuffer__", 0);
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  __pyx_t_1 = (PyArray_HASFIELDS(__pyx_v_self) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":339
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)             # <<<<<<<<<<<<<<
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 PyObject_Free(info.strides)
- */
-    PyObject_Free(__pyx_v_info->format);
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":338
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  }
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.strides)
- *                 # info.shape was stored after info.strides in the same block
- */
-  __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":341
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 PyObject_Free(info.strides)             # <<<<<<<<<<<<<<
- *                 # info.shape was stored after info.strides in the same block
- * 
- */
-    PyObject_Free(__pyx_v_info->strides);
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":340
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.strides)
- *                 # info.shape was stored after info.strides in the same block
- */
-  }
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":337
- *                 f[0] = c'\0' # Terminate format string
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- */
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -8857,29 +8015,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":821
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":820
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -8890,15 +8048,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -8907,29 +8065,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":824
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 824, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":823
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -8940,15 +8098,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -8957,29 +8115,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":827
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":826
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -8990,15 +8148,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -9007,29 +8165,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":830
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 830, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":829
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -9040,15 +8198,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -9057,29 +8215,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":833
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 833, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":832
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -9090,966 +8248,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":837
+    /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":836
+    /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":839
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:
+ * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":835
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
- *         return ()
- * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
- *     # Recursive utility function used in __getbuffer__ to get format
- *     # string. The new location in the format string is returned.
- */
-
-static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *__pyx_v_descr, char *__pyx_v_f, char *__pyx_v_end, int *__pyx_v_offset) {
-  PyArray_Descr *__pyx_v_child = 0;
-  int __pyx_v_endian_detector;
-  int __pyx_v_little_endian;
-  PyObject *__pyx_v_fields = 0;
-  PyObject *__pyx_v_childname = NULL;
-  PyObject *__pyx_v_new_offset = NULL;
-  PyObject *__pyx_v_t = NULL;
-  char *__pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  int __pyx_t_7;
-  long __pyx_t_8;
-  char *__pyx_t_9;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_util_dtypestring", 0);
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":846
- * 
- *     cdef dtype child
- *     cdef int endian_detector = 1             # <<<<<<<<<<<<<<
- *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- *     cdef tuple fields
- */
-  __pyx_v_endian_detector = 1;
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":847
- *     cdef dtype child
- *     cdef int endian_detector = 1
- *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
- *     cdef tuple fields
- * 
- */
-  __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
- *     cdef tuple fields
- * 
- *     for childname in descr.names:             # <<<<<<<<<<<<<<
- *         fields = descr.fields[childname]
- *         child, new_offset = fields
- */
-  if (unlikely(__pyx_v_descr->names == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(2, 850, __pyx_L1_error)
-  }
-  __pyx_t_1 = __pyx_v_descr->names; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
-  for (;;) {
-    if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
-    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(2, 850, __pyx_L1_error)
-    #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 850, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    #endif
-    __Pyx_XDECREF_SET(__pyx_v_childname, __pyx_t_3);
-    __pyx_t_3 = 0;
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":851
- * 
- *     for childname in descr.names:
- *         fields = descr.fields[childname]             # <<<<<<<<<<<<<<
- *         child, new_offset = fields
- * 
- */
-    if (unlikely(__pyx_v_descr->fields == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(2, 851, __pyx_L1_error)
-    }
-    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_descr->fields, __pyx_v_childname); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 851, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(PyTuple_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(2, 851, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_fields, ((PyObject*)__pyx_t_3));
-    __pyx_t_3 = 0;
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":852
- *     for childname in descr.names:
- *         fields = descr.fields[childname]
- *         child, new_offset = fields             # <<<<<<<<<<<<<<
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- */
-    if (likely(__pyx_v_fields != Py_None)) {
-      PyObject* sequence = __pyx_v_fields;
-      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-      if (unlikely(size != 2)) {
-        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(2, 852, __pyx_L1_error)
-      }
-      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
-      __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
-      #else
-      __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 852, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 852, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      #endif
-    } else {
-      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(2, 852, __pyx_L1_error)
-    }
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_dtype))))) __PYX_ERR(2, 852, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_child, ((PyArray_Descr *)__pyx_t_3));
-    __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_new_offset, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
- *         child, new_offset = fields
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- */
-    __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 854, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PyNumber_Subtract(__pyx_v_new_offset, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 854, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 854, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_6 = ((((__pyx_v_end - __pyx_v_f) - ((int)__pyx_t_5)) < 15) != 0);
-    if (unlikely(__pyx_t_6)) {
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 855, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(2, 855, __pyx_L1_error)
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":854
- *         child, new_offset = fields
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- */
-    }
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    __pyx_t_7 = ((__pyx_v_child->byteorder == '>') != 0);
-    if (!__pyx_t_7) {
-      goto __pyx_L8_next_or;
-    } else {
-    }
-    __pyx_t_7 = (__pyx_v_little_endian != 0);
-    if (!__pyx_t_7) {
-    } else {
-      __pyx_t_6 = __pyx_t_7;
-      goto __pyx_L7_bool_binop_done;
-    }
-    __pyx_L8_next_or:;
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":858
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- *             (child.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
- *             raise ValueError(u"Non-native byte order not supported")
- *             # One could encode it in the format string and have Cython
- */
-    __pyx_t_7 = ((__pyx_v_child->byteorder == '<') != 0);
-    if (__pyx_t_7) {
-    } else {
-      __pyx_t_6 = __pyx_t_7;
-      goto __pyx_L7_bool_binop_done;
-    }
-    __pyx_t_7 = ((!(__pyx_v_little_endian != 0)) != 0);
-    __pyx_t_6 = __pyx_t_7;
-    __pyx_L7_bool_binop_done:;
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    if (unlikely(__pyx_t_6)) {
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":859
- *         if ((child.byteorder == c'>' and little_endian) or
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *             # One could encode it in the format string and have Cython
- *             # complain instead, BUT: < and > in format strings also imply
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 859, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(2, 859, __pyx_L1_error)
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":857
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    }
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":869
- * 
- *         # Output padding bytes
- *         while offset[0] < new_offset:             # <<<<<<<<<<<<<<
- *             f[0] = 120 # "x"; pad byte
- *             f += 1
- */
-    while (1) {
-      __pyx_t_3 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 869, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_new_offset, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 869, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 869, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (!__pyx_t_6) break;
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":870
- *         # Output padding bytes
- *         while offset[0] < new_offset:
- *             f[0] = 120 # "x"; pad byte             # <<<<<<<<<<<<<<
- *             f += 1
- *             offset[0] += 1
- */
-      (__pyx_v_f[0]) = 0x78;
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":871
- *         while offset[0] < new_offset:
- *             f[0] = 120 # "x"; pad byte
- *             f += 1             # <<<<<<<<<<<<<<
- *             offset[0] += 1
- * 
- */
-      __pyx_v_f = (__pyx_v_f + 1);
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":872
- *             f[0] = 120 # "x"; pad byte
- *             f += 1
- *             offset[0] += 1             # <<<<<<<<<<<<<<
- * 
- *         offset[0] += child.itemsize
- */
-      __pyx_t_8 = 0;
-      (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + 1);
-    }
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":874
- *             offset[0] += 1
- * 
- *         offset[0] += child.itemsize             # <<<<<<<<<<<<<<
- * 
- *         if not PyDataType_HASFIELDS(child):
- */
-    __pyx_t_8 = 0;
-    (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + __pyx_v_child->elsize);
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
- *         offset[0] += child.itemsize
- * 
- *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
- *             t = child.type_num
- *             if end - f < 5:
- */
-    __pyx_t_6 = ((!(PyDataType_HASFIELDS(__pyx_v_child) != 0)) != 0);
-    if (__pyx_t_6) {
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":877
- * 
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num             # <<<<<<<<<<<<<<
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")
- */
-      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_child->type_num); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 877, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_4);
-      __pyx_t_4 = 0;
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num
- *             if end - f < 5:             # <<<<<<<<<<<<<<
- *                 raise RuntimeError(u"Format string allocated too short.")
- * 
- */
-      __pyx_t_6 = (((__pyx_v_end - __pyx_v_f) < 5) != 0);
-      if (unlikely(__pyx_t_6)) {
-
-        /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
- *             t = child.type_num
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- */
-        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 879, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(2, 879, __pyx_L1_error)
-
-        /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":878
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num
- *             if end - f < 5:             # <<<<<<<<<<<<<<
- *                 raise RuntimeError(u"Format string allocated too short.")
- * 
- */
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":882
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"             # <<<<<<<<<<<<<<
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_BYTE); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 882, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 882, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 882, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 98;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":883
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"             # <<<<<<<<<<<<<<
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UBYTE); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 883, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 883, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 883, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 66;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":884
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"             # <<<<<<<<<<<<<<
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_SHORT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 884, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 884, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 884, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x68;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":885
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"             # <<<<<<<<<<<<<<
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_USHORT); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 885, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 885, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 885, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 72;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":886
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"             # <<<<<<<<<<<<<<
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_INT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 886, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 886, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 886, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x69;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":887
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UINT); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 887, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 887, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 887, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 73;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":888
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"             # <<<<<<<<<<<<<<
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 888, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 888, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 888, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x6C;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":889
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 889, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 889, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 889, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 76;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":890
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"             # <<<<<<<<<<<<<<
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGLONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 890, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 890, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 890, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x71;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":891
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"             # <<<<<<<<<<<<<<
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONGLONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 891, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 891, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 891, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 81;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":892
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"             # <<<<<<<<<<<<<<
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_FLOAT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 892, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 892, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 892, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x66;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":893
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_DOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 893, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 893, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 893, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x64;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":894
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"             # <<<<<<<<<<<<<<
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 894, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 894, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 894, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x67;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":895
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf             # <<<<<<<<<<<<<<
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CFLOAT); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 895, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 895, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 895, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x66;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":896
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd             # <<<<<<<<<<<<<<
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 896, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 896, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 896, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x64;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":897
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg             # <<<<<<<<<<<<<<
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- *             else:
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CLONGDOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 897, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 897, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 897, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x67;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":898
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"             # <<<<<<<<<<<<<<
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_OBJECT); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 898, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 898, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(2, 898, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (likely(__pyx_t_6)) {
-        (__pyx_v_f[0]) = 79;
-        goto __pyx_L15;
-      }
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":900
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
- *             f += 1
- *         else:
- */
-      /*else*/ {
-        __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 900, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 900, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(2, 900, __pyx_L1_error)
-      }
-      __pyx_L15:;
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":901
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *             f += 1             # <<<<<<<<<<<<<<
- *         else:
- *             # Cython ignores struct boundary information ("T{...}"),
- */
-      __pyx_v_f = (__pyx_v_f + 1);
-
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":876
- *         offset[0] += child.itemsize
- * 
- *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
- *             t = child.type_num
- *             if end - f < 5:
- */
-      goto __pyx_L13;
-    }
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":905
- *             # Cython ignores struct boundary information ("T{...}"),
- *             # so don't output it
- *             f = _util_dtypestring(child, f, end, offset)             # <<<<<<<<<<<<<<
- *     return f
- * 
- */
-    /*else*/ {
-      __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_child, __pyx_v_f, __pyx_v_end, __pyx_v_offset); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(2, 905, __pyx_L1_error)
-      __pyx_v_f = __pyx_t_9;
-    }
-    __pyx_L13:;
-
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":850
- *     cdef tuple fields
- * 
- *     for childname in descr.names:             # <<<<<<<<<<<<<<
- *         fields = descr.fields[childname]
- *         child, new_offset = fields
- */
-  }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":906
- *             # so don't output it
- *             f = _util_dtypestring(child, f, end, offset)
- *     return f             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_f;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":841
- *         return ()
- * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
- *     # Recursive utility function used in __getbuffer__ to get format
- *     # string. The new location in the format string is returned.
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("numpy._util_dtypestring", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_child);
-  __Pyx_XDECREF(__pyx_v_fields);
-  __Pyx_XDECREF(__pyx_v_childname);
-  __Pyx_XDECREF(__pyx_v_new_offset);
-  __Pyx_XDECREF(__pyx_v_t);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1022
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1023
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1026
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1028
+    /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+    /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1029
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1025
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -10060,105 +8469,105 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+      /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
- *         _import_array()             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1035, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+      /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1036
+    /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1036, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
- *         _import_array()
+      /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":945
+ *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1037, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 1037, __pyx_L5_except_error)
+      __PYX_ERR(2, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+    /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1033
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_5);
@@ -10168,15 +8577,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10192,15 +8601,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -10208,84 +8617,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+      /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1041, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+      /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1042
+    /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1042, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+      /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1043, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 1043, __pyx_L5_except_error)
+      __PYX_ERR(2, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+    /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1039
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10300,15 +8709,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10324,15 +8733,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -10340,81 +8749,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+      /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1047, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+      /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1048
+    /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
+ * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1048, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1049
+      /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1049, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 1049, __pyx_L5_except_error)
+      __PYX_ERR(2, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+    /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10429,14 +8841,188 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":979
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":994
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
 static PyObject *__pyx_tp_new_8cf_units_9_udunits2_System(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
@@ -10933,20 +9519,16 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_Converter, __pyx_k_Converter, sizeof(__pyx_k_Converter), 0, 0, 1, 1},
   {&__pyx_n_s_ErrorMessageHandler, __pyx_k_ErrorMessageHandler, sizeof(__pyx_k_ErrorMessageHandler), 0, 0, 1, 1},
-  {&__pyx_kp_u_Format_string_allocated_too_shor, __pyx_k_Format_string_allocated_too_shor, sizeof(__pyx_k_Format_string_allocated_too_shor), 0, 1, 0, 0},
-  {&__pyx_kp_u_Format_string_allocated_too_shor_2, __pyx_k_Format_string_allocated_too_shor_2, sizeof(__pyx_k_Format_string_allocated_too_shor_2), 0, 1, 0, 0},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
   {&__pyx_n_s_NULL_UNIT, __pyx_k_NULL_UNIT, sizeof(__pyx_k_NULL_UNIT), 0, 0, 1, 1},
-  {&__pyx_kp_u_Non_native_byte_order_not_suppor, __pyx_k_Non_native_byte_order_not_suppor, sizeof(__pyx_k_Non_native_byte_order_not_suppor), 0, 1, 0, 0},
-  {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
   {&__pyx_n_s_System, __pyx_k_System, sizeof(__pyx_k_System), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_UDUNITS_2_call_resulted_in_an_e, __pyx_k_UDUNITS_2_call_resulted_in_an_e, sizeof(__pyx_k_UDUNITS_2_call_resulted_in_an_e), 0, 0, 1, 0},
   {&__pyx_n_s_UNKNOWN, __pyx_k_UNKNOWN, sizeof(__pyx_k_UNKNOWN), 0, 0, 1, 1},
   {&__pyx_n_s_UT_ASCII, __pyx_k_UT_ASCII, sizeof(__pyx_k_UT_ASCII), 0, 0, 1, 1},
   {&__pyx_n_s_UT_BAD_ARG, __pyx_k_UT_BAD_ARG, sizeof(__pyx_k_UT_BAD_ARG), 0, 0, 1, 1},
   {&__pyx_n_s_UT_CANT_FORMAT, __pyx_k_UT_CANT_FORMAT, sizeof(__pyx_k_UT_CANT_FORMAT), 0, 0, 1, 1},
@@ -10971,15 +9553,14 @@
   {&__pyx_n_s_UT_VISIT_ERROR, __pyx_k_UT_VISIT_ERROR, sizeof(__pyx_k_UT_VISIT_ERROR), 0, 0, 1, 1},
   {&__pyx_n_s_UdunitsError, __pyx_k_UdunitsError, sizeof(__pyx_k_UdunitsError), 0, 0, 1, 1},
   {&__pyx_n_s_UdunitsError___init, __pyx_k_UdunitsError___init, sizeof(__pyx_k_UdunitsError___init), 0, 0, 1, 1},
   {&__pyx_n_s_UdunitsError___str, __pyx_k_UdunitsError___str, sizeof(__pyx_k_UdunitsError___str), 0, 0, 1, 1},
   {&__pyx_n_s_UdunitsError_error_msg, __pyx_k_UdunitsError_error_msg, sizeof(__pyx_k_UdunitsError_error_msg), 0, 0, 1, 1},
   {&__pyx_n_s_UdunitsError_status_msg, __pyx_k_UdunitsError_status_msg, sizeof(__pyx_k_UdunitsError_status_msg), 0, 0, 1, 1},
   {&__pyx_n_s_Unit, __pyx_k_Unit, sizeof(__pyx_k_Unit), 0, 0, 1, 1},
-  {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_kp_s__10, __pyx_k__10, sizeof(__pyx_k__10), 0, 0, 1, 0},
   {&__pyx_kp_s__11, __pyx_k__11, sizeof(__pyx_k__11), 0, 0, 1, 0},
   {&__pyx_kp_s__9, __pyx_k__9, sizeof(__pyx_k__9), 0, 0, 1, 0},
   {&__pyx_n_s_are_convertible, __pyx_k_are_convertible, sizeof(__pyx_k_are_convertible), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_buf, __pyx_k_buf, sizeof(__pyx_k_buf), 0, 0, 1, 1},
   {&__pyx_n_s_cconverter, __pyx_k_cconverter, sizeof(__pyx_k_cconverter), 0, 0, 1, 1},
@@ -11028,16 +9609,14 @@
   {&__pyx_n_s_minutes, __pyx_k_minutes, sizeof(__pyx_k_minutes), 0, 0, 1, 1},
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_month, __pyx_k_month, sizeof(__pyx_k_month), 0, 0, 1, 1},
   {&__pyx_n_s_multiply, __pyx_k_multiply, sizeof(__pyx_k_multiply), 0, 0, 1, 1},
   {&__pyx_n_s_n, __pyx_k_n, sizeof(__pyx_k_n), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
-  {&__pyx_kp_u_ndarray_is_not_C_contiguous, __pyx_k_ndarray_is_not_C_contiguous, sizeof(__pyx_k_ndarray_is_not_C_contiguous), 0, 1, 0, 0},
-  {&__pyx_kp_u_ndarray_is_not_Fortran_contiguou, __pyx_k_ndarray_is_not_Fortran_contiguou, sizeof(__pyx_k_ndarray_is_not_Fortran_contiguou), 0, 1, 0, 0},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numer, __pyx_k_numer, sizeof(__pyx_k_numer), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_s_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 0, 1, 0},
   {&__pyx_kp_s_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 0, 1, 0},
   {&__pyx_n_s_offset, __pyx_k_offset, sizeof(__pyx_k_offset), 0, 0, 1, 1},
@@ -11048,15 +9627,14 @@
   {&__pyx_n_s_parse, __pyx_k_parse, sizeof(__pyx_k_parse), 0, 0, 1, 1},
   {&__pyx_n_s_path, __pyx_k_path, sizeof(__pyx_k_path), 0, 0, 1, 1},
   {&__pyx_n_s_power, __pyx_k_power, sizeof(__pyx_k_power), 0, 0, 1, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
   {&__pyx_n_s_raise, __pyx_k_raise, sizeof(__pyx_k_raise), 0, 0, 1, 1},
   {&__pyx_n_s_raise_error, __pyx_k_raise_error, sizeof(__pyx_k_raise_error), 0, 0, 1, 1},
-  {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_read_xml, __pyx_k_read_xml, sizeof(__pyx_k_read_xml), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_reference, __pyx_k_reference, sizeof(__pyx_k_reference), 0, 0, 1, 1},
   {&__pyx_n_s_resolution, __pyx_k_resolution, sizeof(__pyx_k_resolution), 0, 0, 1, 1},
   {&__pyx_n_s_result, __pyx_k_result, sizeof(__pyx_k_result), 0, 0, 1, 1},
@@ -11076,25 +9654,21 @@
   {&__pyx_n_s_string, __pyx_k_string, sizeof(__pyx_k_string), 0, 0, 1, 1},
   {&__pyx_n_s_system, __pyx_k_system, sizeof(__pyx_k_system), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_to, __pyx_k_to, sizeof(__pyx_k_to), 0, 0, 1, 1},
   {&__pyx_n_s_unit, __pyx_k_unit, sizeof(__pyx_k_unit), 0, 0, 1, 1},
   {&__pyx_n_s_unit1, __pyx_k_unit1, sizeof(__pyx_k_unit1), 0, 0, 1, 1},
   {&__pyx_n_s_unit2, __pyx_k_unit2, sizeof(__pyx_k_unit2), 0, 0, 1, 1},
-  {&__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_k_unknown_dtype_code_in_numpy_pxd, sizeof(__pyx_k_unknown_dtype_code_in_numpy_pxd), 0, 1, 0, 0},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
   {&__pyx_n_s_year, __pyx_k_year, sizeof(__pyx_k_year), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 2, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 272, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(2, 285, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(2, 855, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 1037, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 945, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -11172,483 +9746,428 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":272
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_C_contiguous); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 272, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":276
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
- * 
- *             info.buf = PyArray_DATA(self)
- */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_Fortran_contiguou); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 276, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":306
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 306, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":855
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 855, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":879
- *             t = child.type_num
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor_2); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 879, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1037
- *         _import_array()
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":945
+ *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 1037, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 945, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 1043, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 951, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "cf_units/_udunits2.pyx":148
+  /* "cf_units/_udunits2.pyx":147
  * 
  *     """
  *     def __init__(self, ut_status status, int errnum):             # <<<<<<<<<<<<<<
  *         self.status = status
  *         self.errnum = errnum
  */
-  __pyx_tuple__19 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_status, __pyx_n_s_errnum); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 148, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_init, 148, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(1, 148, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_status, __pyx_n_s_errnum); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 147, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_init, 147, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 147, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":152
+  /* "cf_units/_udunits2.pyx":151
  *         self.errnum = errnum
  * 
  *     def status_msg(self):             # <<<<<<<<<<<<<<
  *         """
  *         String representation of the UDUNITS-2 ut_status value which resulted
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 152, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_status_msg, 152, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(1, 152, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 151, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_status_msg, 151, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(1, 151, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":163
+  /* "cf_units/_udunits2.pyx":162
  *             return 'UNKNOWN'
  * 
  *     def error_msg(self):             # <<<<<<<<<<<<<<
  *         """
  *         The message string associated with the errno value which resulted from
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 163, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_error_msg, 163, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(1, 163, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 162, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_error_msg, 162, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(1, 162, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":171
+  /* "cf_units/_udunits2.pyx":170
  *         return string.strerror(self.errnum) if self.errnum else ''
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         str_err = ': {}'.format(string.strerror(self.errnum)) \
  *                   if self.errnum else ''
  */
-  __pyx_tuple__25 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_str_err); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 171, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
-  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_str, 171, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(1, 171, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_str_err); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 170, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_str, 170, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(1, 170, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":177
+  /* "cf_units/_udunits2.pyx":176
  * 
  * 
  * def _raise_error():             # <<<<<<<<<<<<<<
  *     """
  *     Raise a UdunitsError with the current value of errno and ut_status
  */
-  __pyx_tuple__27 = PyTuple_Pack(2, __pyx_n_s_errnum, __pyx_n_s_status); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 177, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
-  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_raise_error, 177, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(1, 177, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(2, __pyx_n_s_errnum, __pyx_n_s_status); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 176, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_raise_error, 176, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(1, 176, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":193
+  /* "cf_units/_udunits2.pyx":192
  * # See the UDUNITS-2 documentation for details.
  * 
  * def read_xml(char* path=NULL):             # <<<<<<<<<<<<<<
  *     cdef ut_system* csystem = ut_read_xml(path)
  *     return wrap_system(csystem)
  */
-  __pyx_tuple__29 = PyTuple_Pack(2, __pyx_n_s_path, __pyx_n_s_csystem); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_read_xml, 193, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(1, 193, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(2, __pyx_n_s_path, __pyx_n_s_csystem); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 192, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_read_xml, 192, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(1, 192, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":197
+  /* "cf_units/_udunits2.pyx":196
  *     return wrap_system(csystem)
  * 
  * def get_unit_by_name(System system, char* name):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_get_unit_by_name(system.csystem, name)
  *     return wrap_unit(system, cunit)
  */
-  __pyx_tuple__31 = PyTuple_Pack(3, __pyx_n_s_system, __pyx_n_s_name, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 197, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_get_unit_by_name, 197, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(1, 197, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(3, __pyx_n_s_system, __pyx_n_s_name, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_get_unit_by_name, 196, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(1, 196, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":201
+  /* "cf_units/_udunits2.pyx":200
  *     return wrap_unit(system, cunit)
  * 
  * def clone(Unit unit):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_clone(unit.cunit)
  *     return wrap_unit(unit.system, cunit)
  */
-  __pyx_tuple__33 = PyTuple_Pack(2, __pyx_n_s_unit, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 201, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_clone, 201, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(1, 201, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(2, __pyx_n_s_unit, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_clone, 200, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(1, 200, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":205
+  /* "cf_units/_udunits2.pyx":204
  *     return wrap_unit(unit.system, cunit)
  * 
  * def is_dimensionless(Unit unit):             # <<<<<<<<<<<<<<
  *     return <bint>ut_is_dimensionless(unit.cunit)
  * 
  */
-  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_n_s_unit); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(1, 205, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__35);
-  __Pyx_GIVEREF(__pyx_tuple__35);
-  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_is_dimensionless, 205, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(1, 205, __pyx_L1_error)
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_n_s_unit); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 204, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_is_dimensionless, 204, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(1, 204, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":208
+  /* "cf_units/_udunits2.pyx":207
  *     return <bint>ut_is_dimensionless(unit.cunit)
  * 
  * def compare(Unit unit1, Unit unit2):             # <<<<<<<<<<<<<<
  *     return ut_compare(unit1.cunit, unit2.cunit)
  * 
  */
-  __pyx_tuple__37 = PyTuple_Pack(2, __pyx_n_s_unit1, __pyx_n_s_unit2); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(1, 208, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__37);
-  __Pyx_GIVEREF(__pyx_tuple__37);
-  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_compare, 208, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(1, 208, __pyx_L1_error)
+  __pyx_tuple__32 = PyTuple_Pack(2, __pyx_n_s_unit1, __pyx_n_s_unit2); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(1, 207, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_compare, 207, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(1, 207, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":211
+  /* "cf_units/_udunits2.pyx":210
  *     return ut_compare(unit1.cunit, unit2.cunit)
  * 
  * def are_convertible(Unit unit1, Unit unit2):             # <<<<<<<<<<<<<<
  *     return <bint>ut_are_convertible(unit1.cunit, unit2.cunit)
  * 
  */
-  __pyx_tuple__39 = PyTuple_Pack(2, __pyx_n_s_unit1, __pyx_n_s_unit2); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(1, 211, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__39);
-  __Pyx_GIVEREF(__pyx_tuple__39);
-  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_are_convertible, 211, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(1, 211, __pyx_L1_error)
+  __pyx_tuple__34 = PyTuple_Pack(2, __pyx_n_s_unit1, __pyx_n_s_unit2); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(1, 210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_are_convertible, 210, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(1, 210, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":214
+  /* "cf_units/_udunits2.pyx":213
  *     return <bint>ut_are_convertible(unit1.cunit, unit2.cunit)
  * 
  * def get_converter(Unit fr, Unit to):             # <<<<<<<<<<<<<<
  *     cdef cv_converter* cconverter = ut_get_converter(fr.cunit, to.cunit)
  *     return wrap_converter(cconverter)
  */
-  __pyx_tuple__41 = PyTuple_Pack(3, __pyx_n_s_fr, __pyx_n_s_to, __pyx_n_s_cconverter); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(1, 214, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__41);
-  __Pyx_GIVEREF(__pyx_tuple__41);
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_get_converter, 214, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(1, 214, __pyx_L1_error)
+  __pyx_tuple__36 = PyTuple_Pack(3, __pyx_n_s_fr, __pyx_n_s_to, __pyx_n_s_cconverter); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(1, 213, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__36);
+  __Pyx_GIVEREF(__pyx_tuple__36);
+  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_get_converter, 213, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(1, 213, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":218
+  /* "cf_units/_udunits2.pyx":217
  *     return wrap_converter(cconverter)
  * 
  * def scale(double factor, Unit unit):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_scale(factor, unit.cunit)
  *     return wrap_unit(unit.system, cunit)
  */
-  __pyx_tuple__43 = PyTuple_Pack(3, __pyx_n_s_factor, __pyx_n_s_unit, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(1, 218, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__43);
-  __Pyx_GIVEREF(__pyx_tuple__43);
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_scale, 218, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(1, 218, __pyx_L1_error)
+  __pyx_tuple__38 = PyTuple_Pack(3, __pyx_n_s_factor, __pyx_n_s_unit, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(1, 217, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__38);
+  __Pyx_GIVEREF(__pyx_tuple__38);
+  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_scale, 217, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(1, 217, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":222
+  /* "cf_units/_udunits2.pyx":221
  *     return wrap_unit(unit.system, cunit)
  * 
  * def offset(Unit unit, double offset):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_offset(unit.cunit, offset)
  *     return wrap_unit(unit.system, cunit)
  */
-  __pyx_tuple__45 = PyTuple_Pack(3, __pyx_n_s_unit, __pyx_n_s_offset, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(1, 222, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__45);
-  __Pyx_GIVEREF(__pyx_tuple__45);
-  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_offset, 222, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_tuple__40 = PyTuple_Pack(3, __pyx_n_s_unit, __pyx_n_s_offset, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(1, 221, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__40);
+  __Pyx_GIVEREF(__pyx_tuple__40);
+  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_offset, 221, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(1, 221, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":226
+  /* "cf_units/_udunits2.pyx":225
  *     return wrap_unit(unit.system, cunit)
  * 
  * def offset_by_time(Unit unit, double origin):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_offset_by_time(unit.cunit, origin)
  *     return wrap_unit(unit.system, cunit)
  */
-  __pyx_tuple__47 = PyTuple_Pack(3, __pyx_n_s_unit, __pyx_n_s_origin, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(1, 226, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__47);
-  __Pyx_GIVEREF(__pyx_tuple__47);
-  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_offset_by_time, 226, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_tuple__42 = PyTuple_Pack(3, __pyx_n_s_unit, __pyx_n_s_origin, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(1, 225, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__42);
+  __Pyx_GIVEREF(__pyx_tuple__42);
+  __pyx_codeobj__43 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__42, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_offset_by_time, 225, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__43)) __PYX_ERR(1, 225, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":230
+  /* "cf_units/_udunits2.pyx":229
  *     return wrap_unit(unit.system, cunit)
  * 
  * def multiply(Unit unit1, Unit unit2):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_multiply(unit1.cunit, unit2.cunit)
  *     return wrap_unit(unit1.system, cunit)
  */
-  __pyx_tuple__49 = PyTuple_Pack(3, __pyx_n_s_unit1, __pyx_n_s_unit2, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(1, 230, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__49);
-  __Pyx_GIVEREF(__pyx_tuple__49);
-  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_multiply, 230, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(1, 230, __pyx_L1_error)
+  __pyx_tuple__44 = PyTuple_Pack(3, __pyx_n_s_unit1, __pyx_n_s_unit2, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(1, 229, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__44);
+  __Pyx_GIVEREF(__pyx_tuple__44);
+  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__44, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_multiply, 229, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(1, 229, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":234
+  /* "cf_units/_udunits2.pyx":233
  *     return wrap_unit(unit1.system, cunit)
  * 
  * def invert(Unit unit):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit =  ut_invert(unit.cunit)
  *     return wrap_unit(unit.system, cunit)
  */
-  __pyx_tuple__51 = PyTuple_Pack(2, __pyx_n_s_unit, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(1, 234, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__51);
-  __Pyx_GIVEREF(__pyx_tuple__51);
-  __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_invert, 234, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(1, 234, __pyx_L1_error)
+  __pyx_tuple__46 = PyTuple_Pack(2, __pyx_n_s_unit, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(1, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__46);
+  __Pyx_GIVEREF(__pyx_tuple__46);
+  __pyx_codeobj__47 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__46, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_invert, 233, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__47)) __PYX_ERR(1, 233, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":238
+  /* "cf_units/_udunits2.pyx":237
  *     return wrap_unit(unit.system, cunit)
  * 
  * def divide(Unit numer, Unit denom):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_divide(numer.cunit, denom.cunit)
  *     return wrap_unit(numer.system, cunit)
  */
-  __pyx_tuple__53 = PyTuple_Pack(3, __pyx_n_s_numer, __pyx_n_s_denom, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(1, 238, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__53);
-  __Pyx_GIVEREF(__pyx_tuple__53);
-  __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_divide, 238, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_tuple__48 = PyTuple_Pack(3, __pyx_n_s_numer, __pyx_n_s_denom, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(1, 237, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__48);
+  __Pyx_GIVEREF(__pyx_tuple__48);
+  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_divide, 237, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(1, 237, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":242
+  /* "cf_units/_udunits2.pyx":241
  *     return wrap_unit(numer.system, cunit)
  * 
  * def raise_(Unit unit, int power):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_raise(unit.cunit, power)
  *     return wrap_unit(unit.system, cunit)
  */
-  __pyx_tuple__55 = PyTuple_Pack(3, __pyx_n_s_unit, __pyx_n_s_power, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(1, 242, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__55);
-  __Pyx_GIVEREF(__pyx_tuple__55);
-  __pyx_codeobj__56 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__55, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_raise, 242, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__56)) __PYX_ERR(1, 242, __pyx_L1_error)
+  __pyx_tuple__50 = PyTuple_Pack(3, __pyx_n_s_unit, __pyx_n_s_power, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(1, 241, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__50);
+  __Pyx_GIVEREF(__pyx_tuple__50);
+  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_raise, 241, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(1, 241, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":246
+  /* "cf_units/_udunits2.pyx":245
  *     return wrap_unit(unit.system, cunit)
  * 
  * def root(Unit unit, int root):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_root(unit.cunit, root)
  *     return wrap_unit(unit.system, cunit)
  */
-  __pyx_tuple__57 = PyTuple_Pack(3, __pyx_n_s_unit, __pyx_n_s_root, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(1, 246, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__57);
-  __Pyx_GIVEREF(__pyx_tuple__57);
-  __pyx_codeobj__58 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__57, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_root, 246, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__58)) __PYX_ERR(1, 246, __pyx_L1_error)
+  __pyx_tuple__52 = PyTuple_Pack(3, __pyx_n_s_unit, __pyx_n_s_root, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(1, 245, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__52);
+  __Pyx_GIVEREF(__pyx_tuple__52);
+  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_root, 245, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(1, 245, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":250
+  /* "cf_units/_udunits2.pyx":249
  *     return wrap_unit(unit.system, cunit)
  * 
  * def log(double base, Unit reference):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_log(base, reference.cunit)
  *     return wrap_unit(reference.system, cunit)
  */
-  __pyx_tuple__59 = PyTuple_Pack(3, __pyx_n_s_base, __pyx_n_s_reference, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(1, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__59);
-  __Pyx_GIVEREF(__pyx_tuple__59);
-  __pyx_codeobj__60 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__59, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_log, 250, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__60)) __PYX_ERR(1, 250, __pyx_L1_error)
+  __pyx_tuple__54 = PyTuple_Pack(3, __pyx_n_s_base, __pyx_n_s_reference, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(1, 249, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__54);
+  __Pyx_GIVEREF(__pyx_tuple__54);
+  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__54, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_log, 249, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(1, 249, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":255
+  /* "cf_units/_udunits2.pyx":254
  * 
  * 
  * def parse(System system, char* string, ut_encoding encoding):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_parse(system.csystem, string, encoding)
  *     return wrap_unit(system, cunit)
  */
-  __pyx_tuple__61 = PyTuple_Pack(4, __pyx_n_s_system, __pyx_n_s_string, __pyx_n_s_encoding, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(1, 255, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__61);
-  __Pyx_GIVEREF(__pyx_tuple__61);
-  __pyx_codeobj__62 = (PyObject*)__Pyx_PyCode_New(3, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__61, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_parse, 255, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__62)) __PYX_ERR(1, 255, __pyx_L1_error)
+  __pyx_tuple__56 = PyTuple_Pack(4, __pyx_n_s_system, __pyx_n_s_string, __pyx_n_s_encoding, __pyx_n_s_cunit); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(1, 254, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__56);
+  __Pyx_GIVEREF(__pyx_tuple__56);
+  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(3, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_parse, 254, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(1, 254, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":259
+  /* "cf_units/_udunits2.pyx":258
  *     return wrap_unit(system, cunit)
  * 
  * def format(Unit unit, unsigned opts=0):             # <<<<<<<<<<<<<<
  *     cdef bytearray buf = bytearray(_STRING_BUFFER_DEPTH)
  *     n = ut_format(unit.cunit, buf, len(buf), opts)
  */
-  __pyx_tuple__63 = PyTuple_Pack(4, __pyx_n_s_unit, __pyx_n_s_opts, __pyx_n_s_buf, __pyx_n_s_n); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(1, 259, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__63);
-  __Pyx_GIVEREF(__pyx_tuple__63);
-  __pyx_codeobj__64 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__63, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_format, 259, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__64)) __PYX_ERR(1, 259, __pyx_L1_error)
+  __pyx_tuple__58 = PyTuple_Pack(4, __pyx_n_s_unit, __pyx_n_s_opts, __pyx_n_s_buf, __pyx_n_s_n); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(1, 258, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__58);
+  __Pyx_GIVEREF(__pyx_tuple__58);
+  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_format, 258, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(1, 258, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":269
+  /* "cf_units/_udunits2.pyx":268
  *     return bytes(buf[:n])
  * 
  * def encode_date(int year, int month, int day):             # <<<<<<<<<<<<<<
  *     return ut_encode_date(year, month, day)
  * 
  */
-  __pyx_tuple__65 = PyTuple_Pack(3, __pyx_n_s_year, __pyx_n_s_month, __pyx_n_s_day); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(1, 269, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__65);
-  __Pyx_GIVEREF(__pyx_tuple__65);
-  __pyx_codeobj__66 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__65, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_encode_date, 269, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__66)) __PYX_ERR(1, 269, __pyx_L1_error)
+  __pyx_tuple__60 = PyTuple_Pack(3, __pyx_n_s_year, __pyx_n_s_month, __pyx_n_s_day); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(1, 268, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__60);
+  __Pyx_GIVEREF(__pyx_tuple__60);
+  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_encode_date, 268, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(1, 268, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":272
+  /* "cf_units/_udunits2.pyx":271
  *     return ut_encode_date(year, month, day)
  * 
  * def encode_clock(int hours, int minutes, double seconds):             # <<<<<<<<<<<<<<
  *     return ut_encode_clock(hours, minutes, seconds)
  * 
  */
-  __pyx_tuple__67 = PyTuple_Pack(3, __pyx_n_s_hours, __pyx_n_s_minutes, __pyx_n_s_seconds); if (unlikely(!__pyx_tuple__67)) __PYX_ERR(1, 272, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__67);
-  __Pyx_GIVEREF(__pyx_tuple__67);
-  __pyx_codeobj__68 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_encode_clock, 272, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__68)) __PYX_ERR(1, 272, __pyx_L1_error)
+  __pyx_tuple__62 = PyTuple_Pack(3, __pyx_n_s_hours, __pyx_n_s_minutes, __pyx_n_s_seconds); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(1, 271, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__62);
+  __Pyx_GIVEREF(__pyx_tuple__62);
+  __pyx_codeobj__63 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__62, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_encode_clock, 271, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__63)) __PYX_ERR(1, 271, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":275
+  /* "cf_units/_udunits2.pyx":274
  *     return ut_encode_clock(hours, minutes, seconds)
  * 
  * def encode_time(int year, int month, int day,             # <<<<<<<<<<<<<<
  *                 int hour, int minute, double second):
  *     return ut_encode_time(year, month, day, hour, minute, second)
  */
-  __pyx_tuple__69 = PyTuple_Pack(6, __pyx_n_s_year, __pyx_n_s_month, __pyx_n_s_day, __pyx_n_s_hour, __pyx_n_s_minute, __pyx_n_s_second); if (unlikely(!__pyx_tuple__69)) __PYX_ERR(1, 275, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__69);
-  __Pyx_GIVEREF(__pyx_tuple__69);
-  __pyx_codeobj__70 = (PyObject*)__Pyx_PyCode_New(6, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_encode_time, 275, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__70)) __PYX_ERR(1, 275, __pyx_L1_error)
+  __pyx_tuple__64 = PyTuple_Pack(6, __pyx_n_s_year, __pyx_n_s_month, __pyx_n_s_day, __pyx_n_s_hour, __pyx_n_s_minute, __pyx_n_s_second); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(1, 274, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__64);
+  __Pyx_GIVEREF(__pyx_tuple__64);
+  __pyx_codeobj__65 = (PyObject*)__Pyx_PyCode_New(6, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__64, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_encode_time, 274, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__65)) __PYX_ERR(1, 274, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":279
+  /* "cf_units/_udunits2.pyx":278
  *     return ut_encode_time(year, month, day, hour, minute, second)
  * 
  * def decode_time(double value):             # <<<<<<<<<<<<<<
  *     cdef int year, month, day, hour, minute
  *     cdef double second, resolution
  */
-  __pyx_tuple__71 = PyTuple_Pack(9, __pyx_n_s_value, __pyx_n_s_value, __pyx_n_s_year, __pyx_n_s_month, __pyx_n_s_day, __pyx_n_s_hour, __pyx_n_s_minute, __pyx_n_s_second, __pyx_n_s_resolution); if (unlikely(!__pyx_tuple__71)) __PYX_ERR(1, 279, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__71);
-  __Pyx_GIVEREF(__pyx_tuple__71);
-  __pyx_codeobj__72 = (PyObject*)__Pyx_PyCode_New(1, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__71, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_decode_time, 279, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__72)) __PYX_ERR(1, 279, __pyx_L1_error)
+  __pyx_tuple__66 = PyTuple_Pack(9, __pyx_n_s_value, __pyx_n_s_value, __pyx_n_s_year, __pyx_n_s_month, __pyx_n_s_day, __pyx_n_s_hour, __pyx_n_s_minute, __pyx_n_s_second, __pyx_n_s_resolution); if (unlikely(!__pyx_tuple__66)) __PYX_ERR(1, 278, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__66);
+  __Pyx_GIVEREF(__pyx_tuple__66);
+  __pyx_codeobj__67 = (PyObject*)__Pyx_PyCode_New(1, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_decode_time, 278, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__67)) __PYX_ERR(1, 278, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":286
+  /* "cf_units/_udunits2.pyx":285
  *     return (year, month, day, hour, minute, second, resolution)
  * 
  * def set_error_message_handler(ErrorMessageHandler handler):             # <<<<<<<<<<<<<<
  *     cdef ErrorMessageHandler result = ErrorMessageHandler()
  *     result.chandler = ut_set_error_message_handler(handler.chandler)
  */
-  __pyx_tuple__73 = PyTuple_Pack(2, __pyx_n_s_handler, __pyx_n_s_result); if (unlikely(!__pyx_tuple__73)) __PYX_ERR(1, 286, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__73);
-  __Pyx_GIVEREF(__pyx_tuple__73);
-  __pyx_codeobj__74 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__73, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_set_error_message_handler, 286, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__74)) __PYX_ERR(1, 286, __pyx_L1_error)
+  __pyx_tuple__68 = PyTuple_Pack(2, __pyx_n_s_handler, __pyx_n_s_result); if (unlikely(!__pyx_tuple__68)) __PYX_ERR(1, 285, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__68);
+  __Pyx_GIVEREF(__pyx_tuple__68);
+  __pyx_codeobj__69 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_set_error_message_handler, 285, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__69)) __PYX_ERR(1, 285, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":291
+  /* "cf_units/_udunits2.pyx":290
  *     return result
  * 
  * def convert_float(Converter converter, float value):             # <<<<<<<<<<<<<<
  *     return cv_convert_float(converter.cconverter, value)
  * 
  */
-  __pyx_tuple__75 = PyTuple_Pack(2, __pyx_n_s_converter, __pyx_n_s_value); if (unlikely(!__pyx_tuple__75)) __PYX_ERR(1, 291, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__75);
-  __Pyx_GIVEREF(__pyx_tuple__75);
-  __pyx_codeobj__76 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__75, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_convert_float, 291, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__76)) __PYX_ERR(1, 291, __pyx_L1_error)
+  __pyx_tuple__70 = PyTuple_Pack(2, __pyx_n_s_converter, __pyx_n_s_value); if (unlikely(!__pyx_tuple__70)) __PYX_ERR(1, 290, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__70);
+  __Pyx_GIVEREF(__pyx_tuple__70);
+  __pyx_codeobj__71 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__70, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_convert_float, 290, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__71)) __PYX_ERR(1, 290, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":294
+  /* "cf_units/_udunits2.pyx":293
  *     return cv_convert_float(converter.cconverter, value)
  * 
  * def convert_floats(Converter converter, np.ndarray[np.float32_t] in_, np.ndarray[np.float32_t] out):             # <<<<<<<<<<<<<<
  *     cv_convert_floats(converter.cconverter, <float*> in_.data, in_.size, <float*> out.data)
  *     return out
  */
-  __pyx_tuple__77 = PyTuple_Pack(3, __pyx_n_s_converter, __pyx_n_s_in, __pyx_n_s_out); if (unlikely(!__pyx_tuple__77)) __PYX_ERR(1, 294, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__77);
-  __Pyx_GIVEREF(__pyx_tuple__77);
-  __pyx_codeobj__78 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__77, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_convert_floats, 294, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__78)) __PYX_ERR(1, 294, __pyx_L1_error)
+  __pyx_tuple__72 = PyTuple_Pack(3, __pyx_n_s_converter, __pyx_n_s_in, __pyx_n_s_out); if (unlikely(!__pyx_tuple__72)) __PYX_ERR(1, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__72);
+  __Pyx_GIVEREF(__pyx_tuple__72);
+  __pyx_codeobj__73 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__72, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_convert_floats, 293, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__73)) __PYX_ERR(1, 293, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":298
+  /* "cf_units/_udunits2.pyx":297
  *     return out
  * 
  * def convert_double(Converter converter, double value):             # <<<<<<<<<<<<<<
  *     return cv_convert_double(converter.cconverter, value)
  * 
  */
-  __pyx_tuple__79 = PyTuple_Pack(2, __pyx_n_s_converter, __pyx_n_s_value); if (unlikely(!__pyx_tuple__79)) __PYX_ERR(1, 298, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__79);
-  __Pyx_GIVEREF(__pyx_tuple__79);
-  __pyx_codeobj__80 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__79, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_convert_double, 298, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__80)) __PYX_ERR(1, 298, __pyx_L1_error)
+  __pyx_tuple__74 = PyTuple_Pack(2, __pyx_n_s_converter, __pyx_n_s_value); if (unlikely(!__pyx_tuple__74)) __PYX_ERR(1, 297, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__74);
+  __Pyx_GIVEREF(__pyx_tuple__74);
+  __pyx_codeobj__75 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__74, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_convert_double, 297, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__75)) __PYX_ERR(1, 297, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":301
+  /* "cf_units/_udunits2.pyx":300
  *     return cv_convert_double(converter.cconverter, value)
  * 
  * def convert_doubles(Converter converter, np.ndarray[np.float64_t] in_, np.ndarray[np.float64_t] out):             # <<<<<<<<<<<<<<
  *     cv_convert_doubles(converter.cconverter, <double*> in_.data, in_.size, <double*> out.data)
  *     return out
  */
-  __pyx_tuple__81 = PyTuple_Pack(3, __pyx_n_s_converter, __pyx_n_s_in, __pyx_n_s_out); if (unlikely(!__pyx_tuple__81)) __PYX_ERR(1, 301, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__81);
-  __Pyx_GIVEREF(__pyx_tuple__81);
-  __pyx_codeobj__82 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__81, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_convert_doubles, 301, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__82)) __PYX_ERR(1, 301, __pyx_L1_error)
+  __pyx_tuple__76 = PyTuple_Pack(3, __pyx_n_s_converter, __pyx_n_s_in, __pyx_n_s_out); if (unlikely(!__pyx_tuple__76)) __PYX_ERR(1, 300, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__76);
+  __Pyx_GIVEREF(__pyx_tuple__76);
+  __pyx_codeobj__77 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__76, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cf_units__udunits2_pyx, __pyx_n_s_convert_doubles, 300, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__77)) __PYX_ERR(1, 300, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_4 = PyInt_FromLong(4); if (unlikely(!__pyx_int_4)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_8 = PyInt_FromLong(8); if (unlikely(!__pyx_int_8)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   return 0;
@@ -11693,53 +10212,53 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_8cf_units_9_udunits2_System) < 0) __PYX_ERR(1, 42, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8cf_units_9_udunits2_System) < 0) __PYX_ERR(1, 41, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8cf_units_9_udunits2_System.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8cf_units_9_udunits2_System.tp_dictoffset && __pyx_type_8cf_units_9_udunits2_System.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8cf_units_9_udunits2_System.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_System, (PyObject *)&__pyx_type_8cf_units_9_udunits2_System) < 0) __PYX_ERR(1, 42, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8cf_units_9_udunits2_System) < 0) __PYX_ERR(1, 42, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_System, (PyObject *)&__pyx_type_8cf_units_9_udunits2_System) < 0) __PYX_ERR(1, 41, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8cf_units_9_udunits2_System) < 0) __PYX_ERR(1, 41, __pyx_L1_error)
   __pyx_ptype_8cf_units_9_udunits2_System = &__pyx_type_8cf_units_9_udunits2_System;
-  if (PyType_Ready(&__pyx_type_8cf_units_9_udunits2_Unit) < 0) __PYX_ERR(1, 57, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8cf_units_9_udunits2_Unit) < 0) __PYX_ERR(1, 56, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8cf_units_9_udunits2_Unit.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8cf_units_9_udunits2_Unit.tp_dictoffset && __pyx_type_8cf_units_9_udunits2_Unit.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8cf_units_9_udunits2_Unit.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Unit, (PyObject *)&__pyx_type_8cf_units_9_udunits2_Unit) < 0) __PYX_ERR(1, 57, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8cf_units_9_udunits2_Unit) < 0) __PYX_ERR(1, 57, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Unit, (PyObject *)&__pyx_type_8cf_units_9_udunits2_Unit) < 0) __PYX_ERR(1, 56, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8cf_units_9_udunits2_Unit) < 0) __PYX_ERR(1, 56, __pyx_L1_error)
   __pyx_ptype_8cf_units_9_udunits2_Unit = &__pyx_type_8cf_units_9_udunits2_Unit;
-  if (PyType_Ready(&__pyx_type_8cf_units_9_udunits2_Converter) < 0) __PYX_ERR(1, 74, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8cf_units_9_udunits2_Converter) < 0) __PYX_ERR(1, 73, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8cf_units_9_udunits2_Converter.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8cf_units_9_udunits2_Converter.tp_dictoffset && __pyx_type_8cf_units_9_udunits2_Converter.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8cf_units_9_udunits2_Converter.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Converter, (PyObject *)&__pyx_type_8cf_units_9_udunits2_Converter) < 0) __PYX_ERR(1, 74, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8cf_units_9_udunits2_Converter) < 0) __PYX_ERR(1, 74, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Converter, (PyObject *)&__pyx_type_8cf_units_9_udunits2_Converter) < 0) __PYX_ERR(1, 73, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8cf_units_9_udunits2_Converter) < 0) __PYX_ERR(1, 73, __pyx_L1_error)
   __pyx_ptype_8cf_units_9_udunits2_Converter = &__pyx_type_8cf_units_9_udunits2_Converter;
-  if (PyType_Ready(&__pyx_type_8cf_units_9_udunits2_ErrorMessageHandler) < 0) __PYX_ERR(1, 89, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8cf_units_9_udunits2_ErrorMessageHandler) < 0) __PYX_ERR(1, 88, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8cf_units_9_udunits2_ErrorMessageHandler.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8cf_units_9_udunits2_ErrorMessageHandler.tp_dictoffset && __pyx_type_8cf_units_9_udunits2_ErrorMessageHandler.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8cf_units_9_udunits2_ErrorMessageHandler.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ErrorMessageHandler, (PyObject *)&__pyx_type_8cf_units_9_udunits2_ErrorMessageHandler) < 0) __PYX_ERR(1, 89, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8cf_units_9_udunits2_ErrorMessageHandler) < 0) __PYX_ERR(1, 89, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ErrorMessageHandler, (PyObject *)&__pyx_type_8cf_units_9_udunits2_ErrorMessageHandler) < 0) __PYX_ERR(1, 88, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8cf_units_9_udunits2_ErrorMessageHandler) < 0) __PYX_ERR(1, 88, __pyx_L1_error)
   __pyx_ptype_8cf_units_9_udunits2_ErrorMessageHandler = &__pyx_type_8cf_units_9_udunits2_ErrorMessageHandler;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -11752,33 +10271,68 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 206, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 206, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 233, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 242, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 917, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 200, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 223, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 227, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 787, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 789, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -11965,15 +10519,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_cf_units___udunits2) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -11999,43 +10553,43 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
 
-  /* "cf_units/_udunits2.pyx":18
+  /* "cf_units/_udunits2.pyx":17
  * # cython: nonecheck=True
  * 
  * import numpy as np             # <<<<<<<<<<<<<<
  * 
  * cimport numpy as np
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 18, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(1, 18, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":24
+  /* "cf_units/_udunits2.pyx":23
  * 
  * 
  * cdef int _STRING_BUFFER_DEPTH = 128             # <<<<<<<<<<<<<<
  * cdef list _UT_STATUS = ['UT_SUCCESS', 'UT_BAD_ARG', 'UT_EXISTS', 'UT_NO_UNIT',
  *                         'UT_OS', 'UT_NOT_SAME_SYSTEM', 'UT_MEANINGLESS',
  */
   __pyx_v_8cf_units_9_udunits2__STRING_BUFFER_DEPTH = 0x80;
 
-  /* "cf_units/_udunits2.pyx":25
+  /* "cf_units/_udunits2.pyx":24
  * 
  * cdef int _STRING_BUFFER_DEPTH = 128
  * cdef list _UT_STATUS = ['UT_SUCCESS', 'UT_BAD_ARG', 'UT_EXISTS', 'UT_NO_UNIT',             # <<<<<<<<<<<<<<
  *                         'UT_OS', 'UT_NOT_SAME_SYSTEM', 'UT_MEANINGLESS',
  *                         'UT_NO_SECOND', 'UT_VISIT_ERROR', 'UT_CANT_FORMAT',
  */
-  __pyx_t_1 = PyList_New(16); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 25, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(16); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_UT_SUCCESS);
   __Pyx_GIVEREF(__pyx_n_s_UT_SUCCESS);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_UT_SUCCESS);
   __Pyx_INCREF(__pyx_n_s_UT_BAD_ARG);
   __Pyx_GIVEREF(__pyx_n_s_UT_BAD_ARG);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_UT_BAD_ARG);
@@ -12082,547 +10636,547 @@
   __Pyx_GIVEREF(__pyx_n_s_UT_PARSE);
   PyList_SET_ITEM(__pyx_t_1, 15, __pyx_n_s_UT_PARSE);
   __Pyx_XGOTREF(__pyx_v_8cf_units_9_udunits2__UT_STATUS);
   __Pyx_DECREF_SET(__pyx_v_8cf_units_9_udunits2__UT_STATUS, ((PyObject*)__pyx_t_1));
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":31
+  /* "cf_units/_udunits2.pyx":30
  *                         'UT_OPEN_ENV', 'UT_OPEN_DEFAULT', 'UT_PARSE']
  * 
  * UT_ASCII = 0             # <<<<<<<<<<<<<<
  * UT_ISO_8859_1 = 1
  * UT_LATIN1 = UT_ISO_8859_1
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UT_ASCII, __pyx_int_0) < 0) __PYX_ERR(1, 31, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UT_ASCII, __pyx_int_0) < 0) __PYX_ERR(1, 30, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":32
+  /* "cf_units/_udunits2.pyx":31
  * 
  * UT_ASCII = 0
  * UT_ISO_8859_1 = 1             # <<<<<<<<<<<<<<
  * UT_LATIN1 = UT_ISO_8859_1
  * UT_UTF8 = 2
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UT_ISO_8859_1, __pyx_int_1) < 0) __PYX_ERR(1, 32, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UT_ISO_8859_1, __pyx_int_1) < 0) __PYX_ERR(1, 31, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":33
+  /* "cf_units/_udunits2.pyx":32
  * UT_ASCII = 0
  * UT_ISO_8859_1 = 1
  * UT_LATIN1 = UT_ISO_8859_1             # <<<<<<<<<<<<<<
  * UT_UTF8 = 2
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_UT_ISO_8859_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 33, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_UT_ISO_8859_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UT_LATIN1, __pyx_t_1) < 0) __PYX_ERR(1, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UT_LATIN1, __pyx_t_1) < 0) __PYX_ERR(1, 32, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":34
+  /* "cf_units/_udunits2.pyx":33
  * UT_ISO_8859_1 = 1
  * UT_LATIN1 = UT_ISO_8859_1
  * UT_UTF8 = 2             # <<<<<<<<<<<<<<
  * 
  * UT_NAMES = 4
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UT_UTF8, __pyx_int_2) < 0) __PYX_ERR(1, 34, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UT_UTF8, __pyx_int_2) < 0) __PYX_ERR(1, 33, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":36
+  /* "cf_units/_udunits2.pyx":35
  * UT_UTF8 = 2
  * 
  * UT_NAMES = 4             # <<<<<<<<<<<<<<
  * UT_DEFINITION = 8
  * 
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UT_NAMES, __pyx_int_4) < 0) __PYX_ERR(1, 36, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UT_NAMES, __pyx_int_4) < 0) __PYX_ERR(1, 35, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":37
+  /* "cf_units/_udunits2.pyx":36
  * 
  * UT_NAMES = 4
  * UT_DEFINITION = 8             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UT_DEFINITION, __pyx_int_8) < 0) __PYX_ERR(1, 37, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UT_DEFINITION, __pyx_int_8) < 0) __PYX_ERR(1, 36, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":125
+  /* "cf_units/_udunits2.pyx":124
  *     return converter
  * 
  * cdef ErrorMessageHandler _ignore = ErrorMessageHandler()             # <<<<<<<<<<<<<<
  * _ignore.chandler = ut_ignore
  * ignore = _ignore
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8cf_units_9_udunits2_ErrorMessageHandler)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 125, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8cf_units_9_udunits2_ErrorMessageHandler)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(((PyObject *)__pyx_v_8cf_units_9_udunits2__ignore));
   __Pyx_DECREF_SET(__pyx_v_8cf_units_9_udunits2__ignore, ((struct __pyx_obj_8cf_units_9_udunits2_ErrorMessageHandler *)__pyx_t_1));
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":126
+  /* "cf_units/_udunits2.pyx":125
  * 
  * cdef ErrorMessageHandler _ignore = ErrorMessageHandler()
  * _ignore.chandler = ut_ignore             # <<<<<<<<<<<<<<
  * ignore = _ignore
  * 
  */
   __pyx_v_8cf_units_9_udunits2__ignore->chandler = ut_ignore;
 
-  /* "cf_units/_udunits2.pyx":127
+  /* "cf_units/_udunits2.pyx":126
  * cdef ErrorMessageHandler _ignore = ErrorMessageHandler()
  * _ignore.chandler = ut_ignore
  * ignore = _ignore             # <<<<<<<<<<<<<<
  * 
  * # Convenience object to avoid having to do None handling either here or in
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ignore, ((PyObject *)__pyx_v_8cf_units_9_udunits2__ignore)) < 0) __PYX_ERR(1, 127, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ignore, ((PyObject *)__pyx_v_8cf_units_9_udunits2__ignore)) < 0) __PYX_ERR(1, 126, __pyx_L1_error)
 
-  /* "cf_units/_udunits2.pyx":131
+  /* "cf_units/_udunits2.pyx":130
  * # Convenience object to avoid having to do None handling either here or in
  * # user code
  * NULL_UNIT = Unit()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8cf_units_9_udunits2_Unit)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 131, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8cf_units_9_udunits2_Unit)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NULL_UNIT, __pyx_t_1) < 0) __PYX_ERR(1, 131, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NULL_UNIT, __pyx_t_1) < 0) __PYX_ERR(1, 130, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":136
+  /* "cf_units/_udunits2.pyx":135
  * ##### Exception class #####
  * 
  * class UdunitsError(Exception):             # <<<<<<<<<<<<<<
  *     """
  *     UDUNITS-2 call resulted in an error.
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 136, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __Pyx_GIVEREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 136, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_UdunitsError, __pyx_n_s_UdunitsError, (PyObject *) NULL, __pyx_n_s_cf_units__udunits2, __pyx_kp_s_UDUNITS_2_call_resulted_in_an_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 136, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_UdunitsError, __pyx_n_s_UdunitsError, (PyObject *) NULL, __pyx_n_s_cf_units__udunits2, __pyx_kp_s_UDUNITS_2_call_resulted_in_an_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "cf_units/_udunits2.pyx":148
+  /* "cf_units/_udunits2.pyx":147
  * 
  *     """
  *     def __init__(self, ut_status status, int errnum):             # <<<<<<<<<<<<<<
  *         self.status = status
  *         self.errnum = errnum
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8cf_units_9_udunits2_12UdunitsError_1__init__, 0, __pyx_n_s_UdunitsError___init, NULL, __pyx_n_s_cf_units__udunits2, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 148, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8cf_units_9_udunits2_12UdunitsError_1__init__, 0, __pyx_n_s_UdunitsError___init, NULL, __pyx_n_s_cf_units__udunits2, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(1, 148, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(1, 147, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "cf_units/_udunits2.pyx":152
+  /* "cf_units/_udunits2.pyx":151
  *         self.errnum = errnum
  * 
  *     def status_msg(self):             # <<<<<<<<<<<<<<
  *         """
  *         String representation of the UDUNITS-2 ut_status value which resulted
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8cf_units_9_udunits2_12UdunitsError_3status_msg, 0, __pyx_n_s_UdunitsError_status_msg, NULL, __pyx_n_s_cf_units__udunits2, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 152, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8cf_units_9_udunits2_12UdunitsError_3status_msg, 0, __pyx_n_s_UdunitsError_status_msg, NULL, __pyx_n_s_cf_units__udunits2, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_status_msg, __pyx_t_4) < 0) __PYX_ERR(1, 152, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_status_msg, __pyx_t_4) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "cf_units/_udunits2.pyx":163
+  /* "cf_units/_udunits2.pyx":162
  *             return 'UNKNOWN'
  * 
  *     def error_msg(self):             # <<<<<<<<<<<<<<
  *         """
  *         The message string associated with the errno value which resulted from
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8cf_units_9_udunits2_12UdunitsError_5error_msg, 0, __pyx_n_s_UdunitsError_error_msg, NULL, __pyx_n_s_cf_units__udunits2, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 163, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8cf_units_9_udunits2_12UdunitsError_5error_msg, 0, __pyx_n_s_UdunitsError_error_msg, NULL, __pyx_n_s_cf_units__udunits2, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_error_msg, __pyx_t_4) < 0) __PYX_ERR(1, 163, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_error_msg, __pyx_t_4) < 0) __PYX_ERR(1, 162, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "cf_units/_udunits2.pyx":171
+  /* "cf_units/_udunits2.pyx":170
  *         return string.strerror(self.errnum) if self.errnum else ''
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         str_err = ': {}'.format(string.strerror(self.errnum)) \
  *                   if self.errnum else ''
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8cf_units_9_udunits2_12UdunitsError_7__str__, 0, __pyx_n_s_UdunitsError___str, NULL, __pyx_n_s_cf_units__udunits2, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 171, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8cf_units_9_udunits2_12UdunitsError_7__str__, 0, __pyx_n_s_UdunitsError___str, NULL, __pyx_n_s_cf_units__udunits2, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_str, __pyx_t_4) < 0) __PYX_ERR(1, 171, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_str, __pyx_t_4) < 0) __PYX_ERR(1, 170, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "cf_units/_udunits2.pyx":136
+  /* "cf_units/_udunits2.pyx":135
  * ##### Exception class #####
  * 
  * class UdunitsError(Exception):             # <<<<<<<<<<<<<<
  *     """
  *     UDUNITS-2 call resulted in an error.
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_UdunitsError, __pyx_t_1, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 136, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_UdunitsError, __pyx_t_1, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UdunitsError, __pyx_t_4) < 0) __PYX_ERR(1, 136, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UdunitsError, __pyx_t_4) < 0) __PYX_ERR(1, 135, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":177
+  /* "cf_units/_udunits2.pyx":176
  * 
  * 
  * def _raise_error():             # <<<<<<<<<<<<<<
  *     """
  *     Raise a UdunitsError with the current value of errno and ut_status
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_1_raise_error, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 177, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_1_raise_error, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_raise_error, __pyx_t_1) < 0) __PYX_ERR(1, 177, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_raise_error, __pyx_t_1) < 0) __PYX_ERR(1, 176, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":193
+  /* "cf_units/_udunits2.pyx":192
  * # See the UDUNITS-2 documentation for details.
  * 
  * def read_xml(char* path=NULL):             # <<<<<<<<<<<<<<
  *     cdef ut_system* csystem = ut_read_xml(path)
  *     return wrap_system(csystem)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_3read_xml, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 193, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_3read_xml, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 192, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_xml, __pyx_t_1) < 0) __PYX_ERR(1, 193, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_xml, __pyx_t_1) < 0) __PYX_ERR(1, 192, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":197
+  /* "cf_units/_udunits2.pyx":196
  *     return wrap_system(csystem)
  * 
  * def get_unit_by_name(System system, char* name):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_get_unit_by_name(system.csystem, name)
  *     return wrap_unit(system, cunit)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_5get_unit_by_name, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 197, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_5get_unit_by_name, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_unit_by_name, __pyx_t_1) < 0) __PYX_ERR(1, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_unit_by_name, __pyx_t_1) < 0) __PYX_ERR(1, 196, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":201
+  /* "cf_units/_udunits2.pyx":200
  *     return wrap_unit(system, cunit)
  * 
  * def clone(Unit unit):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_clone(unit.cunit)
  *     return wrap_unit(unit.system, cunit)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_7clone, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 201, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_7clone, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_clone, __pyx_t_1) < 0) __PYX_ERR(1, 201, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_clone, __pyx_t_1) < 0) __PYX_ERR(1, 200, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":205
+  /* "cf_units/_udunits2.pyx":204
  *     return wrap_unit(unit.system, cunit)
  * 
  * def is_dimensionless(Unit unit):             # <<<<<<<<<<<<<<
  *     return <bint>ut_is_dimensionless(unit.cunit)
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_9is_dimensionless, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 205, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_9is_dimensionless, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_is_dimensionless, __pyx_t_1) < 0) __PYX_ERR(1, 205, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_is_dimensionless, __pyx_t_1) < 0) __PYX_ERR(1, 204, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":208
+  /* "cf_units/_udunits2.pyx":207
  *     return <bint>ut_is_dimensionless(unit.cunit)
  * 
  * def compare(Unit unit1, Unit unit2):             # <<<<<<<<<<<<<<
  *     return ut_compare(unit1.cunit, unit2.cunit)
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_11compare, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 208, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_11compare, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compare, __pyx_t_1) < 0) __PYX_ERR(1, 208, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compare, __pyx_t_1) < 0) __PYX_ERR(1, 207, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":211
+  /* "cf_units/_udunits2.pyx":210
  *     return ut_compare(unit1.cunit, unit2.cunit)
  * 
  * def are_convertible(Unit unit1, Unit unit2):             # <<<<<<<<<<<<<<
  *     return <bint>ut_are_convertible(unit1.cunit, unit2.cunit)
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_13are_convertible, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 211, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_13are_convertible, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_are_convertible, __pyx_t_1) < 0) __PYX_ERR(1, 211, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_are_convertible, __pyx_t_1) < 0) __PYX_ERR(1, 210, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":214
+  /* "cf_units/_udunits2.pyx":213
  *     return <bint>ut_are_convertible(unit1.cunit, unit2.cunit)
  * 
  * def get_converter(Unit fr, Unit to):             # <<<<<<<<<<<<<<
  *     cdef cv_converter* cconverter = ut_get_converter(fr.cunit, to.cunit)
  *     return wrap_converter(cconverter)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_15get_converter, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 214, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_15get_converter, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_converter, __pyx_t_1) < 0) __PYX_ERR(1, 214, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_converter, __pyx_t_1) < 0) __PYX_ERR(1, 213, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":218
+  /* "cf_units/_udunits2.pyx":217
  *     return wrap_converter(cconverter)
  * 
  * def scale(double factor, Unit unit):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_scale(factor, unit.cunit)
  *     return wrap_unit(unit.system, cunit)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_17scale, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 218, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_17scale, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 217, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_scale, __pyx_t_1) < 0) __PYX_ERR(1, 218, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_scale, __pyx_t_1) < 0) __PYX_ERR(1, 217, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":222
+  /* "cf_units/_udunits2.pyx":221
  *     return wrap_unit(unit.system, cunit)
  * 
  * def offset(Unit unit, double offset):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_offset(unit.cunit, offset)
  *     return wrap_unit(unit.system, cunit)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_19offset, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_19offset, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 221, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_offset, __pyx_t_1) < 0) __PYX_ERR(1, 222, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_offset, __pyx_t_1) < 0) __PYX_ERR(1, 221, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":226
+  /* "cf_units/_udunits2.pyx":225
  *     return wrap_unit(unit.system, cunit)
  * 
  * def offset_by_time(Unit unit, double origin):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_offset_by_time(unit.cunit, origin)
  *     return wrap_unit(unit.system, cunit)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_21offset_by_time, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_21offset_by_time, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_offset_by_time, __pyx_t_1) < 0) __PYX_ERR(1, 226, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_offset_by_time, __pyx_t_1) < 0) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":230
+  /* "cf_units/_udunits2.pyx":229
  *     return wrap_unit(unit.system, cunit)
  * 
  * def multiply(Unit unit1, Unit unit2):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_multiply(unit1.cunit, unit2.cunit)
  *     return wrap_unit(unit1.system, cunit)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_23multiply, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 230, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_23multiply, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_multiply, __pyx_t_1) < 0) __PYX_ERR(1, 230, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_multiply, __pyx_t_1) < 0) __PYX_ERR(1, 229, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":234
+  /* "cf_units/_udunits2.pyx":233
  *     return wrap_unit(unit1.system, cunit)
  * 
  * def invert(Unit unit):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit =  ut_invert(unit.cunit)
  *     return wrap_unit(unit.system, cunit)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_25invert, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 234, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_25invert, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 233, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_invert, __pyx_t_1) < 0) __PYX_ERR(1, 234, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_invert, __pyx_t_1) < 0) __PYX_ERR(1, 233, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":238
+  /* "cf_units/_udunits2.pyx":237
  *     return wrap_unit(unit.system, cunit)
  * 
  * def divide(Unit numer, Unit denom):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_divide(numer.cunit, denom.cunit)
  *     return wrap_unit(numer.system, cunit)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_27divide, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_27divide, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 237, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_divide, __pyx_t_1) < 0) __PYX_ERR(1, 238, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_divide, __pyx_t_1) < 0) __PYX_ERR(1, 237, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":242
+  /* "cf_units/_udunits2.pyx":241
  *     return wrap_unit(numer.system, cunit)
  * 
  * def raise_(Unit unit, int power):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_raise(unit.cunit, power)
  *     return wrap_unit(unit.system, cunit)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_29raise_, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 242, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_29raise_, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_raise, __pyx_t_1) < 0) __PYX_ERR(1, 242, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_raise, __pyx_t_1) < 0) __PYX_ERR(1, 241, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":246
+  /* "cf_units/_udunits2.pyx":245
  *     return wrap_unit(unit.system, cunit)
  * 
  * def root(Unit unit, int root):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_root(unit.cunit, root)
  *     return wrap_unit(unit.system, cunit)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_31root, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 246, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_31root, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_root, __pyx_t_1) < 0) __PYX_ERR(1, 246, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_root, __pyx_t_1) < 0) __PYX_ERR(1, 245, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":250
+  /* "cf_units/_udunits2.pyx":249
  *     return wrap_unit(unit.system, cunit)
  * 
  * def log(double base, Unit reference):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_log(base, reference.cunit)
  *     return wrap_unit(reference.system, cunit)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_33log, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 250, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_33log, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log, __pyx_t_1) < 0) __PYX_ERR(1, 250, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log, __pyx_t_1) < 0) __PYX_ERR(1, 249, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":255
+  /* "cf_units/_udunits2.pyx":254
  * 
  * 
  * def parse(System system, char* string, ut_encoding encoding):             # <<<<<<<<<<<<<<
  *     cdef ut_unit* cunit = ut_parse(system.csystem, string, encoding)
  *     return wrap_unit(system, cunit)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_35parse, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 255, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_35parse, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_parse, __pyx_t_1) < 0) __PYX_ERR(1, 255, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_parse, __pyx_t_1) < 0) __PYX_ERR(1, 254, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":259
+  /* "cf_units/_udunits2.pyx":258
  *     return wrap_unit(system, cunit)
  * 
  * def format(Unit unit, unsigned opts=0):             # <<<<<<<<<<<<<<
  *     cdef bytearray buf = bytearray(_STRING_BUFFER_DEPTH)
  *     n = ut_format(unit.cunit, buf, len(buf), opts)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_37format, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 259, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_37format, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_format, __pyx_t_1) < 0) __PYX_ERR(1, 259, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_format, __pyx_t_1) < 0) __PYX_ERR(1, 258, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":269
+  /* "cf_units/_udunits2.pyx":268
  *     return bytes(buf[:n])
  * 
  * def encode_date(int year, int month, int day):             # <<<<<<<<<<<<<<
  *     return ut_encode_date(year, month, day)
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_39encode_date, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 269, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_39encode_date, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 268, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_encode_date, __pyx_t_1) < 0) __PYX_ERR(1, 269, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_encode_date, __pyx_t_1) < 0) __PYX_ERR(1, 268, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":272
+  /* "cf_units/_udunits2.pyx":271
  *     return ut_encode_date(year, month, day)
  * 
  * def encode_clock(int hours, int minutes, double seconds):             # <<<<<<<<<<<<<<
  *     return ut_encode_clock(hours, minutes, seconds)
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_41encode_clock, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 272, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_41encode_clock, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_encode_clock, __pyx_t_1) < 0) __PYX_ERR(1, 272, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_encode_clock, __pyx_t_1) < 0) __PYX_ERR(1, 271, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":275
+  /* "cf_units/_udunits2.pyx":274
  *     return ut_encode_clock(hours, minutes, seconds)
  * 
  * def encode_time(int year, int month, int day,             # <<<<<<<<<<<<<<
  *                 int hour, int minute, double second):
  *     return ut_encode_time(year, month, day, hour, minute, second)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_43encode_time, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 275, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_43encode_time, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_encode_time, __pyx_t_1) < 0) __PYX_ERR(1, 275, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_encode_time, __pyx_t_1) < 0) __PYX_ERR(1, 274, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":279
+  /* "cf_units/_udunits2.pyx":278
  *     return ut_encode_time(year, month, day, hour, minute, second)
  * 
  * def decode_time(double value):             # <<<<<<<<<<<<<<
  *     cdef int year, month, day, hour, minute
  *     cdef double second, resolution
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_45decode_time, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 279, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_45decode_time, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_decode_time, __pyx_t_1) < 0) __PYX_ERR(1, 279, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_decode_time, __pyx_t_1) < 0) __PYX_ERR(1, 278, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":286
+  /* "cf_units/_udunits2.pyx":285
  *     return (year, month, day, hour, minute, second, resolution)
  * 
  * def set_error_message_handler(ErrorMessageHandler handler):             # <<<<<<<<<<<<<<
  *     cdef ErrorMessageHandler result = ErrorMessageHandler()
  *     result.chandler = ut_set_error_message_handler(handler.chandler)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_47set_error_message_handler, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 286, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_47set_error_message_handler, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 285, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_set_error_message_handler, __pyx_t_1) < 0) __PYX_ERR(1, 286, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_set_error_message_handler, __pyx_t_1) < 0) __PYX_ERR(1, 285, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":291
+  /* "cf_units/_udunits2.pyx":290
  *     return result
  * 
  * def convert_float(Converter converter, float value):             # <<<<<<<<<<<<<<
  *     return cv_convert_float(converter.cconverter, value)
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_49convert_float, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 291, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_49convert_float, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 290, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_convert_float, __pyx_t_1) < 0) __PYX_ERR(1, 291, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_convert_float, __pyx_t_1) < 0) __PYX_ERR(1, 290, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":294
+  /* "cf_units/_udunits2.pyx":293
  *     return cv_convert_float(converter.cconverter, value)
  * 
  * def convert_floats(Converter converter, np.ndarray[np.float32_t] in_, np.ndarray[np.float32_t] out):             # <<<<<<<<<<<<<<
  *     cv_convert_floats(converter.cconverter, <float*> in_.data, in_.size, <float*> out.data)
  *     return out
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_51convert_floats, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 294, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_51convert_floats, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_convert_floats, __pyx_t_1) < 0) __PYX_ERR(1, 294, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_convert_floats, __pyx_t_1) < 0) __PYX_ERR(1, 293, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":298
+  /* "cf_units/_udunits2.pyx":297
  *     return out
  * 
  * def convert_double(Converter converter, double value):             # <<<<<<<<<<<<<<
  *     return cv_convert_double(converter.cconverter, value)
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_53convert_double, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 298, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_53convert_double, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_convert_double, __pyx_t_1) < 0) __PYX_ERR(1, 298, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_convert_double, __pyx_t_1) < 0) __PYX_ERR(1, 297, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cf_units/_udunits2.pyx":301
+  /* "cf_units/_udunits2.pyx":300
  *     return cv_convert_double(converter.cconverter, value)
  * 
  * def convert_doubles(Converter converter, np.ndarray[np.float64_t] in_, np.ndarray[np.float64_t] out):             # <<<<<<<<<<<<<<
  *     cv_convert_doubles(converter.cconverter, <double*> in_.data, in_.size, <double*> out.data)
  *     return out
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_55convert_doubles, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 301, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8cf_units_9_udunits2_55convert_doubles, NULL, __pyx_n_s_cf_units__udunits2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_convert_doubles, __pyx_t_1) < 0) __PYX_ERR(1, 301, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_convert_doubles, __pyx_t_1) < 0) __PYX_ERR(1, 300, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "cf_units/_udunits2.pyx":1
  * # Copyright cf-units contributors             # <<<<<<<<<<<<<<
  * #
- * # This file is part of cf-units and is released under the LGPL license.
+ * # This file is part of cf-units and is released under the BSD license.
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../../tmp/build-env-ad30fk9n/lib/python3.8/site-packages/Cython/Includes/numpy/__init__.pxd":1045
- *         raise ImportError("numpy.core.umath failed to import")
+  /* "../../../../../tmp/build-env-j078x8d5/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -12937,28 +11491,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -13167,15 +11721,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -13464,15 +12018,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -14291,69 +12845,14 @@
   if (buf->suboffsets == NULL) buf->suboffsets = __Pyx_minusones;
   return 0;
 fail:;
   __Pyx_SafeReleaseBuffer(buf);
   return -1;
 }
 
-/* DictGetItem */
-  #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
-    PyObject *value;
-    value = PyDict_GetItemWithError(d, key);
-    if (unlikely(!value)) {
-        if (!PyErr_Occurred()) {
-            if (unlikely(PyTuple_Check(key))) {
-                PyObject* args = PyTuple_Pack(1, key);
-                if (likely(args)) {
-                    PyErr_SetObject(PyExc_KeyError, args);
-                    Py_DECREF(args);
-                }
-            } else {
-                PyErr_SetObject(PyExc_KeyError, key);
-            }
-        }
-        return NULL;
-    }
-    Py_INCREF(value);
-    return value;
-}
-#endif
-
-/* RaiseTooManyValuesToUnpack */
-  static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
-    PyErr_Format(PyExc_ValueError,
-                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
-}
-
-/* RaiseNeedMoreValuesToUnpack */
-  static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
-    PyErr_Format(PyExc_ValueError,
-                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
-                 index, (index == 1) ? "" : "s");
-}
-
-/* RaiseNoneIterError */
-  static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-}
-
-/* ExtTypeTest */
-  static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
-    if (unlikely(!type)) {
-        PyErr_SetString(PyExc_SystemError, "Missing type object");
-        return 0;
-    }
-    if (likely(__Pyx_TypeCheck(obj, type)))
-        return 1;
-    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
-                 Py_TYPE(obj)->tp_name, type->tp_name);
-    return 0;
-}
-
 /* GetTopmostException */
   #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -14681,44 +13180,62 @@
     return ret;
 }
 
 /* TypeImport */
   #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -15378,17 +13895,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -15574,15 +14096,15 @@
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
 /* CLineInTraceback */
   #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -15804,27 +14326,25 @@
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
 #if PY_MAJOR_VERSION < 3
 static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
     if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-        if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) return __pyx_pw_5numpy_7ndarray_1__getbuffer__(obj, view, flags);
     PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
     return -1;
 }
 static void __Pyx_ReleaseBuffer(Py_buffer *view) {
     PyObject *obj = view->obj;
     if (!obj) return;
     if (PyObject_CheckBuffer(obj)) {
         PyBuffer_Release(view);
         return;
     }
     if ((0)) {}
-        else if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) __pyx_pw_5numpy_7ndarray_3__releasebuffer__(obj, view);
     view->obj = NULL;
     Py_DECREF(obj);
 }
 #endif
 
 
   /* CIntFromPyVerify */
@@ -15974,15 +14494,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -16128,15 +14648,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -17210,52 +15730,14 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to size_t");
     return (size_t) -1;
 }
 
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const enum NPY_TYPES neg_one = (enum NPY_TYPES) -1, const_zero = (enum NPY_TYPES) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(enum NPY_TYPES) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(enum NPY_TYPES) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(enum NPY_TYPES),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
```

### Comparing `cf-units-3.1.1/cf_units/_udunits2.pxd` & `cf-units-3.2.0/cf_units/_udunits2.pxd`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 
 cdef extern from "udunits2.h":
     ctypedef struct ut_system:
         pass
 
     ctypedef union ut_unit:
         pass
```

### Comparing `cf-units-3.1.1/cf_units/_udunits2.pyx` & `cf-units-3.2.0/cf_units/_udunits2.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """
 Units of measure.
 
 Wrapper for Unidata/UCAR UDUNITS-2.
 
 See also: `UDUNITS-2
 <http://www.unidata.ucar.edu/software/udunits/udunits-2/udunits2.html>`_.
```

### Comparing `cf-units-3.1.1/cf_units/_udunits2_parser/README.md` & `cf-units-3.2.0/cf_units/_udunits2_parser/README.md`

 * *Files identical despite different names*

### Comparing `cf-units-3.1.1/cf_units/_udunits2_parser/__init__.py` & `cf-units-3.2.0/cf_units/_udunits2_parser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 
 import unicodedata
 
 from antlr4 import CommonTokenStream, InputStream
 from antlr4.error.ErrorListener import ErrorListener
 
 from . import graph
```

### Comparing `cf-units-3.1.1/cf_units/_udunits2_parser/compile.py` & `cf-units-3.2.0/cf_units/_udunits2_parser/compile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 
 """
 Compiles the UDUNITS-2 grammar using ANTLR4.
 
 You may be interested in running this with entr to watch changes to the
 grammar:
```

### Comparing `cf-units-3.1.1/cf_units/_udunits2_parser/graph.py` & `cf-units-3.2.0/cf_units/_udunits2_parser/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 
 
 class Node:
     """
     Represents a node in an expression graph.
 
     """
```

### Comparing `cf-units-3.1.1/cf_units/_udunits2_parser/parser/udunits2Lexer.py` & `cf-units-3.2.0/cf_units/_udunits2_parser/parser/udunits2Lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,14 @@
         buf.write("\4\2\t\3\2\t\4\2\t\5\2\t\6\2\t\7\2\t\b\2\t\t\2\t\n\2\t")
         buf.write("\13\2\t\f\2\t\r\2\t\16\2\t\17\2\t\20\2\t\21\2\t\22\2\t")
         buf.write("\23\2\t\24\2\t\25\2\t\26\2\4\2\2")
         return buf.getvalue()
 
 
 class udunits2Lexer(Lexer):
-
     atn = ATNDeserializer().deserialize(serializedATN())
 
     decisionsToDFA = [DFA(ds, i) for i, ds in enumerate(atn.decisionToState)]
 
     SHIFT_MODE = 1
     ID_SEEN = 2
```

### Comparing `cf-units-3.1.1/cf_units/_udunits2_parser/parser/udunits2Parser.py` & `cf-units-3.2.0/cf_units/_udunits2_parser/parser/udunits2Parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         buf.write("}{\3\2\2\2}|\3\2\2\2~\23\3\2\2\2\177\u0082\7\31\2\2\u0080")
         buf.write("\u0082\5\f\7\2\u0081\177\3\2\2\2\u0081\u0080\3\2\2\2\u0082")
         buf.write('\25\3\2\2\2\26\27\36"(,\60ADFT\\bgknsvx}\u0081')
         return buf.getvalue()
 
 
 class udunits2Parser(Parser):
-
     grammarFileName = "udunits2Parser.g4"
 
     atn = ATNDeserializer().deserialize(serializedATN())
 
     decisionsToDFA = [DFA(ds, i) for i, ds in enumerate(atn.decisionToState)]
 
     sharedContextCache = PredictionContextCache()
@@ -211,15 +210,14 @@
         def accept(self, visitor: ParseTreeVisitor):
             if hasattr(visitor, "visitUnit_spec"):
                 return visitor.visitUnit_spec(self)
             else:
                 return visitor.visitChildren(self)
 
     def unit_spec(self):
-
         localctx = udunits2Parser.Unit_specContext(self, self._ctx, self.state)
         self.enterRule(localctx, 0, self.RULE_unit_spec)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
             self.state = 21
             self._errHandler.sync(self)
@@ -281,15 +279,14 @@
         def accept(self, visitor: ParseTreeVisitor):
             if hasattr(visitor, "visitShift_spec"):
                 return visitor.visitShift_spec(self)
             else:
                 return visitor.visitChildren(self)
 
     def shift_spec(self):
-
         localctx = udunits2Parser.Shift_specContext(
             self, self._ctx, self.state
         )
         self.enterRule(localctx, 2, self.RULE_shift_spec)
         self._la = 0  # Token type
         try:
             self.state = 46
@@ -558,15 +555,14 @@
         def accept(self, visitor: ParseTreeVisitor):
             if hasattr(visitor, "visitPower"):
                 return visitor.visitPower(self)
             else:
                 return visitor.visitChildren(self)
 
     def power(self):
-
         localctx = udunits2Parser.PowerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 6, self.RULE_power)
         try:
             self.state = 82
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input, 9, self._ctx)
             if la_ == 1:
@@ -642,15 +638,14 @@
         def accept(self, visitor: ParseTreeVisitor):
             if hasattr(visitor, "visitBasic_spec"):
                 return visitor.visitBasic_spec(self)
             else:
                 return visitor.visitChildren(self)
 
     def basic_spec(self):
-
         localctx = udunits2Parser.Basic_specContext(
             self, self._ctx, self.state
         )
         self.enterRule(localctx, 8, self.RULE_basic_spec)
         try:
             self.state = 90
             self._errHandler.sync(self)
@@ -711,15 +706,14 @@
         def accept(self, visitor: ParseTreeVisitor):
             if hasattr(visitor, "visitInteger"):
                 return visitor.visitInteger(self)
             else:
                 return visitor.visitChildren(self)
 
     def integer(self):
-
         localctx = udunits2Parser.IntegerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 10, self.RULE_integer)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
             self.state = 92
             _la = self._input.LA(1)
@@ -760,15 +754,14 @@
         def accept(self, visitor: ParseTreeVisitor):
             if hasattr(visitor, "visitNumber"):
                 return visitor.visitNumber(self)
             else:
                 return visitor.visitChildren(self)
 
     def number(self):
-
         localctx = udunits2Parser.NumberContext(self, self._ctx, self.state)
         self.enterRule(localctx, 12, self.RULE_number)
         try:
             self.state = 96
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [udunits2Parser.SIGNED_INT, udunits2Parser.INT]:
@@ -836,15 +829,14 @@
         def accept(self, visitor: ParseTreeVisitor):
             if hasattr(visitor, "visitTimestamp"):
                 return visitor.visitTimestamp(self)
             else:
                 return visitor.visitChildren(self)
 
     def timestamp(self):
-
         localctx = udunits2Parser.TimestampContext(self, self._ctx, self.state)
         self.enterRule(localctx, 14, self.RULE_timestamp)
         self._la = 0  # Token type
         try:
             self.state = 118
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input, 17, self._ctx)
@@ -971,15 +963,14 @@
         def accept(self, visitor: ParseTreeVisitor):
             if hasattr(visitor, "visitSigned_clock"):
                 return visitor.visitSigned_clock(self)
             else:
                 return visitor.visitChildren(self)
 
     def signed_clock(self):
-
         localctx = udunits2Parser.Signed_clockContext(
             self, self._ctx, self.state
         )
         self.enterRule(localctx, 16, self.RULE_signed_clock)
         try:
             self.state = 123
             self._errHandler.sync(self)
@@ -1032,15 +1023,14 @@
         def accept(self, visitor: ParseTreeVisitor):
             if hasattr(visitor, "visitTimezone_offset"):
                 return visitor.visitTimezone_offset(self)
             else:
                 return visitor.visitChildren(self)
 
     def timezone_offset(self):
-
         localctx = udunits2Parser.Timezone_offsetContext(
             self, self._ctx, self.state
         )
         self.enterRule(localctx, 18, self.RULE_timezone_offset)
         try:
             self.state = 127
             self._errHandler.sync(self)
```

### Comparing `cf-units-3.1.1/cf_units/_udunits2_parser/parser/udunits2ParserVisitor.py` & `cf-units-3.2.0/cf_units/_udunits2_parser/parser/udunits2ParserVisitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 else:
     from udunits2Parser import udunits2Parser
 
 # This class defines a complete generic visitor for a parse tree produced by udunits2Parser.
 
 
 class udunits2ParserVisitor(ParseTreeVisitor):
-
     # Visit a parse tree produced by udunits2Parser#unit_spec.
     def visitUnit_spec(self, ctx: udunits2Parser.Unit_specContext):
         return self.visitChildren(ctx)
 
     # Visit a parse tree produced by udunits2Parser#shift_spec.
     def visitShift_spec(self, ctx: udunits2Parser.Shift_specContext):
         return self.visitChildren(ctx)
```

### Comparing `cf-units-3.1.1/cf_units/_udunits2_parser/udunits2Lexer.g4.jinja` & `cf-units-3.2.0/cf_units/_udunits2_parser/udunits2Lexer.g4.jinja`

 * *Files identical despite different names*

### Comparing `cf-units-3.1.1/cf_units/_udunits2_parser/udunits2Parser.g4` & `cf-units-3.2.0/cf_units/_udunits2_parser/udunits2Parser.g4`

 * *Files identical despite different names*

### Comparing `cf-units-3.1.1/cf_units/config.py` & `cf-units-3.2.0/cf_units/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 
 
 import configparser
 import sys
 from pathlib import Path
 from tempfile import NamedTemporaryFile
```

### Comparing `cf-units-3.1.1/cf_units/tests/integration/parse/test_graph.py` & `cf-units-3.2.0/cf_units/tests/integration/parse/test_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 
 import cf_units._udunits2_parser.graph as g
 from cf_units._udunits2_parser import parse
 
 
 def test_Node_attributes():
     n = g.Node(a=1, kwarg="two", arbitrary_kwargs=3)
```

### Comparing `cf-units-3.1.1/cf_units/tests/integration/parse/test_parse.py` & `cf-units-3.2.0/cf_units/tests/integration/parse/test_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 
 import re
 
 import pytest
 
 import cf_units
 from cf_units._udunits2_parser import normalize
```

### Comparing `cf-units-3.1.1/cf_units/tests/integration/test__num2date_to_nearest_second.py` & `cf-units-3.2.0/cf_units/tests/integration/test__num2date_to_nearest_second.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """Test function :func:`cf_units._num2date_to_nearest_second`."""
 
 import datetime
 
 import cftime
 import numpy as np
 import pytest
```

### Comparing `cf-units-3.1.1/cf_units/tests/integration/test_date2num.py` & `cf-units-3.2.0/cf_units/tests/integration/test_date2num.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """Test function :func:`cf_units.date2num`."""
 
 import datetime
 
 import numpy as np
 import pytest
```

### Comparing `cf-units-3.1.1/cf_units/tests/integration/test_num2date.py` & `cf-units-3.2.0/cf_units/tests/integration/test_num2pydate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-"""Test function :func:`cf_units.num2date`."""
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
+"""Test function :func:`cf_units.num2pydate`."""
 
+import datetime
 
 import pytest
 
-from cf_units import num2date
+from cf_units import num2pydate
 
 
 class Test:
-    def test_num2date_wrong_calendar(self):
+    def test_num2pydate_simple(self):
+        result = num2pydate(1, "days since 1970-01-01", calendar="standard")
+        expected = datetime.datetime(1970, 1, 2)
+        assert result == expected
+        assert isinstance(result, datetime.datetime)
+
+    def test_num2pydate_wrong_calendar(self):
         with pytest.raises(
             ValueError, match="illegal calendar or reference date"
         ):
-            num2date(
-                1,
-                "days since 1970-01-01",
-                calendar="360_day",
-                only_use_cftime_datetimes=False,
-                only_use_python_datetimes=True,
-            )
+            num2pydate(1, "days since 1970-01-01", calendar="360_day")
```

### Comparing `cf-units-3.1.1/cf_units/tests/test_coding_standards.py` & `cf-units-3.2.0/cf_units/tests/test_coding_standards.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 
 import os
 import subprocess
 from datetime import datetime
 from fnmatch import fnmatch
 from glob import glob
 
 import pytest
 
 import cf_units
 
 LICENSE_TEMPLATE = """# Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details."""
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details."""
 
 
 # Guess cf_units repo directory of cf_units - realpath is used to mitigate
 # against Python finding the cf_units package via a symlink.
 DIR = os.path.realpath(os.path.dirname(cf_units.__file__))
 REPO_DIR = os.path.dirname(DIR)
 DOCS_DIR = os.path.join(REPO_DIR, "doc")
```

### Comparing `cf-units-3.1.1/cf_units/tests/test_tex.py` & `cf-units-3.2.0/cf_units/tests/test_tex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 
 from cf_units.tex import tex
 
 
 def test_basic():
     u = "kg kg-1"
     assert tex(u) == r"{kg}\cdot{{kg}^{-1}}"
```

### Comparing `cf-units-3.1.1/cf_units/tests/test_unit.py` & `cf-units-3.2.0/cf_units/tests/test_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """
 Test Unit the wrapper class for Unidata udunits2.
 
 """
 
 import copy
 import datetime as datetime
```

### Comparing `cf-units-3.1.1/cf_units/tests/unit/test__discard_microsecond.py` & `cf-units-3.2.0/cf_units/tests/unit/test__discard_microsecond.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """Unit tests for the `cf_units._discard_microsecond` function."""
 
 import datetime
 
 import cftime
 import numpy as np
 import numpy.ma as ma
```

### Comparing `cf-units-3.1.1/cf_units/tests/unit/test__udunits2.py` & `cf-units-3.2.0/cf_units/tests/unit/test__udunits2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """Unit tests for the `cf_units._udunits2` module.
 
 In most cases, we don't test the correctness
 of the operations, only that they return valid objects or raise an
 exception where expected."""
 
 import errno
```

### Comparing `cf-units-3.1.1/cf_units/tests/unit/unit/test_Unit.py` & `cf-units-3.2.0/cf_units/tests/unit/unit/test_Unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """Unit tests for the `cf_units.Unit` class."""
 
 
 import numpy as np
 import pytest
 
 import cf_units
@@ -75,38 +74,38 @@
             u.change_calendar("standard")
 
 
 class Test_convert__calendar:
     class MyStr(str):
         pass
 
-    def test_gregorian_calendar_conversion_setup(self):
+    def gregorian_calendar_conversion_setup(self):
         # Reproduces a situation where a unit's gregorian calendar would not
         # match (using the `is` operator) to the literal string 'gregorian',
         # causing an `is not` test to return a false negative.
         cal_str = cf_units.CALENDAR_GREGORIAN
         calendar = self.MyStr(cal_str)
         assert calendar is not cal_str
         u1 = Unit("hours since 1970-01-01 00:00:00", calendar=calendar)
         u2 = Unit("hours since 1969-11-30 00:00:00", calendar=calendar)
         u1point = np.array([8.0], dtype=np.float32)
         expected = np.array([776.0], dtype=np.float32)
         result = u1.convert(u1point, u2)
         return expected, result
 
     def test_gregorian_calendar_conversion_array(self):
-        expected, result = self.test_gregorian_calendar_conversion_setup()
+        expected, result = self.gregorian_calendar_conversion_setup()
         np.testing.assert_array_equal(expected, result)
 
     def test_gregorian_calendar_conversion_dtype(self):
-        expected, result = self.test_gregorian_calendar_conversion_setup()
+        expected, result = self.gregorian_calendar_conversion_setup()
         assert expected.dtype == result.dtype
 
     def test_gregorian_calendar_conversion_shape(self):
-        expected, result = self.test_gregorian_calendar_conversion_setup()
+        expected, result = self.gregorian_calendar_conversion_setup()
         assert expected.shape == result.shape
 
     def test_non_gregorian_calendar_conversion_dtype(self):
         for start_dtype, exp_convert in (
             (np.float32, True),
             (np.float64, True),
             (np.int32, False),
```

### Comparing `cf-units-3.1.1/cf_units/tests/unit/unit/test_as_unit.py` & `cf-units-3.2.0/cf_units/tests/unit/unit/test_as_unit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """Unit tests for the `cf_units.as_unit` function."""
 
 import copy
 
 from cf_units import Unit, as_unit
```

### Comparing `cf-units-3.1.1/cf_units/tex.py` & `cf-units-3.2.0/cf_units/tex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 
 import cf_units._udunits2_parser.graph as graph  # noqa: E402
 from cf_units._udunits2_parser import parse as _parse  # noqa: E402
 
 
 class TeXVisitor(graph.Visitor):
     def _format(self, fmt, lhs, rhs):
```

### Comparing `cf-units-3.1.1/cf_units/util.py` & `cf-units-3.2.0/cf_units/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """
 Miscellaneous utility functions.
 
 """
 
 import abc
+import warnings
 from collections.abc import Hashable
 
 
 def approx_equal(a, b, max_absolute_error=1e-10, max_relative_error=1e-10):
     """
     Returns whether two numbers are almost equal, allowing for the
     finite precision of floating point numbers.
 
+    .. deprecated:: 3.2.0
+       Instead please use :func:`math.isclose`.
+
     """
+    msg = (
+        "cf_units.util.approx_equal has been deprecated and will be removed.  "
+        "Please use math.isclose instead."
+    )
+    warnings.warn(msg, DeprecationWarning, stacklevel=2)
+
     # Deal with numbers close to zero
     if abs(a - b) < max_absolute_error:
         return True
     # Ensure we get consistent results if "a" and "b" are supplied in the
     # opposite order.
     max_ab = max([a, b], key=abs)
     relative_error = abs(a - b) / max_ab
```

### Comparing `cf-units-3.1.1/cf_units.egg-info/PKG-INFO` & `cf-units-3.2.0/cf_units.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: cf-units
-Version: 3.1.1
+Version: 3.2.0
 Summary: Units of measure as required by the Climate and Forecast (CF) metadata conventions
 Home-page: https://github.com/SciTools/cf-units
 Download-URL: https://github.com/SciTools/cf-units
 Author: SciTools Developers
-License: LGPL-3.0-or-later
+License: BSD
 Project-URL: Code, https://github.com/SciTools/cf-units
 Project-URL: Discussions, https://github.com/SciTools/cf-units/discussions
 Project-URL: Issues, https://github.com/SciTools/cf-units/issues
 Keywords: units,cf,netcdf,science,oceanography,meteorology,climate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: all
-License-File: COPYING
+License-File: LICENSE
 
 # [cf-units](https://cf-units.readthedocs.io/en/latest/)
 
 #### Units of measure as defined by the Climate and Forecast (CF) Metadata Conventions.
 
 [comment]: # (https://shields.io/ is a good source of these)
 [![ci-tests](https://github.com/SciTools/cf-units/actions/workflows/ci-tests.yml/badge.svg?branch=main)](https://github.com/SciTools/cf-units/actions/workflows/ci-tests.yml)
@@ -43,15 +43,15 @@
 [![Latest version](https://img.shields.io/github/tag/SciTools/cf-units)](https://github.com/SciTools/cf-units/releases)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3723086.svg)](https://doi.org/10.5281/zenodo.3723086)
 \
 [![Black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)
 [![Flake8](https://img.shields.io/badge/lint-flake8-lightgrey)](https://github.com/PyCQA/flake8)
 [![isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 \
-[![Licence](https://img.shields.io/github/license/SciTools/cf-units)](COPYING)
+[![Licence](https://img.shields.io/badge/license-BSD--3-orange)](LICENSE)
 [![Contributors](https://img.shields.io/github/contributors/SciTools/cf-units)](https://github.com/SciTools/cf-units/graphs/contributors)
 [![Commits since last release](https://img.shields.io/github/commits-since/SciTools/cf-units/latest.svg)](https://github.com/SciTools/cf-units/commits/main)
 
 ## Table of Contents
 
 [comment]: # (NOTE: toc auto-generated with
   https://github.com/jonschlinkert/markdown-toc
@@ -100,13 +100,13 @@
 A full list of code contributors ("cf-units contributors") can be found at
 https://github.com/SciTools/cf-units/graphs/contributors.
 
 Code is just one of many ways of positively contributing to cf-units, please
 see our [contributing guide](.github/CONTRIBUTING.md) for more details on how
 you can get involved.
 
-cf-units is released under a LGPL license with a shared copyright model.
-See [COPYING](COPYING) and [COPYING.LESSER](COPYING.LESSER) for full terms.
+cf-units is released under a BSD-3 license. See [LICENSE](LICENSE) for full
+terms.
 
 The [Met Office](https://metoffice.gov.uk) has made a significant
 contribution to the development, maintenance and support of this library.
 All Met Office contributions are copyright on behalf of the British Crown.
```

### Comparing `cf-units-3.1.1/cf_units.egg-info/SOURCES.txt` & `cf-units-3.2.0/cf_units.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .git_archival.txt
 .gitattributes
 .pre-commit-config.yaml
 .readthedocs.yml
 CHANGES
-COPYING
-COPYING.LESSER
 INSTALL
+LICENSE
 MANIFEST.in
 README.md
 codecov.yml
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
```

### Comparing `cf-units-3.1.1/docs/Makefile` & `cf-units-3.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cf-units-3.1.1/docs/make.bat` & `cf-units-3.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cf-units-3.1.1/docs/source/conf.py` & `cf-units-3.2.0/docs/source/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright cf-units contributors
 #
-# This file is part of cf-units and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of cf-units and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 
 from importlib import metadata
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
```

### Comparing `cf-units-3.1.1/docs/source/index.rst` & `cf-units-3.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cf-units-3.1.1/pyproject.toml` & `cf-units-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cf-units-3.1.1/requirements/locks/py310-lock-linux-64.txt` & `cf-units-3.2.0/requirements/locks/py310-lock-linux-64.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,99 +1,97 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: ea1e2116397e649a23642472354057daf60092dd21ab77cd028b41a1497c68f3
+# input_hash: aa71a0800d9edd1825a476d7d74f2eed93c8d5de1c9f86d9294d48e641ce0058
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
-https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2022.6.15-ha878542_0.tar.bz2#c320890f77fd1d617fa876e0982002c2
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.36.1-hea4e1c9_2.tar.bz2#bd4f2e711b39af170e7ff15163fe87ee
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-12.1.0-hdcd56e2_16.tar.bz2#b02605b875559ff99f04351fd5040760
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.1.0-ha89aaad_16.tar.bz2#6f5ba041a41eb102a1027d9e68731be7
-https://conda.anaconda.org/conda-forge/noarch/tzdata-2022a-h191b570_0.tar.bz2#84be5301069417a2221187d2f435e0f7
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-12.1.0-h69a702a_16.tar.bz2#6bf15e29a20f614b18ae89368260d0a2
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.1.0-h8d9b700_16.tar.bz2#f013cf7749536ce43d82afbffdf499ab
+https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2022.9.24-ha878542_0.tar.bz2#41e4e87062433e283696cf384f952ef6
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.39-hc81fddc_0.tar.bz2#c2719e2faa7bd7076d3a4b52271e5622
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-12.2.0-h337968e_19.tar.bz2#164b4b1acaedc47ee7e658ae6b308ca3
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.2.0-h46fd767_19.tar.bz2#1030b1f38c129f2634eae026f704fe60
+https://conda.anaconda.org/conda-forge/noarch/tzdata-2022f-h191b570_0.tar.bz2#e366350e2343a798e29833286abe2560
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-12.2.0-h69a702a_19.tar.bz2#cd7a806282c16e1f2d39a7e80d3a3e0d
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.2.0-h65d4601_19.tar.bz2#cedcee7c064c01c403f962c9e8d3c373
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.1.0-h8d9b700_16.tar.bz2#4f05bc9844f7c101e6e147dab3c88d5c
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.2.0-h65d4601_19.tar.bz2#e4c94f80aef025c17ab0828cd85ef535
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
-https://conda.anaconda.org/conda-forge/linux-64/expat-2.4.8-h27087fc_0.tar.bz2#e1b07832504eeba765d648389cc387a9
+https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-h27087fc_0.tar.bz2#c4fbad8d4bddeb3c085f18cbf97fbfad
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
-https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.20-pthreads_h78a6416_0.tar.bz2#9b6d0781953c9e353faee494336cc229
+https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.21-pthreads_h78a6416_3.tar.bz2#8c5963a49b6035c40646a763293fbb35
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.32.1-h7f98852_1000.tar.bz2#772d69f030955d9646d3d0eaf21d859d
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.12-h166bdaf_1.tar.bz2#58eaff4f91891978af3625e7bbf958af
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
 https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2#4acfc691e64342b9dae57cf2adc63238
-https://conda.anaconda.org/conda-forge/linux-64/openssl-1.1.1q-h166bdaf_0.tar.bz2#07acc367c7fc8b716770cd5b36d31717
-https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.5-h516909a_1.tar.bz2#33f601066901f3e1a85af3522a8113f9
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.0.7-h166bdaf_0.tar.bz2#d1ad1824c71e67dea42f07e06cd177dc
+https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
-https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-15_linux64_openblas.tar.bz2#04eb983975a1be3e57d6d667414cd774
+https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-16_linux64_openblas.tar.bz2#d9b7a8639171f6c6fa0a983edabcfe2b
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.40.0-h753d276_0.tar.bz2#2e5f9a37d487e1019fd4d8113adb2f9f
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.1.2-h0f457ee_0.tar.bz2#db2ebbe2943aae81ed051a6a9af8e0fa
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/udunits2-2.2.28-hc3e0081_0.tar.bz2#d4c341e0379c31e9e781d4f204726867
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.12-h166bdaf_1.tar.bz2#e4b67f2b4096807cd7d836227c026a43
-https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-15_linux64_openblas.tar.bz2#f45968428e445fd0c6472b561145812a
-https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-15_linux64_openblas.tar.bz2#b7078220384b8bf8db1a45e66412ac4f
-https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.39.0-h4ff8645_0.tar.bz2#ead30581ba8cfd52d69632868b844d4a
-https://conda.anaconda.org/conda-forge/linux-64/python-3.10.5-h582c2e5_0_cpython.tar.bz2#ccbed83043b9b7b5693164591317f327
+https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-16_linux64_openblas.tar.bz2#20bae26d0a1db73f758fc3754cab4719
+https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-16_linux64_openblas.tar.bz2#955d993f41f9354bf753d29864ea20ad
+https://conda.anaconda.org/conda-forge/linux-64/python-3.10.6-ha86cf86_0_cpython.tar.bz2#98d77e6496f7516d6b3c508f71c102fc
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.12-py_0.tar.bz2#2489a97287f90176ecdc3ca982b4b0a0
-https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
+https://conda.anaconda.org/conda-forge/noarch/attrs-22.1.0-pyh71513ae_1.tar.bz2#6d3ccbc56256204925bfa8378722792f
+https://conda.anaconda.org/conda-forge/noarch/certifi-2022.9.24-pyhd8ed1ab_0.tar.bz2#f66309b099374af91369e67e84af397d
 https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2#ebb5f5f7dc4f1a3780ef7ea7738db08c
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.0-pyhd8ed1ab_0.tar.bz2#abc0453b6e7bfbb87d275d58e333fc98
-https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.5-pyhd8ed1ab_0.tar.bz2#c267da48ce208905d7d976d49dfd9433
-https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.4-pyhd8ed1ab_0.tar.bz2#7b50d840543d9cdae100e91582c33035
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.7.1-pyhd8ed1ab_0.tar.bz2#7556872687250e0ea038eb503da3c44b
-https://conda.anaconda.org/conda-forge/noarch/idna-3.3-pyhd8ed1ab_0.tar.bz2#40b50b8b030f5f2f22085c062ed013dd
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.1-pyhd8ed1ab_0.tar.bz2#c1d5b294fbf9a795dec349a6f4d8be8e
+https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
+https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2#b65b4d50dbd2d50fa0aeac367ec9eed7
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.0.4-pyhd8ed1ab_0.tar.bz2#e0734d1f12de77f9daca98bda3428733
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.8.0-pyhd8ed1ab_0.tar.bz2#10f0218dbd493ab2e5dc6759ddea4526
+https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-1.1.1-pyh9f0ad1d_0.tar.bz2#39161f81cc5e5ca45b8226fbb06c6905
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.1-pyhd8ed1ab_0.tar.bz2#d5df87964a39f67c46a5448f4e78d9b6
-https://conda.anaconda.org/conda-forge/noarch/py-1.11.0-pyh6c4a22f_0.tar.bz2#b4613d7e7a493916d867842a6a148054
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.2-pyhd8ed1ab_1.tar.bz2#2fb3f88922e7aec26ba652fcdfe13950
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.10-2_cp310.tar.bz2#9e7160cd0d865e98f6803f1fe15c8b61
-https://conda.anaconda.org/conda-forge/noarch/pytz-2022.1-pyhd8ed1ab_0.tar.bz2#b87d66d6d3991d988fb31510c95a9267
-https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+https://conda.anaconda.org/conda-forge/noarch/pytz-2022.6-pyhd8ed1ab_0.tar.bz2#b1f26ad83328e486910ef7f6e81dc061
+https://conda.anaconda.org/conda-forge/noarch/setuptools-65.5.1-pyhd8ed1ab_0.tar.bz2#cfb8dc4d9d285ca5fb1177b9dd450e33
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.2-py_0.tar.bz2#20b2eaeaeea4ef9a9a0d99770620fd09
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.0-pyhd8ed1ab_0.tar.bz2#77dad82eb9c8c1525ff7953e0756d708
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.3.0-pyha770c72_0.tar.bz2#a9d85960bc62d53cc4ea0d1d27f73c98
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.37.1-pyhd8ed1ab_0.tar.bz2#1ca02aaf78d9c70d9a81a3bed5752022
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.8.0-pyhd8ed1ab_0.tar.bz2#050b94cf4a8c760656e51d2d44e4632c
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.4.0-pyha770c72_0.tar.bz2#2d93b130d148d7fc77e583677792fc6a
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.38.4-pyhd8ed1ab_0.tar.bz2#c829cfb8cb826acb9de0ac1a2df0a940
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.10.0-pyhd8ed1ab_0.tar.bz2#cd4eb48ebde7de61f92252979aab515c
 https://conda.anaconda.org/conda-forge/linux-64/antlr-python-runtime-4.7.2-py310hff52083_1003.tar.bz2#8324f8fff866055d4b32eb25e091fe31
-https://conda.anaconda.org/conda-forge/noarch/babel-2.10.3-pyhd8ed1ab_0.tar.bz2#72f1c6d03109d7a70087bc1d029a8eda
-https://conda.anaconda.org/conda-forge/linux-64/certifi-2022.6.15-py310hff52083_0.tar.bz2#a5087d46181f812a662fbe20352961ee
-https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py310h255011f_0.tar.bz2#3e4b55b02998782f8ca9ceaaa4f5ada9
-https://conda.anaconda.org/conda-forge/linux-64/coverage-6.4.1-py310h5764c6d_0.tar.bz2#0b9e281c6be0c1a10d943582c190cde3
-https://conda.anaconda.org/conda-forge/linux-64/cython-0.29.30-py310hd8f1fbe_0.tar.bz2#1b9afbc3fabae40f4664d5390681da0a
-https://conda.anaconda.org/conda-forge/linux-64/docutils-0.18.1-py310hff52083_1.tar.bz2#6405f87c427cdbc25b6b6a21bd6bfc2a
-https://conda.anaconda.org/conda-forge/linux-64/importlib-metadata-4.11.4-py310hff52083_0.tar.bz2#8ea386e64531f1ecf4a5765181579e7e
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.1-py310h5764c6d_1.tar.bz2#ec5a727504409ad1380fc2a84f83d002
-https://conda.anaconda.org/conda-forge/linux-64/numpy-1.23.1-py310h53a5b5f_0.tar.bz2#9b86a46d908354fe7f91da24f5ea3f36
+https://conda.anaconda.org/conda-forge/noarch/babel-2.11.0-pyhd8ed1ab_0.tar.bz2#2ea70fde8d581ba9425a761609eed6ba
+https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py310h255011f_2.tar.bz2#6bb8063dd08f9724c18744b0e040cfe2
+https://conda.anaconda.org/conda-forge/linux-64/coverage-6.5.0-py310h5764c6d_1.tar.bz2#feb57771b1d5179cd2fb1a06fed17326
+https://conda.anaconda.org/conda-forge/linux-64/cython-0.29.32-py310hd8f1fbe_1.tar.bz2#20e882881d936dc1ff7ac37fe1bd92e1
+https://conda.anaconda.org/conda-forge/linux-64/docutils-0.19-py310hff52083_1.tar.bz2#21b8fa2179290505e607f5ccd65b01b0
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-5.0.0-pyha770c72_1.tar.bz2#ec069c4db6a0ad84107bac5da62819d2
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.1-py310h5764c6d_2.tar.bz2#2d7028ea2a77f909931e1a173d952261
+https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
+https://conda.anaconda.org/conda-forge/linux-64/numpy-1.23.4-py310h53a5b5f_1.tar.bz2#0b7d4c8253f7191030adf34e2768c412
 https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2#71f1ab2de48613876becddd496371c85
-https://conda.anaconda.org/conda-forge/linux-64/pluggy-1.0.0-py310hff52083_3.tar.bz2#97f9a22577338f91a94dfac5c1a65a50
-https://conda.anaconda.org/conda-forge/linux-64/pysocks-1.7.1-py310hff52083_5.tar.bz2#378f2260e871f3ea46c6fa58d9f05277
-https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py310h5764c6d_4.tar.bz2#505dcf6be997e732d7a33831950dc3cf
-https://conda.anaconda.org/conda-forge/linux-64/setuptools-63.1.0-py310hff52083_0.tar.bz2#4957e3a46761a6c7a3a05233c39ed904
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.3.0-hd8ed1ab_0.tar.bz2#f3e98e944832fb271a0dbda7b7771dc6
-https://conda.anaconda.org/conda-forge/linux-64/virtualenv-20.15.1-py310hff52083_0.tar.bz2#7f6c48710ee99edfa3dfa0b54fa6f020
-https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py310h5764c6d_1004.tar.bz2#6499bb11b7feffb63b26847fc9181319
-https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.1-py310hde88566_0.tar.bz2#1f84cf065287d73aa0233d432d3a1ba9
-https://conda.anaconda.org/conda-forge/linux-64/cryptography-37.0.4-py310h597c629_0.tar.bz2#f285746449d16d92884f4ce0cfe26679
+https://conda.anaconda.org/conda-forge/noarch/pip-22.3.1-pyhd8ed1ab_0.tar.bz2#da66f2851b9836d3a7c5190082a45f7d
+https://conda.anaconda.org/conda-forge/noarch/pygments-2.13.0-pyhd8ed1ab_0.tar.bz2#9f478e8eedd301008b5f395bad0caaed
+https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py310h5764c6d_5.tar.bz2#9e68d2ff6d98737c855b65f48dd3c597
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.4.0-hd8ed1ab_0.tar.bz2#be969210b61b897775a0de63cd9e9026
+https://conda.anaconda.org/conda-forge/linux-64/virtualenv-20.16.7-py310hff52083_0.tar.bz2#02600c102a32274e20fc0604ef35af3c
+https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py310h5764c6d_1005.tar.bz2#87669c3468dff637bbd0363bc0f895cf
+https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.2-py310hde88566_1.tar.bz2#94ce7a76b0c912279f6958e0b6b21d2b
+https://conda.anaconda.org/conda-forge/linux-64/cryptography-38.0.3-py310h600f1e7_0.tar.bz2#6d5e57c85bf49ab9ebeb74241f5fdc41
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
-https://conda.anaconda.org/conda-forge/noarch/pip-22.1.2-pyhd8ed1ab_0.tar.bz2#d29185c662a424f8bea1103270b85c96
-https://conda.anaconda.org/conda-forge/noarch/pygments-2.12.0-pyhd8ed1ab_0.tar.bz2#cb27e2ded147e5bcc7eafc1c6d343cb3
-https://conda.anaconda.org/conda-forge/linux-64/pytest-7.1.2-py310hff52083_0.tar.bz2#5d44c6ab93d445b6c433914753390e86
-https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.4-pyhd8ed1ab_0.tar.bz2#dff6862ca0b54bbeab8ddf657d032920
-https://conda.anaconda.org/conda-forge/linux-64/ukkonen-1.0.1-py310hbf28c38_2.tar.bz2#46784478afa27e33b9d5f017c4deb49d
-https://conda.anaconda.org/conda-forge/noarch/identify-2.5.1-pyhd8ed1ab_0.tar.bz2#6f41e3056fcd3061fbc2b49b3309fe0c
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.0.0-pyhd8ed1ab_0.tar.bz2#1d7e241dfaf5475e893d4b824bb71b44
-https://conda.anaconda.org/conda-forge/noarch/pytest-cov-3.0.0-pyhd8ed1ab_0.tar.bz2#0f7cac11bb696b62d378bde725bfc3eb
-https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.4-hd8ed1ab_0.tar.bz2#b068a47ce183af12a53c6b0d84f96085
-https://conda.anaconda.org/conda-forge/linux-64/pre-commit-2.19.0-py310hff52083_0.tar.bz2#bcf63938923fd8c16c684a4e7157b062
-https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.10-pyhd8ed1ab_0.tar.bz2#14f22c5b9cfd0d93c2806faaa3fe6dec
-https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_0.tar.bz2#70d6e72856de9551f83ae0f2de689a7a
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.2.0-pyhd8ed1ab_2.tar.bz2#ac82c7aebc282e6ac0450fca012ca78c
+https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.5-pyhd8ed1ab_1.tar.bz2#07037fe2931871ed69b2b3d2acd5fdc6
+https://conda.anaconda.org/conda-forge/linux-64/ukkonen-1.0.1-py310hbf28c38_3.tar.bz2#703ff1ac7d1b27fb5944b8052b5d1edb
+https://conda.anaconda.org/conda-forge/noarch/identify-2.5.8-pyhd8ed1ab_0.tar.bz2#8001c46448f385fa43bc4221893704d2
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.1.0-pyhd8ed1ab_0.tar.bz2#fbfa0a180d48c800f922a10a114a8632
+https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.0.0-pyhd8ed1ab_0.tar.bz2#c9e3f8bfdb9bfc34aa1836a6ed4b25d7
+https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.5-hd8ed1ab_1.tar.bz2#6b7cb927a5c505b16b4b4241825e068c
+https://conda.anaconda.org/conda-forge/linux-64/pre-commit-2.20.0-py310hff52083_1.tar.bz2#8c151d720f9fe3b9962efe71fc10b07b
+https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.11-pyhd8ed1ab_0.tar.bz2#0738978569b10669bdef41c671252dd1
+https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_1.tar.bz2#089382ee0e2dc2eae33a04cc3c2bddb0
 https://conda.anaconda.org/conda-forge/noarch/codecov-2.1.11-pyhd3deb0d_0.tar.bz2#9c661c2c14b4667827218402e6624ad5
-https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.2-pyh6c4a22f_0.tar.bz2#d4eaa1f50733a377480ce1d5aac556c7
+https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
```

### Comparing `cf-units-3.1.1/requirements/locks/py310-lock-osx-64.txt` & `cf-units-3.2.0/requirements/locks/py39-lock-osx-64.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,93 +1,92 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: f9da774a5833fd20f50a543bc4edfd743c44b82df7f752461e09eaecb2e93fe0
+# input_hash: 51497796e44400ab6b5691f0888abbfb9adb4c7b304b81b29e4d0352284793a1
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
-https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2022.6.15-h033912b_0.tar.bz2#d16674f96e47de0d08af3fc97803134e
-https://conda.anaconda.org/conda-forge/osx-64/libcxx-14.0.6-hce7ea42_0.tar.bz2#ac504a8074ae8add8b837a93d7bc33ca
+https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2022.9.24-h033912b_0.tar.bz2#67b268c32433047914482def1ce215c2
+https://conda.anaconda.org/conda-forge/osx-64/libcxx-14.0.6-hccf4f1f_0.tar.bz2#208a6a874b073277374de48a782f6b10
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
-https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.12-hfe4f2af_1.tar.bz2#f7d43cae08c86f73be8cbda4f8e43373
-https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-14.0.4-ha654fa7_0.tar.bz2#5d5ab9ab83ce21422be84ecfd3142201
+https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-hfd90126_4.tar.bz2#35eb3fce8d51ed3c1fd4122bad48250b
+https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-15.0.5-h61d9ccf_0.tar.bz2#81ceb8ca1476f31cbaacf7ac845b6fff
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.3-h96cf925_1.tar.bz2#76217ebfbb163ff2770a261f955a5861
-https://conda.anaconda.org/conda-forge/noarch/tzdata-2022a-h191b570_0.tar.bz2#84be5301069417a2221187d2f435e0f7
-https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.5-haf1e3a3_1.tar.bz2#41116deb499e9bc58048c297d6403ce6
+https://conda.anaconda.org/conda-forge/noarch/tzdata-2022f-h191b570_0.tar.bz2#e366350e2343a798e29833286abe2560
+https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
-https://conda.anaconda.org/conda-forge/osx-64/expat-2.4.8-h96cf925_0.tar.bz2#529d357c143fb98b9af77d687f82a3e0
-https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-9.3.0-h6c81a4c_23.tar.bz2#a6956ceb628b14594613cefee5127a7a
-https://conda.anaconda.org/conda-forge/osx-64/openssl-1.1.1q-hfe4f2af_0.tar.bz2#ce822517fb00e8bafea6fe77d07f20bd
+https://conda.anaconda.org/conda-forge/osx-64/expat-2.5.0-hf0c8a7f_0.tar.bz2#7648a729fc8b7272596e90b0ab0a3e98
+https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-11.3.0-h082f757_26.tar.bz2#11835360754e5caca43cfaa3a81dfca5
+https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.40.0-ha978bb4_0.tar.bz2#ceb13b6726534b96e3b4e3dda91e9050
+https://conda.anaconda.org/conda-forge/osx-64/openssl-3.0.7-hfd90126_0.tar.bz2#78d8266753a5db378ef0f9302be9990f
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.1.2-h3899abd_0.tar.bz2#89fa404901fa8fb7d4f4e07083b8d635
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
-https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.12-hfe4f2af_1.tar.bz2#12fdf8350ef315e7ad48693346067405
-https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-9_3_0_h6c81a4c_23.tar.bz2#60f48cef2d50674e0428c5579b6c3f66
-https://conda.anaconda.org/conda-forge/osx-64/sqlite-3.39.0-hd9f0692_0.tar.bz2#956223b8f1d808bab8ca9d8fb08778ec
+https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-9_5_0_h97931a8_26.tar.bz2#ac9c1a84323edab6c3ff9d3e586ab3cc
+https://conda.anaconda.org/conda-forge/osx-64/sqlite-3.40.0-h9ae0607_0.tar.bz2#b66b0b11f1b901f3c2bce9406bedfd40
 https://conda.anaconda.org/conda-forge/osx-64/udunits2-2.2.28-h06ef574_0.tar.bz2#74131a7d532fbff820580d4494118245
-https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.20-openmp_hb3cd9ec_0.tar.bz2#d862e4a5c6e7bf0bc9d66a38f5c73142
-https://conda.anaconda.org/conda-forge/osx-64/python-3.10.5-hdaaf3db_0_cpython.tar.bz2#2c27a532578a3e3b1574e0a50d9b36b9
+https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.21-openmp_h429af6e_3.tar.bz2#968c46aa7f4032c3f3873f3452ed4c34
+https://conda.anaconda.org/conda-forge/osx-64/python-3.9.13-hf8d34f4_0_cpython.tar.bz2#c3c4e87be5a78529972f2fa99c9e9938
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.12-py_0.tar.bz2#2489a97287f90176ecdc3ca982b4b0a0
-https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
+https://conda.anaconda.org/conda-forge/noarch/attrs-22.1.0-pyh71513ae_1.tar.bz2#6d3ccbc56256204925bfa8378722792f
+https://conda.anaconda.org/conda-forge/noarch/certifi-2022.9.24-pyhd8ed1ab_0.tar.bz2#f66309b099374af91369e67e84af397d
 https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2#ebb5f5f7dc4f1a3780ef7ea7738db08c
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.0-pyhd8ed1ab_0.tar.bz2#abc0453b6e7bfbb87d275d58e333fc98
-https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.5-pyhd8ed1ab_0.tar.bz2#c267da48ce208905d7d976d49dfd9433
-https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.4-pyhd8ed1ab_0.tar.bz2#7b50d840543d9cdae100e91582c33035
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.7.1-pyhd8ed1ab_0.tar.bz2#7556872687250e0ea038eb503da3c44b
-https://conda.anaconda.org/conda-forge/noarch/idna-3.3-pyhd8ed1ab_0.tar.bz2#40b50b8b030f5f2f22085c062ed013dd
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.1-pyhd8ed1ab_0.tar.bz2#c1d5b294fbf9a795dec349a6f4d8be8e
+https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
+https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2#b65b4d50dbd2d50fa0aeac367ec9eed7
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.0.4-pyhd8ed1ab_0.tar.bz2#e0734d1f12de77f9daca98bda3428733
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.8.0-pyhd8ed1ab_0.tar.bz2#10f0218dbd493ab2e5dc6759ddea4526
+https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-1.1.1-pyh9f0ad1d_0.tar.bz2#39161f81cc5e5ca45b8226fbb06c6905
-https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-15_osx64_openblas.tar.bz2#48c26d27a96c71cfae2621311aa06215
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.1-pyhd8ed1ab_0.tar.bz2#d5df87964a39f67c46a5448f4e78d9b6
-https://conda.anaconda.org/conda-forge/noarch/py-1.11.0-pyh6c4a22f_0.tar.bz2#b4613d7e7a493916d867842a6a148054
+https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-16_osx64_openblas.tar.bz2#644d63e9379867490b67bace400b2a0f
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.2-pyhd8ed1ab_1.tar.bz2#2fb3f88922e7aec26ba652fcdfe13950
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
-https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.10-2_cp310.tar.bz2#502ca4a8b43b424316f380d864832877
-https://conda.anaconda.org/conda-forge/noarch/pytz-2022.1-pyhd8ed1ab_0.tar.bz2#b87d66d6d3991d988fb31510c95a9267
-https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
+https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.9-2_cp39.tar.bz2#262f557ee8ca777fe2190956038024cd
+https://conda.anaconda.org/conda-forge/noarch/pytz-2022.6-pyhd8ed1ab_0.tar.bz2#b1f26ad83328e486910ef7f6e81dc061
+https://conda.anaconda.org/conda-forge/noarch/setuptools-65.5.1-pyhd8ed1ab_0.tar.bz2#cfb8dc4d9d285ca5fb1177b9dd450e33
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.2-py_0.tar.bz2#20b2eaeaeea4ef9a9a0d99770620fd09
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.0-pyhd8ed1ab_0.tar.bz2#77dad82eb9c8c1525ff7953e0756d708
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.3.0-pyha770c72_0.tar.bz2#a9d85960bc62d53cc4ea0d1d27f73c98
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.37.1-pyhd8ed1ab_0.tar.bz2#1ca02aaf78d9c70d9a81a3bed5752022
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.8.0-pyhd8ed1ab_0.tar.bz2#050b94cf4a8c760656e51d2d44e4632c
-https://conda.anaconda.org/conda-forge/osx-64/antlr-python-runtime-4.7.2-py310h2ec42d9_1003.tar.bz2#647c94b9631bbeb2bea8557a81600980
-https://conda.anaconda.org/conda-forge/noarch/babel-2.10.3-pyhd8ed1ab_0.tar.bz2#72f1c6d03109d7a70087bc1d029a8eda
-https://conda.anaconda.org/conda-forge/osx-64/certifi-2022.6.15-py310h2ec42d9_0.tar.bz2#7f60b1d9d5844975ca9794ce9bde7999
-https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py310h96bbf6e_0.tar.bz2#7247d0e5dc3dc1adb94de8353478a015
-https://conda.anaconda.org/conda-forge/osx-64/coverage-6.4.1-py310h6c45266_0.tar.bz2#9e8853e475bfb18e4414af9ee09e0ae0
-https://conda.anaconda.org/conda-forge/osx-64/cython-0.29.30-py310hd4537e4_0.tar.bz2#1dbaaf42d2bb8289b3b03f4d20a189ba
-https://conda.anaconda.org/conda-forge/osx-64/docutils-0.18.1-py310h2ec42d9_1.tar.bz2#f95000f735a9dbba847e6d03e9ce71ad
-https://conda.anaconda.org/conda-forge/osx-64/importlib-metadata-4.11.4-py310h2ec42d9_0.tar.bz2#f67654246da9adc1ea5f37c160758619
-https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-15_osx64_openblas.tar.bz2#2d26f8ba1e89bcc2704ac7a38d4cc74c
-https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-15_osx64_openblas.tar.bz2#8679c41f1fcb5b54aaecce18ec3e1875
-https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.1-py310h1961e1f_1.tar.bz2#48e4c1949b302e2d16d29df8788adef7
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.4.0-pyha770c72_0.tar.bz2#2d93b130d148d7fc77e583677792fc6a
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.38.4-pyhd8ed1ab_0.tar.bz2#c829cfb8cb826acb9de0ac1a2df0a940
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.10.0-pyhd8ed1ab_0.tar.bz2#cd4eb48ebde7de61f92252979aab515c
+https://conda.anaconda.org/conda-forge/osx-64/antlr-python-runtime-4.7.2-py39h6e9494a_1003.tar.bz2#44ca701f379cb0a5f1045ae64528e349
+https://conda.anaconda.org/conda-forge/noarch/babel-2.11.0-pyhd8ed1ab_0.tar.bz2#2ea70fde8d581ba9425a761609eed6ba
+https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py39h131948b_2.tar.bz2#8543a4e2c7718750cb64a2ad5da71c09
+https://conda.anaconda.org/conda-forge/osx-64/coverage-6.5.0-py39ha30fb19_1.tar.bz2#665e9468b1467699ad9174c4e74e5f8a
+https://conda.anaconda.org/conda-forge/osx-64/cython-0.29.32-py39h7a8716b_1.tar.bz2#7cccbcdd248c406cf543becf88535c3c
+https://conda.anaconda.org/conda-forge/osx-64/docutils-0.19-py39h6e9494a_1.tar.bz2#d9db9ab3a721b9f36017d6b93060b462
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-5.0.0-pyha770c72_1.tar.bz2#ec069c4db6a0ad84107bac5da62819d2
+https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-16_osx64_openblas.tar.bz2#28592eab0f05bcf9969789e87f754e11
+https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-16_osx64_openblas.tar.bz2#406ad426aade5578b90544cc2ed4a79b
+https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.1-py39ha30fb19_2.tar.bz2#ff153f279e1f29f64d98245b8a042e85
+https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
 https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2#71f1ab2de48613876becddd496371c85
-https://conda.anaconda.org/conda-forge/osx-64/pluggy-1.0.0-py310h2ec42d9_3.tar.bz2#b2349ab9b4c83ae573a6985f728e5f37
-https://conda.anaconda.org/conda-forge/osx-64/pysocks-1.7.1-py310h2ec42d9_5.tar.bz2#8b7a82347d1ed70878126333339f4969
-https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py310h1961e1f_4.tar.bz2#51b485b7f9595c2a1188451d54da17b1
-https://conda.anaconda.org/conda-forge/osx-64/setuptools-63.1.0-py310h2ec42d9_0.tar.bz2#322b12e4bc797c03dddd57a34f1fe95d
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.3.0-hd8ed1ab_0.tar.bz2#f3e98e944832fb271a0dbda7b7771dc6
-https://conda.anaconda.org/conda-forge/osx-64/virtualenv-20.15.1-py310h2ec42d9_0.tar.bz2#22182de6c361077ab027404eac1079f1
-https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py310h1961e1f_1004.tar.bz2#e84bd2f66966aa51356dfe14ef887e42
-https://conda.anaconda.org/conda-forge/osx-64/cryptography-37.0.4-py310h52c3658_0.tar.bz2#0dbc94ce0eedf8eae3aded71c5761ad3
+https://conda.anaconda.org/conda-forge/noarch/pip-22.3.1-pyhd8ed1ab_0.tar.bz2#da66f2851b9836d3a7c5190082a45f7d
+https://conda.anaconda.org/conda-forge/noarch/pygments-2.13.0-pyhd8ed1ab_0.tar.bz2#9f478e8eedd301008b5f395bad0caaed
+https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py39ha30fb19_5.tar.bz2#45794cac8eadcc11b3f26dda1705bf62
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.4.0-hd8ed1ab_0.tar.bz2#be969210b61b897775a0de63cd9e9026
+https://conda.anaconda.org/conda-forge/osx-64/virtualenv-20.16.7-py39h6e9494a_0.tar.bz2#617a1f5526eb2c653fa75045d33ecbf5
+https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py39ha30fb19_1005.tar.bz2#201d86c1f0b0132954fc72251b09df8a
+https://conda.anaconda.org/conda-forge/osx-64/cryptography-38.0.3-py39hbeae22c_0.tar.bz2#f6dcaffbf00736b98aa790173e1937ab
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
-https://conda.anaconda.org/conda-forge/osx-64/numpy-1.23.1-py310ha3f357c_0.tar.bz2#68fbd55712a1abb9cb416d38db848df6
-https://conda.anaconda.org/conda-forge/noarch/pip-22.1.2-pyhd8ed1ab_0.tar.bz2#d29185c662a424f8bea1103270b85c96
-https://conda.anaconda.org/conda-forge/noarch/pygments-2.12.0-pyhd8ed1ab_0.tar.bz2#cb27e2ded147e5bcc7eafc1c6d343cb3
-https://conda.anaconda.org/conda-forge/osx-64/pytest-7.1.2-py310h2ec42d9_0.tar.bz2#213fafaad4bdda317efc58119135876b
-https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.4-pyhd8ed1ab_0.tar.bz2#dff6862ca0b54bbeab8ddf657d032920
-https://conda.anaconda.org/conda-forge/osx-64/ukkonen-1.0.1-py310h6be76da_2.tar.bz2#a40365d41e006cdca258de5eb4661509
-https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.1-py310h1bbcd0e_0.tar.bz2#cdcff21e1d0a253e54cdddb8978ce72c
-https://conda.anaconda.org/conda-forge/noarch/identify-2.5.1-pyhd8ed1ab_0.tar.bz2#6f41e3056fcd3061fbc2b49b3309fe0c
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.0.0-pyhd8ed1ab_0.tar.bz2#1d7e241dfaf5475e893d4b824bb71b44
-https://conda.anaconda.org/conda-forge/noarch/pytest-cov-3.0.0-pyhd8ed1ab_0.tar.bz2#0f7cac11bb696b62d378bde725bfc3eb
-https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.4-hd8ed1ab_0.tar.bz2#b068a47ce183af12a53c6b0d84f96085
-https://conda.anaconda.org/conda-forge/osx-64/pre-commit-2.19.0-py310h2ec42d9_0.tar.bz2#a6dc91a273f2deee96efa152d977c993
-https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.10-pyhd8ed1ab_0.tar.bz2#14f22c5b9cfd0d93c2806faaa3fe6dec
-https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_0.tar.bz2#70d6e72856de9551f83ae0f2de689a7a
+https://conda.anaconda.org/conda-forge/osx-64/numpy-1.23.4-py39hdfa1d0c_1.tar.bz2#b3006af08cbaea37b4d8ee814e643adb
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.2.0-pyhd8ed1ab_2.tar.bz2#ac82c7aebc282e6ac0450fca012ca78c
+https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.5-pyhd8ed1ab_1.tar.bz2#07037fe2931871ed69b2b3d2acd5fdc6
+https://conda.anaconda.org/conda-forge/osx-64/ukkonen-1.0.1-py39h92daf61_3.tar.bz2#24edd5c579fdf20b0721c01cc0865000
+https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.2-py39h7cc1f47_1.tar.bz2#bfd7400a69ebcd5c5cd5975507c3a60a
+https://conda.anaconda.org/conda-forge/noarch/identify-2.5.8-pyhd8ed1ab_0.tar.bz2#8001c46448f385fa43bc4221893704d2
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.1.0-pyhd8ed1ab_0.tar.bz2#fbfa0a180d48c800f922a10a114a8632
+https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.0.0-pyhd8ed1ab_0.tar.bz2#c9e3f8bfdb9bfc34aa1836a6ed4b25d7
+https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.5-hd8ed1ab_1.tar.bz2#6b7cb927a5c505b16b4b4241825e068c
+https://conda.anaconda.org/conda-forge/osx-64/pre-commit-2.20.0-py39h6e9494a_1.tar.bz2#3cc7020afa337a373aa9bf8d93482867
+https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.11-pyhd8ed1ab_0.tar.bz2#0738978569b10669bdef41c671252dd1
+https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_1.tar.bz2#089382ee0e2dc2eae33a04cc3c2bddb0
 https://conda.anaconda.org/conda-forge/noarch/codecov-2.1.11-pyhd3deb0d_0.tar.bz2#9c661c2c14b4667827218402e6624ad5
-https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.2-pyh6c4a22f_0.tar.bz2#d4eaa1f50733a377480ce1d5aac556c7
+https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
```

### Comparing `cf-units-3.1.1/requirements/locks/py310-lock-win-64.txt` & `cf-units-3.2.0/requirements/locks/py310-lock-win-64.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,93 +1,90 @@
 # Generated by conda-lock.
 # platform: win-64
-# input_hash: 3fd0c6fef3d17bd216e09ffc63e7738d8b9e59000568ac03db9025f78e20d87e
+# input_hash: 7972ae7bb896cf1c3473f065e447a2d602d8316a65dd1a113de693a3f42538d2
 @EXPLICIT
-https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2022.6.15-h5b45459_0.tar.bz2#b84069692c33afe59f31c7117c80696e
+https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2022.9.24-h5b45459_0.tar.bz2#5fba0abc60bf327a4bc4188cd64678be
 https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2022.1.0-h57928b3_3787.tar.bz2#35dff2b6e944ce136a574c4c006cec28
-https://conda.anaconda.org/conda-forge/noarch/tzdata-2022a-h191b570_0.tar.bz2#84be5301069417a2221187d2f435e0f7
-https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.20348.0-h57928b3_0.tar.bz2#6d666b6ea8251231ff508062d1e41f9c
-https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.29.30037-h902a5da_6.tar.bz2#33d07ebe91062743eabc9e53a60d18e1
-https://conda.anaconda.org/conda-forge/win-64/vc-14.2-hb210afc_6.tar.bz2#c2aecbc9b00ba6f352e27d3d61fd31fb
+https://conda.anaconda.org/conda-forge/noarch/tzdata-2022f-h191b570_0.tar.bz2#e366350e2343a798e29833286abe2560
+https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
+https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.32.31332-h1d6e394_9.tar.bz2#c98b6e39006315599b793592bcc3c978
+https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h3d8a991_9.tar.bz2#ba28983ef4f6d430827d0e7c5cdd7b48
 https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
-https://conda.anaconda.org/conda-forge/win-64/expat-2.4.8-h39d44d4_0.tar.bz2#f8e0f53713756c08456f50c9ce25748c
+https://conda.anaconda.org/conda-forge/win-64/expat-2.5.0-h1537add_0.tar.bz2#6b20c31bd735d2dd5c79ddb5b3524619
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
-https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.12-h8ffe710_1.tar.bz2#8b67614ab0539e803c03db2ed7990c6c
-https://conda.anaconda.org/conda-forge/win-64/openssl-1.1.1q-h8ffe710_0.tar.bz2#2ee16f406ee12fe4dcd08b513e9bd0c6
-https://conda.anaconda.org/conda-forge/win-64/sqlite-3.39.0-h8ffe710_0.tar.bz2#c76b39a7a74df1875e7b2b3fb5549632
-https://conda.anaconda.org/conda-forge/win-64/tbb-2021.5.0-h2d74725_1.tar.bz2#8f00f39dbd7deaba11410b0b6e7b2cb4
+https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.40.0-hcfcfb64_0.tar.bz2#5e5a97795de72f8cc3baf3d9ea6327a2
+https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_4.tar.bz2#0cc5c5cc64ee1637f37f8540a175854c
+https://conda.anaconda.org/conda-forge/win-64/openssl-3.0.7-hcfcfb64_0.tar.bz2#a87ab36dc95970e3b4b63b7599bebdbe
+https://conda.anaconda.org/conda-forge/win-64/tbb-2021.7.0-h91493d7_0.tar.bz2#f57be598137919e4f7e7d159960d66a1
 https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
-https://conda.anaconda.org/conda-forge/win-64/xz-5.2.5-h62dcd97_1.tar.bz2#eabcbfedd14d7c18a514afca09ea0ebb
+https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
 https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
 https://conda.anaconda.org/conda-forge/win-64/mkl-2022.1.0-h6a75c08_874.tar.bz2#2ff89a7337a9636029b4db9466e9f8e3
-https://conda.anaconda.org/conda-forge/win-64/python-3.10.5-h9a09f29_0_cpython.tar.bz2#80c856de93cbe0bbf2b1714f55ae56cc
+https://conda.anaconda.org/conda-forge/win-64/python-3.10.6-hcf16a7b_0_cpython.tar.bz2#fd37ee80fffd9209ce2d2c869920f16e
 https://conda.anaconda.org/conda-forge/win-64/udunits2-2.2.28-h892ecd3_0.tar.bz2#dad8b5fae263e4e36d859524a3794801
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.12-py_0.tar.bz2#2489a97287f90176ecdc3ca982b4b0a0
-https://conda.anaconda.org/conda-forge/noarch/atomicwrites-1.4.1-pyhd8ed1ab_0.tar.bz2#1714887104aab113bde64001ceb17262
-https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
+https://conda.anaconda.org/conda-forge/noarch/attrs-22.1.0-pyh71513ae_1.tar.bz2#6d3ccbc56256204925bfa8378722792f
+https://conda.anaconda.org/conda-forge/noarch/certifi-2022.9.24-pyhd8ed1ab_0.tar.bz2#f66309b099374af91369e67e84af397d
 https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2#ebb5f5f7dc4f1a3780ef7ea7738db08c
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.0-pyhd8ed1ab_0.tar.bz2#abc0453b6e7bfbb87d275d58e333fc98
-https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.5-pyhd8ed1ab_0.tar.bz2#c267da48ce208905d7d976d49dfd9433
-https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.4-pyhd8ed1ab_0.tar.bz2#7b50d840543d9cdae100e91582c33035
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.7.1-pyhd8ed1ab_0.tar.bz2#7556872687250e0ea038eb503da3c44b
-https://conda.anaconda.org/conda-forge/noarch/idna-3.3-pyhd8ed1ab_0.tar.bz2#40b50b8b030f5f2f22085c062ed013dd
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.1-pyhd8ed1ab_0.tar.bz2#c1d5b294fbf9a795dec349a6f4d8be8e
+https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
+https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2#b65b4d50dbd2d50fa0aeac367ec9eed7
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.0.4-pyhd8ed1ab_0.tar.bz2#e0734d1f12de77f9daca98bda3428733
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.8.0-pyhd8ed1ab_0.tar.bz2#10f0218dbd493ab2e5dc6759ddea4526
+https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-1.1.1-pyh9f0ad1d_0.tar.bz2#39161f81cc5e5ca45b8226fbb06c6905
-https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-15_win64_mkl.tar.bz2#661187f959fed1821cdd6921a738336d
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.1-pyhd8ed1ab_0.tar.bz2#d5df87964a39f67c46a5448f4e78d9b6
-https://conda.anaconda.org/conda-forge/noarch/py-1.11.0-pyh6c4a22f_0.tar.bz2#b4613d7e7a493916d867842a6a148054
+https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-16_win64_mkl.tar.bz2#d2e6f4e86cee2b4e8c27ff6884ccdc61
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.2-pyhd8ed1ab_1.tar.bz2#2fb3f88922e7aec26ba652fcdfe13950
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/win-64/python_abi-3.10-2_cp310.tar.bz2#aaa900b98edb2e67106b461ff365ba57
-https://conda.anaconda.org/conda-forge/noarch/pytz-2022.1-pyhd8ed1ab_0.tar.bz2#b87d66d6d3991d988fb31510c95a9267
-https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+https://conda.anaconda.org/conda-forge/noarch/pytz-2022.6-pyhd8ed1ab_0.tar.bz2#b1f26ad83328e486910ef7f6e81dc061
+https://conda.anaconda.org/conda-forge/noarch/setuptools-65.5.1-pyhd8ed1ab_0.tar.bz2#cfb8dc4d9d285ca5fb1177b9dd450e33
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.2-py_0.tar.bz2#20b2eaeaeea4ef9a9a0d99770620fd09
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.0-pyhd8ed1ab_0.tar.bz2#77dad82eb9c8c1525ff7953e0756d708
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.3.0-pyha770c72_0.tar.bz2#a9d85960bc62d53cc4ea0d1d27f73c98
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.37.1-pyhd8ed1ab_0.tar.bz2#1ca02aaf78d9c70d9a81a3bed5752022
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.8.0-pyhd8ed1ab_0.tar.bz2#050b94cf4a8c760656e51d2d44e4632c
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.4.0-pyha770c72_0.tar.bz2#2d93b130d148d7fc77e583677792fc6a
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.38.4-pyhd8ed1ab_0.tar.bz2#c829cfb8cb826acb9de0ac1a2df0a940
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.10.0-pyhd8ed1ab_0.tar.bz2#cd4eb48ebde7de61f92252979aab515c
 https://conda.anaconda.org/conda-forge/win-64/antlr-python-runtime-4.7.2-py310h5588dad_1003.tar.bz2#7acc45deb8ddad60880ccf353729dac7
-https://conda.anaconda.org/conda-forge/noarch/babel-2.10.3-pyhd8ed1ab_0.tar.bz2#72f1c6d03109d7a70087bc1d029a8eda
-https://conda.anaconda.org/conda-forge/win-64/certifi-2022.6.15-py310h5588dad_0.tar.bz2#0d68bfe987b9e8414847e6eef95e6370
-https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py310hcbf9ad4_0.tar.bz2#291e525e56b35d2ae277b592e08141a8
-https://conda.anaconda.org/conda-forge/win-64/coverage-6.4.1-py310he2412df_0.tar.bz2#3e1377150bbc29acf9a3521f8802dc83
-https://conda.anaconda.org/conda-forge/win-64/cython-0.29.30-py310h8a704f9_0.tar.bz2#db67f622ae4b095c0e9673deb63b63b7
-https://conda.anaconda.org/conda-forge/win-64/docutils-0.18.1-py310h5588dad_1.tar.bz2#10fe0cdd2629f3fe5d27db3f084545f5
-https://conda.anaconda.org/conda-forge/win-64/importlib-metadata-4.11.4-py310h5588dad_0.tar.bz2#16ef54587496fadabd26ba48ff221750
-https://conda.anaconda.org/conda-forge/win-64/libcblas-3.9.0-15_win64_mkl.tar.bz2#c6012601cd7dde1b4108128fb847de9f
-https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-15_win64_mkl.tar.bz2#7915daedfea4cc94ffcaa71cde184f50
-https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.1-py310he2412df_1.tar.bz2#c33fd016ec3b4c3cb0e676fbd0b18953
+https://conda.anaconda.org/conda-forge/noarch/babel-2.11.0-pyhd8ed1ab_0.tar.bz2#2ea70fde8d581ba9425a761609eed6ba
+https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py310h628cb3f_2.tar.bz2#ec6be66017eb91c9077abe15dcb19e75
+https://conda.anaconda.org/conda-forge/win-64/coverage-6.5.0-py310h8d17308_1.tar.bz2#002e8db221bc7447cdb84cbf6b8284c8
+https://conda.anaconda.org/conda-forge/win-64/cython-0.29.32-py310h00ffb61_1.tar.bz2#376e373477df8d5ef2c4bf3726dc8808
+https://conda.anaconda.org/conda-forge/win-64/docutils-0.19-py310h5588dad_1.tar.bz2#88111d95b12d83681d0ecdbbc24eee8e
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-5.0.0-pyha770c72_1.tar.bz2#ec069c4db6a0ad84107bac5da62819d2
+https://conda.anaconda.org/conda-forge/win-64/libcblas-3.9.0-16_win64_mkl.tar.bz2#14c2fb03b2bb14dfa3806186ca91d557
+https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-16_win64_mkl.tar.bz2#be2f9d5712a5bb05cd900005ee752a05
+https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.1-py310h8d17308_2.tar.bz2#24e57be449c71b8edc52cc6a48ff846d
+https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
 https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2#71f1ab2de48613876becddd496371c85
-https://conda.anaconda.org/conda-forge/win-64/pluggy-1.0.0-py310h5588dad_3.tar.bz2#48b66805d9d5b1d24fcb0d547471a0f0
-https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py310he2412df_4.tar.bz2#e1386e64a5e6d3ef30860a233ce8b371
-https://conda.anaconda.org/conda-forge/win-64/setuptools-63.1.0-py310h5588dad_0.tar.bz2#348f2504ad88914760b0964caa47bc03
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.3.0-hd8ed1ab_0.tar.bz2#f3e98e944832fb271a0dbda7b7771dc6
-https://conda.anaconda.org/conda-forge/win-64/virtualenv-20.15.1-py310h5588dad_0.tar.bz2#ce3cce75cf81e1c435c7348680422720
-https://conda.anaconda.org/conda-forge/win-64/win_inet_pton-1.1.0-py310h5588dad_4.tar.bz2#674aa7b17ab884a99afeec3547a03bb8
-https://conda.anaconda.org/conda-forge/win-64/brotlipy-0.7.0-py310he2412df_1004.tar.bz2#6967391ab90fb96d3e75bf423012fa79
-https://conda.anaconda.org/conda-forge/win-64/cryptography-37.0.4-py310ha857299_0.tar.bz2#5a5a9422f119a85b1c5d826d04fb703b
+https://conda.anaconda.org/conda-forge/noarch/pip-22.3.1-pyhd8ed1ab_0.tar.bz2#da66f2851b9836d3a7c5190082a45f7d
+https://conda.anaconda.org/conda-forge/noarch/pygments-2.13.0-pyhd8ed1ab_0.tar.bz2#9f478e8eedd301008b5f395bad0caaed
+https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py310h8d17308_5.tar.bz2#d0daf3eed98dd2bf4337ed08d8011eb8
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.4.0-hd8ed1ab_0.tar.bz2#be969210b61b897775a0de63cd9e9026
+https://conda.anaconda.org/conda-forge/win-64/virtualenv-20.16.7-py310h5588dad_0.tar.bz2#a03ef415e02f6c7b9e676a5924c8612a
+https://conda.anaconda.org/conda-forge/win-64/brotlipy-0.7.0-py310h8d17308_1005.tar.bz2#6cb010e0fa21d7b606a13038a89ccbc2
+https://conda.anaconda.org/conda-forge/win-64/cryptography-38.0.3-py310h6e82f81_0.tar.bz2#b08acdd3674bab4a28fa53853e444921
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
-https://conda.anaconda.org/conda-forge/win-64/numpy-1.23.1-py310h8a5b91a_0.tar.bz2#8c393e7e00a412bd122520d08bf5a327
-https://conda.anaconda.org/conda-forge/noarch/pip-22.1.2-pyhd8ed1ab_0.tar.bz2#d29185c662a424f8bea1103270b85c96
-https://conda.anaconda.org/conda-forge/noarch/pygments-2.12.0-pyhd8ed1ab_0.tar.bz2#cb27e2ded147e5bcc7eafc1c6d343cb3
-https://conda.anaconda.org/conda-forge/win-64/pysocks-1.7.1-py310h5588dad_5.tar.bz2#8b84a5de3ffa12a5aaeea385140bba27
-https://conda.anaconda.org/conda-forge/win-64/pytest-7.1.2-py310h5588dad_0.tar.bz2#752fb46d83358bc421474e1abc542e9d
-https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.4-pyhd8ed1ab_0.tar.bz2#dff6862ca0b54bbeab8ddf657d032920
-https://conda.anaconda.org/conda-forge/win-64/ukkonen-1.0.1-py310h476a331_2.tar.bz2#a6a3ce7a3f9d95648bfc8eef30961012
-https://conda.anaconda.org/conda-forge/win-64/cftime-1.6.1-py310h2873277_0.tar.bz2#230b933708145ff2bfb0dae0c82d864f
-https://conda.anaconda.org/conda-forge/noarch/identify-2.5.1-pyhd8ed1ab_0.tar.bz2#6f41e3056fcd3061fbc2b49b3309fe0c
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.0.0-pyhd8ed1ab_0.tar.bz2#1d7e241dfaf5475e893d4b824bb71b44
-https://conda.anaconda.org/conda-forge/noarch/pytest-cov-3.0.0-pyhd8ed1ab_0.tar.bz2#0f7cac11bb696b62d378bde725bfc3eb
-https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.4-hd8ed1ab_0.tar.bz2#b068a47ce183af12a53c6b0d84f96085
-https://conda.anaconda.org/conda-forge/win-64/pre-commit-2.19.0-py310h5588dad_0.tar.bz2#79f4ed963909c3283064c31ba1039c04
-https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.10-pyhd8ed1ab_0.tar.bz2#14f22c5b9cfd0d93c2806faaa3fe6dec
-https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_0.tar.bz2#70d6e72856de9551f83ae0f2de689a7a
+https://conda.anaconda.org/conda-forge/win-64/numpy-1.23.4-py310h4a8f9c9_1.tar.bz2#3e912fdde0f115791cb783fd35d41ad8
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.2.0-pyhd8ed1ab_2.tar.bz2#ac82c7aebc282e6ac0450fca012ca78c
+https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.5-pyhd8ed1ab_1.tar.bz2#07037fe2931871ed69b2b3d2acd5fdc6
+https://conda.anaconda.org/conda-forge/win-64/ukkonen-1.0.1-py310h232114e_3.tar.bz2#e058ad110afa0356b03a91ad949c510d
+https://conda.anaconda.org/conda-forge/win-64/cftime-1.6.2-py310h9b08ddd_1.tar.bz2#6d26114b7e1313d82e85570789bd9ad0
+https://conda.anaconda.org/conda-forge/noarch/identify-2.5.8-pyhd8ed1ab_0.tar.bz2#8001c46448f385fa43bc4221893704d2
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.1.0-pyhd8ed1ab_0.tar.bz2#fbfa0a180d48c800f922a10a114a8632
+https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.0.0-pyhd8ed1ab_0.tar.bz2#c9e3f8bfdb9bfc34aa1836a6ed4b25d7
+https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.5-hd8ed1ab_1.tar.bz2#6b7cb927a5c505b16b4b4241825e068c
+https://conda.anaconda.org/conda-forge/win-64/pre-commit-2.20.0-py310h5588dad_1.tar.bz2#dc1748bb5b743c7c11a685df20c537a3
+https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.11-pyhd8ed1ab_0.tar.bz2#0738978569b10669bdef41c671252dd1
+https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_1.tar.bz2#089382ee0e2dc2eae33a04cc3c2bddb0
 https://conda.anaconda.org/conda-forge/noarch/codecov-2.1.11-pyhd3deb0d_0.tar.bz2#9c661c2c14b4667827218402e6624ad5
-https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.2-pyh6c4a22f_0.tar.bz2#d4eaa1f50733a377480ce1d5aac556c7
+https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
```

### Comparing `cf-units-3.1.1/requirements/locks/py38-lock-linux-64.txt` & `cf-units-3.2.0/requirements/locks/py38-lock-linux-64.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,98 +1,97 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 42997195f33081b98c38cecc147736289c59f410c2e13124ca97c1effd65c4df
+# input_hash: 71f386a9c27dfeb118445ec0906a081b4193c16385821e36939d3f3590b0b2fc
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
-https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2022.6.15-ha878542_0.tar.bz2#c320890f77fd1d617fa876e0982002c2
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.36.1-hea4e1c9_2.tar.bz2#bd4f2e711b39af170e7ff15163fe87ee
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-12.1.0-hdcd56e2_16.tar.bz2#b02605b875559ff99f04351fd5040760
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.1.0-ha89aaad_16.tar.bz2#6f5ba041a41eb102a1027d9e68731be7
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-12.1.0-h69a702a_16.tar.bz2#6bf15e29a20f614b18ae89368260d0a2
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.1.0-h8d9b700_16.tar.bz2#f013cf7749536ce43d82afbffdf499ab
+https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2022.9.24-ha878542_0.tar.bz2#41e4e87062433e283696cf384f952ef6
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.39-hc81fddc_0.tar.bz2#c2719e2faa7bd7076d3a4b52271e5622
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-12.2.0-h337968e_19.tar.bz2#164b4b1acaedc47ee7e658ae6b308ca3
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.2.0-h46fd767_19.tar.bz2#1030b1f38c129f2634eae026f704fe60
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-12.2.0-h69a702a_19.tar.bz2#cd7a806282c16e1f2d39a7e80d3a3e0d
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.2.0-h65d4601_19.tar.bz2#cedcee7c064c01c403f962c9e8d3c373
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.1.0-h8d9b700_16.tar.bz2#4f05bc9844f7c101e6e147dab3c88d5c
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.2.0-h65d4601_19.tar.bz2#e4c94f80aef025c17ab0828cd85ef535
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
-https://conda.anaconda.org/conda-forge/linux-64/expat-2.4.8-h27087fc_0.tar.bz2#e1b07832504eeba765d648389cc387a9
+https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-h27087fc_0.tar.bz2#c4fbad8d4bddeb3c085f18cbf97fbfad
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
-https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.20-pthreads_h78a6416_0.tar.bz2#9b6d0781953c9e353faee494336cc229
+https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.21-pthreads_h78a6416_3.tar.bz2#8c5963a49b6035c40646a763293fbb35
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.32.1-h7f98852_1000.tar.bz2#772d69f030955d9646d3d0eaf21d859d
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.12-h166bdaf_1.tar.bz2#58eaff4f91891978af3625e7bbf958af
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
 https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2#4acfc691e64342b9dae57cf2adc63238
-https://conda.anaconda.org/conda-forge/linux-64/openssl-1.1.1q-h166bdaf_0.tar.bz2#07acc367c7fc8b716770cd5b36d31717
-https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.5-h516909a_1.tar.bz2#33f601066901f3e1a85af3522a8113f9
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.0.7-h166bdaf_0.tar.bz2#d1ad1824c71e67dea42f07e06cd177dc
+https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
-https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-15_linux64_openblas.tar.bz2#04eb983975a1be3e57d6d667414cd774
+https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-16_linux64_openblas.tar.bz2#d9b7a8639171f6c6fa0a983edabcfe2b
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.40.0-h753d276_0.tar.bz2#2e5f9a37d487e1019fd4d8113adb2f9f
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.1.2-h0f457ee_0.tar.bz2#db2ebbe2943aae81ed051a6a9af8e0fa
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/udunits2-2.2.28-hc3e0081_0.tar.bz2#d4c341e0379c31e9e781d4f204726867
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.12-h166bdaf_1.tar.bz2#e4b67f2b4096807cd7d836227c026a43
-https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-15_linux64_openblas.tar.bz2#f45968428e445fd0c6472b561145812a
-https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-15_linux64_openblas.tar.bz2#b7078220384b8bf8db1a45e66412ac4f
-https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.39.0-h4ff8645_0.tar.bz2#ead30581ba8cfd52d69632868b844d4a
-https://conda.anaconda.org/conda-forge/linux-64/python-3.8.13-h582c2e5_0_cpython.tar.bz2#8ec74710472994e2411a8020fa8589ce
+https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-16_linux64_openblas.tar.bz2#20bae26d0a1db73f758fc3754cab4719
+https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-16_linux64_openblas.tar.bz2#955d993f41f9354bf753d29864ea20ad
+https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.40.0-h4ff8645_0.tar.bz2#bb11803129cbbb53ed56f9506ff74145
+https://conda.anaconda.org/conda-forge/linux-64/python-3.8.13-ha86cf86_0_cpython.tar.bz2#39183fc3fc91579b466dfa767d2ef4b1
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.12-py_0.tar.bz2#2489a97287f90176ecdc3ca982b4b0a0
-https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
+https://conda.anaconda.org/conda-forge/noarch/attrs-22.1.0-pyh71513ae_1.tar.bz2#6d3ccbc56256204925bfa8378722792f
+https://conda.anaconda.org/conda-forge/noarch/certifi-2022.9.24-pyhd8ed1ab_0.tar.bz2#f66309b099374af91369e67e84af397d
 https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2#ebb5f5f7dc4f1a3780ef7ea7738db08c
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.0-pyhd8ed1ab_0.tar.bz2#abc0453b6e7bfbb87d275d58e333fc98
-https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.5-pyhd8ed1ab_0.tar.bz2#c267da48ce208905d7d976d49dfd9433
-https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.4-pyhd8ed1ab_0.tar.bz2#7b50d840543d9cdae100e91582c33035
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.7.1-pyhd8ed1ab_0.tar.bz2#7556872687250e0ea038eb503da3c44b
-https://conda.anaconda.org/conda-forge/noarch/idna-3.3-pyhd8ed1ab_0.tar.bz2#40b50b8b030f5f2f22085c062ed013dd
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.1-pyhd8ed1ab_0.tar.bz2#c1d5b294fbf9a795dec349a6f4d8be8e
+https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
+https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2#b65b4d50dbd2d50fa0aeac367ec9eed7
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.0.4-pyhd8ed1ab_0.tar.bz2#e0734d1f12de77f9daca98bda3428733
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.8.0-pyhd8ed1ab_0.tar.bz2#10f0218dbd493ab2e5dc6759ddea4526
+https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-1.1.1-pyh9f0ad1d_0.tar.bz2#39161f81cc5e5ca45b8226fbb06c6905
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.1-pyhd8ed1ab_0.tar.bz2#d5df87964a39f67c46a5448f4e78d9b6
-https://conda.anaconda.org/conda-forge/noarch/py-1.11.0-pyh6c4a22f_0.tar.bz2#b4613d7e7a493916d867842a6a148054
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.2-pyhd8ed1ab_1.tar.bz2#2fb3f88922e7aec26ba652fcdfe13950
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.8-2_cp38.tar.bz2#bfbb29d517281e78ac53e48d21e6e860
-https://conda.anaconda.org/conda-forge/noarch/pytz-2022.1-pyhd8ed1ab_0.tar.bz2#b87d66d6d3991d988fb31510c95a9267
-https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+https://conda.anaconda.org/conda-forge/noarch/pytz-2022.6-pyhd8ed1ab_0.tar.bz2#b1f26ad83328e486910ef7f6e81dc061
+https://conda.anaconda.org/conda-forge/noarch/setuptools-65.5.1-pyhd8ed1ab_0.tar.bz2#cfb8dc4d9d285ca5fb1177b9dd450e33
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.2-py_0.tar.bz2#20b2eaeaeea4ef9a9a0d99770620fd09
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.0-pyhd8ed1ab_0.tar.bz2#77dad82eb9c8c1525ff7953e0756d708
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.3.0-pyha770c72_0.tar.bz2#a9d85960bc62d53cc4ea0d1d27f73c98
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.37.1-pyhd8ed1ab_0.tar.bz2#1ca02aaf78d9c70d9a81a3bed5752022
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.8.0-pyhd8ed1ab_0.tar.bz2#050b94cf4a8c760656e51d2d44e4632c
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.4.0-pyha770c72_0.tar.bz2#2d93b130d148d7fc77e583677792fc6a
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.38.4-pyhd8ed1ab_0.tar.bz2#c829cfb8cb826acb9de0ac1a2df0a940
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.10.0-pyhd8ed1ab_0.tar.bz2#cd4eb48ebde7de61f92252979aab515c
 https://conda.anaconda.org/conda-forge/linux-64/antlr-python-runtime-4.7.2-py38h578d9bd_1003.tar.bz2#db8b471d9a764f561a129f94ea215c0a
-https://conda.anaconda.org/conda-forge/noarch/babel-2.10.3-pyhd8ed1ab_0.tar.bz2#72f1c6d03109d7a70087bc1d029a8eda
-https://conda.anaconda.org/conda-forge/linux-64/certifi-2022.6.15-py38h578d9bd_0.tar.bz2#1f4339b25d1030cfbf4ee0b06690bbce
-https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py38h4a40e3a_0.tar.bz2#a970d201055ec06a75db83bf25447eb2
-https://conda.anaconda.org/conda-forge/linux-64/coverage-6.4.1-py38h0a891b7_0.tar.bz2#520839b0ef944bffcfb8d88b876a5fbc
-https://conda.anaconda.org/conda-forge/linux-64/cython-0.29.30-py38hfa26641_0.tar.bz2#189de973189a5550f34a6c1131dcd15d
-https://conda.anaconda.org/conda-forge/linux-64/docutils-0.18.1-py38h578d9bd_1.tar.bz2#40086fd82fe8af5a0ccc769245f67c6a
-https://conda.anaconda.org/conda-forge/linux-64/importlib-metadata-4.11.4-py38h578d9bd_0.tar.bz2#037225c33a50e99c5d4f86fac90f6de8
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.1-py38h0a891b7_1.tar.bz2#20d003ad5f584e212c299f64cac46c05
-https://conda.anaconda.org/conda-forge/linux-64/numpy-1.23.1-py38h3a7f9d9_0.tar.bz2#90cf44c14b2bfe19ce7b875979b90cb9
+https://conda.anaconda.org/conda-forge/noarch/babel-2.11.0-pyhd8ed1ab_0.tar.bz2#2ea70fde8d581ba9425a761609eed6ba
+https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py38h4a40e3a_2.tar.bz2#2276b1f4d1ede3f5f14cc7e4ae6f9a33
+https://conda.anaconda.org/conda-forge/linux-64/coverage-6.5.0-py38h0a891b7_1.tar.bz2#ce9ab2be3e564c1626f9bab2416b20a7
+https://conda.anaconda.org/conda-forge/linux-64/cython-0.29.32-py38hfa26641_1.tar.bz2#eef241f25124f2f486f9994bcbf19751
+https://conda.anaconda.org/conda-forge/linux-64/docutils-0.19-py38h578d9bd_1.tar.bz2#3746b24949251f1a00ae0d616d4cdc1b
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-5.0.0-pyha770c72_1.tar.bz2#ec069c4db6a0ad84107bac5da62819d2
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.1-py38h0a891b7_2.tar.bz2#c342a370480791db83d5dd20f2d8899f
+https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
+https://conda.anaconda.org/conda-forge/linux-64/numpy-1.23.4-py38h7042d01_1.tar.bz2#7fa0e9ed4e8a096e2f00b2426ebba0de
 https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2#71f1ab2de48613876becddd496371c85
-https://conda.anaconda.org/conda-forge/linux-64/pluggy-1.0.0-py38h578d9bd_3.tar.bz2#6ce4ce3d4490a56eb33b52c179609193
-https://conda.anaconda.org/conda-forge/linux-64/pysocks-1.7.1-py38h578d9bd_5.tar.bz2#11113c7e50bb81f30762fe8325f305e1
-https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py38h0a891b7_4.tar.bz2#ba24ff01bb38c5cd5be54b45ef685db3
-https://conda.anaconda.org/conda-forge/linux-64/setuptools-63.1.0-py38h578d9bd_0.tar.bz2#5f57352931001b831e0f3702801e6fc8
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.3.0-hd8ed1ab_0.tar.bz2#f3e98e944832fb271a0dbda7b7771dc6
-https://conda.anaconda.org/conda-forge/linux-64/virtualenv-20.15.1-py38h578d9bd_0.tar.bz2#0a703d05848de7738a1466b5e0a99274
-https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py38h0a891b7_1004.tar.bz2#9fcaaca218dcfeb8da806d4fd4824aa0
-https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.1-py38h71d37f0_0.tar.bz2#acf7ef1f057459e9e707142a4b92e481
-https://conda.anaconda.org/conda-forge/linux-64/cryptography-37.0.4-py38h2b5fc30_0.tar.bz2#28e9acd6f13ed29f27d5550a1cf0554b
+https://conda.anaconda.org/conda-forge/noarch/pip-22.3.1-pyhd8ed1ab_0.tar.bz2#da66f2851b9836d3a7c5190082a45f7d
+https://conda.anaconda.org/conda-forge/noarch/pygments-2.13.0-pyhd8ed1ab_0.tar.bz2#9f478e8eedd301008b5f395bad0caaed
+https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py38h0a891b7_5.tar.bz2#0856c59f9ddb710c640dc0428d66b1b7
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.4.0-hd8ed1ab_0.tar.bz2#be969210b61b897775a0de63cd9e9026
+https://conda.anaconda.org/conda-forge/linux-64/virtualenv-20.16.7-py38h578d9bd_0.tar.bz2#fc6d74114bb0006224f252393bdacee6
+https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py38h0a891b7_1005.tar.bz2#e99e08812dfff30fdd17b3f8838e2759
+https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.2-py38h26c90d9_1.tar.bz2#dcc025a7bb54374979c500c2e161fac9
+https://conda.anaconda.org/conda-forge/linux-64/cryptography-38.0.3-py38h80a4ca7_0.tar.bz2#9822ec88bb44cddbe3fdeebc41135808
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
-https://conda.anaconda.org/conda-forge/noarch/pip-22.1.2-pyhd8ed1ab_0.tar.bz2#d29185c662a424f8bea1103270b85c96
-https://conda.anaconda.org/conda-forge/noarch/pygments-2.12.0-pyhd8ed1ab_0.tar.bz2#cb27e2ded147e5bcc7eafc1c6d343cb3
-https://conda.anaconda.org/conda-forge/linux-64/pytest-7.1.2-py38h578d9bd_0.tar.bz2#626d2b8f96c8c3d20198e6bd84d1cfb7
-https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.4-pyhd8ed1ab_0.tar.bz2#dff6862ca0b54bbeab8ddf657d032920
-https://conda.anaconda.org/conda-forge/linux-64/ukkonen-1.0.1-py38h43d8883_2.tar.bz2#3f6ce81c7d28563fe2af763d9ff43e62
-https://conda.anaconda.org/conda-forge/noarch/identify-2.5.1-pyhd8ed1ab_0.tar.bz2#6f41e3056fcd3061fbc2b49b3309fe0c
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.0.0-pyhd8ed1ab_0.tar.bz2#1d7e241dfaf5475e893d4b824bb71b44
-https://conda.anaconda.org/conda-forge/noarch/pytest-cov-3.0.0-pyhd8ed1ab_0.tar.bz2#0f7cac11bb696b62d378bde725bfc3eb
-https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.4-hd8ed1ab_0.tar.bz2#b068a47ce183af12a53c6b0d84f96085
-https://conda.anaconda.org/conda-forge/linux-64/pre-commit-2.19.0-py38h578d9bd_0.tar.bz2#aa6a241a741c27c9560fd3cebb3f43ce
-https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.10-pyhd8ed1ab_0.tar.bz2#14f22c5b9cfd0d93c2806faaa3fe6dec
-https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_0.tar.bz2#70d6e72856de9551f83ae0f2de689a7a
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.2.0-pyhd8ed1ab_2.tar.bz2#ac82c7aebc282e6ac0450fca012ca78c
+https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.5-pyhd8ed1ab_1.tar.bz2#07037fe2931871ed69b2b3d2acd5fdc6
+https://conda.anaconda.org/conda-forge/linux-64/ukkonen-1.0.1-py38h43d8883_3.tar.bz2#82b3797d08a43a101b645becbb938e65
+https://conda.anaconda.org/conda-forge/noarch/identify-2.5.8-pyhd8ed1ab_0.tar.bz2#8001c46448f385fa43bc4221893704d2
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.1.0-pyhd8ed1ab_0.tar.bz2#fbfa0a180d48c800f922a10a114a8632
+https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.0.0-pyhd8ed1ab_0.tar.bz2#c9e3f8bfdb9bfc34aa1836a6ed4b25d7
+https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.5-hd8ed1ab_1.tar.bz2#6b7cb927a5c505b16b4b4241825e068c
+https://conda.anaconda.org/conda-forge/linux-64/pre-commit-2.20.0-py38h578d9bd_1.tar.bz2#38d9029214399e4bfc378b62b0171bf0
+https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.11-pyhd8ed1ab_0.tar.bz2#0738978569b10669bdef41c671252dd1
+https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_1.tar.bz2#089382ee0e2dc2eae33a04cc3c2bddb0
 https://conda.anaconda.org/conda-forge/noarch/codecov-2.1.11-pyhd3deb0d_0.tar.bz2#9c661c2c14b4667827218402e6624ad5
-https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.2-pyh6c4a22f_0.tar.bz2#d4eaa1f50733a377480ce1d5aac556c7
+https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
```

### Comparing `cf-units-3.1.1/requirements/locks/py38-lock-osx-64.txt` & `cf-units-3.2.0/requirements/locks/py310-lock-osx-64.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,92 +1,91 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: cda0794e9276f2a0af5faf9bd4f04e187e552589c7342729b361877654ec2202
+# input_hash: 04f506c100edfc7cab7ed810b19b3ee215480e059a6acb742569260a7bd8c018
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
-https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2022.6.15-h033912b_0.tar.bz2#d16674f96e47de0d08af3fc97803134e
-https://conda.anaconda.org/conda-forge/osx-64/libcxx-14.0.6-hce7ea42_0.tar.bz2#ac504a8074ae8add8b837a93d7bc33ca
+https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2022.9.24-h033912b_0.tar.bz2#67b268c32433047914482def1ce215c2
+https://conda.anaconda.org/conda-forge/osx-64/libcxx-14.0.6-hccf4f1f_0.tar.bz2#208a6a874b073277374de48a782f6b10
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
-https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.12-hfe4f2af_1.tar.bz2#f7d43cae08c86f73be8cbda4f8e43373
-https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-14.0.4-ha654fa7_0.tar.bz2#5d5ab9ab83ce21422be84ecfd3142201
+https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-hfd90126_4.tar.bz2#35eb3fce8d51ed3c1fd4122bad48250b
+https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-15.0.5-h61d9ccf_0.tar.bz2#81ceb8ca1476f31cbaacf7ac845b6fff
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.3-h96cf925_1.tar.bz2#76217ebfbb163ff2770a261f955a5861
-https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.5-haf1e3a3_1.tar.bz2#41116deb499e9bc58048c297d6403ce6
+https://conda.anaconda.org/conda-forge/noarch/tzdata-2022f-h191b570_0.tar.bz2#e366350e2343a798e29833286abe2560
+https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
-https://conda.anaconda.org/conda-forge/osx-64/expat-2.4.8-h96cf925_0.tar.bz2#529d357c143fb98b9af77d687f82a3e0
-https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-9.3.0-h6c81a4c_23.tar.bz2#a6956ceb628b14594613cefee5127a7a
-https://conda.anaconda.org/conda-forge/osx-64/openssl-1.1.1q-hfe4f2af_0.tar.bz2#ce822517fb00e8bafea6fe77d07f20bd
+https://conda.anaconda.org/conda-forge/osx-64/expat-2.5.0-hf0c8a7f_0.tar.bz2#7648a729fc8b7272596e90b0ab0a3e98
+https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-11.3.0-h082f757_26.tar.bz2#11835360754e5caca43cfaa3a81dfca5
+https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.40.0-ha978bb4_0.tar.bz2#ceb13b6726534b96e3b4e3dda91e9050
+https://conda.anaconda.org/conda-forge/osx-64/openssl-3.0.7-hfd90126_0.tar.bz2#78d8266753a5db378ef0f9302be9990f
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.1.2-h3899abd_0.tar.bz2#89fa404901fa8fb7d4f4e07083b8d635
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
-https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.12-hfe4f2af_1.tar.bz2#12fdf8350ef315e7ad48693346067405
-https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-9_3_0_h6c81a4c_23.tar.bz2#60f48cef2d50674e0428c5579b6c3f66
-https://conda.anaconda.org/conda-forge/osx-64/sqlite-3.39.0-hd9f0692_0.tar.bz2#956223b8f1d808bab8ca9d8fb08778ec
+https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-9_5_0_h97931a8_26.tar.bz2#ac9c1a84323edab6c3ff9d3e586ab3cc
+https://conda.anaconda.org/conda-forge/osx-64/python-3.10.6-hc14f532_0_cpython.tar.bz2#9b19a68323edeaedb2ee94942c1ec017
 https://conda.anaconda.org/conda-forge/osx-64/udunits2-2.2.28-h06ef574_0.tar.bz2#74131a7d532fbff820580d4494118245
-https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.20-openmp_hb3cd9ec_0.tar.bz2#d862e4a5c6e7bf0bc9d66a38f5c73142
-https://conda.anaconda.org/conda-forge/osx-64/python-3.8.13-h394c593_0_cpython.tar.bz2#6d0c7bf13396e2f00e57cbd929f697f8
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.12-py_0.tar.bz2#2489a97287f90176ecdc3ca982b4b0a0
-https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
+https://conda.anaconda.org/conda-forge/noarch/attrs-22.1.0-pyh71513ae_1.tar.bz2#6d3ccbc56256204925bfa8378722792f
+https://conda.anaconda.org/conda-forge/noarch/certifi-2022.9.24-pyhd8ed1ab_0.tar.bz2#f66309b099374af91369e67e84af397d
 https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2#ebb5f5f7dc4f1a3780ef7ea7738db08c
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.0-pyhd8ed1ab_0.tar.bz2#abc0453b6e7bfbb87d275d58e333fc98
-https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.5-pyhd8ed1ab_0.tar.bz2#c267da48ce208905d7d976d49dfd9433
-https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.4-pyhd8ed1ab_0.tar.bz2#7b50d840543d9cdae100e91582c33035
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.7.1-pyhd8ed1ab_0.tar.bz2#7556872687250e0ea038eb503da3c44b
-https://conda.anaconda.org/conda-forge/noarch/idna-3.3-pyhd8ed1ab_0.tar.bz2#40b50b8b030f5f2f22085c062ed013dd
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.1-pyhd8ed1ab_0.tar.bz2#c1d5b294fbf9a795dec349a6f4d8be8e
+https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
+https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2#b65b4d50dbd2d50fa0aeac367ec9eed7
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.0.4-pyhd8ed1ab_0.tar.bz2#e0734d1f12de77f9daca98bda3428733
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.8.0-pyhd8ed1ab_0.tar.bz2#10f0218dbd493ab2e5dc6759ddea4526
+https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-1.1.1-pyh9f0ad1d_0.tar.bz2#39161f81cc5e5ca45b8226fbb06c6905
-https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-15_osx64_openblas.tar.bz2#48c26d27a96c71cfae2621311aa06215
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.1-pyhd8ed1ab_0.tar.bz2#d5df87964a39f67c46a5448f4e78d9b6
-https://conda.anaconda.org/conda-forge/noarch/py-1.11.0-pyh6c4a22f_0.tar.bz2#b4613d7e7a493916d867842a6a148054
+https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.21-openmp_h429af6e_3.tar.bz2#968c46aa7f4032c3f3873f3452ed4c34
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.2-pyhd8ed1ab_1.tar.bz2#2fb3f88922e7aec26ba652fcdfe13950
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
-https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-2_cp38.tar.bz2#156803acb0247c263c9586f190b72f1c
-https://conda.anaconda.org/conda-forge/noarch/pytz-2022.1-pyhd8ed1ab_0.tar.bz2#b87d66d6d3991d988fb31510c95a9267
-https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
+https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.10-2_cp310.tar.bz2#502ca4a8b43b424316f380d864832877
+https://conda.anaconda.org/conda-forge/noarch/pytz-2022.6-pyhd8ed1ab_0.tar.bz2#b1f26ad83328e486910ef7f6e81dc061
+https://conda.anaconda.org/conda-forge/noarch/setuptools-65.5.1-pyhd8ed1ab_0.tar.bz2#cfb8dc4d9d285ca5fb1177b9dd450e33
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.2-py_0.tar.bz2#20b2eaeaeea4ef9a9a0d99770620fd09
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.0-pyhd8ed1ab_0.tar.bz2#77dad82eb9c8c1525ff7953e0756d708
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.3.0-pyha770c72_0.tar.bz2#a9d85960bc62d53cc4ea0d1d27f73c98
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.37.1-pyhd8ed1ab_0.tar.bz2#1ca02aaf78d9c70d9a81a3bed5752022
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.8.0-pyhd8ed1ab_0.tar.bz2#050b94cf4a8c760656e51d2d44e4632c
-https://conda.anaconda.org/conda-forge/osx-64/antlr-python-runtime-4.7.2-py38h50d1736_1003.tar.bz2#2bec12040acb2867173db5d4f6bd4d62
-https://conda.anaconda.org/conda-forge/noarch/babel-2.10.3-pyhd8ed1ab_0.tar.bz2#72f1c6d03109d7a70087bc1d029a8eda
-https://conda.anaconda.org/conda-forge/osx-64/certifi-2022.6.15-py38h50d1736_0.tar.bz2#15c9cfd8dba4059423e558bed3a10ed9
-https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py38h86886aa_0.tar.bz2#fe186a0e00ae437c95dac9df968bd5b4
-https://conda.anaconda.org/conda-forge/osx-64/coverage-6.4.1-py38h0dd4459_0.tar.bz2#e2df6acb440ee1d1062d89d01013be39
-https://conda.anaconda.org/conda-forge/osx-64/cython-0.29.30-py38h1c67a95_0.tar.bz2#df9a04a3bac1fc8988e2de23cc123f2d
-https://conda.anaconda.org/conda-forge/osx-64/docutils-0.18.1-py38h50d1736_1.tar.bz2#e822e3f052bd5216f620d618b3b6d4d7
-https://conda.anaconda.org/conda-forge/osx-64/importlib-metadata-4.11.4-py38h50d1736_0.tar.bz2#0d6e3d579cdc3b3ec70bb174cf8802ba
-https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-15_osx64_openblas.tar.bz2#2d26f8ba1e89bcc2704ac7a38d4cc74c
-https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-15_osx64_openblas.tar.bz2#8679c41f1fcb5b54aaecce18ec3e1875
-https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.1-py38hed1de0f_1.tar.bz2#a353e85eb742fcfa2496c9f64b053354
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.4.0-pyha770c72_0.tar.bz2#2d93b130d148d7fc77e583677792fc6a
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.38.4-pyhd8ed1ab_0.tar.bz2#c829cfb8cb826acb9de0ac1a2df0a940
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.10.0-pyhd8ed1ab_0.tar.bz2#cd4eb48ebde7de61f92252979aab515c
+https://conda.anaconda.org/conda-forge/osx-64/antlr-python-runtime-4.7.2-py310h2ec42d9_1003.tar.bz2#647c94b9631bbeb2bea8557a81600980
+https://conda.anaconda.org/conda-forge/noarch/babel-2.11.0-pyhd8ed1ab_0.tar.bz2#2ea70fde8d581ba9425a761609eed6ba
+https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py310ha78151a_2.tar.bz2#dacdbcd6bcec3dc5b34f1f6a06915b66
+https://conda.anaconda.org/conda-forge/osx-64/coverage-6.5.0-py310h90acd4f_1.tar.bz2#36ab933f9eab0a2f25f032311715a726
+https://conda.anaconda.org/conda-forge/osx-64/cython-0.29.32-py310h7a76584_1.tar.bz2#3c1d5b388c47fe199df1c12d9918a830
+https://conda.anaconda.org/conda-forge/osx-64/docutils-0.19-py310h2ec42d9_1.tar.bz2#932d057a35046e6eb92561c723d4ebe6
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-5.0.0-pyha770c72_1.tar.bz2#ec069c4db6a0ad84107bac5da62819d2
+https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-16_osx64_openblas.tar.bz2#644d63e9379867490b67bace400b2a0f
+https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.1-py310h90acd4f_2.tar.bz2#232c20719e4290fa284ae1e9a4661dfa
+https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
 https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2#71f1ab2de48613876becddd496371c85
-https://conda.anaconda.org/conda-forge/osx-64/pluggy-1.0.0-py38h50d1736_3.tar.bz2#49de2850464c426eec1959b97858ec58
-https://conda.anaconda.org/conda-forge/osx-64/pysocks-1.7.1-py38h50d1736_5.tar.bz2#b417ade9775612d9a2520b12bbab2cb0
-https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py38hed1de0f_4.tar.bz2#827c0e27214cb208fa43fe4d6230546e
-https://conda.anaconda.org/conda-forge/osx-64/setuptools-63.1.0-py38h50d1736_0.tar.bz2#6919c07eb88c1c442bcdd9c239d5e9fb
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.3.0-hd8ed1ab_0.tar.bz2#f3e98e944832fb271a0dbda7b7771dc6
-https://conda.anaconda.org/conda-forge/osx-64/virtualenv-20.15.1-py38h50d1736_0.tar.bz2#e7f9ab382ab9862c28db563eedb16ea9
-https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py38hed1de0f_1004.tar.bz2#157c0392031cd8d8c3153f92121642de
-https://conda.anaconda.org/conda-forge/osx-64/cryptography-37.0.4-py38h0f8513e_0.tar.bz2#ecb981de30cbb99043b5399039c7446b
+https://conda.anaconda.org/conda-forge/noarch/pip-22.3.1-pyhd8ed1ab_0.tar.bz2#da66f2851b9836d3a7c5190082a45f7d
+https://conda.anaconda.org/conda-forge/noarch/pygments-2.13.0-pyhd8ed1ab_0.tar.bz2#9f478e8eedd301008b5f395bad0caaed
+https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py310h90acd4f_5.tar.bz2#e0ba2009f52ccda088c63dedf0d1c5ec
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.4.0-hd8ed1ab_0.tar.bz2#be969210b61b897775a0de63cd9e9026
+https://conda.anaconda.org/conda-forge/osx-64/virtualenv-20.16.7-py310h2ec42d9_0.tar.bz2#014dba342fdf74479c3250e949e51c55
+https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py310h90acd4f_1005.tar.bz2#63accc45f2b9ae1dad4db9cdfaa903b4
+https://conda.anaconda.org/conda-forge/osx-64/cryptography-38.0.3-py310hdd0c95c_0.tar.bz2#c2f16aca866a1c60fc5dfad6ba4c9158
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
-https://conda.anaconda.org/conda-forge/osx-64/numpy-1.23.1-py38h604f2a5_0.tar.bz2#41bf5f397b17a1619a43756163e785c9
-https://conda.anaconda.org/conda-forge/noarch/pip-22.1.2-pyhd8ed1ab_0.tar.bz2#d29185c662a424f8bea1103270b85c96
-https://conda.anaconda.org/conda-forge/noarch/pygments-2.12.0-pyhd8ed1ab_0.tar.bz2#cb27e2ded147e5bcc7eafc1c6d343cb3
-https://conda.anaconda.org/conda-forge/osx-64/pytest-7.1.2-py38h50d1736_0.tar.bz2#ab3679da5581765f2fa1b0a16ca89a03
-https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.4-pyhd8ed1ab_0.tar.bz2#dff6862ca0b54bbeab8ddf657d032920
-https://conda.anaconda.org/conda-forge/osx-64/ukkonen-1.0.1-py38h8b7791e_2.tar.bz2#e3b3dbd512c27223c7df30a185780152
-https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.1-py38hc1426ef_0.tar.bz2#c2fe5d23792e6e1927509c72ac1673f8
-https://conda.anaconda.org/conda-forge/noarch/identify-2.5.1-pyhd8ed1ab_0.tar.bz2#6f41e3056fcd3061fbc2b49b3309fe0c
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.0.0-pyhd8ed1ab_0.tar.bz2#1d7e241dfaf5475e893d4b824bb71b44
-https://conda.anaconda.org/conda-forge/noarch/pytest-cov-3.0.0-pyhd8ed1ab_0.tar.bz2#0f7cac11bb696b62d378bde725bfc3eb
-https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.4-hd8ed1ab_0.tar.bz2#b068a47ce183af12a53c6b0d84f96085
-https://conda.anaconda.org/conda-forge/osx-64/pre-commit-2.19.0-py38h50d1736_0.tar.bz2#13241d949a7f164a98bd385f963382b8
-https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.10-pyhd8ed1ab_0.tar.bz2#14f22c5b9cfd0d93c2806faaa3fe6dec
-https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_0.tar.bz2#70d6e72856de9551f83ae0f2de689a7a
+https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-16_osx64_openblas.tar.bz2#28592eab0f05bcf9969789e87f754e11
+https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-16_osx64_openblas.tar.bz2#406ad426aade5578b90544cc2ed4a79b
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.2.0-pyhd8ed1ab_2.tar.bz2#ac82c7aebc282e6ac0450fca012ca78c
+https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.5-pyhd8ed1ab_1.tar.bz2#07037fe2931871ed69b2b3d2acd5fdc6
+https://conda.anaconda.org/conda-forge/osx-64/ukkonen-1.0.1-py310ha23aa8a_3.tar.bz2#b3727e37919b1f4ef885d65ed97f3ca1
+https://conda.anaconda.org/conda-forge/noarch/identify-2.5.8-pyhd8ed1ab_0.tar.bz2#8001c46448f385fa43bc4221893704d2
+https://conda.anaconda.org/conda-forge/osx-64/numpy-1.23.4-py310h1b7c290_1.tar.bz2#83930a7444dab73641a2dd927f3c6a0d
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.1.0-pyhd8ed1ab_0.tar.bz2#fbfa0a180d48c800f922a10a114a8632
+https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.0.0-pyhd8ed1ab_0.tar.bz2#c9e3f8bfdb9bfc34aa1836a6ed4b25d7
+https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.5-hd8ed1ab_1.tar.bz2#6b7cb927a5c505b16b4b4241825e068c
+https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.2-py310h936d966_1.tar.bz2#fcc07bec2f8577cc1a8009cef81f78ff
+https://conda.anaconda.org/conda-forge/osx-64/pre-commit-2.20.0-py310h2ec42d9_1.tar.bz2#f6b6551cdd230ca9a94c6995d495bf72
+https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.11-pyhd8ed1ab_0.tar.bz2#0738978569b10669bdef41c671252dd1
+https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_1.tar.bz2#089382ee0e2dc2eae33a04cc3c2bddb0
 https://conda.anaconda.org/conda-forge/noarch/codecov-2.1.11-pyhd3deb0d_0.tar.bz2#9c661c2c14b4667827218402e6624ad5
-https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.2-pyh6c4a22f_0.tar.bz2#d4eaa1f50733a377480ce1d5aac556c7
+https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
```

### Comparing `cf-units-3.1.1/requirements/locks/py38-lock-win-64.txt` & `cf-units-3.2.0/requirements/locks/py38-lock-win-64.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,92 +1,90 @@
 # Generated by conda-lock.
 # platform: win-64
-# input_hash: b8c36dcda628c0ab25b6b3a132dd08c70d85b5579d646eb59d038779f204e13e
+# input_hash: 1de6d7e320845d8daa22702c0c6fdd52501382981883582cbae39dc02f13a1b3
 @EXPLICIT
-https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2022.6.15-h5b45459_0.tar.bz2#b84069692c33afe59f31c7117c80696e
+https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2022.9.24-h5b45459_0.tar.bz2#5fba0abc60bf327a4bc4188cd64678be
 https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2022.1.0-h57928b3_3787.tar.bz2#35dff2b6e944ce136a574c4c006cec28
-https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.20348.0-h57928b3_0.tar.bz2#6d666b6ea8251231ff508062d1e41f9c
-https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.29.30037-h902a5da_6.tar.bz2#33d07ebe91062743eabc9e53a60d18e1
-https://conda.anaconda.org/conda-forge/win-64/vc-14.2-hb210afc_6.tar.bz2#c2aecbc9b00ba6f352e27d3d61fd31fb
+https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
+https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.32.31332-h1d6e394_9.tar.bz2#c98b6e39006315599b793592bcc3c978
+https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h3d8a991_9.tar.bz2#ba28983ef4f6d430827d0e7c5cdd7b48
 https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
-https://conda.anaconda.org/conda-forge/win-64/expat-2.4.8-h39d44d4_0.tar.bz2#f8e0f53713756c08456f50c9ce25748c
+https://conda.anaconda.org/conda-forge/win-64/expat-2.5.0-h1537add_0.tar.bz2#6b20c31bd735d2dd5c79ddb5b3524619
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
-https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.12-h8ffe710_1.tar.bz2#8b67614ab0539e803c03db2ed7990c6c
-https://conda.anaconda.org/conda-forge/win-64/openssl-1.1.1q-h8ffe710_0.tar.bz2#2ee16f406ee12fe4dcd08b513e9bd0c6
-https://conda.anaconda.org/conda-forge/win-64/sqlite-3.39.0-h8ffe710_0.tar.bz2#c76b39a7a74df1875e7b2b3fb5549632
-https://conda.anaconda.org/conda-forge/win-64/tbb-2021.5.0-h2d74725_1.tar.bz2#8f00f39dbd7deaba11410b0b6e7b2cb4
+https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.40.0-hcfcfb64_0.tar.bz2#5e5a97795de72f8cc3baf3d9ea6327a2
+https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_4.tar.bz2#0cc5c5cc64ee1637f37f8540a175854c
+https://conda.anaconda.org/conda-forge/win-64/openssl-3.0.7-hcfcfb64_0.tar.bz2#a87ab36dc95970e3b4b63b7599bebdbe
+https://conda.anaconda.org/conda-forge/win-64/tbb-2021.7.0-h91493d7_0.tar.bz2#f57be598137919e4f7e7d159960d66a1
 https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
-https://conda.anaconda.org/conda-forge/win-64/xz-5.2.5-h62dcd97_1.tar.bz2#eabcbfedd14d7c18a514afca09ea0ebb
+https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
 https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
 https://conda.anaconda.org/conda-forge/win-64/mkl-2022.1.0-h6a75c08_874.tar.bz2#2ff89a7337a9636029b4db9466e9f8e3
-https://conda.anaconda.org/conda-forge/win-64/python-3.8.13-h9a09f29_0_cpython.tar.bz2#41de0ad5db009f4f829f9d415a6a4200
+https://conda.anaconda.org/conda-forge/win-64/sqlite-3.40.0-hcfcfb64_0.tar.bz2#c71d4be22d8402e7e17386aeb18b930e
 https://conda.anaconda.org/conda-forge/win-64/udunits2-2.2.28-h892ecd3_0.tar.bz2#dad8b5fae263e4e36d859524a3794801
+https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-16_win64_mkl.tar.bz2#d2e6f4e86cee2b4e8c27ff6884ccdc61
+https://conda.anaconda.org/conda-forge/win-64/python-3.8.13-hcf16a7b_0_cpython.tar.bz2#f7f182fd26238021044097981fd25a4e
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.12-py_0.tar.bz2#2489a97287f90176ecdc3ca982b4b0a0
-https://conda.anaconda.org/conda-forge/noarch/atomicwrites-1.4.1-pyhd8ed1ab_0.tar.bz2#1714887104aab113bde64001ceb17262
-https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
+https://conda.anaconda.org/conda-forge/noarch/attrs-22.1.0-pyh71513ae_1.tar.bz2#6d3ccbc56256204925bfa8378722792f
+https://conda.anaconda.org/conda-forge/noarch/certifi-2022.9.24-pyhd8ed1ab_0.tar.bz2#f66309b099374af91369e67e84af397d
 https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2#ebb5f5f7dc4f1a3780ef7ea7738db08c
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.0-pyhd8ed1ab_0.tar.bz2#abc0453b6e7bfbb87d275d58e333fc98
-https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.5-pyhd8ed1ab_0.tar.bz2#c267da48ce208905d7d976d49dfd9433
-https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.4-pyhd8ed1ab_0.tar.bz2#7b50d840543d9cdae100e91582c33035
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.7.1-pyhd8ed1ab_0.tar.bz2#7556872687250e0ea038eb503da3c44b
-https://conda.anaconda.org/conda-forge/noarch/idna-3.3-pyhd8ed1ab_0.tar.bz2#40b50b8b030f5f2f22085c062ed013dd
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.1-pyhd8ed1ab_0.tar.bz2#c1d5b294fbf9a795dec349a6f4d8be8e
+https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
+https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2#b65b4d50dbd2d50fa0aeac367ec9eed7
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.0.4-pyhd8ed1ab_0.tar.bz2#e0734d1f12de77f9daca98bda3428733
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.8.0-pyhd8ed1ab_0.tar.bz2#10f0218dbd493ab2e5dc6759ddea4526
+https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-1.1.1-pyh9f0ad1d_0.tar.bz2#39161f81cc5e5ca45b8226fbb06c6905
-https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-15_win64_mkl.tar.bz2#661187f959fed1821cdd6921a738336d
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.1-pyhd8ed1ab_0.tar.bz2#d5df87964a39f67c46a5448f4e78d9b6
-https://conda.anaconda.org/conda-forge/noarch/py-1.11.0-pyh6c4a22f_0.tar.bz2#b4613d7e7a493916d867842a6a148054
+https://conda.anaconda.org/conda-forge/win-64/libcblas-3.9.0-16_win64_mkl.tar.bz2#14c2fb03b2bb14dfa3806186ca91d557
+https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-16_win64_mkl.tar.bz2#be2f9d5712a5bb05cd900005ee752a05
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.2-pyhd8ed1ab_1.tar.bz2#2fb3f88922e7aec26ba652fcdfe13950
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/win-64/python_abi-3.8-2_cp38.tar.bz2#80b95487563108d4cf92ff6384050751
-https://conda.anaconda.org/conda-forge/noarch/pytz-2022.1-pyhd8ed1ab_0.tar.bz2#b87d66d6d3991d988fb31510c95a9267
-https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+https://conda.anaconda.org/conda-forge/noarch/pytz-2022.6-pyhd8ed1ab_0.tar.bz2#b1f26ad83328e486910ef7f6e81dc061
+https://conda.anaconda.org/conda-forge/noarch/setuptools-65.5.1-pyhd8ed1ab_0.tar.bz2#cfb8dc4d9d285ca5fb1177b9dd450e33
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.2-py_0.tar.bz2#20b2eaeaeea4ef9a9a0d99770620fd09
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.0-pyhd8ed1ab_0.tar.bz2#77dad82eb9c8c1525ff7953e0756d708
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.3.0-pyha770c72_0.tar.bz2#a9d85960bc62d53cc4ea0d1d27f73c98
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.37.1-pyhd8ed1ab_0.tar.bz2#1ca02aaf78d9c70d9a81a3bed5752022
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.8.0-pyhd8ed1ab_0.tar.bz2#050b94cf4a8c760656e51d2d44e4632c
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.4.0-pyha770c72_0.tar.bz2#2d93b130d148d7fc77e583677792fc6a
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.38.4-pyhd8ed1ab_0.tar.bz2#c829cfb8cb826acb9de0ac1a2df0a940
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.10.0-pyhd8ed1ab_0.tar.bz2#cd4eb48ebde7de61f92252979aab515c
 https://conda.anaconda.org/conda-forge/win-64/antlr-python-runtime-4.7.2-py38haa244fe_1003.tar.bz2#2c5af71a6a0af1bbc13e5a90fd6994a7
-https://conda.anaconda.org/conda-forge/noarch/babel-2.10.3-pyhd8ed1ab_0.tar.bz2#72f1c6d03109d7a70087bc1d029a8eda
-https://conda.anaconda.org/conda-forge/win-64/certifi-2022.6.15-py38haa244fe_0.tar.bz2#88eb5b7ef2bb7238573273a6ff04e461
-https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py38hd8c33c5_0.tar.bz2#6039ace67b5ab57a65d5335e62e14656
-https://conda.anaconda.org/conda-forge/win-64/coverage-6.4.1-py38h294d835_0.tar.bz2#fa2dbdc7e9995695030afb133f4f4bb4
-https://conda.anaconda.org/conda-forge/win-64/cython-0.29.30-py38h885f38d_0.tar.bz2#7cdd65a187c9c04207b394b67c6cf64b
-https://conda.anaconda.org/conda-forge/win-64/docutils-0.18.1-py38haa244fe_1.tar.bz2#a0925f3b4d9e941c9363bc15a865ba6b
-https://conda.anaconda.org/conda-forge/win-64/importlib-metadata-4.11.4-py38haa244fe_0.tar.bz2#a62d4bc7fda74924b9979fe227cfce0f
-https://conda.anaconda.org/conda-forge/win-64/libcblas-3.9.0-15_win64_mkl.tar.bz2#c6012601cd7dde1b4108128fb847de9f
-https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-15_win64_mkl.tar.bz2#7915daedfea4cc94ffcaa71cde184f50
-https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.1-py38h294d835_1.tar.bz2#bdd30c12b6f30761710781b9f3a17153
+https://conda.anaconda.org/conda-forge/noarch/babel-2.11.0-pyhd8ed1ab_0.tar.bz2#2ea70fde8d581ba9425a761609eed6ba
+https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py38h57701bc_2.tar.bz2#4e290e24ff3aa60183f928d4e144c4fb
+https://conda.anaconda.org/conda-forge/win-64/coverage-6.5.0-py38h91455d4_1.tar.bz2#7ba1bb13999b89fdce5f3385d5e28c2b
+https://conda.anaconda.org/conda-forge/win-64/cython-0.29.32-py38hd3f51b4_1.tar.bz2#cae84cafa303ba6c676bdcc3047bfa08
+https://conda.anaconda.org/conda-forge/win-64/docutils-0.19-py38haa244fe_1.tar.bz2#24070757ab686062b4b329d44ba40919
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-5.0.0-pyha770c72_1.tar.bz2#ec069c4db6a0ad84107bac5da62819d2
+https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.1-py38h91455d4_2.tar.bz2#c745139f04bbdd7a8ba9a1f5e95838c1
+https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
+https://conda.anaconda.org/conda-forge/win-64/numpy-1.23.4-py38h90ce339_1.tar.bz2#45762f734e80979a46853f74984b25a5
 https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2#71f1ab2de48613876becddd496371c85
-https://conda.anaconda.org/conda-forge/win-64/pluggy-1.0.0-py38haa244fe_3.tar.bz2#bd23d4e34ce9647a448d8048be89b2dd
-https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py38h294d835_4.tar.bz2#ed6594bdc18612c07ba434428759a7cb
-https://conda.anaconda.org/conda-forge/win-64/setuptools-63.1.0-py38haa244fe_0.tar.bz2#3f9ecb2bc747e8e0ba18e557c1b0b8bf
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.3.0-hd8ed1ab_0.tar.bz2#f3e98e944832fb271a0dbda7b7771dc6
-https://conda.anaconda.org/conda-forge/win-64/virtualenv-20.15.1-py38haa244fe_0.tar.bz2#41cfdac3e0d5d37a2b9953273d5d1781
-https://conda.anaconda.org/conda-forge/win-64/win_inet_pton-1.1.0-py38haa244fe_4.tar.bz2#8adadd81dc9c22710b69628ec6e6d41a
-https://conda.anaconda.org/conda-forge/win-64/brotlipy-0.7.0-py38h294d835_1004.tar.bz2#f12a527d29a252cef0abbfd752d3ab01
-https://conda.anaconda.org/conda-forge/win-64/cryptography-37.0.4-py38hb7941b4_0.tar.bz2#9498b6b13423971d96da00e5e98b88d2
+https://conda.anaconda.org/conda-forge/noarch/pip-22.3.1-pyhd8ed1ab_0.tar.bz2#da66f2851b9836d3a7c5190082a45f7d
+https://conda.anaconda.org/conda-forge/noarch/pygments-2.13.0-pyhd8ed1ab_0.tar.bz2#9f478e8eedd301008b5f395bad0caaed
+https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py38h91455d4_5.tar.bz2#f62ab7e18711e3cbc068319448ecf771
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.4.0-hd8ed1ab_0.tar.bz2#be969210b61b897775a0de63cd9e9026
+https://conda.anaconda.org/conda-forge/win-64/virtualenv-20.16.7-py38haa244fe_0.tar.bz2#59b5c2aa91dd40576a5a014432dcad87
+https://conda.anaconda.org/conda-forge/win-64/brotlipy-0.7.0-py38h91455d4_1005.tar.bz2#9fabc7fadfb37addbe91cc67c09cda69
+https://conda.anaconda.org/conda-forge/win-64/cftime-1.6.2-py38hbaf524b_1.tar.bz2#38212e2289cd9946fc92eabb9ef78bb8
+https://conda.anaconda.org/conda-forge/win-64/cryptography-38.0.3-py38h95f5157_0.tar.bz2#acaf9ff637ae6d38cdda4aba9bacf734
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
-https://conda.anaconda.org/conda-forge/win-64/numpy-1.23.1-py38h223ccf5_0.tar.bz2#cc2580ede01216335dece5e24e7382fe
-https://conda.anaconda.org/conda-forge/noarch/pip-22.1.2-pyhd8ed1ab_0.tar.bz2#d29185c662a424f8bea1103270b85c96
-https://conda.anaconda.org/conda-forge/noarch/pygments-2.12.0-pyhd8ed1ab_0.tar.bz2#cb27e2ded147e5bcc7eafc1c6d343cb3
-https://conda.anaconda.org/conda-forge/win-64/pysocks-1.7.1-py38haa244fe_5.tar.bz2#81fd9157802c3d99efc4a24563cfe885
-https://conda.anaconda.org/conda-forge/win-64/pytest-7.1.2-py38haa244fe_0.tar.bz2#523814dad1e91a414e8e449aae2202ec
-https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.4-pyhd8ed1ab_0.tar.bz2#dff6862ca0b54bbeab8ddf657d032920
-https://conda.anaconda.org/conda-forge/win-64/ukkonen-1.0.1-py38hbd9d945_2.tar.bz2#631db1d5cccbe3cd67f8e74995f7ca2a
-https://conda.anaconda.org/conda-forge/win-64/cftime-1.6.1-py38hbdcd294_0.tar.bz2#6bbf42b1185009092929ba1e1532dd1d
-https://conda.anaconda.org/conda-forge/noarch/identify-2.5.1-pyhd8ed1ab_0.tar.bz2#6f41e3056fcd3061fbc2b49b3309fe0c
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.0.0-pyhd8ed1ab_0.tar.bz2#1d7e241dfaf5475e893d4b824bb71b44
-https://conda.anaconda.org/conda-forge/noarch/pytest-cov-3.0.0-pyhd8ed1ab_0.tar.bz2#0f7cac11bb696b62d378bde725bfc3eb
-https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.4-hd8ed1ab_0.tar.bz2#b068a47ce183af12a53c6b0d84f96085
-https://conda.anaconda.org/conda-forge/win-64/pre-commit-2.19.0-py38haa244fe_0.tar.bz2#7de5db465307310c7f215a63cb182e6f
-https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.10-pyhd8ed1ab_0.tar.bz2#14f22c5b9cfd0d93c2806faaa3fe6dec
-https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_0.tar.bz2#70d6e72856de9551f83ae0f2de689a7a
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.2.0-pyhd8ed1ab_2.tar.bz2#ac82c7aebc282e6ac0450fca012ca78c
+https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.5-pyhd8ed1ab_1.tar.bz2#07037fe2931871ed69b2b3d2acd5fdc6
+https://conda.anaconda.org/conda-forge/win-64/ukkonen-1.0.1-py38hb1fd069_3.tar.bz2#8f1c0c4b1de3472bc880fd55648d36ab
+https://conda.anaconda.org/conda-forge/noarch/identify-2.5.8-pyhd8ed1ab_0.tar.bz2#8001c46448f385fa43bc4221893704d2
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.1.0-pyhd8ed1ab_0.tar.bz2#fbfa0a180d48c800f922a10a114a8632
+https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.0.0-pyhd8ed1ab_0.tar.bz2#c9e3f8bfdb9bfc34aa1836a6ed4b25d7
+https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.5-hd8ed1ab_1.tar.bz2#6b7cb927a5c505b16b4b4241825e068c
+https://conda.anaconda.org/conda-forge/win-64/pre-commit-2.20.0-py38haa244fe_1.tar.bz2#373f9bcad5ae81e34c9ccf673b402626
+https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.11-pyhd8ed1ab_0.tar.bz2#0738978569b10669bdef41c671252dd1
+https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_1.tar.bz2#089382ee0e2dc2eae33a04cc3c2bddb0
 https://conda.anaconda.org/conda-forge/noarch/codecov-2.1.11-pyhd3deb0d_0.tar.bz2#9c661c2c14b4667827218402e6624ad5
-https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.2-pyh6c4a22f_0.tar.bz2#d4eaa1f50733a377480ce1d5aac556c7
+https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
```

### Comparing `cf-units-3.1.1/requirements/locks/py39-lock-linux-64.txt` & `cf-units-3.2.0/requirements/locks/py39-lock-win-64.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,99 +1,91 @@
 # Generated by conda-lock.
-# platform: linux-64
-# input_hash: 3a40bd39abc099d2566e23d479f135e9d94f78c7981a7f98e24b2dada080f260
+# platform: win-64
+# input_hash: c7074f810e8e7b783a0265bd06acaced425cf19976fa69b161266906ec591a77
 @EXPLICIT
-https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
-https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2022.6.15-ha878542_0.tar.bz2#c320890f77fd1d617fa876e0982002c2
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.36.1-hea4e1c9_2.tar.bz2#bd4f2e711b39af170e7ff15163fe87ee
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-12.1.0-hdcd56e2_16.tar.bz2#b02605b875559ff99f04351fd5040760
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.1.0-ha89aaad_16.tar.bz2#6f5ba041a41eb102a1027d9e68731be7
-https://conda.anaconda.org/conda-forge/noarch/tzdata-2022a-h191b570_0.tar.bz2#84be5301069417a2221187d2f435e0f7
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-12.1.0-h69a702a_16.tar.bz2#6bf15e29a20f614b18ae89368260d0a2
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.1.0-h8d9b700_16.tar.bz2#f013cf7749536ce43d82afbffdf499ab
-https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.1.0-h8d9b700_16.tar.bz2#4f05bc9844f7c101e6e147dab3c88d5c
-https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
-https://conda.anaconda.org/conda-forge/linux-64/expat-2.4.8-h27087fc_0.tar.bz2#e1b07832504eeba765d648389cc387a9
-https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
-https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
-https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.20-pthreads_h78a6416_0.tar.bz2#9b6d0781953c9e353faee494336cc229
-https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.32.1-h7f98852_1000.tar.bz2#772d69f030955d9646d3d0eaf21d859d
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.12-h166bdaf_1.tar.bz2#58eaff4f91891978af3625e7bbf958af
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2#4acfc691e64342b9dae57cf2adc63238
-https://conda.anaconda.org/conda-forge/linux-64/openssl-1.1.1q-h166bdaf_0.tar.bz2#07acc367c7fc8b716770cd5b36d31717
-https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.5-h516909a_1.tar.bz2#33f601066901f3e1a85af3522a8113f9
-https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
-https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-15_linux64_openblas.tar.bz2#04eb983975a1be3e57d6d667414cd774
-https://conda.anaconda.org/conda-forge/linux-64/readline-8.1.2-h0f457ee_0.tar.bz2#db2ebbe2943aae81ed051a6a9af8e0fa
-https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
-https://conda.anaconda.org/conda-forge/linux-64/udunits2-2.2.28-hc3e0081_0.tar.bz2#d4c341e0379c31e9e781d4f204726867
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.12-h166bdaf_1.tar.bz2#e4b67f2b4096807cd7d836227c026a43
-https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-15_linux64_openblas.tar.bz2#f45968428e445fd0c6472b561145812a
-https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-15_linux64_openblas.tar.bz2#b7078220384b8bf8db1a45e66412ac4f
-https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.39.0-h4ff8645_0.tar.bz2#ead30581ba8cfd52d69632868b844d4a
-https://conda.anaconda.org/conda-forge/linux-64/python-3.9.13-h9a8a25e_0_cpython.tar.bz2#69bc307cc4d7396c5fccb26bbcc9c379
+https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2022.9.24-h5b45459_0.tar.bz2#5fba0abc60bf327a4bc4188cd64678be
+https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2022.1.0-h57928b3_3787.tar.bz2#35dff2b6e944ce136a574c4c006cec28
+https://conda.anaconda.org/conda-forge/noarch/tzdata-2022f-h191b570_0.tar.bz2#e366350e2343a798e29833286abe2560
+https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
+https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.32.31332-h1d6e394_9.tar.bz2#c98b6e39006315599b793592bcc3c978
+https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h3d8a991_9.tar.bz2#ba28983ef4f6d430827d0e7c5cdd7b48
+https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
+https://conda.anaconda.org/conda-forge/win-64/expat-2.5.0-h1537add_0.tar.bz2#6b20c31bd735d2dd5c79ddb5b3524619
+https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
+https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.40.0-hcfcfb64_0.tar.bz2#5e5a97795de72f8cc3baf3d9ea6327a2
+https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_4.tar.bz2#0cc5c5cc64ee1637f37f8540a175854c
+https://conda.anaconda.org/conda-forge/win-64/openssl-3.0.7-hcfcfb64_0.tar.bz2#a87ab36dc95970e3b4b63b7599bebdbe
+https://conda.anaconda.org/conda-forge/win-64/tbb-2021.7.0-h91493d7_0.tar.bz2#f57be598137919e4f7e7d159960d66a1
+https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
+https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
+https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
+https://conda.anaconda.org/conda-forge/win-64/mkl-2022.1.0-h6a75c08_874.tar.bz2#2ff89a7337a9636029b4db9466e9f8e3
+https://conda.anaconda.org/conda-forge/win-64/sqlite-3.40.0-hcfcfb64_0.tar.bz2#c71d4be22d8402e7e17386aeb18b930e
+https://conda.anaconda.org/conda-forge/win-64/udunits2-2.2.28-h892ecd3_0.tar.bz2#dad8b5fae263e4e36d859524a3794801
+https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-16_win64_mkl.tar.bz2#d2e6f4e86cee2b4e8c27ff6884ccdc61
+https://conda.anaconda.org/conda-forge/win-64/python-3.9.13-hcf16a7b_0_cpython.tar.bz2#6017838044b4b984cffd2600d31a11de
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.12-py_0.tar.bz2#2489a97287f90176ecdc3ca982b4b0a0
-https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
+https://conda.anaconda.org/conda-forge/noarch/attrs-22.1.0-pyh71513ae_1.tar.bz2#6d3ccbc56256204925bfa8378722792f
+https://conda.anaconda.org/conda-forge/noarch/certifi-2022.9.24-pyhd8ed1ab_0.tar.bz2#f66309b099374af91369e67e84af397d
 https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2#ebb5f5f7dc4f1a3780ef7ea7738db08c
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.0-pyhd8ed1ab_0.tar.bz2#abc0453b6e7bfbb87d275d58e333fc98
-https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.5-pyhd8ed1ab_0.tar.bz2#c267da48ce208905d7d976d49dfd9433
-https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.4-pyhd8ed1ab_0.tar.bz2#7b50d840543d9cdae100e91582c33035
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.7.1-pyhd8ed1ab_0.tar.bz2#7556872687250e0ea038eb503da3c44b
-https://conda.anaconda.org/conda-forge/noarch/idna-3.3-pyhd8ed1ab_0.tar.bz2#40b50b8b030f5f2f22085c062ed013dd
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.1-pyhd8ed1ab_0.tar.bz2#c1d5b294fbf9a795dec349a6f4d8be8e
+https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
+https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2#b65b4d50dbd2d50fa0aeac367ec9eed7
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.0.4-pyhd8ed1ab_0.tar.bz2#e0734d1f12de77f9daca98bda3428733
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.8.0-pyhd8ed1ab_0.tar.bz2#10f0218dbd493ab2e5dc6759ddea4526
+https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-1.1.1-pyh9f0ad1d_0.tar.bz2#39161f81cc5e5ca45b8226fbb06c6905
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.1-pyhd8ed1ab_0.tar.bz2#d5df87964a39f67c46a5448f4e78d9b6
-https://conda.anaconda.org/conda-forge/noarch/py-1.11.0-pyh6c4a22f_0.tar.bz2#b4613d7e7a493916d867842a6a148054
+https://conda.anaconda.org/conda-forge/win-64/libcblas-3.9.0-16_win64_mkl.tar.bz2#14c2fb03b2bb14dfa3806186ca91d557
+https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-16_win64_mkl.tar.bz2#be2f9d5712a5bb05cd900005ee752a05
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.2-pyhd8ed1ab_1.tar.bz2#2fb3f88922e7aec26ba652fcdfe13950
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
-https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.9-2_cp39.tar.bz2#39adde4247484de2bb4000122fdcf665
-https://conda.anaconda.org/conda-forge/noarch/pytz-2022.1-pyhd8ed1ab_0.tar.bz2#b87d66d6d3991d988fb31510c95a9267
-https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
+https://conda.anaconda.org/conda-forge/win-64/python_abi-3.9-2_cp39.tar.bz2#757068981fb2f97d0cadbba9ae6ae191
+https://conda.anaconda.org/conda-forge/noarch/pytz-2022.6-pyhd8ed1ab_0.tar.bz2#b1f26ad83328e486910ef7f6e81dc061
+https://conda.anaconda.org/conda-forge/noarch/setuptools-65.5.1-pyhd8ed1ab_0.tar.bz2#cfb8dc4d9d285ca5fb1177b9dd450e33
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.2-py_0.tar.bz2#20b2eaeaeea4ef9a9a0d99770620fd09
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.0-pyhd8ed1ab_0.tar.bz2#77dad82eb9c8c1525ff7953e0756d708
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.3.0-pyha770c72_0.tar.bz2#a9d85960bc62d53cc4ea0d1d27f73c98
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.37.1-pyhd8ed1ab_0.tar.bz2#1ca02aaf78d9c70d9a81a3bed5752022
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.8.0-pyhd8ed1ab_0.tar.bz2#050b94cf4a8c760656e51d2d44e4632c
-https://conda.anaconda.org/conda-forge/linux-64/antlr-python-runtime-4.7.2-py39hf3d152e_1003.tar.bz2#5e8330e806e50bd6137ebd125f4bc1bb
-https://conda.anaconda.org/conda-forge/noarch/babel-2.10.3-pyhd8ed1ab_0.tar.bz2#72f1c6d03109d7a70087bc1d029a8eda
-https://conda.anaconda.org/conda-forge/linux-64/certifi-2022.6.15-py39hf3d152e_0.tar.bz2#cf0efee4ef53a6d3ea4dce06ac360f14
-https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py39he91dace_0.tar.bz2#61e961a94c8fd535e4496b17e7452dfe
-https://conda.anaconda.org/conda-forge/linux-64/coverage-6.4.1-py39hb9d737c_0.tar.bz2#57b811f9997fcf49363b80b5d178dae9
-https://conda.anaconda.org/conda-forge/linux-64/cython-0.29.30-py39h5a03fae_0.tar.bz2#78d64530b059de26a60f979e02c9fa3c
-https://conda.anaconda.org/conda-forge/linux-64/docutils-0.18.1-py39hf3d152e_1.tar.bz2#9851752658704495f8adf28f6d2b3cb3
-https://conda.anaconda.org/conda-forge/linux-64/importlib-metadata-4.11.4-py39hf3d152e_0.tar.bz2#4c2a0eabf0b8980b2c755646a6f750eb
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.1-py39hb9d737c_1.tar.bz2#7cda413e43b252044a270c2477031c5c
-https://conda.anaconda.org/conda-forge/linux-64/numpy-1.23.1-py39hba7629e_0.tar.bz2#ee8dff1fb28e0e2c458e845aae9d915a
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.4.0-pyha770c72_0.tar.bz2#2d93b130d148d7fc77e583677792fc6a
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.38.4-pyhd8ed1ab_0.tar.bz2#c829cfb8cb826acb9de0ac1a2df0a940
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.10.0-pyhd8ed1ab_0.tar.bz2#cd4eb48ebde7de61f92252979aab515c
+https://conda.anaconda.org/conda-forge/win-64/antlr-python-runtime-4.7.2-py39hcbf5309_1003.tar.bz2#b0b10b9f91524f316108c3ce6d9afc4f
+https://conda.anaconda.org/conda-forge/noarch/babel-2.11.0-pyhd8ed1ab_0.tar.bz2#2ea70fde8d581ba9425a761609eed6ba
+https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py39h68f70e3_2.tar.bz2#706a5a7b26617c284987cc95d7465e18
+https://conda.anaconda.org/conda-forge/win-64/coverage-6.5.0-py39ha55989b_1.tar.bz2#412ce3bd1952cba354187ec33be37f5f
+https://conda.anaconda.org/conda-forge/win-64/cython-0.29.32-py39h99910a6_1.tar.bz2#c12c1819d4c119d3031eee21e9f14c96
+https://conda.anaconda.org/conda-forge/win-64/docutils-0.19-py39hcbf5309_1.tar.bz2#7d4d56a24614c7a919f3a39571997376
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-5.0.0-pyha770c72_1.tar.bz2#ec069c4db6a0ad84107bac5da62819d2
+https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.1-py39ha55989b_2.tar.bz2#b6dd8303ea8f1fc1417014b53742cef6
+https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
+https://conda.anaconda.org/conda-forge/win-64/numpy-1.23.4-py39hbccbffa_1.tar.bz2#5efa809d78fa26365de52841400e40a5
 https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2#71f1ab2de48613876becddd496371c85
-https://conda.anaconda.org/conda-forge/linux-64/pluggy-1.0.0-py39hf3d152e_3.tar.bz2#c375c89340e563053f3656c7f134d265
-https://conda.anaconda.org/conda-forge/linux-64/pysocks-1.7.1-py39hf3d152e_5.tar.bz2#d34b97a2386932b97c7cb80916a673e7
-https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py39hb9d737c_4.tar.bz2#dcc47a3b751508507183d17e569805e5
-https://conda.anaconda.org/conda-forge/linux-64/setuptools-63.1.0-py39hf3d152e_0.tar.bz2#7014afab44a0e69fba02c8bf8d084e7f
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.3.0-hd8ed1ab_0.tar.bz2#f3e98e944832fb271a0dbda7b7771dc6
-https://conda.anaconda.org/conda-forge/linux-64/virtualenv-20.15.1-py39hf3d152e_0.tar.bz2#59361d2352ad38bbcec48f9275eff7d5
-https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py39hb9d737c_1004.tar.bz2#05a99367d885ec9990f25e74128a8a08
-https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.1-py39hd257fcd_0.tar.bz2#0911339f31c5fa644c312e4b3af95ea5
-https://conda.anaconda.org/conda-forge/linux-64/cryptography-37.0.4-py39hd97740a_0.tar.bz2#edc3668e7b71657237f94cf25e286478
+https://conda.anaconda.org/conda-forge/noarch/pip-22.3.1-pyhd8ed1ab_0.tar.bz2#da66f2851b9836d3a7c5190082a45f7d
+https://conda.anaconda.org/conda-forge/noarch/pygments-2.13.0-pyhd8ed1ab_0.tar.bz2#9f478e8eedd301008b5f395bad0caaed
+https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py39ha55989b_5.tar.bz2#03968ff66723b72b793e94033d0fbb2f
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.4.0-hd8ed1ab_0.tar.bz2#be969210b61b897775a0de63cd9e9026
+https://conda.anaconda.org/conda-forge/win-64/virtualenv-20.16.7-py39hcbf5309_0.tar.bz2#af8c45092675ced3b42595cfe2859ade
+https://conda.anaconda.org/conda-forge/win-64/brotlipy-0.7.0-py39ha55989b_1005.tar.bz2#5ffea1498e831c783af65e274d6c58f5
+https://conda.anaconda.org/conda-forge/win-64/cftime-1.6.2-py39hc266a54_1.tar.bz2#2ac76c76fae9ed6163c9755b7adb380c
+https://conda.anaconda.org/conda-forge/win-64/cryptography-38.0.3-py39hb6bd5e6_0.tar.bz2#974ccd716c07d67afda218edbd75a0c5
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
-https://conda.anaconda.org/conda-forge/noarch/pip-22.1.2-pyhd8ed1ab_0.tar.bz2#d29185c662a424f8bea1103270b85c96
-https://conda.anaconda.org/conda-forge/noarch/pygments-2.12.0-pyhd8ed1ab_0.tar.bz2#cb27e2ded147e5bcc7eafc1c6d343cb3
-https://conda.anaconda.org/conda-forge/linux-64/pytest-7.1.2-py39hf3d152e_0.tar.bz2#a6bcf633d12aabdfc4cb32a09ebc0f31
-https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.4-pyhd8ed1ab_0.tar.bz2#dff6862ca0b54bbeab8ddf657d032920
-https://conda.anaconda.org/conda-forge/linux-64/ukkonen-1.0.1-py39hf939315_2.tar.bz2#5a3bb9dc2fe08a4a6f2b61548a1431d6
-https://conda.anaconda.org/conda-forge/noarch/identify-2.5.1-pyhd8ed1ab_0.tar.bz2#6f41e3056fcd3061fbc2b49b3309fe0c
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.0.0-pyhd8ed1ab_0.tar.bz2#1d7e241dfaf5475e893d4b824bb71b44
-https://conda.anaconda.org/conda-forge/noarch/pytest-cov-3.0.0-pyhd8ed1ab_0.tar.bz2#0f7cac11bb696b62d378bde725bfc3eb
-https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.4-hd8ed1ab_0.tar.bz2#b068a47ce183af12a53c6b0d84f96085
-https://conda.anaconda.org/conda-forge/linux-64/pre-commit-2.19.0-py39hf3d152e_0.tar.bz2#dddc330e78d96d59c0cf68bf39dc09b1
-https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.10-pyhd8ed1ab_0.tar.bz2#14f22c5b9cfd0d93c2806faaa3fe6dec
-https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_0.tar.bz2#70d6e72856de9551f83ae0f2de689a7a
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.2.0-pyhd8ed1ab_2.tar.bz2#ac82c7aebc282e6ac0450fca012ca78c
+https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.5-pyhd8ed1ab_1.tar.bz2#07037fe2931871ed69b2b3d2acd5fdc6
+https://conda.anaconda.org/conda-forge/win-64/ukkonen-1.0.1-py39h1f6ef14_3.tar.bz2#56f8cce1c3df2ae1a861b0f12245c46f
+https://conda.anaconda.org/conda-forge/noarch/identify-2.5.8-pyhd8ed1ab_0.tar.bz2#8001c46448f385fa43bc4221893704d2
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.1.0-pyhd8ed1ab_0.tar.bz2#fbfa0a180d48c800f922a10a114a8632
+https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.0.0-pyhd8ed1ab_0.tar.bz2#c9e3f8bfdb9bfc34aa1836a6ed4b25d7
+https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.5-hd8ed1ab_1.tar.bz2#6b7cb927a5c505b16b4b4241825e068c
+https://conda.anaconda.org/conda-forge/win-64/pre-commit-2.20.0-py39hcbf5309_1.tar.bz2#d2a17c95b84cb357c63f4cd124164b95
+https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.11-pyhd8ed1ab_0.tar.bz2#0738978569b10669bdef41c671252dd1
+https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_1.tar.bz2#089382ee0e2dc2eae33a04cc3c2bddb0
 https://conda.anaconda.org/conda-forge/noarch/codecov-2.1.11-pyhd3deb0d_0.tar.bz2#9c661c2c14b4667827218402e6624ad5
-https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.2-pyh6c4a22f_0.tar.bz2#d4eaa1f50733a377480ce1d5aac556c7
+https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
```

### Comparing `cf-units-3.1.1/requirements/locks/py39-lock-osx-64.txt` & `cf-units-3.2.0/requirements/locks/py38-lock-osx-64.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,93 +1,91 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: de271c61adbb061303939af84f51cbb7c074db7c9c1b0941891b54358c83a08e
+# input_hash: 2c7ae6bc511322f720a01a0da8e047ea5a521435aa372ed9f857b3e72f9c769c
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
-https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2022.6.15-h033912b_0.tar.bz2#d16674f96e47de0d08af3fc97803134e
-https://conda.anaconda.org/conda-forge/osx-64/libcxx-14.0.6-hce7ea42_0.tar.bz2#ac504a8074ae8add8b837a93d7bc33ca
+https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2022.9.24-h033912b_0.tar.bz2#67b268c32433047914482def1ce215c2
+https://conda.anaconda.org/conda-forge/osx-64/libcxx-14.0.6-hccf4f1f_0.tar.bz2#208a6a874b073277374de48a782f6b10
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
-https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.12-hfe4f2af_1.tar.bz2#f7d43cae08c86f73be8cbda4f8e43373
-https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-14.0.4-ha654fa7_0.tar.bz2#5d5ab9ab83ce21422be84ecfd3142201
+https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-hfd90126_4.tar.bz2#35eb3fce8d51ed3c1fd4122bad48250b
+https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-15.0.5-h61d9ccf_0.tar.bz2#81ceb8ca1476f31cbaacf7ac845b6fff
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.3-h96cf925_1.tar.bz2#76217ebfbb163ff2770a261f955a5861
-https://conda.anaconda.org/conda-forge/noarch/tzdata-2022a-h191b570_0.tar.bz2#84be5301069417a2221187d2f435e0f7
-https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.5-haf1e3a3_1.tar.bz2#41116deb499e9bc58048c297d6403ce6
+https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
-https://conda.anaconda.org/conda-forge/osx-64/expat-2.4.8-h96cf925_0.tar.bz2#529d357c143fb98b9af77d687f82a3e0
-https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-9.3.0-h6c81a4c_23.tar.bz2#a6956ceb628b14594613cefee5127a7a
-https://conda.anaconda.org/conda-forge/osx-64/openssl-1.1.1q-hfe4f2af_0.tar.bz2#ce822517fb00e8bafea6fe77d07f20bd
+https://conda.anaconda.org/conda-forge/osx-64/expat-2.5.0-hf0c8a7f_0.tar.bz2#7648a729fc8b7272596e90b0ab0a3e98
+https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-11.3.0-h082f757_26.tar.bz2#11835360754e5caca43cfaa3a81dfca5
+https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.40.0-ha978bb4_0.tar.bz2#ceb13b6726534b96e3b4e3dda91e9050
+https://conda.anaconda.org/conda-forge/osx-64/openssl-3.0.7-hfd90126_0.tar.bz2#78d8266753a5db378ef0f9302be9990f
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.1.2-h3899abd_0.tar.bz2#89fa404901fa8fb7d4f4e07083b8d635
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
-https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.12-hfe4f2af_1.tar.bz2#12fdf8350ef315e7ad48693346067405
-https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-9_3_0_h6c81a4c_23.tar.bz2#60f48cef2d50674e0428c5579b6c3f66
-https://conda.anaconda.org/conda-forge/osx-64/sqlite-3.39.0-hd9f0692_0.tar.bz2#956223b8f1d808bab8ca9d8fb08778ec
+https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-9_5_0_h97931a8_26.tar.bz2#ac9c1a84323edab6c3ff9d3e586ab3cc
+https://conda.anaconda.org/conda-forge/osx-64/sqlite-3.40.0-h9ae0607_0.tar.bz2#b66b0b11f1b901f3c2bce9406bedfd40
 https://conda.anaconda.org/conda-forge/osx-64/udunits2-2.2.28-h06ef574_0.tar.bz2#74131a7d532fbff820580d4494118245
-https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.20-openmp_hb3cd9ec_0.tar.bz2#d862e4a5c6e7bf0bc9d66a38f5c73142
-https://conda.anaconda.org/conda-forge/osx-64/python-3.9.13-h57e37ff_0_cpython.tar.bz2#0fced1dc8919c66139c45d1e2d8dc6a6
+https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.21-openmp_h429af6e_3.tar.bz2#968c46aa7f4032c3f3873f3452ed4c34
+https://conda.anaconda.org/conda-forge/osx-64/python-3.8.13-h66c20e1_0_cpython.tar.bz2#fa77293a39fa8fa9d240f411ab88844a
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.12-py_0.tar.bz2#2489a97287f90176ecdc3ca982b4b0a0
-https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
+https://conda.anaconda.org/conda-forge/noarch/attrs-22.1.0-pyh71513ae_1.tar.bz2#6d3ccbc56256204925bfa8378722792f
+https://conda.anaconda.org/conda-forge/noarch/certifi-2022.9.24-pyhd8ed1ab_0.tar.bz2#f66309b099374af91369e67e84af397d
 https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2#ebb5f5f7dc4f1a3780ef7ea7738db08c
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.0-pyhd8ed1ab_0.tar.bz2#abc0453b6e7bfbb87d275d58e333fc98
-https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.5-pyhd8ed1ab_0.tar.bz2#c267da48ce208905d7d976d49dfd9433
-https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.4-pyhd8ed1ab_0.tar.bz2#7b50d840543d9cdae100e91582c33035
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.7.1-pyhd8ed1ab_0.tar.bz2#7556872687250e0ea038eb503da3c44b
-https://conda.anaconda.org/conda-forge/noarch/idna-3.3-pyhd8ed1ab_0.tar.bz2#40b50b8b030f5f2f22085c062ed013dd
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.1-pyhd8ed1ab_0.tar.bz2#c1d5b294fbf9a795dec349a6f4d8be8e
+https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
+https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2#b65b4d50dbd2d50fa0aeac367ec9eed7
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.0.4-pyhd8ed1ab_0.tar.bz2#e0734d1f12de77f9daca98bda3428733
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.8.0-pyhd8ed1ab_0.tar.bz2#10f0218dbd493ab2e5dc6759ddea4526
+https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-1.1.1-pyh9f0ad1d_0.tar.bz2#39161f81cc5e5ca45b8226fbb06c6905
-https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-15_osx64_openblas.tar.bz2#48c26d27a96c71cfae2621311aa06215
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.1-pyhd8ed1ab_0.tar.bz2#d5df87964a39f67c46a5448f4e78d9b6
-https://conda.anaconda.org/conda-forge/noarch/py-1.11.0-pyh6c4a22f_0.tar.bz2#b4613d7e7a493916d867842a6a148054
+https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-16_osx64_openblas.tar.bz2#644d63e9379867490b67bace400b2a0f
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.2-pyhd8ed1ab_1.tar.bz2#2fb3f88922e7aec26ba652fcdfe13950
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
-https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.9-2_cp39.tar.bz2#262f557ee8ca777fe2190956038024cd
-https://conda.anaconda.org/conda-forge/noarch/pytz-2022.1-pyhd8ed1ab_0.tar.bz2#b87d66d6d3991d988fb31510c95a9267
-https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
+https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-2_cp38.tar.bz2#156803acb0247c263c9586f190b72f1c
+https://conda.anaconda.org/conda-forge/noarch/pytz-2022.6-pyhd8ed1ab_0.tar.bz2#b1f26ad83328e486910ef7f6e81dc061
+https://conda.anaconda.org/conda-forge/noarch/setuptools-65.5.1-pyhd8ed1ab_0.tar.bz2#cfb8dc4d9d285ca5fb1177b9dd450e33
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.2-py_0.tar.bz2#20b2eaeaeea4ef9a9a0d99770620fd09
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.0-pyhd8ed1ab_0.tar.bz2#77dad82eb9c8c1525ff7953e0756d708
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.3.0-pyha770c72_0.tar.bz2#a9d85960bc62d53cc4ea0d1d27f73c98
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.37.1-pyhd8ed1ab_0.tar.bz2#1ca02aaf78d9c70d9a81a3bed5752022
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.8.0-pyhd8ed1ab_0.tar.bz2#050b94cf4a8c760656e51d2d44e4632c
-https://conda.anaconda.org/conda-forge/osx-64/antlr-python-runtime-4.7.2-py39h6e9494a_1003.tar.bz2#44ca701f379cb0a5f1045ae64528e349
-https://conda.anaconda.org/conda-forge/noarch/babel-2.10.3-pyhd8ed1ab_0.tar.bz2#72f1c6d03109d7a70087bc1d029a8eda
-https://conda.anaconda.org/conda-forge/osx-64/certifi-2022.6.15-py39h6e9494a_0.tar.bz2#8c2a4066f245865e39a32d322f44901d
-https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py39hae9ecf2_0.tar.bz2#558979c1c4b8d8912e4ec89b711ffe55
-https://conda.anaconda.org/conda-forge/osx-64/coverage-6.4.1-py39h701faf5_0.tar.bz2#1bf1889ccfcb9dfb2ff0b1477d8c5c37
-https://conda.anaconda.org/conda-forge/osx-64/cython-0.29.30-py39hd408605_0.tar.bz2#97cbd43ecd35505710dc59ded52a901a
-https://conda.anaconda.org/conda-forge/osx-64/docutils-0.18.1-py39h6e9494a_1.tar.bz2#7fc3b564ada71856fd214c8c89530659
-https://conda.anaconda.org/conda-forge/osx-64/importlib-metadata-4.11.4-py39h6e9494a_0.tar.bz2#adc0fa796414c4235c3ba372d2c93c26
-https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-15_osx64_openblas.tar.bz2#2d26f8ba1e89bcc2704ac7a38d4cc74c
-https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-15_osx64_openblas.tar.bz2#8679c41f1fcb5b54aaecce18ec3e1875
-https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.1-py39h63b48b0_1.tar.bz2#478672fe1f0c0fafc4e99152cd7e33fe
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.4.0-pyha770c72_0.tar.bz2#2d93b130d148d7fc77e583677792fc6a
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.38.4-pyhd8ed1ab_0.tar.bz2#c829cfb8cb826acb9de0ac1a2df0a940
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.10.0-pyhd8ed1ab_0.tar.bz2#cd4eb48ebde7de61f92252979aab515c
+https://conda.anaconda.org/conda-forge/osx-64/antlr-python-runtime-4.7.2-py38h50d1736_1003.tar.bz2#2bec12040acb2867173db5d4f6bd4d62
+https://conda.anaconda.org/conda-forge/noarch/babel-2.11.0-pyhd8ed1ab_0.tar.bz2#2ea70fde8d581ba9425a761609eed6ba
+https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py38hb368cf1_2.tar.bz2#afd6952109c766c7a64ea430ec61268d
+https://conda.anaconda.org/conda-forge/osx-64/coverage-6.5.0-py38hef030d1_1.tar.bz2#29f55325d84a69ba6f388a207607a559
+https://conda.anaconda.org/conda-forge/osx-64/cython-0.29.32-py38h4cd09af_1.tar.bz2#ecea585965e1066bca9ac6fd3da1120f
+https://conda.anaconda.org/conda-forge/osx-64/docutils-0.19-py38h50d1736_1.tar.bz2#3f1c8c2a5182b30fe3c7efbd51963871
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-5.0.0-pyha770c72_1.tar.bz2#ec069c4db6a0ad84107bac5da62819d2
+https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-16_osx64_openblas.tar.bz2#28592eab0f05bcf9969789e87f754e11
+https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-16_osx64_openblas.tar.bz2#406ad426aade5578b90544cc2ed4a79b
+https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.1-py38hef030d1_2.tar.bz2#88814e2ec0ec1ef43f8a8d2c018e4c1e
+https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
 https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2#71f1ab2de48613876becddd496371c85
-https://conda.anaconda.org/conda-forge/osx-64/pluggy-1.0.0-py39h6e9494a_3.tar.bz2#8241cb5aaabd8a108a78c1a13c048cec
-https://conda.anaconda.org/conda-forge/osx-64/pysocks-1.7.1-py39h6e9494a_5.tar.bz2#e6845a71941ffc957c9e4ac0c4c88edd
-https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py39h63b48b0_4.tar.bz2#d7aa7f40b99d7bc9e06b20a613d6a7b0
-https://conda.anaconda.org/conda-forge/osx-64/setuptools-63.1.0-py39h6e9494a_0.tar.bz2#e793bfac1b0a61a8cd88058f98208a6e
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.3.0-hd8ed1ab_0.tar.bz2#f3e98e944832fb271a0dbda7b7771dc6
-https://conda.anaconda.org/conda-forge/osx-64/virtualenv-20.15.1-py39h6e9494a_0.tar.bz2#3c4a36003d506a61c147e643ba0f5647
-https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py39h63b48b0_1004.tar.bz2#7b42f41f7606f46a6b00ff4ac3c71b76
-https://conda.anaconda.org/conda-forge/osx-64/cryptography-37.0.4-py39h9c2a9ce_0.tar.bz2#fbda1a6b92bc0a98f2564319682e8988
+https://conda.anaconda.org/conda-forge/noarch/pip-22.3.1-pyhd8ed1ab_0.tar.bz2#da66f2851b9836d3a7c5190082a45f7d
+https://conda.anaconda.org/conda-forge/noarch/pygments-2.13.0-pyhd8ed1ab_0.tar.bz2#9f478e8eedd301008b5f395bad0caaed
+https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py38hef030d1_5.tar.bz2#e27d698dc29c6d5b49f1385bcd1d50f9
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.4.0-hd8ed1ab_0.tar.bz2#be969210b61b897775a0de63cd9e9026
+https://conda.anaconda.org/conda-forge/osx-64/virtualenv-20.16.7-py38h50d1736_0.tar.bz2#89d2a1d8a562f852f43ab5268f6c5031
+https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py38hef030d1_1005.tar.bz2#2fa6826f6f94c847bf26709f2162a09c
+https://conda.anaconda.org/conda-forge/osx-64/cryptography-38.0.3-py38h4257468_0.tar.bz2#81a87c3627e79449c38e7cc2d85fe1a0
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
-https://conda.anaconda.org/conda-forge/osx-64/numpy-1.23.1-py39hda39a74_0.tar.bz2#211ba9d7690a13e512b118d0576c4551
-https://conda.anaconda.org/conda-forge/noarch/pip-22.1.2-pyhd8ed1ab_0.tar.bz2#d29185c662a424f8bea1103270b85c96
-https://conda.anaconda.org/conda-forge/noarch/pygments-2.12.0-pyhd8ed1ab_0.tar.bz2#cb27e2ded147e5bcc7eafc1c6d343cb3
-https://conda.anaconda.org/conda-forge/osx-64/pytest-7.1.2-py39h6e9494a_0.tar.bz2#9ba12ba5320396b22658c1b370217866
-https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.4-pyhd8ed1ab_0.tar.bz2#dff6862ca0b54bbeab8ddf657d032920
-https://conda.anaconda.org/conda-forge/osx-64/ukkonen-1.0.1-py39h7248d28_2.tar.bz2#67656bdd0c9bc9350e932ab89eb37a67
-https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.1-py39h15b18c7_0.tar.bz2#d17641cfdcd2648fd385f4c089234111
-https://conda.anaconda.org/conda-forge/noarch/identify-2.5.1-pyhd8ed1ab_0.tar.bz2#6f41e3056fcd3061fbc2b49b3309fe0c
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.0.0-pyhd8ed1ab_0.tar.bz2#1d7e241dfaf5475e893d4b824bb71b44
-https://conda.anaconda.org/conda-forge/noarch/pytest-cov-3.0.0-pyhd8ed1ab_0.tar.bz2#0f7cac11bb696b62d378bde725bfc3eb
-https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.4-hd8ed1ab_0.tar.bz2#b068a47ce183af12a53c6b0d84f96085
-https://conda.anaconda.org/conda-forge/osx-64/pre-commit-2.19.0-py39h6e9494a_0.tar.bz2#4a0504c41a160f968e68e09ea146dbd0
-https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.10-pyhd8ed1ab_0.tar.bz2#14f22c5b9cfd0d93c2806faaa3fe6dec
-https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_0.tar.bz2#70d6e72856de9551f83ae0f2de689a7a
+https://conda.anaconda.org/conda-forge/osx-64/numpy-1.23.4-py38hc2f29e8_1.tar.bz2#cb376fdb53d30f7454fafc9d2072e63c
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.2.0-pyhd8ed1ab_2.tar.bz2#ac82c7aebc282e6ac0450fca012ca78c
+https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.5-pyhd8ed1ab_1.tar.bz2#07037fe2931871ed69b2b3d2acd5fdc6
+https://conda.anaconda.org/conda-forge/osx-64/ukkonen-1.0.1-py38h98b9b1b_3.tar.bz2#e97bba5bb846f9c009e8c54a79776c80
+https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.2-py38hbd87e4b_1.tar.bz2#6b61efa56393b9655334192cc5423659
+https://conda.anaconda.org/conda-forge/noarch/identify-2.5.8-pyhd8ed1ab_0.tar.bz2#8001c46448f385fa43bc4221893704d2
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.1.0-pyhd8ed1ab_0.tar.bz2#fbfa0a180d48c800f922a10a114a8632
+https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.0.0-pyhd8ed1ab_0.tar.bz2#c9e3f8bfdb9bfc34aa1836a6ed4b25d7
+https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.5-hd8ed1ab_1.tar.bz2#6b7cb927a5c505b16b4b4241825e068c
+https://conda.anaconda.org/conda-forge/osx-64/pre-commit-2.20.0-py38h50d1736_1.tar.bz2#bdfea8e7230fd3a1c10a6f2d836a8342
+https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.11-pyhd8ed1ab_0.tar.bz2#0738978569b10669bdef41c671252dd1
+https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_1.tar.bz2#089382ee0e2dc2eae33a04cc3c2bddb0
 https://conda.anaconda.org/conda-forge/noarch/codecov-2.1.11-pyhd3deb0d_0.tar.bz2#9c661c2c14b4667827218402e6624ad5
-https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.2-pyh6c4a22f_0.tar.bz2#d4eaa1f50733a377480ce1d5aac556c7
+https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
```

### Comparing `cf-units-3.1.1/requirements/locks/py39-lock-win-64.txt` & `cf-units-3.2.0/requirements/locks/py39-lock-linux-64.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,98 @@
 # Generated by conda-lock.
-# platform: win-64
-# input_hash: b4c2ad458e2bf72ee1318559132b84017551bf2a4e008418aea1f99ef63ecdb4
+# platform: linux-64
+# input_hash: 5d6d22ad10249dbede4f61cd2e5024f4e76f9258b28baab2d8e1273f4a197f95
 @EXPLICIT
-https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2022.6.15-h5b45459_0.tar.bz2#b84069692c33afe59f31c7117c80696e
-https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2022.1.0-h57928b3_3787.tar.bz2#35dff2b6e944ce136a574c4c006cec28
-https://conda.anaconda.org/conda-forge/noarch/tzdata-2022a-h191b570_0.tar.bz2#84be5301069417a2221187d2f435e0f7
-https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.20348.0-h57928b3_0.tar.bz2#6d666b6ea8251231ff508062d1e41f9c
-https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.29.30037-h902a5da_6.tar.bz2#33d07ebe91062743eabc9e53a60d18e1
-https://conda.anaconda.org/conda-forge/win-64/vc-14.2-hb210afc_6.tar.bz2#c2aecbc9b00ba6f352e27d3d61fd31fb
-https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
-https://conda.anaconda.org/conda-forge/win-64/expat-2.4.8-h39d44d4_0.tar.bz2#f8e0f53713756c08456f50c9ce25748c
-https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
-https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.12-h8ffe710_1.tar.bz2#8b67614ab0539e803c03db2ed7990c6c
-https://conda.anaconda.org/conda-forge/win-64/openssl-1.1.1q-h8ffe710_0.tar.bz2#2ee16f406ee12fe4dcd08b513e9bd0c6
-https://conda.anaconda.org/conda-forge/win-64/sqlite-3.39.0-h8ffe710_0.tar.bz2#c76b39a7a74df1875e7b2b3fb5549632
-https://conda.anaconda.org/conda-forge/win-64/tbb-2021.5.0-h2d74725_1.tar.bz2#8f00f39dbd7deaba11410b0b6e7b2cb4
-https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
-https://conda.anaconda.org/conda-forge/win-64/xz-5.2.5-h62dcd97_1.tar.bz2#eabcbfedd14d7c18a514afca09ea0ebb
-https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
-https://conda.anaconda.org/conda-forge/win-64/mkl-2022.1.0-h6a75c08_874.tar.bz2#2ff89a7337a9636029b4db9466e9f8e3
-https://conda.anaconda.org/conda-forge/win-64/python-3.9.13-h9a09f29_0_cpython.tar.bz2#37804c90e761e13ba0d09ddc239f6de6
-https://conda.anaconda.org/conda-forge/win-64/udunits2-2.2.28-h892ecd3_0.tar.bz2#dad8b5fae263e4e36d859524a3794801
+https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
+https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2022.9.24-ha878542_0.tar.bz2#41e4e87062433e283696cf384f952ef6
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.39-hc81fddc_0.tar.bz2#c2719e2faa7bd7076d3a4b52271e5622
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-12.2.0-h337968e_19.tar.bz2#164b4b1acaedc47ee7e658ae6b308ca3
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.2.0-h46fd767_19.tar.bz2#1030b1f38c129f2634eae026f704fe60
+https://conda.anaconda.org/conda-forge/noarch/tzdata-2022f-h191b570_0.tar.bz2#e366350e2343a798e29833286abe2560
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-12.2.0-h69a702a_19.tar.bz2#cd7a806282c16e1f2d39a7e80d3a3e0d
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.2.0-h65d4601_19.tar.bz2#cedcee7c064c01c403f962c9e8d3c373
+https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.2.0-h65d4601_19.tar.bz2#e4c94f80aef025c17ab0828cd85ef535
+https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
+https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-h27087fc_0.tar.bz2#c4fbad8d4bddeb3c085f18cbf97fbfad
+https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
+https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
+https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.21-pthreads_h78a6416_3.tar.bz2#8c5963a49b6035c40646a763293fbb35
+https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.32.1-h7f98852_1000.tar.bz2#772d69f030955d9646d3d0eaf21d859d
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2#4acfc691e64342b9dae57cf2adc63238
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.0.7-h166bdaf_0.tar.bz2#d1ad1824c71e67dea42f07e06cd177dc
+https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
+https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
+https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-16_linux64_openblas.tar.bz2#d9b7a8639171f6c6fa0a983edabcfe2b
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.40.0-h753d276_0.tar.bz2#2e5f9a37d487e1019fd4d8113adb2f9f
+https://conda.anaconda.org/conda-forge/linux-64/readline-8.1.2-h0f457ee_0.tar.bz2#db2ebbe2943aae81ed051a6a9af8e0fa
+https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
+https://conda.anaconda.org/conda-forge/linux-64/udunits2-2.2.28-hc3e0081_0.tar.bz2#d4c341e0379c31e9e781d4f204726867
+https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-16_linux64_openblas.tar.bz2#20bae26d0a1db73f758fc3754cab4719
+https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-16_linux64_openblas.tar.bz2#955d993f41f9354bf753d29864ea20ad
+https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.40.0-h4ff8645_0.tar.bz2#bb11803129cbbb53ed56f9506ff74145
+https://conda.anaconda.org/conda-forge/linux-64/python-3.9.13-h2660328_0_cpython.tar.bz2#894f6c234741ffc61505de11b7a588ba
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.12-py_0.tar.bz2#2489a97287f90176ecdc3ca982b4b0a0
-https://conda.anaconda.org/conda-forge/noarch/atomicwrites-1.4.1-pyhd8ed1ab_0.tar.bz2#1714887104aab113bde64001ceb17262
-https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
+https://conda.anaconda.org/conda-forge/noarch/attrs-22.1.0-pyh71513ae_1.tar.bz2#6d3ccbc56256204925bfa8378722792f
+https://conda.anaconda.org/conda-forge/noarch/certifi-2022.9.24-pyhd8ed1ab_0.tar.bz2#f66309b099374af91369e67e84af397d
 https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2#ebb5f5f7dc4f1a3780ef7ea7738db08c
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.0-pyhd8ed1ab_0.tar.bz2#abc0453b6e7bfbb87d275d58e333fc98
-https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.5-pyhd8ed1ab_0.tar.bz2#c267da48ce208905d7d976d49dfd9433
-https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.4-pyhd8ed1ab_0.tar.bz2#7b50d840543d9cdae100e91582c33035
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.7.1-pyhd8ed1ab_0.tar.bz2#7556872687250e0ea038eb503da3c44b
-https://conda.anaconda.org/conda-forge/noarch/idna-3.3-pyhd8ed1ab_0.tar.bz2#40b50b8b030f5f2f22085c062ed013dd
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.1.1-pyhd8ed1ab_0.tar.bz2#c1d5b294fbf9a795dec349a6f4d8be8e
+https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
+https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2#b65b4d50dbd2d50fa0aeac367ec9eed7
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.0.4-pyhd8ed1ab_0.tar.bz2#e0734d1f12de77f9daca98bda3428733
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.8.0-pyhd8ed1ab_0.tar.bz2#10f0218dbd493ab2e5dc6759ddea4526
+https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-1.1.1-pyh9f0ad1d_0.tar.bz2#39161f81cc5e5ca45b8226fbb06c6905
-https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-15_win64_mkl.tar.bz2#661187f959fed1821cdd6921a738336d
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.1-pyhd8ed1ab_0.tar.bz2#d5df87964a39f67c46a5448f4e78d9b6
-https://conda.anaconda.org/conda-forge/noarch/py-1.11.0-pyh6c4a22f_0.tar.bz2#b4613d7e7a493916d867842a6a148054
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.5.2-pyhd8ed1ab_1.tar.bz2#2fb3f88922e7aec26ba652fcdfe13950
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
-https://conda.anaconda.org/conda-forge/win-64/python_abi-3.9-2_cp39.tar.bz2#757068981fb2f97d0cadbba9ae6ae191
-https://conda.anaconda.org/conda-forge/noarch/pytz-2022.1-pyhd8ed1ab_0.tar.bz2#b87d66d6d3991d988fb31510c95a9267
-https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
+https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.9-2_cp39.tar.bz2#39adde4247484de2bb4000122fdcf665
+https://conda.anaconda.org/conda-forge/noarch/pytz-2022.6-pyhd8ed1ab_0.tar.bz2#b1f26ad83328e486910ef7f6e81dc061
+https://conda.anaconda.org/conda-forge/noarch/setuptools-65.5.1-pyhd8ed1ab_0.tar.bz2#cfb8dc4d9d285ca5fb1177b9dd450e33
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.2-py_0.tar.bz2#20b2eaeaeea4ef9a9a0d99770620fd09
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.0-pyhd8ed1ab_0.tar.bz2#77dad82eb9c8c1525ff7953e0756d708
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.3.0-pyha770c72_0.tar.bz2#a9d85960bc62d53cc4ea0d1d27f73c98
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.37.1-pyhd8ed1ab_0.tar.bz2#1ca02aaf78d9c70d9a81a3bed5752022
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.8.0-pyhd8ed1ab_0.tar.bz2#050b94cf4a8c760656e51d2d44e4632c
-https://conda.anaconda.org/conda-forge/win-64/antlr-python-runtime-4.7.2-py39hcbf5309_1003.tar.bz2#b0b10b9f91524f316108c3ce6d9afc4f
-https://conda.anaconda.org/conda-forge/noarch/babel-2.10.3-pyhd8ed1ab_0.tar.bz2#72f1c6d03109d7a70087bc1d029a8eda
-https://conda.anaconda.org/conda-forge/win-64/certifi-2022.6.15-py39hcbf5309_0.tar.bz2#c4b2f33eda3dd532aa11a238164d6ebc
-https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py39h0878f49_0.tar.bz2#675f9c83aa08e84c35da318c5164e27b
-https://conda.anaconda.org/conda-forge/win-64/coverage-6.4.1-py39hb82d6ee_0.tar.bz2#a50f6957240583bfdd81d6f48cc2fc05
-https://conda.anaconda.org/conda-forge/win-64/cython-0.29.30-py39h415ef7b_0.tar.bz2#832da769cf733577b429c5cb4ca80eae
-https://conda.anaconda.org/conda-forge/win-64/docutils-0.18.1-py39hcbf5309_1.tar.bz2#e576a452da7846d25e435c2134182c8d
-https://conda.anaconda.org/conda-forge/win-64/importlib-metadata-4.11.4-py39hcbf5309_0.tar.bz2#299cad452ed23d1ddc29bd877f0135ba
-https://conda.anaconda.org/conda-forge/win-64/libcblas-3.9.0-15_win64_mkl.tar.bz2#c6012601cd7dde1b4108128fb847de9f
-https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-15_win64_mkl.tar.bz2#7915daedfea4cc94ffcaa71cde184f50
-https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.1-py39hb82d6ee_1.tar.bz2#119fcbf11662ac0b8b4d4fcfa52e49e2
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.4.0-pyha770c72_0.tar.bz2#2d93b130d148d7fc77e583677792fc6a
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.38.4-pyhd8ed1ab_0.tar.bz2#c829cfb8cb826acb9de0ac1a2df0a940
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.10.0-pyhd8ed1ab_0.tar.bz2#cd4eb48ebde7de61f92252979aab515c
+https://conda.anaconda.org/conda-forge/linux-64/antlr-python-runtime-4.7.2-py39hf3d152e_1003.tar.bz2#5e8330e806e50bd6137ebd125f4bc1bb
+https://conda.anaconda.org/conda-forge/noarch/babel-2.11.0-pyhd8ed1ab_0.tar.bz2#2ea70fde8d581ba9425a761609eed6ba
+https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py39he91dace_2.tar.bz2#fc70a133e8162f51e363cff3b6dc741c
+https://conda.anaconda.org/conda-forge/linux-64/coverage-6.5.0-py39hb9d737c_1.tar.bz2#f39dd47f6201a0e7b71c5741009c4359
+https://conda.anaconda.org/conda-forge/linux-64/cython-0.29.32-py39h5a03fae_1.tar.bz2#fb8cd95c2b97eaa8e6eba63021b41567
+https://conda.anaconda.org/conda-forge/linux-64/docutils-0.19-py39hf3d152e_1.tar.bz2#adb733ec2ee669f6d010758d054da60f
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-5.0.0-pyha770c72_1.tar.bz2#ec069c4db6a0ad84107bac5da62819d2
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.1-py39hb9d737c_2.tar.bz2#c678e07e7862b3157fb9f6d908233ffa
+https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
+https://conda.anaconda.org/conda-forge/linux-64/numpy-1.23.4-py39h3d75532_1.tar.bz2#ba4f1c0466d4ba7f53090c150fc88434
 https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2#71f1ab2de48613876becddd496371c85
-https://conda.anaconda.org/conda-forge/win-64/pluggy-1.0.0-py39hcbf5309_3.tar.bz2#7c78954b71d00dcede886c75fd116060
-https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py39hb82d6ee_4.tar.bz2#09b598ab49bb572ba3d41ea52b0c1775
-https://conda.anaconda.org/conda-forge/win-64/setuptools-63.1.0-py39hcbf5309_0.tar.bz2#c02b1cbcdf8d6c01413382e714889c0a
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.3.0-hd8ed1ab_0.tar.bz2#f3e98e944832fb271a0dbda7b7771dc6
-https://conda.anaconda.org/conda-forge/win-64/virtualenv-20.15.1-py39hcbf5309_0.tar.bz2#5577ad351a5842e913185cd0242c84c0
-https://conda.anaconda.org/conda-forge/win-64/win_inet_pton-1.1.0-py39hcbf5309_4.tar.bz2#cde3346ce427c3c58aab6a5d2fe04e37
-https://conda.anaconda.org/conda-forge/win-64/brotlipy-0.7.0-py39hb82d6ee_1004.tar.bz2#be56edb5ff4a3049eafa825b98b26ef4
-https://conda.anaconda.org/conda-forge/win-64/cryptography-37.0.4-py39h7bc7c5c_0.tar.bz2#2dbe11aeb77c5355244e15972e82e088
+https://conda.anaconda.org/conda-forge/noarch/pip-22.3.1-pyhd8ed1ab_0.tar.bz2#da66f2851b9836d3a7c5190082a45f7d
+https://conda.anaconda.org/conda-forge/noarch/pygments-2.13.0-pyhd8ed1ab_0.tar.bz2#9f478e8eedd301008b5f395bad0caaed
+https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py39hb9d737c_5.tar.bz2#ef9db3c38ae7275f6b14491cfe61a248
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.4.0-hd8ed1ab_0.tar.bz2#be969210b61b897775a0de63cd9e9026
+https://conda.anaconda.org/conda-forge/linux-64/virtualenv-20.16.7-py39hf3d152e_0.tar.bz2#242b09f574d87f15a1d1479970037594
+https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py39hb9d737c_1005.tar.bz2#a639fdd9428d8b25f8326a3838d54045
+https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.2-py39h2ae25f5_1.tar.bz2#c943fb9a2818ecc5be1e0ecc8b7738f1
+https://conda.anaconda.org/conda-forge/linux-64/cryptography-38.0.3-py39h3ccb8fc_0.tar.bz2#64119cc315958472211288435368f1e5
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.7.0-pyhd8ed1ab_0.tar.bz2#fbe1182f650c04513046d6894046cd6c
-https://conda.anaconda.org/conda-forge/win-64/numpy-1.23.1-py39h1a62c8c_0.tar.bz2#cd53b7f3a9e3976265d48a6c68a22c2d
-https://conda.anaconda.org/conda-forge/noarch/pip-22.1.2-pyhd8ed1ab_0.tar.bz2#d29185c662a424f8bea1103270b85c96
-https://conda.anaconda.org/conda-forge/noarch/pygments-2.12.0-pyhd8ed1ab_0.tar.bz2#cb27e2ded147e5bcc7eafc1c6d343cb3
-https://conda.anaconda.org/conda-forge/win-64/pysocks-1.7.1-py39hcbf5309_5.tar.bz2#535d7e13023ec2e35c5ebe3f22cc7131
-https://conda.anaconda.org/conda-forge/win-64/pytest-7.1.2-py39hcbf5309_0.tar.bz2#8b0c65a4f6c5b7724600ad2d7e81c6f9
-https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.4-pyhd8ed1ab_0.tar.bz2#dff6862ca0b54bbeab8ddf657d032920
-https://conda.anaconda.org/conda-forge/win-64/ukkonen-1.0.1-py39h2e07f2f_2.tar.bz2#ee89f8328c70472980934f7874e65fb6
-https://conda.anaconda.org/conda-forge/win-64/cftime-1.6.1-py39h5d4886f_0.tar.bz2#82c1546447b5f520d682f90234b7c88d
-https://conda.anaconda.org/conda-forge/noarch/identify-2.5.1-pyhd8ed1ab_0.tar.bz2#6f41e3056fcd3061fbc2b49b3309fe0c
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.0.0-pyhd8ed1ab_0.tar.bz2#1d7e241dfaf5475e893d4b824bb71b44
-https://conda.anaconda.org/conda-forge/noarch/pytest-cov-3.0.0-pyhd8ed1ab_0.tar.bz2#0f7cac11bb696b62d378bde725bfc3eb
-https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.4-hd8ed1ab_0.tar.bz2#b068a47ce183af12a53c6b0d84f96085
-https://conda.anaconda.org/conda-forge/win-64/pre-commit-2.19.0-py39hcbf5309_0.tar.bz2#4e2f37956a7bc9e98dc2948ce7c950df
-https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.10-pyhd8ed1ab_0.tar.bz2#14f22c5b9cfd0d93c2806faaa3fe6dec
-https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_0.tar.bz2#70d6e72856de9551f83ae0f2de689a7a
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.2.0-pyhd8ed1ab_2.tar.bz2#ac82c7aebc282e6ac0450fca012ca78c
+https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.0.5-pyhd8ed1ab_1.tar.bz2#07037fe2931871ed69b2b3d2acd5fdc6
+https://conda.anaconda.org/conda-forge/linux-64/ukkonen-1.0.1-py39hf939315_3.tar.bz2#0f11bcdf9669a5ae0f39efd8c830209a
+https://conda.anaconda.org/conda-forge/noarch/identify-2.5.8-pyhd8ed1ab_0.tar.bz2#8001c46448f385fa43bc4221893704d2
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.1.0-pyhd8ed1ab_0.tar.bz2#fbfa0a180d48c800f922a10a114a8632
+https://conda.anaconda.org/conda-forge/noarch/pytest-cov-4.0.0-pyhd8ed1ab_0.tar.bz2#c9e3f8bfdb9bfc34aa1836a6ed4b25d7
+https://conda.anaconda.org/conda-forge/noarch/setuptools_scm-7.0.5-hd8ed1ab_1.tar.bz2#6b7cb927a5c505b16b4b4241825e068c
+https://conda.anaconda.org/conda-forge/linux-64/pre-commit-2.20.0-py39hf3d152e_1.tar.bz2#921f8a7c2a16d18d7168fdac88b2adfe
+https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.11-pyhd8ed1ab_0.tar.bz2#0738978569b10669bdef41c671252dd1
+https://conda.anaconda.org/conda-forge/noarch/requests-2.28.1-pyhd8ed1ab_1.tar.bz2#089382ee0e2dc2eae33a04cc3c2bddb0
 https://conda.anaconda.org/conda-forge/noarch/codecov-2.1.11-pyhd3deb0d_0.tar.bz2#9c661c2c14b4667827218402e6624ad5
-https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.2-pyh6c4a22f_0.tar.bz2#d4eaa1f50733a377480ce1d5aac556c7
+https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
```

### Comparing `cf-units-3.1.1/setup.cfg` & `cf-units-3.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 author = SciTools Developers
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Science/Research
-	License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering
 description = Units of measure as required by the Climate and Forecast (CF) metadata conventions
@@ -16,16 +16,16 @@
 	units
 	cf
 	netcdf
 	science
 	oceanography
 	meteorology
 	climate
-license = LGPL-3.0-or-later
-license_files = COPYING
+license = BSD
+license_files = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = cf-units
 project_urls = 
 	Code = https://github.com/SciTools/cf-units
 	Discussions = https://github.com/SciTools/cf-units/discussions
 	Issues = https://github.com/SciTools/cf-units/issues
```

### Comparing `cf-units-3.1.1/setup.py` & `cf-units-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `cf-units-3.1.1/tox.ini` & `cf-units-3.2.0/tox.ini`

 * *Files identical despite different names*

