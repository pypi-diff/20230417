# Comparing `tmp/tarantool-0.9.0.tar.gz` & `tmp/tarantool-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tarantool-0.9.0.tar", last modified: Mon Jun 20 18:22:55 2022, max compression
+gzip compressed data, was "tarantool-1.0.0.tar", last modified: Mon Apr 17 11:04:13 2023, max compression
```

## Comparing `tarantool-0.9.0.tar` & `tarantool-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,159 @@
-drwxrwxr-x   0 georgymoiseev  (1000) georgymoiseev  (1000)        0 2022-06-20 18:22:55.000000 tarantool-0.9.0/
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)       38 2022-06-20 18:22:55.000000 tarantool-0.9.0/setup.cfg
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)       15 2022-01-18 10:45:23.000000 tarantool-0.9.0/README.txt
--rwxrwxr-x   0 georgymoiseev  (1000) georgymoiseev  (1000)     2405 2022-04-22 14:28:18.000000 tarantool-0.9.0/setup.py
-drwxrwxr-x   0 georgymoiseev  (1000) georgymoiseev  (1000)        0 2022-06-20 18:22:55.000000 tarantool-0.9.0/tarantool/
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)    16051 2022-06-20 11:54:22.000000 tarantool-0.9.0/tarantool/connection_pool.py
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)    14313 2022-06-20 11:54:22.000000 tarantool-0.9.0/tarantool/mesh_connection.py
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)     8068 2022-01-18 10:45:23.000000 tarantool-0.9.0/tarantool/dbapi.py
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)     2824 2022-06-20 11:54:22.000000 tarantool-0.9.0/tarantool/const.py
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)     2531 2022-01-18 10:45:23.000000 tarantool-0.9.0/tarantool/space.py
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)     9096 2022-01-18 10:45:23.000000 tarantool-0.9.0/tarantool/response.py
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)     8719 2022-01-18 10:45:23.000000 tarantool-0.9.0/tarantool/schema.py
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)    17741 2022-06-20 11:54:22.000000 tarantool-0.9.0/tarantool/error.py
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)     3009 2022-06-20 18:19:39.000000 tarantool-0.9.0/tarantool/__init__.py
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)     3340 2022-04-19 08:29:01.000000 tarantool-0.9.0/tarantool/utils.py
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)    11927 2022-04-19 08:30:33.000000 tarantool-0.9.0/tarantool/request.py
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)    36113 2022-06-20 11:54:22.000000 tarantool-0.9.0/tarantool/connection.py
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)     5579 2022-06-20 18:22:55.000000 tarantool-0.9.0/PKG-INFO
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)     4032 2022-04-19 08:29:13.000000 tarantool-0.9.0/README.rst
-drwxrwxr-x   0 georgymoiseev  (1000) georgymoiseev  (1000)        0 2022-06-20 18:22:55.000000 tarantool-0.9.0/tarantool.egg-info/
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)      468 2022-06-20 18:22:55.000000 tarantool-0.9.0/tarantool.egg-info/SOURCES.txt
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)     5579 2022-06-20 18:22:55.000000 tarantool-0.9.0/tarantool.egg-info/PKG-INFO
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)       10 2022-06-20 18:22:55.000000 tarantool-0.9.0/tarantool.egg-info/top_level.txt
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)       15 2022-06-20 18:22:55.000000 tarantool-0.9.0/tarantool.egg-info/requires.txt
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)        1 2022-06-20 18:22:55.000000 tarantool-0.9.0/tarantool.egg-info/dependency_links.txt
--rw-rw-r--   0 georgymoiseev  (1000) georgymoiseev  (1000)       93 2022-01-18 10:45:23.000000 tarantool-0.9.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.290784 tarantool-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-04-17 11:03:59.000000 tarantool-1.0.0/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-17 11:03:59.000000 tarantool-1.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.270784 tarantool-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.274784 tarantool-1.0.0/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-04-17 11:03:59.000000 tarantool-1.0.0/.github/scripts/remove_source_code.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.274784 tarantool-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)    15987 2023-04-17 11:03:59.000000 tarantool-1.0.0/.github/workflows/packing.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-17 11:03:59.000000 tarantool-1.0.0/.github/workflows/reusable_testing.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    12676 2023-04-17 11:03:59.000000 tarantool-1.0.0/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-04-17 11:03:59.000000 tarantool-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 11:03:59.000000 tarantool-1.0.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-04-17 11:03:59.000000 tarantool-1.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-17 11:03:59.000000 tarantool-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-04-17 11:03:59.000000 tarantool-1.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)    14512 2023-04-17 11:03:59.000000 tarantool-1.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-04-17 11:03:59.000000 tarantool-1.0.0/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (122)     1321 2023-04-17 11:03:59.000000 tarantool-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-17 11:03:59.000000 tarantool-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-04-17 11:03:59.000000 tarantool-1.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     5549 2023-04-17 11:04:13.290784 tarantool-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4953 2023-04-17 11:03:59.000000 tarantool-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-17 11:03:59.000000 tarantool-1.0.0/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.274784 tarantool-1.0.0/debian/
+-rw-r--r--   0 runner    (1001) docker     (122)    27362 2023-04-17 11:03:59.000000 tarantool-1.0.0/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (122)        3 2023-04-17 11:03:59.000000 tarantool-1.0.0/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-04-17 11:03:59.000000 tarantool-1.0.0/debian/control
+-rwxr-xr-x   0 runner    (1001) docker     (122)      517 2023-04-17 11:03:59.000000 tarantool-1.0.0/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.274784 tarantool-1.0.0/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-17 11:03:59.000000 tarantool-1.0.0/debian/source/format
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-17 11:03:59.000000 tarantool-1.0.0/debian/source/options
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.274784 tarantool-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.274784 tarantool-1.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.270784 tarantool-1.0.0/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.278784 tarantool-1.0.0/docs/source/_static/favicon/
+-rw-r--r--   0 runner    (1001) docker     (122)    10003 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-114x114.png
+-rw-r--r--   0 runner    (1001) docker     (122)    10722 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (122)    14138 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (122)    15200 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3743 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-57x57.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5571 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-76x76.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)      266 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/generate-png.sh
+-rw-r--r--   0 runner    (1001) docker     (122)    11989 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/icon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/icon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (122)    21876 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/icon-196x196.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/icon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7747 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/icon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5668 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.278784 tarantool-1.0.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/module-tarantool.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-connection-pool.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-connection.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-crud.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-dbapi.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-error.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-mesh-connection.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-msgpack-ext-types.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-msgpack-ext.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-request.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-response.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-schema.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-space.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-types.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-utils.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10929 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6420 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/dev-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    14953 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/quick-start.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-17 11:03:59.000000 tarantool-1.0.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-17 11:03:59.000000 tarantool-1.0.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.270784 tarantool-1.0.0/rpm/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.278784 tarantool-1.0.0/rpm/SPECS/
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-04-17 11:03:59.000000 tarantool-1.0.0/rpm/SPECS/python-tarantool.spec
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-17 11:04:13.290784 tarantool-1.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3136 2023-04-17 11:03:59.000000 tarantool-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.282784 tarantool-1.0.0/tarantool/
+-rw-r--r--   0 runner    (1001) docker     (122)     4353 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   103863 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56825 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3709 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/const.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/crud.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12894 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20552 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22294 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/mesh_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.282784 tarantool-1.0.0/tarantool/msgpack_ext/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5279 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9985 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/decimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/interval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/packer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.282784 tarantool-1.0.0/tarantool/msgpack_ext/types/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26728 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6527 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/types/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.282784 tarantool-1.0.0/tarantool/msgpack_ext/types/timezones/
+-rw-r--r--   0 runner    (1001) docker     (122)      284 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/types/timezones/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2254 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/types/timezones/gen-timezones.sh
+-rw-r--r--   0 runner    (1001) docker     (122)    48588 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/types/timezones/timezones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/unpacker.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17713 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10967 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/response.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13804 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/space.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3390 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.282784 tarantool-1.0.0/tarantool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5549 2023-04-17 11:04:13.000000 tarantool-1.0.0/tarantool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3964 2023-04-17 11:04:13.000000 tarantool-1.0.0/tarantool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 11:04:13.000000 tarantool-1.0.0/tarantool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-17 11:04:13.000000 tarantool-1.0.0/tarantool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-17 11:04:13.000000 tarantool-1.0.0/tarantool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.282784 tarantool-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.286784 tarantool-1.0.0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/ca.crt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/empty
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1702 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/generate.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/invalidhost.crt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/invalidpasswords
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/localhost.crt
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/localhost.enc.key
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/localhost.key
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/passwords
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1176 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/setup_command.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.286784 tarantool-1.0.0/test/suites/
+-rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/box.lua
+-rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/crud_server.lua
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.290784 tarantool-1.0.0/test/suites/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3363 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/lib/remote_tarantool_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8386 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/lib/skip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2532 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/lib/tarantool_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9032 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/lib/tarantool_python_ci.lua
+-rw-r--r--   0 runner    (1001) docker     (122)    11116 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/lib/tarantool_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6140 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26768 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_crud.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30406 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4218 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18278 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19641 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_dml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7419 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17512 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_error_ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13376 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11464 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20214 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8583 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_push.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_reconnect.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25356 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33077 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5326 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_uuid.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tarantool-0.9.0/tarantool/connection_pool.py` & `tarantool-1.0.0/tarantool/request.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,500 +1,667 @@
-# -*- coding: utf-8 -*-
+"""
+Request types definitions. For internal use only, there is no API to
+send pre-build request objects.
+"""
 
-import abc
-import itertools
-import queue
-import threading
-import time
-import typing
-from dataclasses import dataclass, field
-from enum import Enum
+import hashlib
+from collections.abc import Sequence, Mapping
+
+import msgpack
 
-from tarantool.connection import Connection, ConnectionInterface
 from tarantool.const import (
-    CONNECTION_TIMEOUT,
-    POOL_INSTANCE_RECONNECT_DELAY,
-    POOL_INSTANCE_RECONNECT_MAX_ATTEMPTS,
-    POOL_REFRESH_DELAY,
-    SOCKET_TIMEOUT
+    IPROTO_REQUEST_TYPE,
+    IPROTO_SYNC,
+    IPROTO_SPACE_ID,
+    IPROTO_INDEX_ID,
+    IPROTO_LIMIT,
+    IPROTO_OFFSET,
+    IPROTO_KEY,
+    IPROTO_USER_NAME,
+    IPROTO_TUPLE,
+    IPROTO_FUNCTION_NAME,
+    IPROTO_ITERATOR,
+    IPROTO_EXPR,
+    IPROTO_OPS,
+    IPROTO_SCHEMA_ID,
+    IPROTO_SQL_TEXT,
+    IPROTO_SQL_BIND,
+    IPROTO_VERSION,
+    IPROTO_FEATURES,
+    REQUEST_TYPE_OK,
+    REQUEST_TYPE_PING,
+    REQUEST_TYPE_SELECT,
+    REQUEST_TYPE_INSERT,
+    REQUEST_TYPE_REPLACE,
+    REQUEST_TYPE_DELETE,
+    REQUEST_TYPE_UPDATE,
+    REQUEST_TYPE_UPSERT,
+    REQUEST_TYPE_CALL16,
+    REQUEST_TYPE_CALL,
+    REQUEST_TYPE_EXECUTE,
+    REQUEST_TYPE_EVAL,
+    REQUEST_TYPE_AUTHENTICATE,
+    REQUEST_TYPE_ID,
+    AUTH_TYPE_CHAP_SHA1,
+    AUTH_TYPE_PAP_SHA256,
+)
+from tarantool.response import (
+    Response,
+    ResponseExecute,
+    ResponseProtocolVersion,
 )
