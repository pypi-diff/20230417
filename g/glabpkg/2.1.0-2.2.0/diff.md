# Comparing `tmp/glabpkg-2.1.0.tar.gz` & `tmp/glabpkg-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glabpkg-2.1.0.tar", last modified: Tue Feb  7 12:59:04 2023, max compression
+gzip compressed data, was "glabpkg-2.2.0.tar", last modified: Mon Apr 17 13:12:13 2023, max compression
```

## Comparing `glabpkg-2.1.0.tar` & `glabpkg-2.2.0.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.474513 glabpkg-2.1.0/
--rw-rw-rw-   0        0        0      352 2023-02-07 12:47:00.000000 glabpkg-2.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3310 2023-02-07 12:47:00.000000 glabpkg-2.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2023-02-07 12:47:00.000000 glabpkg-2.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2023-02-07 12:47:00.000000 glabpkg-2.1.0/LICENSE
--rw-rw-rw-   0        0        0      435 2023-02-07 12:47:00.000000 glabpkg-2.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2460 2023-02-07 12:59:04.474513 glabpkg-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1561 2023-02-07 12:47:00.000000 glabpkg-2.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.661089 glabpkg-2.1.0/doc/
--rw-rw-rw-   0        0        0     6967 2023-02-07 12:47:00.000000 glabpkg-2.1.0/doc/Makefile
--rw-rw-rw-   0        0        0       29 2023-02-07 12:47:00.000000 glabpkg-2.1.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.661089 glabpkg-2.1.0/doc/badges/
--rw-rw-rw-   0        0        0      282 2023-02-07 12:47:00.000000 glabpkg-2.1.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.688347 glabpkg-2.1.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2023-02-07 12:47:00.000000 glabpkg-2.1.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     4287 2023-02-07 12:47:00.000000 glabpkg-2.1.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2023-02-07 12:47:00.000000 glabpkg-2.1.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-02-07 12:47:00.000000 glabpkg-2.1.0/doc/history.rst
--rw-rw-rw-   0        0        0      579 2023-02-07 12:47:00.000000 glabpkg-2.1.0/doc/index.rst
--rw-rw-rw-   0        0        0      217 2023-02-07 12:47:00.000000 glabpkg-2.1.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2023-02-07 12:47:00.000000 glabpkg-2.1.0/doc/make.bat
--rw-rw-rw-   0        0        0      133 2023-02-07 12:47:00.000000 glabpkg-2.1.0/doc/management.rst
--rw-rw-rw-   0        0        0     1483 2023-02-07 12:47:00.000000 glabpkg-2.1.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2023-02-07 12:47:00.000000 glabpkg-2.1.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.691532 glabpkg-2.1.0/doc/user/
--rw-rw-rw-   0        0        0       86 2023-02-07 12:47:00.000000 glabpkg-2.1.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2023-02-07 12:47:00.000000 glabpkg-2.1.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      277 2023-02-07 12:47:00.000000 glabpkg-2.1.0/requirements.txt
--rw-rw-rw-   0        0        0       44 2023-02-07 12:47:00.000000 glabpkg-2.1.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2023-02-07 12:59:04.496703 glabpkg-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2464 2023-02-07 12:47:00.000000 glabpkg-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.413558 glabpkg-2.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.722800 glabpkg-2.1.0/src/glabpkg/
--rw-rw-rw-   0        0        0      167 2023-02-07 12:47:00.000000 glabpkg-2.1.0/src/glabpkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.782692 glabpkg-2.1.0/src/glabpkg/base/
--rw-rw-rw-   0        0        0        0 2020-02-06 17:37:05.000000 glabpkg-2.1.0/src/glabpkg/base/__init__.py
--rw-rw-rw-   0        0        0      853 2021-06-25 18:38:58.000000 glabpkg-2.1.0/src/glabpkg/base/option.py
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.798344 glabpkg-2.1.0/src/glabpkg/base/resource/
--rw-rw-rw-   0        0        0      434 2020-02-06 17:37:05.000000 glabpkg-2.1.0/src/glabpkg/base/resource/.gitattributes.tpl
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.413558 glabpkg-2.1.0/src/glabpkg/base/resource/.gitlab/
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.813976 glabpkg-2.1.0/src/glabpkg/base/resource/.gitlab/issue_templates/
--rw-rw-rw-   0        0        0      160 2020-02-21 10:42:42.000000 glabpkg-2.1.0/src/glabpkg/base/resource/.gitlab/issue_templates/bug.md
--rw-rw-rw-   0        0        0      102 2020-02-21 10:42:42.000000 glabpkg-2.1.0/src/glabpkg/base/resource/.gitlab/issue_templates/feature.md
--rw-rw-rw-   0        0        0       53 2020-02-21 10:42:42.000000 glabpkg-2.1.0/src/glabpkg/base/resource/.gitlab/issue_templates/technical_task.md
--rw-rw-rw-   0        0        0      363 2021-08-26 14:10:46.000000 glabpkg-2.1.0/src/glabpkg/base/resource/.gitlab-ci.yml
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.829594 glabpkg-2.1.0/src/glabpkg/data/
--rw-rw-rw-   0        0        0        0 2021-07-06 09:14:59.000000 glabpkg-2.1.0/src/glabpkg/data/__init__.py
--rw-rw-rw-   0        0        0      332 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/data/option.py
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.429182 glabpkg-2.1.0/src/glabpkg/data/resource/
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.829594 glabpkg-2.1.0/src/glabpkg/data/resource/script/
--rw-rw-rw-   0        0        0      122 2021-07-06 09:14:59.000000 glabpkg-2.1.0/src/glabpkg/data/resource/script/readme.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.429182 glabpkg-2.1.0/src/glabpkg/data/resource/src/
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.829594 glabpkg-2.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0       82 2021-07-06 09:14:59.000000 glabpkg-2.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/__init__.py.tpl
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.829594 glabpkg-2.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/clean/
--rw-rw-rw-   0        0        0      134 2021-07-06 09:14:59.000000 glabpkg-2.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/clean/readme.rst
--rw-rw-rw-   0        0        0      193 2021-07-06 09:14:59.000000 glabpkg-2.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/info.py.tpl
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.829594 glabpkg-2.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/raw/
--rw-rw-rw-   0        0        0      117 2021-07-06 09:14:59.000000 glabpkg-2.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/raw/readme.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.860838 glabpkg-2.1.0/src/glabpkg/data_alt/
--rw-rw-rw-   0        0        0        0 2022-01-13 14:44:45.000000 glabpkg-2.1.0/src/glabpkg/data_alt/__init__.py
--rw-rw-rw-   0        0        0      331 2022-01-13 14:44:45.000000 glabpkg-2.1.0/src/glabpkg/data_alt/option.py
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.444822 glabpkg-2.1.0/src/glabpkg/data_alt/resource/
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.860838 glabpkg-2.1.0/src/glabpkg/data_alt/resource/script/
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.876465 glabpkg-2.1.0/src/glabpkg/data_alt/resource/script/raw/
--rw-rw-rw-   0        0        0      117 2022-01-13 14:44:45.000000 glabpkg-2.1.0/src/glabpkg/data_alt/resource/script/raw/readme.rst
--rw-rw-rw-   0        0        0      122 2022-01-13 14:44:45.000000 glabpkg-2.1.0/src/glabpkg/data_alt/resource/script/readme.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.444822 glabpkg-2.1.0/src/glabpkg/data_alt/resource/src/
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.898624 glabpkg-2.1.0/src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0       73 2022-01-13 14:44:45.000000 glabpkg-2.1.0/src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/__init__.py.tpl
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.998906 glabpkg-2.1.0/src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/clean/
--rw-rw-rw-   0        0        0      134 2022-01-13 14:44:45.000000 glabpkg-2.1.0/src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/clean/readme.rst
--rw-rw-rw-   0        0        0      152 2022-01-13 14:44:45.000000 glabpkg-2.1.0/src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/info.py.tpl
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.061407 glabpkg-2.1.0/src/glabpkg/pkg/
--rw-rw-rw-   0        0        0        0 2021-06-25 14:18:59.000000 glabpkg-2.1.0/src/glabpkg/pkg/__init__.py
--rw-rw-rw-   0        0        0     1686 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg/option.py
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.460460 glabpkg-2.1.0/src/glabpkg/pkg/resource/
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.093672 glabpkg-2.1.0/src/glabpkg/pkg/resource/doc/
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.176625 glabpkg-2.1.0/src/glabpkg/pkg/resource/doc/badges/
--rw-rw-rw-   0        0        0     1094 2021-07-06 09:29:24.000000 glabpkg-2.1.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_conda.svg
--rw-rw-rw-   0        0        0     1090 2021-07-06 09:29:24.000000 glabpkg-2.1.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_pip.svg
--rw-rw-rw-   0        0        0      172 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg/resource/doc/badges/listing.rst
--rw-rw-rw-   0        0        0      184 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg/resource/doc/installation.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.247651 glabpkg-2.1.0/src/glabpkg/pkg_dev/
--rw-rw-rw-   0        0        0        0 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/__init__.py
--rw-rw-rw-   0        0        0     1880 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/option.py
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.257784 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/
--rw-rw-rw-   0        0        0     1831 2023-02-07 12:30:22.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      444 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.277976 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/
--rw-rw-rw-   0        0        0       29 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.286063 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/badges/
--rw-rw-rw-   0        0        0     1002 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/badges/badge_doc.svg
--rw-rw-rw-   0        0        0      110 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.296072 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/biblio/
--rw-rw-rw-   0        0        0      513 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0       34 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/history.rst
--rw-rw-rw-   0        0        0      634 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/index.rst
--rw-rw-rw-   0        0        0      209 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/installation.rst
--rw-rw-rw-   0        0        0      133 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/management.rst
--rw-rw-rw-   0        0        0      541 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.296072 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/user/
--rw-rw-rw-   0        0        0       86 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/user/overview.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.296072 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/example/
--rw-rw-rw-   0        0        0      254 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/example/readme.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.296072 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/test/
--rw-rw-rw-   0        0        0      114 2022-12-04 11:33:38.000000 glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/test/test_packaging.py.tpl
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.311712 glabpkg-2.1.0/src/glabpkg/report/
--rw-rw-rw-   0        0        0        0 2021-07-06 09:29:24.000000 glabpkg-2.1.0/src/glabpkg/report/__init__.py
--rw-rw-rw-   0        0        0     1560 2021-07-06 09:29:24.000000 glabpkg-2.1.0/src/glabpkg/report/option.py
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.342961 glabpkg-2.1.0/src/glabpkg/report/resource/
--rw-rw-rw-   0        0        0     1025 2023-02-07 12:30:22.000000 glabpkg-2.1.0/src/glabpkg/report/resource/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      923 2022-03-28 12:29:45.000000 glabpkg-2.1.0/src/glabpkg/report/resource/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.374223 glabpkg-2.1.0/src/glabpkg/report/resource/report/
--rw-rw-rw-   0        0        0       51 2021-07-06 09:29:24.000000 glabpkg-2.1.0/src/glabpkg/report/resource/report/authors.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.412014 glabpkg-2.1.0/src/glabpkg/report/resource/report/badges/
--rw-rw-rw-   0        0        0     1001 2021-07-06 09:29:24.000000 glabpkg-2.1.0/src/glabpkg/report/resource/report/badges/badge_doc.svg
--rw-rw-rw-   0        0        0      109 2021-07-06 09:29:24.000000 glabpkg-2.1.0/src/glabpkg/report/resource/report/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.427649 glabpkg-2.1.0/src/glabpkg/report/resource/report/biblio/
--rw-rw-rw-   0        0        0      513 2021-07-06 09:29:24.000000 glabpkg-2.1.0/src/glabpkg/report/resource/report/biblio/biblio.rst
--rw-rw-rw-   0        0        0      130 2021-07-06 09:29:24.000000 glabpkg-2.1.0/src/glabpkg/report/resource/report/conf.py.tpl
--rw-rw-rw-   0        0        0      376 2021-07-06 09:29:24.000000 glabpkg-2.1.0/src/glabpkg/report/resource/report/index.rst
--rw-rw-rw-   0        0        0       89 2021-07-06 09:29:24.000000 glabpkg-2.1.0/src/glabpkg/report/resource/report/introduction.rst
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.443285 glabpkg-2.1.0/src/glabpkg/report/resource/script/
--rw-rw-rw-   0        0        0       56 2021-07-06 09:29:24.000000 glabpkg-2.1.0/src/glabpkg/report/resource/script/readme.rst
--rw-rw-rw-   0        0        0      367 2023-02-07 12:47:00.000000 glabpkg-2.1.0/src/glabpkg/version.py
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:03.769674 glabpkg-2.1.0/src/glabpkg.egg-info/
--rw-rw-rw-   0        0        0     2460 2023-02-07 12:59:03.000000 glabpkg-2.1.0/src/glabpkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3457 2023-02-07 12:59:03.000000 glabpkg-2.1.0/src/glabpkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-07 12:59:03.000000 glabpkg-2.1.0/src/glabpkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      307 2023-02-07 12:59:03.000000 glabpkg-2.1.0/src/glabpkg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2021-06-25 14:53:47.000000 glabpkg-2.1.0/src/glabpkg.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-02-07 12:59:03.000000 glabpkg-2.1.0/src/glabpkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-07 12:59:03.000000 glabpkg-2.1.0/src/glabpkg.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-07 12:59:04.474513 glabpkg-2.1.0/test/
--rw-rw-rw-   0        0        0      971 2023-02-07 12:47:00.000000 glabpkg-2.1.0/test/conftest.py
--rw-rw-rw-   0        0        0       80 2023-02-07 12:47:00.000000 glabpkg-2.1.0/test/test_packaging.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:13.005523 glabpkg-2.2.0/
+-rw-rw-rw-   0        0        0      352 2023-04-17 13:00:02.000000 glabpkg-2.2.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3310 2023-04-17 13:00:02.000000 glabpkg-2.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2023-04-17 13:00:02.000000 glabpkg-2.2.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2023-04-17 13:00:02.000000 glabpkg-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0      435 2023-04-17 13:00:02.000000 glabpkg-2.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2460 2023-04-17 13:12:13.005523 glabpkg-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1561 2023-04-17 13:00:02.000000 glabpkg-2.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.559940 glabpkg-2.2.0/doc/
+-rw-rw-rw-   0        0        0     6967 2023-04-17 13:00:02.000000 glabpkg-2.2.0/doc/Makefile
+-rw-rw-rw-   0        0        0       29 2023-04-17 13:00:02.000000 glabpkg-2.2.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.563938 glabpkg-2.2.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2023-04-17 13:00:02.000000 glabpkg-2.2.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.567941 glabpkg-2.2.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2023-04-17 13:00:02.000000 glabpkg-2.2.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     4287 2023-04-17 13:00:02.000000 glabpkg-2.2.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-17 13:00:02.000000 glabpkg-2.2.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-17 13:00:02.000000 glabpkg-2.2.0/doc/history.rst
+-rw-rw-rw-   0        0        0      579 2023-04-17 13:00:02.000000 glabpkg-2.2.0/doc/index.rst
+-rw-rw-rw-   0        0        0      217 2023-04-17 13:00:02.000000 glabpkg-2.2.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2023-04-17 13:00:02.000000 glabpkg-2.2.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2023-04-17 13:00:02.000000 glabpkg-2.2.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1483 2023-04-17 13:00:02.000000 glabpkg-2.2.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2023-04-17 13:00:02.000000 glabpkg-2.2.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.579941 glabpkg-2.2.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2023-04-17 13:00:02.000000 glabpkg-2.2.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2023-04-17 13:00:02.000000 glabpkg-2.2.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0      277 2023-04-17 13:00:02.000000 glabpkg-2.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       44 2023-04-17 13:00:02.000000 glabpkg-2.2.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0      201 2023-04-17 13:12:13.013523 glabpkg-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2464 2023-04-17 13:00:02.000000 glabpkg-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.322987 glabpkg-2.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.591939 glabpkg-2.2.0/src/glabpkg/
+-rw-rw-rw-   0        0        0      167 2023-04-17 13:00:02.000000 glabpkg-2.2.0/src/glabpkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.626693 glabpkg-2.2.0/src/glabpkg/base/
+-rw-rw-rw-   0        0        0        0 2020-02-06 17:37:05.000000 glabpkg-2.2.0/src/glabpkg/base/__init__.py
+-rw-rw-rw-   0        0        0      853 2021-06-25 18:38:58.000000 glabpkg-2.2.0/src/glabpkg/base/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.636282 glabpkg-2.2.0/src/glabpkg/base/resource/
+-rw-rw-rw-   0        0        0      434 2020-02-06 17:37:05.000000 glabpkg-2.2.0/src/glabpkg/base/resource/.gitattributes.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.346948 glabpkg-2.2.0/src/glabpkg/base/resource/.gitlab/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.648294 glabpkg-2.2.0/src/glabpkg/base/resource/.gitlab/issue_templates/
+-rw-rw-rw-   0        0        0      160 2020-02-21 10:42:42.000000 glabpkg-2.2.0/src/glabpkg/base/resource/.gitlab/issue_templates/bug.md
+-rw-rw-rw-   0        0        0      102 2020-02-21 10:42:42.000000 glabpkg-2.2.0/src/glabpkg/base/resource/.gitlab/issue_templates/feature.md
+-rw-rw-rw-   0        0        0       53 2020-02-21 10:42:42.000000 glabpkg-2.2.0/src/glabpkg/base/resource/.gitlab/issue_templates/technical_task.md
+-rw-rw-rw-   0        0        0      363 2021-08-26 14:10:46.000000 glabpkg-2.2.0/src/glabpkg/base/resource/.gitlab-ci.yml
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.656278 glabpkg-2.2.0/src/glabpkg/data/
+-rw-rw-rw-   0        0        0        0 2021-07-06 09:14:59.000000 glabpkg-2.2.0/src/glabpkg/data/__init__.py
+-rw-rw-rw-   0        0        0      332 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/data/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.358949 glabpkg-2.2.0/src/glabpkg/data/resource/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.672319 glabpkg-2.2.0/src/glabpkg/data/resource/script/
+-rw-rw-rw-   0        0        0      122 2021-07-06 09:14:59.000000 glabpkg-2.2.0/src/glabpkg/data/resource/script/readme.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.369127 glabpkg-2.2.0/src/glabpkg/data/resource/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.680284 glabpkg-2.2.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0       82 2021-07-06 09:14:59.000000 glabpkg-2.2.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/__init__.py.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.684278 glabpkg-2.2.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/clean/
+-rw-rw-rw-   0        0        0      134 2021-07-06 09:14:59.000000 glabpkg-2.2.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/clean/readme.rst
+-rw-rw-rw-   0        0        0      193 2021-07-06 09:14:59.000000 glabpkg-2.2.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/info.py.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.690515 glabpkg-2.2.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/raw/
+-rw-rw-rw-   0        0        0      117 2021-07-06 09:14:59.000000 glabpkg-2.2.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/raw/readme.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.750492 glabpkg-2.2.0/src/glabpkg/data_alt/
+-rw-rw-rw-   0        0        0        0 2022-01-13 14:44:45.000000 glabpkg-2.2.0/src/glabpkg/data_alt/__init__.py
+-rw-rw-rw-   0        0        0      331 2022-01-13 14:44:45.000000 glabpkg-2.2.0/src/glabpkg/data_alt/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.395307 glabpkg-2.2.0/src/glabpkg/data_alt/resource/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.764748 glabpkg-2.2.0/src/glabpkg/data_alt/resource/script/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.772714 glabpkg-2.2.0/src/glabpkg/data_alt/resource/script/raw/
+-rw-rw-rw-   0        0        0      117 2022-01-13 14:44:45.000000 glabpkg-2.2.0/src/glabpkg/data_alt/resource/script/raw/readme.rst
+-rw-rw-rw-   0        0        0      122 2022-01-13 14:44:45.000000 glabpkg-2.2.0/src/glabpkg/data_alt/resource/script/readme.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.399277 glabpkg-2.2.0/src/glabpkg/data_alt/resource/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.792713 glabpkg-2.2.0/src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0       73 2022-01-13 14:44:45.000000 glabpkg-2.2.0/src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/__init__.py.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.808737 glabpkg-2.2.0/src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/clean/
+-rw-rw-rw-   0        0        0      134 2022-01-13 14:44:45.000000 glabpkg-2.2.0/src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/clean/readme.rst
+-rw-rw-rw-   0        0        0      152 2022-01-13 14:44:45.000000 glabpkg-2.2.0/src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/info.py.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.816713 glabpkg-2.2.0/src/glabpkg/pkg/
+-rw-rw-rw-   0        0        0        0 2021-06-25 14:18:59.000000 glabpkg-2.2.0/src/glabpkg/pkg/__init__.py
+-rw-rw-rw-   0        0        0     1686 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.403273 glabpkg-2.2.0/src/glabpkg/pkg/resource/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.824734 glabpkg-2.2.0/src/glabpkg/pkg/resource/doc/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.838931 glabpkg-2.2.0/src/glabpkg/pkg/resource/doc/badges/
+-rw-rw-rw-   0        0        0     1094 2021-07-06 09:29:24.000000 glabpkg-2.2.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_conda.svg
+-rw-rw-rw-   0        0        0     1090 2021-07-06 09:29:24.000000 glabpkg-2.2.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_pip.svg
+-rw-rw-rw-   0        0        0      172 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg/resource/doc/badges/listing.rst
+-rw-rw-rw-   0        0        0      184 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg/resource/doc/installation.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.850933 glabpkg-2.2.0/src/glabpkg/pkg_dev/
+-rw-rw-rw-   0        0        0        0 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-03-13 17:02:21.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.866929 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/
+-rw-rw-rw-   0        0        0     1655 2023-04-17 12:58:19.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      444 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.905069 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/
+-rw-rw-rw-   0        0        0       29 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.913071 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/badges/
+-rw-rw-rw-   0        0        0     1002 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/badges/badge_doc.svg
+-rw-rw-rw-   0        0        0      110 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.921072 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0       34 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/history.rst
+-rw-rw-rw-   0        0        0      634 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/index.rst
+-rw-rw-rw-   0        0        0      209 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/installation.rst
+-rw-rw-rw-   0        0        0      133 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/management.rst
+-rw-rw-rw-   0        0        0      541 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.933093 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/user/
+-rw-rw-rw-   0        0        0       86 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/user/overview.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.937070 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/example/
+-rw-rw-rw-   0        0        0      254 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/example/readme.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.941083 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/test/
+-rw-rw-rw-   0        0        0      114 2022-12-04 11:33:38.000000 glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/test/test_packaging.py.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.945070 glabpkg-2.2.0/src/glabpkg/report/
+-rw-rw-rw-   0        0        0        0 2021-07-06 09:29:24.000000 glabpkg-2.2.0/src/glabpkg/report/__init__.py
+-rw-rw-rw-   0        0        0     1560 2021-07-06 09:29:24.000000 glabpkg-2.2.0/src/glabpkg/report/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.953070 glabpkg-2.2.0/src/glabpkg/report/resource/
+-rw-rw-rw-   0        0        0      949 2023-03-09 14:37:10.000000 glabpkg-2.2.0/src/glabpkg/report/resource/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      923 2022-03-28 12:29:45.000000 glabpkg-2.2.0/src/glabpkg/report/resource/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.979493 glabpkg-2.2.0/src/glabpkg/report/resource/report/
+-rw-rw-rw-   0        0        0       51 2021-07-06 09:29:24.000000 glabpkg-2.2.0/src/glabpkg/report/resource/report/authors.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.985558 glabpkg-2.2.0/src/glabpkg/report/resource/report/badges/
+-rw-rw-rw-   0        0        0     1001 2021-07-06 09:29:24.000000 glabpkg-2.2.0/src/glabpkg/report/resource/report/badges/badge_doc.svg
+-rw-rw-rw-   0        0        0      109 2021-07-06 09:29:24.000000 glabpkg-2.2.0/src/glabpkg/report/resource/report/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.989529 glabpkg-2.2.0/src/glabpkg/report/resource/report/biblio/
+-rw-rw-rw-   0        0        0      513 2021-07-06 09:29:24.000000 glabpkg-2.2.0/src/glabpkg/report/resource/report/biblio/biblio.rst
+-rw-rw-rw-   0        0        0      130 2021-07-06 09:29:24.000000 glabpkg-2.2.0/src/glabpkg/report/resource/report/conf.py.tpl
+-rw-rw-rw-   0        0        0      376 2021-07-06 09:29:24.000000 glabpkg-2.2.0/src/glabpkg/report/resource/report/index.rst
+-rw-rw-rw-   0        0        0       89 2021-07-06 09:29:24.000000 glabpkg-2.2.0/src/glabpkg/report/resource/report/introduction.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.993539 glabpkg-2.2.0/src/glabpkg/report/resource/script/
+-rw-rw-rw-   0        0        0       56 2021-07-06 09:29:24.000000 glabpkg-2.2.0/src/glabpkg/report/resource/script/readme.rst
+-rw-rw-rw-   0        0        0      367 2023-04-17 13:00:02.000000 glabpkg-2.2.0/src/glabpkg/version.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:12.618127 glabpkg-2.2.0/src/glabpkg.egg-info/
+-rw-rw-rw-   0        0        0     2460 2023-04-17 13:12:11.000000 glabpkg-2.2.0/src/glabpkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3457 2023-04-17 13:12:12.000000 glabpkg-2.2.0/src/glabpkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 13:12:11.000000 glabpkg-2.2.0/src/glabpkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      307 2023-04-17 13:12:11.000000 glabpkg-2.2.0/src/glabpkg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2021-06-25 14:53:47.000000 glabpkg-2.2.0/src/glabpkg.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-04-17 13:12:11.000000 glabpkg-2.2.0/src/glabpkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 13:12:11.000000 glabpkg-2.2.0/src/glabpkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 13:12:13.001524 glabpkg-2.2.0/test/
+-rw-rw-rw-   0        0        0      983 2023-04-17 13:00:02.000000 glabpkg-2.2.0/test/conftest.py
+-rw-rw-rw-   0        0        0       80 2023-04-17 13:00:02.000000 glabpkg-2.2.0/test/test_packaging.py
```

### Comparing `glabpkg-2.1.0/CONTRIBUTING.rst` & `glabpkg-2.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/LICENSE` & `glabpkg-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/PKG-INFO` & `glabpkg-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glabpkg
-Version: 2.1.0
+Version: 2.2.0
 Summary: template for python packages hosted on gitlab
 Home-page: https://gitlab.com/revesansparole/glabpkg
 Author: revesansparole
 Author-email: revesansparole@gmail.com
 License: cc_by_nc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -23,15 +23,15 @@
 glabpkg
 ========================
 
 .. {# pkglts, doc
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/glabpkg/2.1.0/
+    :target: https://pypi.org/project/glabpkg/2.2.0/
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/glabpkg
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_doc.svg
     :alt: Documentation status
```

### Comparing `glabpkg-2.1.0/README.rst` & `glabpkg-2.2.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 glabpkg
 ========================
 
 .. {# pkglts, doc
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/glabpkg/2.1.0/
+    :target: https://pypi.org/project/glabpkg/2.2.0/
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/glabpkg
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_doc.svg
     :alt: Documentation status
```

### Comparing `glabpkg-2.1.0/doc/Makefile` & `glabpkg-2.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/doc/biblio/biblio.rst` & `glabpkg-2.2.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/doc/conf.py` & `glabpkg-2.2.0/doc/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,17 +75,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "2.1.0"
+version = "2.2.0"
 # The full version, including alpha/beta/rc tags.
-release = "2.1.0"
+release = "2.2.0"
 
 
 exclude_patterns = ['build', 'dist']
 
 pygments_style = 'sphinx'
 
 # -- Options for HTML output -------------------------------------------
```

### Comparing `glabpkg-2.1.0/doc/index.rst` & `glabpkg-2.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/doc/make.bat` & `glabpkg-2.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/doc/readme.rst` & `glabpkg-2.2.0/doc/readme.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Overview
 ========
 
 .. {# pkglts, glabpkg_dev
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/glabpkg/2.1.0/
+    :target: https://pypi.org/project/glabpkg/2.2.0/
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/glabpkg
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_doc.svg
     :alt: Documentation status
```

### Comparing `glabpkg-2.1.0/setup.py` & `glabpkg-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         if pth.suffix in ['', '.bat', '.cfg', '.json', '.md', '.in', '.ini', '.png', '.ps1', '.rst', '.sh', '.svg', '.tpl', '.txt', '.yaml', '.yml']:
             data_files.append(str(pth.relative_to(src_dir)))
 
 pkg_data = {'glabpkg': data_files}
 
 setup_kwds = dict(
     name='glabpkg',
-    version="2.1.0",
+    version="2.2.0",
     description=short_descr,
     long_description=readme + '\n\n' + history,
     author="revesansparole",
     author_email="revesansparole@gmail.com",
     url='https://gitlab.com/revesansparole/glabpkg',
     license='cc_by_nc',
     zip_safe=False,
```

### Comparing `glabpkg-2.1.0/src/glabpkg/base/option.py` & `glabpkg-2.2.0/src/glabpkg/base/option.py`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/src/glabpkg/pkg/option.py` & `glabpkg-2.2.0/src/glabpkg/pkg/option.py`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_conda.svg` & `glabpkg-2.2.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_conda.svg`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_pip.svg` & `glabpkg-2.2.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_pip.svg`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/src/glabpkg/pkg_dev/option.py` & `glabpkg-2.2.0/src/glabpkg/pkg_dev/option.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         for ext in [".csv", ".ini", ".json", ".rst", ".svg"]:
             if ext not in cfg['data']['filetype']:
                 cfg['data']['filetype'].append(ext)
         cfg['data']['use_ext_dir'] = False
 
         cfg['doc']['fmt'] = "rst"
 
-        cfg['pysetup']['intended_versions'] = ["39"]
+        cfg['pysetup']['intended_versions'] = ["3.10"]
 
         cfg['sphinx']['theme'] = "sphinx_rtd_theme"
         cfg['sphinx']['gallery'] = "example"
 
         cfg['test']['suite_name'] = "pytest"
 
         cfg['gitlab']['server'] = "gitlab.com"
```

### Comparing `glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/.gitlab-ci.yml` & `glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # {# pkglts, glabpkg_dev.stages, after glabbase.stages
   - deploy
 # #}
 
 # {# pkglts, glabpkg_dev.before, after glabbase.before
   # install dependencies
   {% if reqs.conda_reqs(['install', 'test', 'dvlpt']) != "" -%}
-  - {{ reqs.conda_reqs(['install', 'test', 'dvlpt']) | replace("-c sunagri", "-c $CDCHAN") }}
+  - {{ reqs.conda_reqs(['install', 'test', 'dvlpt']) }}
   {%- endif %}
   {% if reqs.pip_reqs(['install', 'test', 'dvlpt']) != "" -%}
   - {{ reqs.pip_reqs(['install', 'test', 'dvlpt']) }}
   {%- endif %}
   # install package
   - pip install .
 # #}
@@ -17,47 +17,47 @@
 # {# pkglts, glabpkg_dev.test, replace glabbase.test
 ci:test:
   stage: test
   except:
     - tags
     - main
   script:
-    - pytest --cov={{ base.pkg_full_name }}
+    - pytest
   coverage: '/^TOTAL\s+\d+\s+\d+\s+(\d+\%)\s*$/'
 # #}
 
 # {# pkglts, glabpkg_dev.test_all
 ci:test_all:
   stage: test
   only:
     - main
   except:
     - tags
   script:
-    - pytest --cov={{ base.pkg_full_name }} --runslow
+    - pytest --runslow
   coverage: '/^TOTAL\s+\d+\s+\d+\s+(\d+\%)\s*$/'
 # #}
 
 # {# pkglts, glabpkg_dev.pages
 pages:
   stage: deploy
   only:
     - main
   script:
     # install dependencies
     {% if reqs.conda_reqs(['doc']) != "" -%}
-    - {{ reqs.conda_reqs(['doc']) | replace("-c sunagri", "-c $CDCHAN") }}
+    - {{ reqs.conda_reqs(['doc']) }}
     {%- endif %}
     {% if reqs.pip_reqs(['doc']) != "" -%}
     - {{ reqs.pip_reqs(['doc']) }}
     {%- endif %}
     {%if sphinx.gallery != "" -%}
     # install specific packages for sphinx gallery
     {% if reqs.conda_reqs([sphinx.gallery]) != "" -%}
-    - {{ reqs.conda_reqs([sphinx.gallery]) | replace("-c sunagri", "-c $CDCHAN") }}
+    - {{ reqs.conda_reqs([sphinx.gallery]) }}
     {%- endif %}
     {% if reqs.pip_reqs([sphinx.gallery]) != "" -%}
     - {{ reqs.pip_reqs([sphinx.gallery]) }}
     {%- endif %}
     {%- endif %}
     - cd doc && { make html; cd ..; }
     - mv doc/build/html public
```

### Comparing `glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/badges/badge_doc.svg` & `glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/badges/badge_doc.svg`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/biblio/biblio.rst` & `glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/index.rst` & `glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/index.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/src/glabpkg/pkg_dev/resource/doc/readme.rst` & `glabpkg-2.2.0/src/glabpkg/pkg_dev/resource/doc/readme.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/src/glabpkg/report/option.py` & `glabpkg-2.2.0/src/glabpkg/report/option.py`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/src/glabpkg/report/resource/.gitlab-ci.yml` & `glabpkg-2.2.0/src/glabpkg/report/resource/.gitlab-ci.yml`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 pages:
   stage: deploy
   only:
     - main
   script:
     # install dependencies
     {% if reqs.conda_reqs(['doc', 'report']) != "" -%}
-    - {{ reqs.conda_reqs(['doc', 'report']) | replace("-c sunagri", "-c $CDCHAN") }}
+    - {{ reqs.conda_reqs(['doc', 'report']) }}
     {%- endif %}
     {% if reqs.pip_reqs(['doc', 'report']) != "" -%}
     - {{ reqs.pip_reqs(['doc', 'report']) }}
     {%- endif %}
     {%if sphinx.gallery != "" -%}
     # specific installs for sphinx gallery
     {% if reqs.conda_reqs([sphinx.gallery]) != "" -%}
-    - {{ reqs.conda_reqs([sphinx.gallery]) | replace("-c sunagri", "-c $CDCHAN") }}
+    - {{ reqs.conda_reqs([sphinx.gallery]) }}
     {%- endif %}
     {% if reqs.pip_reqs([sphinx.gallery]) != "" -%}
     - {{ reqs.pip_reqs([sphinx.gallery]) }}
     {%- endif %}
     {%- endif %}
     - apt-get update
     - apt-get install -y make
```

### Comparing `glabpkg-2.1.0/src/glabpkg/report/resource/README.rst` & `glabpkg-2.2.0/src/glabpkg/report/resource/README.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/src/glabpkg/report/resource/report/badges/badge_doc.svg` & `glabpkg-2.2.0/src/glabpkg/report/resource/report/badges/badge_doc.svg`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/src/glabpkg/report/resource/report/biblio/biblio.rst` & `glabpkg-2.2.0/src/glabpkg/report/resource/report/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/src/glabpkg.egg-info/PKG-INFO` & `glabpkg-2.2.0/src/glabpkg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glabpkg
-Version: 2.1.0
+Version: 2.2.0
 Summary: template for python packages hosted on gitlab
 Home-page: https://gitlab.com/revesansparole/glabpkg
 Author: revesansparole
 Author-email: revesansparole@gmail.com
 License: cc_by_nc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -23,15 +23,15 @@
 glabpkg
 ========================
 
 .. {# pkglts, doc
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/glabpkg/2.1.0/
+    :target: https://pypi.org/project/glabpkg/2.2.0/
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/glabpkg
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_doc.svg
     :alt: Documentation status
```

### Comparing `glabpkg-2.1.0/src/glabpkg.egg-info/SOURCES.txt` & `glabpkg-2.2.0/src/glabpkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glabpkg-2.1.0/test/conftest.py` & `glabpkg-2.2.0/test/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=glabpkg")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=glabpkg")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