-from tarantool.error import (
-    ClusterConnectWarning,
-    PoolTolopogyError,
-    PoolTolopogyWarning,
-    ConfigurationError,
-    NetworkError,
-    warn
+from tarantool.utils import (
+    strxor,
 )
-from tarantool.utils import ENCODING_DEFAULT
-from tarantool.mesh_connection import prepare_address
 
+from tarantool.msgpack_ext.packer import default as packer_default
+
+
+def packer_factory(conn):
+    """
+    Build packer to pack request.
+
+    :param conn: Request sender.
+    :type conn: :class:`~tarantool.Connection`
+
+    :rtype: :class:`msgpack.Packer`
+    """
+
+    packer_kwargs = {}
+
+    # use_bin_type=True is default since msgpack-1.0.0.
+    #
+    # The option controls whether to pack binary (non-unicode)
+    # string values as mp_bin or as mp_str.
+    #
+    # The default behaviour of the Python 3 connector (since
+    # default encoding is "utf-8") is to pack bytes as mp_bin
+    # and Unicode strings as mp_str. encoding=None mode must
+    # be used to work with non-utf strings.
+    #
+    # encoding = 'utf-8'
+    #
+    # Python 3 -> Tarantool          -> Python 3
+    # str      -> mp_str (string)    -> str
+    # bytes    -> mp_bin (varbinary) -> bytes
+    #
+    # encoding = None
+    #
+    # Python 3 -> Tarantool          -> Python 3
+    # bytes    -> mp_str (string)    -> bytes
+    # str      -> mp_str (string)    -> bytes
+    #             mp_bin (varbinary) -> bytes
+    #
+    # msgpack-0.5.0 (and only this version) warns when the
+    # option is unset:
+    #
+    #  | FutureWarning: use_bin_type option is not specified.
+    #  | Default value of the option will be changed in future
+    #  | version.
+    #
+    # The option is supported since msgpack-0.4.0, so we can
+    # just always set it for all msgpack versions to get rid
+    # of the warning on msgpack-0.5.0 and to keep our
+    # behaviour on msgpack-1.0.0.
+    if conn.encoding is None:
+        packer_kwargs['use_bin_type'] = False
+    else:
+        packer_kwargs['use_bin_type'] = True
+
+    # We need configured packer to work with error extension
+    # type payload, but module do not provide access to self
+    # inside extension type packers.
+    def default(obj):
+        packer_no_ext = msgpack.Packer(**packer_kwargs)
+        return packer_default(obj, packer_no_ext)
+    packer_kwargs['default'] = default
+
+    return msgpack.Packer(**packer_kwargs)
 
-class Mode(Enum):
-    ANY = 1
-    RW = 2
-    RO = 3
-    PREFER_RW = 4
-    PREFER_RO = 5
 
+class Request():
+    """
+    Represents a single request to the server in compliance with the
+    Tarantool protocol. Responsible for data encapsulation and building
+    the binary packet to be sent to the server.
+
+    This is the abstract base class. Specific request types are
+    implemented in the inherited classes.
+    """
+
+    request_type = None
+
+    def __init__(self, conn):
+        """
+        :param conn: Request sender.
+        :type conn: :class:`~tarantool.Connection`
+        """
+
+        self._bytes = None
+        self.conn = conn
+        self._sync = None
+        self._body = ''
+        self.response_class = Response
 
-class Status(Enum):
-    HEALTHY = 1
-    UNHEALTHY = 2
+        self.packer = conn._packer_factory()
 
+    def _dumps(self, src):
+        """
+        Encode MsgPack data.
+        """
 
-@dataclass
-class InstanceState():
-    status: Status = Status.UNHEALTHY
-    ro: typing.Optional[bool] = None
+        return self.packer.pack(src)
 
+    def __bytes__(self):
+        return self.header(len(self._body)) + self._body
 
-def QueueFactory():
-    return queue.Queue(maxsize=1)
+    __str__ = __bytes__
 
+    @property
+    def sync(self):
+        """
+        :type: :obj:`int`
 
-@dataclass
-class PoolUnit():
-    addr: dict
-    conn: Connection
-    input_queue: queue.Queue = field(default_factory=QueueFactory)
-    output_queue: queue.Queue = field(default_factory=QueueFactory)
-    thread: typing.Optional[threading.Thread] = None
-    state: InstanceState = field(default_factory=InstanceState)
-    # request_processing_enabled is used to stop requests processing
-    # in background thread on close or destruction.
-    request_processing_enabled: bool = False
+        Contains request header IPROTO_SYNC.
+        """
 
+        return self._sync
 
-# Based on https://realpython.com/python-interface/
-class StrategyInterface(metaclass=abc.ABCMeta):
-    @classmethod
-    def __subclasshook__(cls, subclass):
-        return (hasattr(subclass, '__init__') and
-                callable(subclass.__init__) and
-                hasattr(subclass, 'update') and
-                callable(subclass.update) and
-                hasattr(subclass, 'getnext') and
-                callable(subclass.getnext) or
-                NotImplemented)
+    def header(self, length):
+        """
+        Pack total (header + payload) length info together with header
+        itself.
 
-    @abc.abstractmethod
-    def __init__(self, pool):
-        raise NotImplementedError
+        :param length: Payload length.
+        :type: :obj:`int`
 
-    @abc.abstractmethod
-    def update(self):
-        raise NotImplementedError
+        :return: MsgPack data with encoded total (header + payload)
+            length info and header.
+        :rtype: :obj:`bytes`
+        """
 
-    @abc.abstractmethod
-    def getnext(self, mode):
-        raise NotImplementedError
+        self._sync = self.conn.generate_sync()
+        header_fields = {
+            IPROTO_REQUEST_TYPE: self.request_type,
+            IPROTO_SYNC: self._sync,
+        }
+        if self.conn.schema is not None:
+            header_fields[IPROTO_SCHEMA_ID] = self.conn.schema_version
+        header = self._dumps(header_fields)
 
-class RoundRobinStrategy(StrategyInterface):
+        return self._dumps(length + len(header)) + header
+
+
+class RequestInsert(Request):
     """
-    Simple round-robin connection rotation
+    Represents INSERT request.
     """
-    def __init__(self, pool):
-        self.ANY_iter = None
-        self.RW_iter = None
-        self.RO_iter = None
-        self.pool = pool
-        self.rebuild_needed = True
 
-    def build(self):
-        ANY_pool = []
-        RW_pool = []
-        RO_pool = []
+    request_type = REQUEST_TYPE_INSERT
+
+    def __init__(self, conn, space_no, values):
+        """
+        :param conn: Request sender.
+        :type conn: :class:`~tarantool.Connection`
+
+        :param space_no: Space id.
+        :type space_no: :obj:`int`
+
+        :param values: Record to be inserted.
+        :type values: :obj:`tuple` or :obj:`list`
 
-        for key in self.pool:
-            state = self.pool[key].state
+        :raise: :exc:`~AssertionError`
+        """
 
-            if state.status == Status.UNHEALTHY:
-                continue
+        super().__init__(conn)
+        assert isinstance(values, (tuple, list))
 
-            ANY_pool.append(key)
+        request_body = self._dumps({IPROTO_SPACE_ID: space_no,
+                                    IPROTO_TUPLE: values})
 
-            if state.ro == False:
-                RW_pool.append(key)
+        self._body = request_body
+
+
+def sha1(values):
+    """
+    Compute hash.
+
+    :param values: Values to hash.
+    :type values: :obj:`tuple`
+
+    :rtype: :obj:`str`
+
+    :meta private:
+    """
+
+    sha = hashlib.sha1()
+    for i in values:
+        if i is not None:
+            if isinstance(i, bytes):
+                sha.update(i)
             else:
-                RO_pool.append(key)
+                sha.update(i.encode())
+    return sha.digest()
 
-        if len(ANY_pool) > 0:
-            self.ANY_iter = itertools.cycle(ANY_pool)
-        else:
-            self.ANY_iter = None
 
-        if len(RW_pool) > 0:
-            self.RW_iter = itertools.cycle(RW_pool)
-        else:
-            self.RW_iter = None
+class RequestAuthenticate(Request):
+    """
+    Represents AUTHENTICATE request.
+    """
+
+    request_type = REQUEST_TYPE_AUTHENTICATE
 
-        if len(RO_pool) > 0:
-            self.RO_iter = itertools.cycle(RO_pool)
+    def __init__(self, conn, salt, user, password, auth_type=AUTH_TYPE_CHAP_SHA1):
+        """
+        :param conn: Request sender.
+        :type conn: :class:`~tarantool.Connection`
+
+        :param salt: base64-encoded session salt.
+        :type salt: :obj:`str`
+
+        :param user: User name for authentication on the Tarantool
+            server.
+        :type user: :obj:`str`
+
+        :param password: User password for authentication on the
+            Tarantool server.
+        :type password: :obj:`str`
+
+        :param auth_type: Refer to :paramref:`~tarantool.Connection.auth_type`.
+        :type auth_type: :obj:`str`, optional
+        """
+        # pylint: disable=too-many-arguments
+
+        super().__init__(conn)
+
+        if auth_type == AUTH_TYPE_CHAP_SHA1:
+            hash1 = sha1((password,))
+            hash2 = sha1((hash1,))
+            scramble = sha1((salt, hash2))
+            scramble = strxor(hash1, scramble)
+        elif auth_type == AUTH_TYPE_PAP_SHA256:
+            scramble = password
         else:
-            self.RO_iter = None
+            raise ValueError(f'Unexpected auth_type {auth_type}')
 
-        self.rebuild_needed = False
+        self._body = self._dumps({IPROTO_USER_NAME: user,
+                                  IPROTO_TUPLE: (auth_type, scramble)})
 
-    def update(self):
-        self.rebuild_needed = True
+    def header(self, length):
+        """
+        Pack total (header + payload) length info together with header
+        itself.
 
-    def getnext(self, mode):
-        if self.rebuild_needed:
-            self.build()
+        :param length: Payload length.
+        :type: :obj:`int`
 
-        if mode == Mode.ANY:
-            if self.ANY_iter is not None:
-                return next(self.ANY_iter)
-            else:
-                raise PoolTolopogyError("Can't find healthy instance in pool")
-        elif mode == Mode.RW:
-            if self.RW_iter is not None:
-                return next(self.RW_iter)
-            else:
-                raise PoolTolopogyError("Can't find healthy rw instance in pool")
-        elif mode == Mode.RO:
-            if self.RO_iter is not None:
-                return next(self.RO_iter)
-            else:
-                raise PoolTolopogyError("Can't find healthy ro instance in pool")
-        elif mode == Mode.PREFER_RO:
-            if self.RO_iter is not None:
-                return next(self.RO_iter)
-            elif self.RW_iter is not None:
-                return next(self.RW_iter)
-            else:
-                raise PoolTolopogyError("Can't find healthy instance in pool")
-        elif mode == Mode.PREFER_RW:
-            if self.RW_iter is not None:
-                return next(self.RW_iter)
-            elif self.RO_iter is not None:
-                return next(self.RO_iter)
-            else:
-                raise PoolTolopogyError("Can't find healthy instance in pool")
+        :return: MsgPack data with encoded total (header + payload)
+            length info and header.
+        :rtype: :obj:`bytes`
+        """
+
+        self._sync = self.conn.generate_sync()
+        # Set IPROTO_SCHEMA_ID: 0 to avoid SchemaReloadException
+        # It is ok to use 0 in auth every time.
+        header = self._dumps({IPROTO_REQUEST_TYPE: self.request_type,
+                              IPROTO_SYNC: self._sync,
+                              IPROTO_SCHEMA_ID: 0})
+
+        return self._dumps(length + len(header)) + header
+
+
+class RequestReplace(Request):
+    """
+    Represents REPLACE request.
+    """
+
+    request_type = REQUEST_TYPE_REPLACE
+
+    def __init__(self, conn, space_no, values):
+        """
+        :param conn: Request sender.
+        :type conn: :class:`~tarantool.Connection`
+
+        :param space_no: Space id.
+        :type space_no: :obj:`int`
+
+        :param values: Record to be replaced.
+        :type values: :obj:`tuple` or :obj:`list`
+
+        :raise: :exc:`~AssertionError`
+        """
+
+        super().__init__(conn)
+        assert isinstance(values, (tuple, list))
+
+        request_body = self._dumps({IPROTO_SPACE_ID: space_no,
+                                    IPROTO_TUPLE: values})
+
+        self._body = request_body
+
+
+class RequestDelete(Request):
+    """
+    Represents DELETE request.
+    """
+
+    request_type = REQUEST_TYPE_DELETE
+
+    def __init__(self, conn, space_no, index_no, key):
+        """
+        :param conn: Request sender.
+        :type conn: :class:`~tarantool.Connection`
+
+        :param space_no: Space id.
+        :type space_no: :obj:`int`
+
+        :param index_no: Index id.
+        :type index_no: :obj:`int`
+
+        :param key: Key of a tuple to be deleted.
+        :type key: :obj:`list`
+
+        :raise: :exc:`~AssertionError`
+        """
+
+        super().__init__(conn)
+
+        request_body = self._dumps({IPROTO_SPACE_ID: space_no,
+                                    IPROTO_INDEX_ID: index_no,
+                                    IPROTO_KEY: key})
+
+        self._body = request_body
+
+
+class RequestSelect(Request):
+    """
+    Represents SELECT request.
+    """
+
+    request_type = REQUEST_TYPE_SELECT
+
+    def __init__(self, conn, space_no, index_no, key, offset, limit, iterator):
+        """
+        :param conn: Request sender.
+        :type conn: :class:`~tarantool.Connection`
+
+        :param space_no: Space id.
+        :type space_no: :obj:`int`
+
+        :param index_no: Index id.
+        :type index_no: :obj:`int`
+
+        :param key: Key of a tuple to be selected.
+        :type key: :obj:`list`
+
+        :param offset: Number of tuples to skip.
+        :type offset: :obj:`int`
+
+        :param limit: Maximum number of tuples to select.
+        :type limit: :obj:`int`
+
+        :param iterator: Index iterator type, see
+            :paramref:`~tarantool.Connection.select.params.iterator`.
+        :type iterator: :obj:`str`
+
+        :raise: :exc:`~AssertionError`
+        """
+        # pylint: disable=too-many-arguments
+
+        super().__init__(conn)
+        request_body = self._dumps({IPROTO_SPACE_ID: space_no,
+                                    IPROTO_INDEX_ID: index_no,
+                                    IPROTO_OFFSET: offset,
+                                    IPROTO_LIMIT: limit,
+                                    IPROTO_ITERATOR: iterator,
+                                    IPROTO_KEY: key})
+
+        self._body = request_body
+
+
+class RequestUpdate(Request):
+    """
+    Represents UPDATE request.
+    """
+
+    request_type = REQUEST_TYPE_UPDATE
+
+    def __init__(self, conn, space_no, index_no, key, op_list):
+        """
+        :param conn: Request sender.
+        :type conn: :class:`~tarantool.Connection`
+
+        :param space_no: Space id.
+        :type space_no: :obj:`int`
+
+        :param index_no: Index id.
+        :type index_no: :obj:`int`
+
+        :param key: Key of a tuple to be updated.
+        :type key: :obj:`list`
+
+        :param op_list: The list of operations to update individual
+            fields, refer to
+            :paramref:`~tarantool.Connection.update.params.op_list`.
+        :type op_list: :obj:`tuple` or :obj:`list`
+
+        :raise: :exc:`~AssertionError`
+        """
+        # pylint: disable=too-many-arguments
+
+        super().__init__(conn)
+
+        request_body = self._dumps({IPROTO_SPACE_ID: space_no,
+                                    IPROTO_INDEX_ID: index_no,
+                                    IPROTO_KEY: key,
+                                    IPROTO_TUPLE: op_list})
+
+        self._body = request_body
+
+
+class RequestCall(Request):
+    """
+    Represents CALL request.
+    """
+
+    request_type = REQUEST_TYPE_CALL
+
+    def __init__(self, conn, name, args, call_16):
+        """
+        :param conn: Request sender.
+        :type conn: :class:`~tarantool.Connection`
+
+        :param name: Stored Lua function name.
+        :type func_name: :obj:`str`
+
+        :param args: Stored Lua function arguments.
+        :type args: :obj:`tuple`
+
+        :param call_16: If ``True``, use compatibility mode with
+            Tarantool 1.6 or older.
+        :type call_16: :obj:`bool`
+
+        :raise: :exc:`~AssertionError`
+        """
+
+        if call_16:
+            self.request_type = REQUEST_TYPE_CALL16
+        super().__init__(conn)
+        assert isinstance(args, (list, tuple))
+
+        request_body = self._dumps({IPROTO_FUNCTION_NAME: name,
+                                    IPROTO_TUPLE: args})
+
+        self._body = request_body
+
+
+class RequestEval(Request):
+    """
+    Represents EVAL request.
+    """
+
+    request_type = REQUEST_TYPE_EVAL
+
+    def __init__(self, conn, name, args):
+        """
+        :param conn: Request sender.
+        :type conn: :class:`~tarantool.Connection`
+
+        :param name: Lua expression.
+        :type func_name: :obj:`str`
+
+        :param args: Lua expression arguments.
+        :type args: :obj:`tuple`
+
+        :raise: :exc:`~AssertionError`
+        """
+
+        super().__init__(conn)
+        assert isinstance(args, (list, tuple))
+
+        request_body = self._dumps({IPROTO_EXPR: name,
+                                    IPROTO_TUPLE: args})
+
+        self._body = request_body
+
+
+class RequestPing(Request):
+    """
+    Represents a ping request with the empty body.
+    """
+
+    request_type = REQUEST_TYPE_PING
+
+    def __init__(self, conn):
+        """
+        :param conn: Request sender.
+        :type conn: :class:`~tarantool.Connection`
+        """
+
+        super().__init__(conn)
+        self._body = b''
+
+
+class RequestUpsert(Request):
+    """
+    Represents UPSERT request.
+    """
+
+    request_type = REQUEST_TYPE_UPSERT
+
+    def __init__(self, conn, space_no, index_no, tuple_value, op_list):
+        """
+        :param conn: Request sender.
+        :type conn: :class:`~tarantool.Connection`
+
+        :param space_no: Space id.
+        :type space_no: :obj:`int`
+
+        :param index_no: Index id.
+        :type index_no: :obj:`int`
+
+        :param tuple_value: Tuple to be upserted.
+        :type tuple_value: :obj:`tuple` or :obj:`list`
+
+        :param op_list: The list of operations to update individual
+            fields, refer to
+            :paramref:`~tarantool.Connection.update.params.op_list`.
+        :type op_list: :obj:`tuple` or :obj:`list`
+
+        :raise: :exc:`~AssertionError`
+        """
+        # pylint: disable=too-many-arguments
+
+        super().__init__(conn)
+
+        request_body = self._dumps({IPROTO_SPACE_ID: space_no,
+                                    IPROTO_INDEX_ID: index_no,
+                                    IPROTO_TUPLE: tuple_value,
+                                    IPROTO_OPS: op_list})
+
+        self._body = request_body
+
+
+class RequestOK(Request):
+    """
+    Represents OK acknowledgement.
+    """
+
+    request_type = REQUEST_TYPE_OK
+
+    def __init__(self, conn, sync):
+        """
+        :param conn: Request sender.
+        :type conn: :class:`~tarantool.Connection`
+
+        :param sync: Previous request sync id.
+        :type sync: :obj:`int`
+        """
+
+        super().__init__(conn)
+        request_body = self._dumps({IPROTO_REQUEST_TYPE: self.request_type,
+                                    IPROTO_SYNC: sync})
+        self._body = request_body
+
+
+class RequestExecute(Request):
+    """
+    Represents EXECUTE SQL request.
+    """
+
+    request_type = REQUEST_TYPE_EXECUTE
+
+    def __init__(self, conn, sql, args):
+        """
+        :param conn: Request sender.
+        :type conn: :class:`~tarantool.Connection`
+
+        :param sql: SQL query.
+        :type sql: :obj:`str`
+
+        :param args: SQL query bind values.
+        :type args: :obj:`dict` or :obj:`list`
+
+        :raise: :exc:`~TypeError`
+        """
+
+        super().__init__(conn)
+        if isinstance(args, Mapping):
+            args = [{f":{name}": value} for name, value in args.items()]
+        elif not isinstance(args, Sequence):
+            raise TypeError(f"Parameter type '{type(args)}' is not supported. "
+                            "Must be a mapping or sequence")
+
+        request_body = self._dumps({IPROTO_SQL_TEXT: sql,
+                                    IPROTO_SQL_BIND: args})
+
+        self._body = request_body
+        self.response_class = ResponseExecute
+
+
+class RequestProtocolVersion(Request):
+    """
+    Represents ID request: inform the server about the protocol
+    version and features connector support.
+    """
+
+    request_type = REQUEST_TYPE_ID
+
+    def __init__(self, conn, protocol_version, features):
+        """
+        :param conn: Request sender.
+        :type conn: :class:`~tarantool.Connection`
+
+        :param protocol_version: Connector protocol version.
+        :type protocol_version: :obj:`int`
 
+        :param features: List of supported features.
+        :type features: :obj:`list`
+        """
 
-@dataclass
-class PoolTask():
-    method_name: str
-    args: tuple
-    kwargs: dict
-
-
-class ConnectionPool(ConnectionInterface):
-    '''
-    Represents pool of connections to the cluster of Tarantool servers.
-
-    ConnectionPool API is the same as a plain Connection API.
-    On each request, a connection is chosen to execute this request.
-    Connection is selected based on request mode:
-
-    * Mode.ANY chooses any instance.
-    * Mode.RW chooses an RW instance.
-    * Mode.RO chooses an RO instance.
-    * Mode.PREFER_RW chooses an RW instance, if possible, RO instance
-      otherwise.
-    * Mode.PREFER_RO chooses an RO instance, if possible, RW instance
-      otherwise.
-
-    All requests that are guaranteed to write (insert, replace, delete,
-    upsert, update) use RW mode by default. select uses ANY by default. You
-    can set the mode explicitly. call, eval, execute and ping requests
-    require to set the mode explicitly.
-    '''
-    def __init__(self,
-                 addrs,
-                 user=None,
-                 password=None,
-                 socket_timeout=SOCKET_TIMEOUT,
-                 reconnect_max_attempts=POOL_INSTANCE_RECONNECT_MAX_ATTEMPTS,
-                 reconnect_delay=POOL_INSTANCE_RECONNECT_DELAY,
-                 connect_now=True,
-                 encoding=ENCODING_DEFAULT,
-                 call_16=False,
-                 connection_timeout=CONNECTION_TIMEOUT,
-                 strategy_class=RoundRobinStrategy,
-                 refresh_delay=POOL_REFRESH_DELAY):
-        '''
-        Initialize connections to the cluster of servers.
-
-        :param list addrs: List of
-
-            .. code-block:: python
-
-                {
-                  host: "str",          # optional
-                  port: int or "str",   # mandatory
-                  transport: "str",     # optional
-                  ssl_key_file: "str",  # optional
-                  ssl_cert_file: "str", # optional
-                  ssl_ca_file: "str",   # optional
-                  ssl_ciphers: "str"    # optional
-                }
-
-            dictionaries, describing server addresses.
-            See :func:`tarantool.Connection` parameters with same names.
-        :param str user: Username used to authenticate. User must be able
-            to call box.info function. For example, to give grants to
-            'guest' user, evaluate
-            box.schema.func.create('box.info')
-            box.schema.user.grant('guest', 'execute', 'function', 'box.info')
-            on Tarantool instances.
-        :param int reconnect_max_attempts: Max attempts to reconnect
-            for each connection in the pool. Be careful with reconnect
-            parameters in ConnectionPool since every status refresh is
-            also a request with reconnection. Default is 0 (fail after
-            first attempt).
-        :param float reconnect_delay: Time between reconnect
-            attempts for each connection in the pool. Be careful with
-            reconnect parameters in ConnectionPool since every status
-            refresh is also a request with reconnection. Default is 0.
-        :param StrategyInterface strategy_class: Class for choosing
-            instance based on request mode. By default, round-robin
-            strategy is used.
-        :param int refresh_delay: Minimal time between RW/RO status
-            refreshes.
-        '''
-
-        if not isinstance(addrs, list) or len(addrs) == 0:
-            raise ConfigurationError("addrs must be non-empty list")
-
-        # Prepare addresses for usage.
-        new_addrs = []
-        for addr in addrs:
-            new_addr, msg = prepare_address(addr)
-            if not new_addr:
-                raise ConfigurationError(msg)
-            new_addrs.append(new_addr)
-        self.addrs = new_addrs
-
-        # Create connections
-        self.pool = {}
-        self.refresh_delay = refresh_delay
-        self.strategy = strategy_class(self.pool)
-
-        for addr in self.addrs:
-            key = self._make_key(addr)
-            self.pool[key] = PoolUnit(
-                addr=addr,
-                conn=Connection(
-                    host=addr['host'],
-                    port=addr['port'],
-                    user=user,
-                    password=password,
-                    socket_timeout=socket_timeout,
-                    reconnect_max_attempts=reconnect_max_attempts,
-                    reconnect_delay=reconnect_delay,
-                    connect_now=False, # Connect in ConnectionPool.connect()
-                    encoding=encoding,
-                    call_16=call_16,
-                    connection_timeout=connection_timeout,
-                    transport=addr['transport'],
-                    ssl_key_file=addr['ssl_key_file'],
-                    ssl_cert_file=addr['ssl_cert_file'],
-                    ssl_ca_file=addr['ssl_ca_file'],
-                    ssl_ciphers=addr['ssl_ciphers'])
-            )
-
-        if connect_now:
-            self.connect()
-
-    def __del__(self):
-        self.close()
-
-    def _make_key(self, addr):
-        return '{0}:{1}'.format(addr['host'], addr['port'])
-
-    def _get_new_state(self, unit):
-        conn = unit.conn
-
-        if conn.is_closed():
-            try:
-                conn.connect()
-            except NetworkError as e:
-                msg = "Failed to connect to {0}:{1}".format(
-                    unit.addr['host'], unit.addr['port'])
-                warn(msg, ClusterConnectWarning)
-                return InstanceState(Status.UNHEALTHY)
-
-        try:
-            resp = conn.call('box.info')
-        except NetworkError as e:
-            msg = "Failed to get box.info for {0}:{1}, reason: {2}".format(
-                unit.addr['host'], unit.addr['port'], repr(e))
-            warn(msg, PoolTolopogyWarning)
-            return InstanceState(Status.UNHEALTHY)
-
-        try:
-            ro = resp.data[0]['ro']
-        except (IndexError, KeyError) as e:
-            msg = "Incorrect box.info response from {0}:{1}".format(
-                unit.addr['host'], unit.addr['port'])
-            warn(msg, PoolTolopogyWarning)
-            return InstanceState(Status.UNHEALTHY)
-
-        try:
-            status = resp.data[0]['status']
-
-            if status != 'running':
-                msg = "{0}:{1} instance status is not 'running'".format(
-                    unit.addr['host'], unit.addr['port'])
-                warn(msg, PoolTolopogyWarning)
-                return InstanceState(Status.UNHEALTHY)
-        except (IndexError, KeyError) as e:
-            msg = "Incorrect box.info response from {0}:{1}".format(
-                unit.addr['host'], unit.addr['port'])
-            warn(msg, PoolTolopogyWarning)
-            return InstanceState(Status.UNHEALTHY)
-
-        return InstanceState(Status.HEALTHY, ro)
-
-    def _refresh_state(self, key):
-        unit = self.pool[key]
-
-        state = self._get_new_state(unit)
-        if state != unit.state:
-            unit.state = state
-            self.strategy.update()
-
-    def close(self):
-        for unit in self.pool.values():
-            unit.request_processing_enabled = False
-            unit.thread.join()
-
-            if not unit.conn.is_closed():
-                unit.conn.close()
-
-    def is_closed(self):
-        return all(unit.request_processing_enabled == False for unit in self.pool.values())
-
-    def _request_process_loop(self, key, unit, last_refresh):
-        while unit.request_processing_enabled:
-            if not unit.input_queue.empty():
-                task = unit.input_queue.get()
-                method = getattr(Connection, task.method_name)
-                try:
-                    resp = method(unit.conn, *task.args, **task.kwargs)
-                except Exception as e:
-                    unit.output_queue.put(e)
-                else:
-                    unit.output_queue.put(resp)
-
-            now = time.time()
-
-            if now - last_refresh > self.refresh_delay:
-                self._refresh_state(key)
-                last_refresh = time.time()
-
-    def connect(self):
-        for key in self.pool:
-            unit = self.pool[key]
-
-            self._refresh_state(key)
-            last_refresh = time.time()
-
-            unit.thread = threading.Thread(
-                target=self._request_process_loop,
-                args=(key, unit, last_refresh),
-                daemon=True,
-            )
-            unit.request_processing_enabled = True
-            unit.thread.start()
-
-    def _send(self, mode, method_name, *args, **kwargs):
-        key = self.strategy.getnext(mode)
-        unit = self.pool[key]
-
-        task = PoolTask(method_name=method_name, args=args, kwargs=kwargs)
-
-        unit.input_queue.put(task)
-        resp = unit.output_queue.get()
-
-        if isinstance(resp, Exception):
-            raise resp
-
-        return resp
-
-    def call(self, func_name, *args, mode=None):
-        '''
-        :param tarantool.Mode mode: Request mode.
-        '''
-
-        if mode is None:
-            raise ValueError("Please, specify 'mode' keyword argument")
-
-        return self._send(mode, 'call', func_name, *args)
-
-    def eval(self, expr, *args, mode=None):
-        '''
-        :param tarantool.Mode mode: Request mode.
-        '''
-
-        if mode is None:
-            raise ValueError("Please, specify 'mode' keyword argument")
-
-        return self._send(mode, 'eval', expr, *args)
-
-    def replace(self, space_name, values, *, mode=Mode.RW):
-        '''
-        :param tarantool.Mode mode: Request mode (default is RW).
-        '''
-
-        return self._send(mode, 'replace', space_name, values)
-
-    def insert(self, space_name, values, *, mode=Mode.RW):
-        '''
-        :param tarantool.Mode mode: Request mode (default is RW).
-        '''
-
-        return self._send(mode, 'insert', space_name, values)
-
-    def delete(self, space_name, key, *, mode=Mode.RW, **kwargs):
-        '''
-        :param tarantool.Mode mode: Request mode (default is RW).
-        '''
-
-        return self._send(mode, 'delete', space_name, key, **kwargs)
-
-    def upsert(self, space_name, tuple_value, op_list, *, mode=Mode.RW, **kwargs):
-        '''
-        :param tarantool.Mode mode: Request mode (default is RW).
-        '''
-
-        return self._send(mode, 'upsert', space_name, tuple_value,
-            op_list, **kwargs)
-
-    def update(self, space_name, key, op_list, *, mode=Mode.RW, **kwargs):
-        '''
-        :param tarantool.Mode mode: Request mode (default is RW).
-        '''
-
-        return self._send(mode, 'update', space_name, key, 
-            op_list, **kwargs)
-
-    def ping(self, *, mode=None, **kwargs):
-        '''
-        :param tarantool.Mode mode: Request mode.
-        '''
-
-        if mode is None:
-            raise ValueError("Please, specify 'mode' keyword argument")
-
-        return self._send(mode, 'ping', **kwargs)
-
-    def select(self, space_name, key, *, mode=Mode.ANY, **kwargs):
-        '''
-        :param tarantool.Mode mode: Request mode (default is
-            ANY).
-        '''
-
-        return self._send(mode, 'select', space_name, key, **kwargs)
-
-    def execute(self, query, params=None, *, mode=None):
-        '''
-        :param tarantool.Mode mode: Request mode (default is RW).
-        '''
+        super().__init__(conn)
 
-        if mode is None:
-            raise ValueError("Please, specify 'mode' keyword argument")
+        request_body = self._dumps({IPROTO_VERSION: protocol_version,
+                                    IPROTO_FEATURES: features})
 
-        return self._send(mode, 'execute', query, params)
+        self._body = request_body
+        self.response_class = ResponseProtocolVersion
```

### Comparing `tarantool-0.9.0/tarantool/const.py` & `tarantool-1.0.0/tarantool/const.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# -*- coding: utf-8 -*-
-# pylint: disable=C0301,W0105,W0401,W0614
+"""
+This module a set of constants for the package.
+"""
 
-IPROTO_CODE = 0x00
+IPROTO_REQUEST_TYPE = 0x00
 IPROTO_SYNC = 0x01
 # replication keys (header)
 IPROTO_SERVER_ID = 0x02
 IPROTO_LSN = 0x03
 IPROTO_TIMESTAMP = 0x04
 IPROTO_SCHEMA_ID = 0X05
 #
@@ -24,41 +25,49 @@
 IPROTO_SERVER_UUID = 0x24
 IPROTO_CLUSTER_UUID = 0x25
 IPROTO_VCLOCK = 0x26
 IPROTO_EXPR = 0x27
 IPROTO_OPS = 0x28
 #
 IPROTO_DATA = 0x30
-IPROTO_ERROR = 0x31
+IPROTO_ERROR_24 = 0x31
 #
 IPROTO_METADATA = 0x32
 IPROTO_SQL_TEXT = 0x40
 IPROTO_SQL_BIND = 0x41
 IPROTO_SQL_INFO = 0x42
 IPROTO_SQL_INFO_ROW_COUNT = 0x00
 IPROTO_SQL_INFO_AUTOINCREMENT_IDS = 0x01
+#
+IPROTO_ERROR = 0x52
+#
+IPROTO_VERSION = 0x54
+IPROTO_FEATURES = 0x55
+IPROTO_AUTH_TYPE = 0x5b
+IPROTO_CHUNK = 0x80
 
 IPROTO_GREETING_SIZE = 128
 IPROTO_BODY_MAX_LEN = 2147483648
 
-REQUEST_TYPE_OK = 0
-REQUEST_TYPE_SELECT = 1
-REQUEST_TYPE_INSERT = 2
-REQUEST_TYPE_REPLACE = 3
-REQUEST_TYPE_UPDATE = 4
-REQUEST_TYPE_DELETE = 5
-REQUEST_TYPE_CALL16 = 6
-REQUEST_TYPE_AUTHENTICATE = 7
-REQUEST_TYPE_EVAL = 8
-REQUEST_TYPE_UPSERT = 9
-REQUEST_TYPE_CALL = 10
-REQUEST_TYPE_EXECUTE = 11
-REQUEST_TYPE_PING = 64
-REQUEST_TYPE_JOIN = 65
-REQUEST_TYPE_SUBSCRIBE = 66
+REQUEST_TYPE_OK = 0x00
+REQUEST_TYPE_SELECT = 0x01
+REQUEST_TYPE_INSERT = 0x02
+REQUEST_TYPE_REPLACE = 0x03
+REQUEST_TYPE_UPDATE = 0x04
+REQUEST_TYPE_DELETE = 0x05
+REQUEST_TYPE_CALL16 = 0x06
+REQUEST_TYPE_AUTHENTICATE = 0x07
+REQUEST_TYPE_EVAL = 0x08
+REQUEST_TYPE_UPSERT = 0x09
+REQUEST_TYPE_CALL = 0x0a
+REQUEST_TYPE_EXECUTE = 0x0b
+REQUEST_TYPE_PING = 0x40
+REQUEST_TYPE_JOIN = 0x41
+REQUEST_TYPE_SUBSCRIBE = 0x42
+REQUEST_TYPE_ID = 0x49
 REQUEST_TYPE_ERROR = 1 << 15
 
 SPACE_SCHEMA = 272
 SPACE_SPACE = 280
 SPACE_INDEX = 288
 SPACE_FUNC = 296
 SPACE_VSPACE = 281
@@ -82,14 +91,19 @@
 ITERATOR_GT = 6
 ITERATOR_BITSET_ALL_SET = 7
 ITERATOR_BITSET_ANY_SET = 8
 ITERATOR_BITSET_ALL_NOT_SET = 9
 ITERATOR_OVERLAPS = 10
 ITERATOR_NEIGHBOR = 11
 
+IPROTO_FEATURE_STREAMS = 0
+IPROTO_FEATURE_TRANSACTIONS = 1
+IPROTO_FEATURE_ERROR_EXTENSION = 2
+IPROTO_FEATURE_WATCHERS = 3
+
 # Default value for connection timeout (seconds)
 CONNECTION_TIMEOUT = None
 # Default value for socket timeout (seconds)
 SOCKET_TIMEOUT = None
 # Default maximum number of attempts to reconnect
 RECONNECT_MAX_ATTEMPTS = 10
 # Default delay between attempts to reconnect (seconds)
@@ -102,15 +116,31 @@
 DEFAULT_SSL_KEY_FILE = None
 # Default value for a path to SSL certificate file
 DEFAULT_SSL_CERT_FILE = None
 # Default value for a path to SSL certificatea uthorities file
 DEFAULT_SSL_CA_FILE = None
 # Default value for list of SSL ciphers
 DEFAULT_SSL_CIPHERS = None
+# Default value for SSL key file password
+DEFAULT_SSL_PASSWORD = None
+# Default value for a path to file with SSL key file password
+DEFAULT_SSL_PASSWORD_FILE = None
 # Default cluster nodes list refresh interval (seconds)
 CLUSTER_DISCOVERY_DELAY = 60
 # Default cluster nodes state refresh interval (seconds)
 POOL_REFRESH_DELAY = 1
 # Default maximum number of attempts to reconnect for pool instance
 POOL_INSTANCE_RECONNECT_MAX_ATTEMPTS = 0
 # Default delay between attempts to reconnect (seconds)
 POOL_INSTANCE_RECONNECT_DELAY = 0
+
+# Tarantool 2.10 protocol version is 3
+CONNECTOR_IPROTO_VERSION = 3
+# List of connector-supported features
+CONNECTOR_FEATURES = [IPROTO_FEATURE_ERROR_EXTENSION]
+
+# Authenticate with CHAP-SHA1 (Tarantool CE and EE)
+AUTH_TYPE_CHAP_SHA1 = "chap-sha1"
+# Authenticate with PAP-SHA256 (Tarantool EE)
+AUTH_TYPE_PAP_SHA256 = "pap-sha256"
+# List of supported auth types.
+AUTH_TYPES = [AUTH_TYPE_CHAP_SHA1, AUTH_TYPE_PAP_SHA256]
```

### Comparing `tarantool-0.9.0/tarantool/response.py` & `tarantool-1.0.0/tarantool/response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,314 +1,403 @@
-# -*- coding: utf-8 -*-
-# pylint: disable=C0301,W0105,W0401,W0614
+"""
+Request response types definitions.
+"""
 
-try:
-    # Python 3.3+
-    from collections.abc import Sequence
-except ImportError:
-    # Python 2
-    from collections import Sequence
+from collections.abc import Sequence
 
 import json
 import msgpack
 
 from tarantool.const import (
-    IPROTO_CODE,
+    IPROTO_REQUEST_TYPE,
     IPROTO_DATA,
+    IPROTO_ERROR_24,
     IPROTO_ERROR,
     IPROTO_SYNC,
     IPROTO_SCHEMA_ID,
     REQUEST_TYPE_ERROR,
     IPROTO_SQL_INFO,
     IPROTO_SQL_INFO_ROW_COUNT,
-    IPROTO_SQL_INFO_AUTOINCREMENT_IDS
+    IPROTO_SQL_INFO_AUTOINCREMENT_IDS,
+    IPROTO_VERSION,
+    IPROTO_FEATURES,
+    IPROTO_AUTH_TYPE,
 )
+from tarantool.types import decode_box_error
 from tarantool.error import (
     DatabaseError,
     InterfaceError,
     SchemaReloadException,
     tnt_strerror
 )
+from tarantool.schema import to_unicode
+
+from tarantool.msgpack_ext.unpacker import ext_hook as unpacker_ext_hook
+
+
+def unpacker_factory(conn):
+    """
+    Build unpacker to unpack request response.
+
+    :param conn: Request sender.
+    :type conn: :class:`~tarantool.Connection`
+
+    :rtype: :class:`msgpack.Unpacker`
+    """
+
+    unpacker_kwargs = {}
+
+    # Decode MsgPack arrays into Python lists by default (not tuples).
+    # Can be configured in the Connection init
+    unpacker_kwargs['use_list'] = conn.use_list
+
+    # Use raw=False instead of encoding='utf-8'.
+    if msgpack.version >= (0, 5, 2) and conn.encoding == 'utf-8':
+        # Get rid of the following warning.
+        # > PendingDeprecationWarning: encoding is deprecated,
+        # > Use raw=False instead.
+        unpacker_kwargs['raw'] = False
+    elif conn.encoding is not None:
+        unpacker_kwargs['encoding'] = conn.encoding
+
+    # raw=False is default since msgpack-1.0.0.
+    #
+    # The option decodes mp_str to bytes, not a Unicode
+    # string (when True).
+    if msgpack.version >= (1, 0, 0) and conn.encoding is None:
+        unpacker_kwargs['raw'] = True
+
+    # encoding option is not supported since msgpack-1.0.0,
+    # but it is handled in the Connection constructor.
+    assert msgpack.version < (1, 0, 0) or conn.encoding in (None, 'utf-8')
+
+    # strict_map_key=True is default since msgpack-1.0.0.
+    #
+    # The option forbids non-string keys in a map (when True).
+    if msgpack.version >= (1, 0, 0):
+        unpacker_kwargs['strict_map_key'] = False
+
+    # We need configured unpacker to work with error extension
+    # type payload, but module do not provide access to self
+    # inside extension type unpackers.
+    def ext_hook(code, data):
+        unpacker_no_ext = msgpack.Unpacker(**unpacker_kwargs)
+        return unpacker_ext_hook(code, data, unpacker_no_ext)
+    unpacker_kwargs['ext_hook'] = ext_hook
+
+    return msgpack.Unpacker(**unpacker_kwargs)
 
 
 class Response(Sequence):
-    '''
+    """
     Represents a single response from the server in compliance with the
-    Tarantool protocol.
-    Responsible for data encapsulation (i.e. received list of tuples)
-    and parses binary packet received from the server.
-    '''
+    Tarantool protocol. Responsible for data encapsulation (i.e.
+    received list of tuples) and parsing of binary packets received from
+    the server.
+    """
+    # pylint: disable=too-many-instance-attributes
 
     def __init__(self, conn, response):
-        '''
-        Create an instance of `Response` using data received from the server.
+        """
+        :param conn: Request sender.
+        :type conn: :class:`~tarantool.Connection`
 
-        __init__() itself reads data from the socket, parses response body and
-        sets appropriate instance attributes.
+        :param response: Response binary data.
+        :type response: :obj:`bytes`
 
-        :param body: body of the response
-        :type body: array of bytes
-        '''
+        :raise: :exc:`~tarantool.error.DatabaseError`,
+            :exc:`~tarantool.error.SchemaReloadException`
+        """
 
         # This is not necessary, because underlying list data structures are
         # created in the __new__().
         # super(Response, self).__init__()
 
-        unpacker_kwargs = dict()
-
-        # Decode msgpack arrays into Python lists by default (not tuples).
-        # Can be configured in the Connection init
-        unpacker_kwargs['use_list'] = conn.use_list
-
-        # Use raw=False instead of encoding='utf-8'.
-        if msgpack.version >= (0, 5, 2) and conn.encoding == 'utf-8':
-            # Get rid of the following warning.
-            # > PendingDeprecationWarning: encoding is deprecated,
-            # > Use raw=False instead.
-            unpacker_kwargs['raw'] = False
-        elif conn.encoding is not None:
-            unpacker_kwargs['encoding'] = conn.encoding
-
-        # raw=False is default since msgpack-1.0.0.
-        #
-        # The option decodes mp_str to bytes, not a Unicode
-        # string (when True).
-        if msgpack.version >= (1, 0, 0) and conn.encoding is None:
-            unpacker_kwargs['raw'] = True
-
-        # encoding option is not supported since msgpack-1.0.0,
-        # but it is handled in the Connection constructor.
-        assert(msgpack.version < (1, 0, 0) or conn.encoding in (None, 'utf-8'))
-
-        # strict_map_key=True is default since msgpack-1.0.0.
-        #
-        # The option forbids non-string keys in a map (when True).
-        if msgpack.version >= (1, 0, 0):
-            unpacker_kwargs['strict_map_key'] = False
-
-        unpacker = msgpack.Unpacker(**unpacker_kwargs)
+        unpacker = conn._unpacker_factory()
 
         unpacker.feed(response)
         header = unpacker.unpack()
 
         self.conn = conn
         self._sync = header.get(IPROTO_SYNC, 0)
-        self._code = header[IPROTO_CODE]
+        self._code = header[IPROTO_REQUEST_TYPE]
         self._body = {}
         self._schema_version = header.get(IPROTO_SCHEMA_ID, None)
         try:
             self._body = unpacker.unpack()
         except msgpack.OutOfData:
             pass
 
         if self._code < REQUEST_TYPE_ERROR:
             self._return_code = 0
             self._schema_version = header.get(IPROTO_SCHEMA_ID, None)
             self._data = self._body.get(IPROTO_DATA, None)
-            if (not isinstance(self._data, (list, tuple)) and
-                    self._data is not None):
+            if (not isinstance(self._data, (list, tuple))
+                    and self._data is not None):
                 self._data = [self._data]
             # # Backward-compatibility
             # if isinstance(self._data, (list, tuple)):
             #     self.extend(self._data)
             # else:
             #     self.append(self._data)
         else:
             # Separate return_code and completion_code
-            self._return_message = self._body.get(IPROTO_ERROR, "")
+            self._return_message = self._body.get(IPROTO_ERROR_24, "")
             self._return_code = self._code & (REQUEST_TYPE_ERROR - 1)
+
+            self._return_error = None
+            return_error_map = self._body.get(IPROTO_ERROR)
+            if return_error_map is not None:
+                self._return_error = decode_box_error(return_error_map)
+
             self._data = []
             if self._return_code == 109:
                 raise SchemaReloadException(self._return_message,
                                             self._schema_version)
             if self.conn.error:
-                raise DatabaseError(self._return_code, self._return_message)
+                raise DatabaseError(self._return_code,
+                                    self._return_message,
+                                    extra_info=self._return_error)
 
     def __getitem__(self, idx):
         if self._data is None:
-            raise InterfaceError("Trying to access data, when there's no data")
+            raise InterfaceError("Trying to access data when there's no data")
         return self._data.__getitem__(idx)
 
     def __len__(self):
         if self._data is None:
-            raise InterfaceError("Trying to access data, when there's no data")
+            raise InterfaceError("Trying to access data when there's no data")
         return len(self._data)
 
     def __contains__(self, item):
         if self._data is None:
-            raise InterfaceError("Trying to access data, when there's no data")
+            raise InterfaceError("Trying to access data when there's no data")
         return item in self._data
 
     def __iter__(self):
         if self._data is None:
-            raise InterfaceError("Trying to access data, when there's no data")
+            raise InterfaceError("Trying to access data when there's no data")
         return iter(self._data)
 
     def __reversed__(self):
         if self._data is None:
-            raise InterfaceError("Trying to access data, when there's no data")
+            raise InterfaceError("Trying to access data when there's no data")
         return reversed(self._data)
 
     def index(self, *args):
+        """
+        Refer to :class:`collections.abc.Sequence`.
+
+        :raises: :exc:`~tarantool.error.InterfaceError.`
+        """
+
         if self._data is None:
-            raise InterfaceError("Trying to access data, when there's no data")
+            raise InterfaceError("Trying to access data when there's no data")
         return self._data.index(*args)
 
-    def count(self, item):
+    def count(self, value):
+        """
+        Refer to :class:`collections.abc.Sequence`.
+
+        :raises: :exc:`~tarantool.error.InterfaceError`
+        """
+
         if self._data is None:
-            raise InterfaceError("Trying to access data, when there's no data")
-        return self._data.count(item)
+            raise InterfaceError("Trying to access data when there's no data")
+        return self._data.count(value)
 
     @property
     def rowcount(self):
-        '''
-        :type: int
+        """
+        :type: :obj:`int`
 
         Number of rows affected or returned by a query.
-        '''
+        """
+
         return len(self)
 
     @property
     def body(self):
-        '''
-        :type: dict
+        """
+        :type: :obj:`dict`
+
+        Raw response body.
+        """
 
-        Required field in the server response.
-        Contains raw response body.
-        '''
         return self._body
 
     @property
     def code(self):
-        '''
-        :type: int
+        """
+        :type: :obj:`int`
+
+        Response type id.
+        """
 
-        Required field in the server response.
-        Contains response type id.
-        '''
         return self._code
 
     @property
     def sync(self):
-        '''
-        :type: int
+        """
+        :type: :obj:`int`
+
+        Response header IPROTO_SYNC.
+        """
 
-        Required field in the server response.
-        Contains response header IPROTO_SYNC.
-        '''
         return self._sync
 
     @property
     def return_code(self):
-        '''
-        :type: int
+        """
+        :type: :obj:`int`
+
+        If the request was successful, the value of is ``0``.
+        Otherwise, it contains an error code. If the value is non-zero,
+        :attr:`return_message` contains an error message.
+        """
 
-        Required field in the server response.
-        Value of :attr:`return_code` can be ``0`` if request was sucessfull
-        or contains an error code.
-        If :attr:`return_code` is non-zero than :attr:`return_message`
-        contains an error message.
-        '''
         return self._return_code
 
     @property
     def data(self):
-        '''
-        :type: object
+        """
+        :type: :obj:`object`
+
+        Contains the list of tuples for SELECT, REPLACE and DELETE
+        requests and arbitrary data for CALL.
+        """
 
-        Required field in the server response.
-        Contains list of tuples of SELECT, REPLACE and DELETE requests
-        and arbitrary data for CALL.
-        '''
         return self._data
 
     @property
     def strerror(self):
-        '''
-        :type: str
+        """
+        Refer to :func:`~tarantool.error.tnt_strerror`.
+        """
 
-        It may be ER_OK if request was successful,
-        or contain error code string.
-        '''
         return tnt_strerror(self._return_code)
 
     @property
     def return_message(self):
-        '''
-        :type: str
+        """
+        :type: :obj:`str`
+
+        The error message returned by the server in case of non-zero
+        :attr:`return_code` (empty string otherwise).
+        """
 
-        The error message returned by the server in case
-        of :attr:`return_code` is non-zero.
-        '''
         return self._return_message
 
     @property
     def schema_version(self):
-        '''
-        :type: int
+        """
+        :type: :obj:`int`
+
+        Request current schema version.
+        """
 
-        Current schema version of request.
-        '''
         return self._schema_version
 
     def __str__(self):
-        '''
-        Return user friendy string representation of the object.
-        Useful for the interactive sessions and debuging.
-
-        :rtype: str or None
-        '''
         if self.return_code:
             return json.dumps({
                 'error': {
                     'code': self.strerror[0],
                     'reason': self.return_message
                 }
-            }, sort_keys = True, indent = 4, separators=(', ', ': '))
+            }, sort_keys=True, indent=4, separators=(', ', ': '))
         output = []
         for tpl in self._data or ():
             output.extend(("- ", repr(tpl), "\n"))
         if len(output) > 0:
             output.pop()
         return ''.join(output)
 
     __repr__ = __str__
 
 
 class ResponseExecute(Response):
+    """
+    Represents an SQL EXECUTE request response.
+    """
+
     @property
     def autoincrement_ids(self):
         """
-        Returns a list with the new primary-key value
-        (or values) for an INSERT in a table defined with
-        PRIMARY KEY AUTOINCREMENT
-        (NOT result set size)
+        A list with the new primary-key value (or values) for an
+        INSERT in a table defined with PRIMARY KEY AUTOINCREMENT (NOT
+        result set size).
 
-        :rtype: list or None
+        :rtype: :obj:`list` or :obj:`None`
         """
+
         if self._return_code != 0:
             return None
         info = self._body.get(IPROTO_SQL_INFO)
 
         if info is None:
             return None
 
         autoincrement_ids = info.get(IPROTO_SQL_INFO_AUTOINCREMENT_IDS)
 
         return autoincrement_ids
 
     @property
     def affected_row_count(self):
         """
-        Returns the number of changed rows for responses
-        to DML requests and None for DQL requests.
+        The number of changed rows for responses to DML requests and
+        ``None`` for DQL requests.
 
-        :rtype: int
+        :rtype: :obj:`int` or :obj:`None`
         """
+
         if self._return_code != 0:
             return None
         info = self._body.get(IPROTO_SQL_INFO)
 
         if info is None:
             return None
 
         return info.get(IPROTO_SQL_INFO_ROW_COUNT)
+
+
+class ResponseProtocolVersion(Response):
+    """
+    Represents an ID request response: information about server protocol
+    version and features it supports.
+    """
+
+    @property
+    def protocol_version(self):
+        """
+        Server protocol version.
+
+        :rtype: :obj:`int` or :obj:`None`
+        """
+
+        if self._return_code != 0:
+            return None
+        return self._body.get(IPROTO_VERSION)
+
+    @property
+    def features(self):
+        """
+        Server supported features.
+
+        :rtype: :obj:`list`
+        """
+
+        if self._return_code != 0:
+            return []
+        return self._body.get(IPROTO_FEATURES)
+
+    @property
+    def auth_type(self):
+        """
+        Server expected authentication method.
+
+        :rtype: :obj:`str` or :obj:`None`
+        """
+
+        if self._return_code != 0:
+            return None
+        return to_unicode(self._body.get(IPROTO_AUTH_TYPE))
```

### Comparing `tarantool-0.9.0/tarantool/error.py` & `tarantool-1.0.0/tarantool/error.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,122 +1,134 @@
-# -*- coding: utf-8 -*-
-# pylint: disable=C0301,W0105,W0401,W0614
-'''
-Python DB API compatible exceptions
-http://www.python.org/dev/peps/pep-0249/
-
-The PEP-249 says that database related exceptions must be inherited as follows:
-
-    StandardError
-    |__Warning
-    |__Error
-       |__InterfaceError
-       |__DatabaseError
-          |__DataError
-          |__OperationalError
-          |__IntegrityError
-          |__InternalError
-          |__ProgrammingError
-          |__NotSupportedError
-'''
+"""
+Python DB API compatible exceptions, see `PEP-249`_.
+
+.. _PEP-249: http://www.python.org/dev/peps/pep-0249/
+"""
 
 import os
 import socket
-try:
-    import ssl
-    is_ssl_supported = True
-except ImportError:
-    is_ssl_supported = False
 import sys
 import warnings
 
 
-try:
-    class Warning(StandardError):
-        '''Exception raised for important warnings
-        like data truncations while inserting, etc. '''
-except NameError:
-    class Warning(Exception):
-        '''Exception raised for important warnings
-        like data truncations while inserting, etc. '''
-
-try:
-    class Error(StandardError):
-        '''Base class for error exceptions'''
-except NameError:
-    class Error(Exception):
-        '''Base class for error exceptions'''
+class Error(Exception):
+    """
+    Base class for error exceptions.
+    """
 
 
 class InterfaceError(Error):
-    '''
-    Exception raised for errors that are related to the database interface
-    rather than the database itself.
-    '''
+    """
+    Exception raised for errors that are related to the database
+    interface rather than the database itself.
+    """
 
 
 class DatabaseError(Error):
-    '''Exception raised for errors that are related to the database.'''
+    """
+    Exception raised for errors that are related to the database.
+    """
+
+    def __init__(self, *args, extra_info=None):
+        """
+        :param args: ``(code, message)`` or ``(message,)``.
+        :type args: :obj:`tuple`
+
+        :param extra_info: Additional `box.error`_ information
+            with backtrace.
+        :type extra_info: :class:`~tarantool.types.BoxError` or
+            :obj:`None`, optional
+
+        .. _box.error: https://www.tarantool.io/en/doc/latest/reference/reference_lua/box_error/error/
+        """
+
+        super().__init__(*args)
+
+        if (len(args) == 2) and isinstance(args[0], int) and isinstance(args[1], (str, bytes)):
+            self.code = args[0]
+            self.message = args[1]
+        elif (len(args) == 1) and isinstance(args[0], (str, bytes)):
+            self.code = 0
+            self.message = args[0]
+        else:
+            self.code = 0
+            self.message = ''
+
+        self.extra_info = extra_info
 
 
 class DataError(DatabaseError):
-    '''
-    Exception raised for errors that are due to problems with the processed
-    data like division by zero, numeric value out of range, etc.
-    '''
+    """
+    Exception raised for errors that are due to problems with the
+    processed data like division by zero, numeric value out of range,
+    etc.
+    """
 
 
 class OperationalError(DatabaseError):
-    '''
-    Exception raised for errors that are related to the database's operation
-    and not necessarily under the control of the programmer, e.g. an
-    unexpected disconnect occurs, the data source name is not found,
-    a transaction could not be processed, a memory allocation error occurred
-    during processing, etc.
-    '''
+    """
+    Exception raised for errors that are related to the database's
+    operation and not necessarily under the control of the programmer,
+    e.g. an unexpected disconnect occurs, the data source name is not
+    found, a transaction could not be processed, a memory allocation
+    error occurred during processing, etc.
+    """
 
 
 class IntegrityError(DatabaseError):
-    '''
-    Exception raised when the relational integrity of the database is affected,
-    e.g. a foreign key check fails.
-    '''
+    """
+    Exception raised when the relational integrity of the database is
+    affected, e.g. a foreign key check fails.
+    """
 
 
 class InternalError(DatabaseError):
-    '''
-    Exception raised when the database encounters an internal error, e.g. the
-    cursor is not valid anymore, the transaction is out of sync, etc.
-    '''
+    """
+    Exception raised when the database encounters an internal error,
+    e.g. the cursor is not valid anymore, the transaction is out of
+    sync, etc.
+    """
 
 
 class ProgrammingError(DatabaseError):
-    '''
-    Exception raised when the database encounters an internal error, e.g. the
-    cursor is not valid anymore, the transaction is out of sync, etc.
-    '''
+    """
+    Exception raised when the database encounters an internal error,
+    e.g. the cursor is not valid anymore, the transaction is out of
+    sync, etc.
+    """
 
 
 class NotSupportedError(DatabaseError):
-    '''
-    Exception raised in case a method or database API was used which is not
-    supported by the database, e.g. requesting a .rollback() on a connection
-    that does not support transaction or has transactions turned off.
-    '''
+    """
+    Exception raised in case a method or database API was used which is
+    not supported by the database, e.g. requesting a .rollback() on a
+    connection that does not support transactions or has transactions
+    turned off.
+    """
 
 
 class ConfigurationError(Error):
-    '''
+    """
     Error of initialization with a user-provided configuration.
-    '''
+    """
+
+
+class MsgpackError(Error):
+    """
+    Error with encoding or decoding of `MP_EXT`_ types.
+
+    .. _MP_EXT: https://www.tarantool.io/en/doc/latest/dev_guide/internals/msgpack_extensions/
+    """
 
 
-__all__ = ("Warning", "Error", "InterfaceError", "DatabaseError", "DataError",
-           "OperationalError", "IntegrityError", "InternalError",
-           "ProgrammingError", "NotSupportedError")
+class MsgpackWarning(UserWarning):
+    """
+    Warning with encoding or decoding of `MP_EXT`_ types.
+    """
+
 
 # Monkey patch os.strerror for win32
 if sys.platform == "win32":
     # Windows Sockets Error Codes (not all, but related on network errors)
     # http://msdn.microsoft.com/en-us/library/windows/desktop/ms740668(v=vs.85).aspx
     _code2str = {
         10004: "Interrupted system call",
@@ -158,118 +170,228 @@
         11001: "Host not found",
         11004: "Name or service not known"
     }
 
     os_strerror_orig = os.strerror
 
     def os_strerror_patched(code):
-        '''
+        """
         Return cross-platform message about socket-related errors
 
         This function exists because under Windows os.strerror returns
         'Unknown error' on all socket-related errors.
         And socket-related exception contain broken non-ascii encoded messages.
-        '''
+        """
         message = os_strerror_orig(code)
         if not message.startswith("Unknown"):
             return message
-        else:
-            return _code2str.get(code, "Unknown error %s" % code)
+
+        return _code2str.get(code, f"Unknown error {code}")
 
     os.strerror = os_strerror_patched
     del os_strerror_patched
 
 
 class SchemaError(DatabaseError):
+    """
+    Error related to extracting space and index schema.
+    """
+
     def __init__(self, value):
-        super(SchemaError, self).__init__(0, value)
+        """
+        :param value: Error value.
+        """
+
+        super().__init__(0, value)
         self.value = value
 
     def __str__(self):
         return str(self.value)
 
 
 class SchemaReloadException(DatabaseError):
+    """
+    Error related to outdated space and index schema.
+    """
+
     def __init__(self, message, schema_version):
-        super(SchemaReloadException, self).__init__(109, message)
-        self.code = 109
-        self.message = message
+        """
+        :param message: Error message.
+        :type message: :obj:`str`
+
+        :param schema_version: Response schema version.
+        :type schema_version: :obj:`int`
+        """
+
+        super().__init__(109, message)
         self.schema_version = schema_version
 
     def __str__(self):
         return str(self.message)
 
 
 class NetworkError(DatabaseError):
-    '''Error related to network'''
+    """
+    Error related to network.
+    """
+
+    def __init__(self, *args, **kwargs):
+        """
+        :param args: Exception arguments. If the first argument is
+           a socket exception, it is wrapped.
+        :type args: :obj:`tuple`, optional
+
+        :param kwargs: Exception to wrap.
+        :type args: :obj:`dict`, optional
+        """
 
-    def __init__(self, orig_exception=None, *args):
         self.errno = 0
-        if hasattr(orig_exception, 'errno'):
-            self.errno = orig_exception.errno
-        if orig_exception:
+
+        if len(args) > 0:
+            orig_exception = args[0]
+
+            if hasattr(orig_exception, 'errno'):
+                self.errno = orig_exception.errno
+
             if isinstance(orig_exception, socket.timeout):
                 self.message = "Socket timeout"
-                super(NetworkError, self).__init__(0, self.message)
-            elif isinstance(orig_exception, socket.error):
+                super().__init__(0, self.message)
+                return
+
+            if isinstance(orig_exception, socket.error):
                 self.message = os.strerror(orig_exception.errno)
-                super(NetworkError, self).__init__(
-                    orig_exception.errno, self.message)
-            else:
-                super(NetworkError, self).__init__(orig_exception, *args)
+                super().__init__(orig_exception.errno, self.message)
+                return
+
+        super().__init__(*args, **kwargs)
 
 
 class NetworkWarning(UserWarning):
-    '''Warning related to network'''
-    pass
+    """
+    Warning related to network.
+    """
+
 
 class SslError(DatabaseError):
-    '''Error related to SSL'''
+    """
+    Error related to SSL.
+    """
+
+    def __init__(self, *args, **kwargs):
+        """
+        :param args: Exception arguments. If the first argument is
+           a socket exception, it is wrapped.
+        :type args: :obj:`tuple`, optional
+
+        :param kwargs: Exception to wrap.
+        :type args: :obj:`dict`, optional
+        """
 
-    def __init__(self, orig_exception=None, *args):
         self.errno = 0
-        if hasattr(orig_exception, 'errno'):
-            self.errno = orig_exception.errno
-        if orig_exception:
-            if is_ssl_supported and isinstance(orig_exception, ssl.SSLError):
-                super(SslError, self).__init__(orig_exception, *args)
-            else:
-                super(SslError, self).__init__(orig_exception, *args)
+
+        if len(args) > 0:
+            orig_exception = args[0]
+
+            if hasattr(orig_exception, 'errno'):
+                self.errno = orig_exception.errno
+
+        super().__init__(*args, **kwargs)
 
 
 class ClusterDiscoveryWarning(UserWarning):
-    '''Warning related to cluster discovery'''
-    pass
+    """
+    Warning related to cluster discovery.
+    """
 
 
 class ClusterConnectWarning(UserWarning):
-    '''Warning related to cluster pool connection'''
-    pass
+    """
+    Warning related to cluster pool connection.
+    """
 
 
 class PoolTolopogyWarning(UserWarning):
-    '''Warning related to ro/rw cluster pool topology'''
-    pass
+    """
+    Warning related to unsatisfying `box.info.ro`_ state of
+    pool instances.
+    """
 
 
 class PoolTolopogyError(DatabaseError):
-    '''Exception raised due to unsatisfying ro/rw cluster pool topology'''
-    pass
+    """
+    Exception raised due to unsatisfying `box.info.ro`_ state of
+    pool instances.
+
+    .. _box.info.ro: https://www.tarantool.io/en/doc/latest/reference/reference_lua/box_info/
+    """
+
+
+class CrudModuleError(DatabaseError):
+    """
+    Exception raised for errors that are related to
+    the operation result of `crud`_ module.
+
+    .. _crud: https://github.com/tarantool/crud
+    """
+
+    def __init__(self, _, error):
+        """
+        Sets fields with result and errors.
+
+        :param args: The tuple from the crud module with result and errors.
+        :type args: :obj:`tuple`
+        """
+
+        super().__init__(0, error.err)
+        # Sets tarantool.crud.CrudError object.
+        self.extra_info_error = error
+
+
+class CrudModuleManyError(DatabaseError):
+    """
+    Exception raised for errors that are related to
+    the batching operation result of `crud`_ module.
+
+    .. _crud: https://github.com/tarantool/crud
+    """
+
+    def __init__(self, success, error):
+        """
+        Sets fields with result and errors.
+
+        :param args: The tuple from the crud module with result and errors.
+        :type args: :obj:`tuple`
+        """
+
+        exc_msg = "Got multiple errors, see errors_list and success_list"
+        super().__init__(0, exc_msg)
+        # Sets list of tarantool.crud.CrudResult objects.
+        self.success_list = success
+        # Sets list of tarantool.crud.CrudError objects.
+        self.errors_list = error
 
 
 # always print this warnings
 warnings.filterwarnings("always", category=NetworkWarning)
 
 
 def warn(message, warning_class):
-    '''
-    Emit warinig message.
+    """
+    Emit a warning message.
     Just like standard warnings.warn() but don't output full filename.
-    '''
-    frame = sys._getframe(2)  # pylint: disable=W0212
+
+    :param message: Warning message.
+    :type message: :obj:`str`
+
+    :param warning_class: Warning class.
+    :type warning_class: :class:`~tarantool.error.Warning`
+    """
+    # pylint: disable=protected-access
+
+    frame = sys._getframe(2)
     module_name = frame.f_globals.get("__name__")
     line_no = frame.f_lineno
     warnings.warn_explicit(message, warning_class, module_name, line_no)
 
 
 _strerror = {
     0: ("ER_UNKNOWN", "Unknown error"),
@@ -443,11 +565,27 @@
     111: ("ER_WRONG_SPACE_OPTIONS", "Wrong space options (field %u): %s"),
     112: ("ER_UNSUPPORTED_INDEX_FEATURE",
           "Index '%s' (%s) of space '%s' (%s) does not support %s"),
     113: ("ER_VIEW_IS_RO", "View '%s' is read-only"),
 }
 
 
+# Response error code for case "Requested procedure is not defined".
+ER_NO_SUCH_PROC = 33
+# Response error code for case "Access is denied for user".
+ER_ACCESS_DENIED = 42
+
+
 def tnt_strerror(num):
+    """
+    Parse Tarantool error to string data.
+
+    :param num: Tarantool error code.
+    :type num: :obj:`int`
+
+    :return: Tuple ``(ER_NAME, message)`` or ``"UNDEFINED"``.
+    :rtype: :obj:`tuple` or :obj:`str`
+    """
+
     if num in _strerror:
         return _strerror[num]
     return "UNDEFINED"
```

### Comparing `tarantool-0.9.0/PKG-INFO` & `tarantool-1.0.0/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,140 +1,184 @@
-Metadata-Version: 2.1
-Name: tarantool
-Version: 0.9.0
-Summary: Python client library for Tarantool 1.6 Database
-Home-page: https://github.com/tarantool/tarantool-python
-Author: Konstantin Cherkasoff
-Author-email: k.cherkasoff@gmail.com
-License: BSD
-Description: Python driver for Tarantool
-        ===========================
-        
-        This package is a pure-python client library for `Tarantool`_.
-        
-        `Documentation`_  |  `Downloads`_  |  `PyPI`_  |  `GitHub`_  | `Issue tracker`_
-        
-        .. _`Documentation`: http://tarantool-python.readthedocs.org/en/latest/
-        .. _`Downloads`: http://pypi.python.org/pypi/tarantool#downloads
-        .. _`PyPI`: http://pypi.python.org/pypi/tarantool
-        .. _`GitHub`: https://github.com/tarantool/tarantool-python
-        .. _`Issue tracker`: https://github.com/tarantool/tarantool-python/issues
-        
-        .. image:: https://github.com/tarantool/tarantool-python/actions/workflows/testing.yml/badge.svg?branch=master
-            :target: https://github.com/tarantool/tarantool-python/actions/workflows/testing.yml
-        
-        Download and Install
-        --------------------
-        
-        The recommended way to install ``tarantool`` package is using PIP
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        For Tarantool version < 1.6.0 you must get ``0.3.*`` connector version::
-        
-            $ pip install tarantool\<0.4
-        
-        For later Tarantool use version ``0.5.*`` connector version::
-        
-            $ pip install tarantool\>0.4
-        
-        You can also download zip archive, unpack it and run
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        .. code-block:: console
-        
-            $ python setup.py install
-        
-        To install development version of the package using pip
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        For Tarantool version < 1.6.0 you must get ``stable`` branch::
-        
-            $ pip install git+https://github.com/tarantool/tarantool-python.git@stable
-        
-        For later Tarantool use ``master`` branch::
-        
-            $ pip install git+https://github.com/tarantool/tarantool-python.git@master
-        
-        --------------------------------------------------------------------------------
-        
-        What is Tarantool?
-        ------------------
-        
-        `Tarantool`_ is a NoSQL database running inside a Lua program. It combines the
-        network programming power of Node.JS with data persistency capabilities of
-        Redis. It's open source, `BSD-2-Clause`_ licensed.
-        
-        Features
-        --------
-        
-        * ANSI SQL, including views, joins, referential and check constraints
-        * Lua packages for non-blocking I/O, fibers and HTTP
-        * MsgPack data format and MsgPack based client-server protocol
-        * Two data engines:
-        
-          * memtx - the in-memory storage engine with optional persistence
-          * vinyl - the on-disk storage engine to use with large data sets
-        
-        * secondary key and index iterators support (can be non-unique and composite)
-        * multiple index types: HASH, BITSET, TREE, RTREE
-        * asynchronous master-master replication
-        * authentication and access control
-        
-        See More
-        ^^^^^^^^
-        
-        * `Tarantool Homepage`_
-        * `Tarantool at Github`_
-        * `Tarantool User Guide`_
-        * `Client-server Protocol Specification`_
-        
-        NOTE
-        ^^^^
-        
-        This driver is synchronous, so connection mustn't be shared between threads/processes.
-        
-        Look at `asynctnt`_ for asynchronous Python driver based on asyncio. See
-        also the `feature comparison table`_.
-        
-        Run tests
-        ^^^^^^^^^
-        
-        On Linux:
-        
-        .. code-block:: console
-        
-           $ python setup.py test
-        
-        On Windows:
-        
-        * Setup a Linux machine with installed tarantool (called ``remote`` later).
-        * (on ``remote``) Copy ``test/suites/lib/tarantool_python_ci.lua`` to
-          ``/etc/tarantool/instances.available``.
-        * (on ``remote``) Run ``tarantoolctl start tarantool_python_ci``.
-        * Set the following environment variables:
-          * ``REMOTE_TARANTOOL_HOST=...``,
-          * ``REMOTE_TARANTOOL_CONSOLE_PORT=3302``.
-        * Run ``python setup.py test``.
-        
-        .. _`Tarantool`:
-        .. _`Tarantool Database`:
-        .. _`Tarantool Homepage`: https://tarantool.io
-        .. _`Tarantool at Github`: https://github.com/tarantool/tarantool
-        .. _`Tarantool User Guide`: https://www.tarantool.io/en/doc/latest/
-        .. _`Client-server protocol specification`: https://www.tarantool.io/en/doc/latest/dev_guide/internals/box_protocol/
-        .. _`BSD-2-Clause`: https://opensource.org/licenses/BSD-2-Clause
-        .. _`asynctnt`: https://github.com/igorcoding/asynctnt
-        .. _`feature comparison table`: https://www.tarantool.io/en/doc/latest/book/connectors/#python-feature-comparison
-        
-        License
-        ^^^^^^^
-        
-        BSD-2-Clause. See the ``LICENSE`` file.
-        
-Platform: all
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Database :: Front-Ends
-Requires-Python: >=3
-Description-Content-Type: text/x-rst
+Python driver for Tarantool
+===========================
+
+.. image:: https://github.com/tarantool/tarantool-python/actions/workflows/testing.yml/badge.svg?branch=master
+    :target: https://github.com/tarantool/tarantool-python/actions/workflows/testing.yml
+.. image:: https://github.com/tarantool/tarantool-python/actions/workflows/packing.yml/badge.svg?branch=master
+    :target: https://github.com/tarantool/tarantool-python/actions/workflows/packing.yml
+
+This package is a pure-python client library for `Tarantool`_.
+
+`Documentation`_  |  `Downloads`_  |  `PyPI`_  |  `GitHub`_  | `Issue tracker`_
+
+.. _`Documentation`: http://tarantool-python.readthedocs.org/en/latest/
+.. _`Downloads`: http://pypi.python.org/pypi/tarantool#downloads
+.. _`PyPI`: http://pypi.python.org/pypi/tarantool
+.. _`GitHub`: https://github.com/tarantool/tarantool-python
+.. _`Issue tracker`: https://github.com/tarantool/tarantool-python/issues
+
+Download and install
+--------------------
+
+With pip (recommended)
+^^^^^^^^^^^^^^^^^^^^^^
+
+The recommended way to install the ``tarantool`` package is using ``pip``.
+
+.. code-block:: bash
+
+     $ pip3 install tarantool
+
+With dnf
+^^^^^^^^
+
+You can install ``python3-tarantool`` RPM package if you use Fedora (34, 35, 36).
+
+Add the repository
+
+.. code-block:: bash
+
+     $ curl -L https://tarantool.io/OtKysgx/release/2/installer.sh | bash
+
+and then install the package
+
+.. code-block:: bash
+
+     $ dnf install -y python3-tarantool
+
+With apt
+^^^^^^^^
+
+You can install ``python3-tarantool`` deb package if you use
+Debian (10, 11) or Ubuntu (20.04, 22.04).
+
+Add the repository
+
+.. code-block:: bash
+
+     $ curl -L https://tarantool.io/OtKysgx/release/2/installer.sh | bash
+
+and then install the package
+
+.. code-block:: bash
+
+     $ apt install -y python3-tarantool
+
+ZIP archive
+^^^^^^^^^^^
+
+You can also download zip archive, unpack it and run:
+
+.. code-block:: bash
+
+    $ make install
+
+Development version
+^^^^^^^^^^^^^^^^^^^
+
+You can also install the development version of the package using ``pip``.
+
+.. code-block:: bash
+
+    $ pip3 install git+https://github.com/tarantool/tarantool-python.git@master
+
+--------------------------------------------------------------------------------
+
+What is Tarantool?
+------------------
+
+`Tarantool`_ is an in-memory computing platform originally designed by
+`VK`_ and released under the terms of `BSD license`_.
+
+Features
+--------
+
+* ANSI SQL, including views, joins, referential and check constraints
+* Lua packages for non-blocking I/O, fibers, and HTTP
+* MessagePack data format and MessagePack-based client-server protocol
+* Two data engines:
+
+  * memtx – in-memory storage engine with optional persistence
+  * vinyl – on-disk storage engine to use with larger data sets
+
+* Secondary key and index iterator support (can be non-unique and composite)
+* Multiple index types: HASH, BITSET, TREE, RTREE
+* Asynchronous master-master replication
+* Authentication and access control
+
+See More
+^^^^^^^^
+
+* `Tarantool homepage`_
+* `Tarantool on GitHub`_
+* `Tarantool documentation`_
+* `Client-server protocol specification`_
+
+NOTE
+^^^^
+
+This driver is synchronous, so connection mustn't be shared between threads/processes.
+
+If you're looking for an asynchronous Python driver based on ``asyncio``,
+consider using `asynctnt`_ . See also the `feature comparison table`_.
+
+Run tests
+^^^^^^^^^
+
+On Linux:
+
+.. code-block:: bash
+
+   $ make test
+
+On Windows:
+
+* Setup a Linux machine with Tarantool installed.
+  This machine will be referred to as ``remote`` in this instruction.
+* (On ``remote``) Copy ``test/suites/lib/tarantool_python_ci.lua`` to
+  ``/etc/tarantool/instances.available``.
+* (On ``remote``) Run ``tarantoolctl start tarantool_python_ci``.
+* Set the following environment variables:
+  * ``REMOTE_TARANTOOL_HOST=...``,
+  * ``REMOTE_TARANTOOL_CONSOLE_PORT=3302``.
+* Run ``make test``.
+
+Build docs
+^^^^^^^^^^
+
+To build documentation, first you must install its build requirements:
+
+.. code-block:: bash
+
+    $ pip3 install -r docs/requirements.txt
+
+Then run
+
+.. code-block:: bash
+
+    $ make docs
+
+You may host local documentation server with
+
+.. code-block:: bash
+
+    $ python3 -m http.server --directory build/sphinx/html
+
+Open ``localhost:8000`` in your browser to read the docs.
+
+.. _`Tarantool`:
+.. _`Tarantool Database`:
+.. _`Tarantool homepage`: https://tarantool.io
+.. _`Tarantool on GitHub`: https://github.com/tarantool/tarantool
+.. _`Tarantool documentation`: https://www.tarantool.io/en/doc/latest/
+.. _`VK`: https://vk.company
+.. _`Client-server protocol specification`: https://www.tarantool.io/en/doc/latest/dev_guide/internals/box_protocol/
+.. _`BSD`:
+.. _`BSD license`:
+.. _`BSD-2-Clause`: https://opensource.org/licenses/BSD-2-Clause
+.. _`asynctnt`: https://github.com/igorcoding/asynctnt
+.. _`feature comparison table`: https://www.tarantool.io/en/doc/latest/book/connectors/#python-feature-comparison
+
+License
+^^^^^^^
+
+BSD-2-Clause. See the ``LICENSE`` file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

