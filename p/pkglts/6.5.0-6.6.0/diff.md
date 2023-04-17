# Comparing `tmp/pkglts-6.5.0.tar.gz` & `tmp/pkglts-6.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkglts-6.5.0.tar", last modified: Mon Mar 13 19:10:09 2023, max compression
+gzip compressed data, was "pkglts-6.6.0.tar", last modified: Mon Apr 17 13:16:04 2023, max compression
```

## Comparing `pkglts-6.5.0.tar` & `pkglts-6.6.0.tar`

### file list

```diff
@@ -1,517 +1,517 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:09.507639 pkglts-6.5.0/
--rw-rw-rw-   0        0        0      460 2023-03-13 18:15:33.000000 pkglts-6.5.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3937 2023-03-13 18:15:33.000000 pkglts-6.5.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      167 2023-03-13 18:15:33.000000 pkglts-6.5.0/HISTORY.rst
--rw-rw-rw-   0        0        0    22406 2023-03-13 18:15:33.000000 pkglts-6.5.0/LICENSE
--rw-rw-rw-   0        0        0      434 2023-03-13 18:15:33.000000 pkglts-6.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4782 2023-03-13 19:10:09.507639 pkglts-6.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3741 2023-03-13 18:15:33.000000 pkglts-6.5.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.027378 pkglts-6.5.0/doc/
--rw-rw-rw-   0        0        0     6967 2023-03-13 18:15:33.000000 pkglts-6.5.0/doc/Makefile
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.059383 pkglts-6.5.0/doc/_notebook/
--rw-rw-rw-   0        0        0      754 2018-08-05 08:23:37.000000 pkglts-6.5.0/doc/_notebook/example.rst
--rw-rw-rw-   0        0        0       97 2018-08-05 07:42:43.000000 pkglts-6.5.0/doc/_notebook/index.rst
--rw-rw-rw-   0        0        0       29 2017-08-08 14:05:32.000000 pkglts-6.5.0/doc/authors.rst
--rw-rw-rw-   0        0        0     4272 2023-03-13 18:21:24.000000 pkglts-6.5.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2017-08-08 14:05:32.000000 pkglts-6.5.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2017-08-08 14:05:32.000000 pkglts-6.5.0/doc/history.rst
--rw-rw-rw-   0        0        0      420 2018-02-15 07:33:01.000000 pkglts-6.5.0/doc/index.rst
--rw-rw-rw-   0        0        0      726 2018-02-15 09:25:07.000000 pkglts-6.5.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2023-03-13 18:15:33.000000 pkglts-6.5.0/doc/make.bat
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.308618 pkglts-6.5.0/doc/option/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.075378 pkglts-6.5.0/doc/option/base/
--rw-rw-rw-   0        0        0     1778 2018-02-27 09:14:53.000000 pkglts-6.5.0/doc/option/base/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.091377 pkglts-6.5.0/doc/option/conda/
--rw-rw-rw-   0        0        0      621 2018-08-01 07:30:08.000000 pkglts-6.5.0/doc/option/conda/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.103378 pkglts-6.5.0/doc/option/coverage/
--rw-rw-rw-   0        0        0     2177 2018-02-27 09:14:53.000000 pkglts-6.5.0/doc/option/coverage/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.139383 pkglts-6.5.0/doc/option/coveralls/
--rw-rw-rw-   0        0        0     1766 2017-01-03 08:51:05.000000 pkglts-6.5.0/doc/option/coveralls/coveralls_tutorial.rst
--rw-rw-rw-   0        0        0      972 2018-02-27 09:14:53.000000 pkglts-6.5.0/doc/option/coveralls/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.175381 pkglts-6.5.0/doc/option/data/
--rw-rw-rw-   0        0        0     1150 2018-02-27 09:14:53.000000 pkglts-6.5.0/doc/option/data/data_tutorial.rst
--rw-rw-rw-   0        0        0      329 2017-01-03 08:51:05.000000 pkglts-6.5.0/doc/option/data/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.211379 pkglts-6.5.0/doc/option/doc/
--rw-rw-rw-   0        0        0      533 2018-02-27 09:14:53.000000 pkglts-6.5.0/doc/option/doc/history.rst
--rw-rw-rw-   0        0        0     2053 2018-02-27 09:14:53.000000 pkglts-6.5.0/doc/option/doc/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.231374 pkglts-6.5.0/doc/option/flake8/
--rw-rw-rw-   0        0        0      474 2018-02-27 09:14:53.000000 pkglts-6.5.0/doc/option/flake8/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.243401 pkglts-6.5.0/doc/option/git/
--rw-rw-rw-   0        0        0      400 2018-02-15 07:33:01.000000 pkglts-6.5.0/doc/option/git/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.279376 pkglts-6.5.0/doc/option/github/
--rw-rw-rw-   0        0        0     2785 2017-01-03 08:51:05.000000 pkglts-6.5.0/doc/option/github/github_tutorial.rst
--rw-rw-rw-   0        0        0      451 2018-02-15 07:33:01.000000 pkglts-6.5.0/doc/option/github/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.311378 pkglts-6.5.0/doc/option/gitlab/
--rw-rw-rw-   0        0        0     2627 2018-02-15 07:33:01.000000 pkglts-6.5.0/doc/option/gitlab/gitlab_tutorial.rst
--rw-rw-rw-   0        0        0      402 2018-02-15 07:33:01.000000 pkglts-6.5.0/doc/option/gitlab/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.347385 pkglts-6.5.0/doc/option/landscape/
--rw-rw-rw-   0        0        0     1207 2017-01-03 08:51:05.000000 pkglts-6.5.0/doc/option/landscape/landscape_tutorial.rst
--rw-rw-rw-   0        0        0     1006 2018-02-27 09:14:53.000000 pkglts-6.5.0/doc/option/landscape/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.363384 pkglts-6.5.0/doc/option/lgtm/
--rw-rw-rw-   0        0        0      557 2019-10-30 07:39:24.000000 pkglts-6.5.0/doc/option/lgtm/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.391376 pkglts-6.5.0/doc/option/license/
--rw-rw-rw-   0        0        0     7038 2019-10-29 19:00:47.000000 pkglts-6.5.0/doc/option/license/license_list.rst
--rw-rw-rw-   0        0        0      932 2018-02-27 09:14:53.000000 pkglts-6.5.0/doc/option/license/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.423391 pkglts-6.5.0/doc/option/notebook/
--rw-rw-rw-   0        0        0      906 2018-04-06 16:07:32.000000 pkglts-6.5.0/doc/option/notebook/main.rst
--rw-rw-rw-   0        0        0      854 2018-04-06 16:07:32.000000 pkglts-6.5.0/doc/option/notebook/nbcompile.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.459377 pkglts-6.5.0/doc/option/plugin/
--rw-rw-rw-   0        0        0      642 2017-01-03 08:51:05.000000 pkglts-6.5.0/doc/option/plugin/main.rst
--rw-rw-rw-   0        0        0      148 2017-01-03 08:51:05.000000 pkglts-6.5.0/doc/option/plugin/plugin_tutorial.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.479379 pkglts-6.5.0/doc/option/plugin_project/
--rw-rw-rw-   0        0        0     1080 2017-07-15 20:09:55.000000 pkglts-6.5.0/doc/option/plugin_project/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.523419 pkglts-6.5.0/doc/option/pypi/
--rw-rw-rw-   0        0        0      343 2018-02-27 09:14:53.000000 pkglts-6.5.0/doc/option/pypi/main.rst
--rw-rw-rw-   0        0        0     3660 2017-01-03 08:51:05.000000 pkglts-6.5.0/doc/option/pypi/pypi_tutorial.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.551379 pkglts-6.5.0/doc/option/pysetup/
--rw-rw-rw-   0        0        0     1122 2018-08-05 08:23:37.000000 pkglts-6.5.0/doc/option/pysetup/main.rst
--rw-rw-rw-   0        0        0      355 2018-08-05 08:23:37.000000 pkglts-6.5.0/doc/option/pysetup/reqs.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.595382 pkglts-6.5.0/doc/option/readthedocs/
--rw-rw-rw-   0        0        0      723 2018-02-27 09:14:53.000000 pkglts-6.5.0/doc/option/readthedocs/main.rst
--rw-rw-rw-   0        0        0     2666 2017-01-03 08:51:05.000000 pkglts-6.5.0/doc/option/readthedocs/readthedocs_tutorial.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.639375 pkglts-6.5.0/doc/option/requires/
--rw-rw-rw-   0        0        0      743 2018-02-27 09:14:53.000000 pkglts-6.5.0/doc/option/requires/main.rst
--rw-rw-rw-   0        0        0     1117 2018-02-15 07:33:01.000000 pkglts-6.5.0/doc/option/requires/requires_tutorial.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.651376 pkglts-6.5.0/doc/option/sphinx/
--rw-rw-rw-   0        0        0     1460 2018-04-06 16:07:32.000000 pkglts-6.5.0/doc/option/sphinx/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.671399 pkglts-6.5.0/doc/option/test/
--rw-rw-rw-   0        0        0     1179 2018-02-27 09:14:53.000000 pkglts-6.5.0/doc/option/test/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.687390 pkglts-6.5.0/doc/option/tox/
--rw-rw-rw-   0        0        0      698 2018-02-27 09:14:53.000000 pkglts-6.5.0/doc/option/tox/main.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.715399 pkglts-6.5.0/doc/option/travis/
--rw-rw-rw-   0        0        0      519 2021-05-27 13:53:46.000000 pkglts-6.5.0/doc/option/travis/main.rst
--rw-rw-rw-   0        0        0     2089 2021-05-27 13:53:46.000000 pkglts-6.5.0/doc/option/travis/travis_tutorial.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.751375 pkglts-6.5.0/doc/option/version/
--rw-rw-rw-   0        0        0      421 2018-08-05 08:23:37.000000 pkglts-6.5.0/doc/option/version/bump.rst
--rw-rw-rw-   0        0        0      556 2018-02-27 09:14:53.000000 pkglts-6.5.0/doc/option/version/main.rst
--rw-rw-rw-   0        0        0     2192 2018-02-15 07:33:01.000000 pkglts-6.5.0/doc/option_list.rst
--rw-rw-rw-   0        0        0     5879 2019-03-14 16:09:18.000000 pkglts-6.5.0/doc/readme.rst
--rw-rw-rw-   0        0        0      318 2018-08-05 08:23:37.000000 pkglts-6.5.0/doc/tool_list.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:02.811379 pkglts-6.5.0/doc/tutorial/
--rw-rw-rw-   0        0        0      668 2017-01-03 08:51:05.000000 pkglts-6.5.0/doc/tutorial/dvlpt_env.rst
--rw-rw-rw-   0        0        0      468 2017-01-03 08:51:05.000000 pkglts-6.5.0/doc/tutorial/migration.rst
--rw-rw-rw-   0        0        0     1145 2018-10-31 18:23:46.000000 pkglts-6.5.0/doc/tutorial/pypi.rst
--rw-rw-rw-   0        0        0      635 2017-01-03 08:51:05.000000 pkglts-6.5.0/doc/tutorial/web_tools.rst
--rw-rw-rw-   0        0        0      773 2018-02-15 07:33:01.000000 pkglts-6.5.0/doc/tutorials.rst
--rw-rw-rw-   0        0        0     1117 2017-08-08 14:05:32.000000 pkglts-6.5.0/doc/usage.rst
--rw-rw-rw-   0        0        0      323 2023-03-13 18:15:33.000000 pkglts-6.5.0/requirements.txt
--rw-rw-rw-   0        0        0       66 2023-03-13 18:15:33.000000 pkglts-6.5.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      223 2023-03-13 19:10:09.529788 pkglts-6.5.0/setup.cfg
--rw-rw-rw-   0        0        0     3937 2023-03-13 18:21:24.000000 pkglts-6.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.320472 pkglts-6.5.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.128756 pkglts-6.5.0/src/pkglts/
--rw-rw-rw-   0        0        0      183 2023-03-13 18:15:33.000000 pkglts-6.5.0/src/pkglts/__init__.py
--rw-rw-rw-   0        0        0      202 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/config.py
--rw-rw-rw-   0        0        0    12875 2023-03-13 18:21:24.000000 pkglts-6.5.0/src/pkglts/config_management.py
--rw-rw-rw-   0        0        0     5526 2019-10-29 06:16:57.000000 pkglts-6.5.0/src/pkglts/dependency.py
--rw-rw-rw-   0        0        0      407 2019-08-27 13:00:03.000000 pkglts-6.5.0/src/pkglts/file_management.py
--rw-rw-rw-   0        0        0     2754 2019-11-13 12:35:41.000000 pkglts-6.5.0/src/pkglts/hash_management.py
--rw-rw-rw-   0        0        0     1427 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/local.py
--rw-rw-rw-   0        0        0     1634 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/logging_tools.py
--rw-rw-rw-   0        0        0     9009 2021-03-03 16:14:09.000000 pkglts-6.5.0/src/pkglts/manage.py
--rw-rw-rw-   0        0        0     7395 2020-10-22 13:45:14.000000 pkglts-6.5.0/src/pkglts/manage_script.py
--rw-rw-rw-   0        0        0     4113 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/manage_tools.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.244749 pkglts-6.5.0/src/pkglts/option/
--rw-rw-rw-   0        0        0       45 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.276768 pkglts-6.5.0/src/pkglts/option/appveyor/
--rw-rw-rw-   0        0        0       23 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/appveyor/__init__.py
--rw-rw-rw-   0        0        0      978 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/appveyor/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.288748 pkglts-6.5.0/src/pkglts/option/appveyor/resource/
--rw-rw-rw-   0        0        0     1123 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/appveyor/resource/appveyor.yml
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.320765 pkglts-6.5.0/src/pkglts/option/base/
--rw-rw-rw-   0        0        0       19 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/base/__init__.py
--rw-rw-rw-   0        0        0     1197 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/base/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.348754 pkglts-6.5.0/src/pkglts/option/conda/
--rw-rw-rw-   0        0        0       20 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/conda/__init__.py
--rw-rw-rw-   0        0        0     1008 2023-01-19 13:13:37.000000 pkglts-6.5.0/src/pkglts/option/conda/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.336449 pkglts-6.5.0/src/pkglts/option/conda/resource/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.396758 pkglts-6.5.0/src/pkglts/option/conda/resource/conda/
--rw-rw-rw-   0        0        0     1083 2021-12-15 17:52:05.000000 pkglts-6.5.0/src/pkglts/option/conda/resource/conda/meta.yaml
--rw-rw-rw-   0        0        0      848 2023-03-13 18:21:24.000000 pkglts-6.5.0/src/pkglts/option/conda/resource/conda/requirements.yml
--rw-rw-rw-   0        0        0      682 2023-03-13 18:21:24.000000 pkglts-6.5.0/src/pkglts/option/conda/resource/conda/requirements_minimal.yml
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.424749 pkglts-6.5.0/src/pkglts/option/coverage/
--rw-rw-rw-   0        0        0       23 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/coverage/__init__.py
--rw-rw-rw-   0        0        0      560 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/coverage/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.444795 pkglts-6.5.0/src/pkglts/option/coverage/resource/
--rw-rw-rw-   0        0        0      367 2018-06-06 09:43:05.000000 pkglts-6.5.0/src/pkglts/option/coverage/resource/.coveragerc
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.484754 pkglts-6.5.0/src/pkglts/option/coveralls/
--rw-rw-rw-   0        0        0       24 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/coveralls/__init__.py
--rw-rw-rw-   0        0        0      929 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/coveralls/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.522894 pkglts-6.5.0/src/pkglts/option/data/
--rw-rw-rw-   0        0        0       19 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.361486 pkglts-6.5.0/src/pkglts/option/data/example/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.353503 pkglts-6.5.0/src/pkglts/option/data/example/src/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.554891 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/
--rw-rw-rw-   0        0        0   342163 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.png
--rw-rw-rw-   0        0        0       13 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.txt
--rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.ui
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.580478 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/
--rw-rw-rw-   0        0        0   342163 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.png
--rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.txt
--rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.ui
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.620485 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/
--rw-rw-rw-   0        0        0   342163 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.png
--rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.txt
--rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.ui
--rw-rw-rw-   0        0        0      365 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/list_data.py.tpl
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.648474 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/
--rw-rw-rw-   0        0        0        0 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/__init__.py.tpl
--rw-rw-rw-   0        0        0   342163 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.png
--rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.txt
--rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.ui
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.679088 pkglts-6.5.0/src/pkglts/option/data/example/test/
--rw-rw-rw-   0        0        0      538 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/test/{% if data.use_ext_dir %}test_data{% else %}_{% endif %}.py.tpl
--rw-rw-rw-   0        0        0      296 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/example/test/{% if not data.use_ext_dir %}test_data{% else %}_{% endif %}.py.tpl
--rw-rw-rw-   0        0        0      495 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/data/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.365486 pkglts-6.5.0/src/pkglts/option/data/resource/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.369536 pkglts-6.5.0/src/pkglts/option/data/resource/src/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.683045 pkglts-6.5.0/src/pkglts/option/data/resource/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/
--rw-rw-rw-   0        0        0        0 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/data/resource/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/__init__.py.tpl
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.796579 pkglts-6.5.0/src/pkglts/option/data/resource/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0     1500 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/data/resource/src/{{ base.pkgname }}/{% if data.use_ext_dir %}data_access{% else %}_{% endif %}.py.tpl
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.983024 pkglts-6.5.0/src/pkglts/option/doc/
--rw-rw-rw-   0        0        0      796 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/doc/__init__.py
--rw-rw-rw-   0        0        0     5564 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/doc/history.py
--rw-rw-rw-   0        0        0     1664 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/doc/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:04.435246 pkglts-6.5.0/src/pkglts/option/doc/resource/
--rw-rw-rw-   0        0        0      411 2020-04-15 06:18:47.000000 pkglts-6.5.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}AUTHORS{% else %}_{% endif %}.md
--rw-rw-rw-   0        0        0     4505 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}CONTRIBUTING{% else %}_{% endif %}.md
--rw-rw-rw-   0        0        0       70 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}HISTORY{% else %}_{% endif %}.md
--rw-rw-rw-   0        0        0      158 2020-04-15 06:18:47.000000 pkglts-6.5.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}README{% else %}_{% endif %}.md
--rw-rw-rw-   0        0        0      377 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}mkdocs{% else %}_{% endif %}.yml
--rw-rw-rw-   0        0        0      424 2020-04-15 06:04:23.000000 pkglts-6.5.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}AUTHORS{% else %}_{% endif %}.rst
--rw-rw-rw-   0        0        0     4706 2023-03-13 18:21:24.000000 pkglts-6.5.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}CONTRIBUTING{% else %}_{% endif %}.rst
--rw-rw-rw-   0        0        0      109 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}HISTORY{% else %}_{% endif %}.rst
--rw-rw-rw-   0        0        0      192 2020-04-15 06:18:47.000000 pkglts-6.5.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}README{% else %}_{% endif %}.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:04.511522 pkglts-6.5.0/src/pkglts/option/flake8/
--rw-rw-rw-   0        0        0       21 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/flake8/__init__.py
--rw-rw-rw-   0        0        0      464 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/flake8/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:04.547702 pkglts-6.5.0/src/pkglts/option/flake8/resource/
--rw-rw-rw-   0        0        0      173 2019-10-29 06:16:57.000000 pkglts-6.5.0/src/pkglts/option/flake8/resource/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:04.623022 pkglts-6.5.0/src/pkglts/option/git/
--rw-rw-rw-   0        0        0       18 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/git/__init__.py
--rw-rw-rw-   0        0        0     1388 2022-03-25 13:56:41.000000 pkglts-6.5.0/src/pkglts/option/git/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:04.654291 pkglts-6.5.0/src/pkglts/option/git/resource/
--rw-rw-rw-   0        0        0     1580 2021-03-03 16:14:09.000000 pkglts-6.5.0/src/pkglts/option/git/resource/.gitignore
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:04.708421 pkglts-6.5.0/src/pkglts/option/github/
--rw-rw-rw-   0        0        0       21 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/github/__init__.py
--rw-rw-rw-   0        0        0      792 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/github/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:04.780466 pkglts-6.5.0/src/pkglts/option/gitlab/
--rw-rw-rw-   0        0        0       21 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/gitlab/__init__.py
--rw-rw-rw-   0        0        0      837 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/gitlab/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:04.850541 pkglts-6.5.0/src/pkglts/option/landscape/
--rw-rw-rw-   0        0        0       24 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/landscape/__init__.py
--rw-rw-rw-   0        0        0      735 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/landscape/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:04.888702 pkglts-6.5.0/src/pkglts/option/landscape/resource/
--rw-rw-rw-   0        0        0      323 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/landscape/resource/.landscape.yml
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:05.089278 pkglts-6.5.0/src/pkglts/option/lgtm/
--rw-rw-rw-   0        0        0       19 2019-10-30 07:39:24.000000 pkglts-6.5.0/src/pkglts/option/lgtm/__init__.py
--rw-rw-rw-   0        0        0      808 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/lgtm/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:05.202607 pkglts-6.5.0/src/pkglts/option/license/
--rw-rw-rw-   0        0        0       22 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/license/__init__.py
--rw-rw-rw-   0        0        0     1822 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/license/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:05.240783 pkglts-6.5.0/src/pkglts/option/license/resource/
--rw-rw-rw-   0        0        0       49 2020-03-17 18:25:54.000000 pkglts-6.5.0/src/pkglts/option/license/resource/LICENSE.tpl
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:05.998659 pkglts-6.5.0/src/pkglts/option/license/templates/
--rw-rw-rw-   0        0        0      741 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/agpl3-header.txt
--rw-rw-rw-   0        0        0    35211 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/agpl3.txt
--rw-rw-rw-   0        0        0      596 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/apache-header.txt
--rw-rw-rw-   0        0        0    11131 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/apache.txt
--rw-rw-rw-   0        0        0     1373 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/bsd2.txt
--rw-rw-rw-   0        0        0     1585 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/bsd3.txt
--rw-rw-rw-   0        0        0      389 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cc0-header.txt
--rw-rw-rw-   0        0        0     7169 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cc0.txt
--rw-rw-rw-   0        0        0      316 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cc_by-header.txt
--rw-rw-rw-   0        0        0    19785 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cc_by.txt
--rw-rw-rw-   0        0        0      333 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cc_by_nc-header.txt
--rw-rw-rw-   0        0        0    20812 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cc_by_nc.txt
--rw-rw-rw-   0        0        0      345 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cc_by_nc_nd-header.txt
--rw-rw-rw-   0        0        0    18957 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cc_by_nc_nd.txt
--rw-rw-rw-   0        0        0      347 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cc_by_nc_sa-header.txt
--rw-rw-rw-   0        0        0    22669 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cc_by_nc_sa.txt
--rw-rw-rw-   0        0        0      328 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cc_by_nd-header.txt
--rw-rw-rw-   0        0        0    17942 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cc_by_nd.txt
--rw-rw-rw-   0        0        0      330 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cc_by_sa-header.txt
--rw-rw-rw-   0        0        0    22597 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cc_by_sa.txt
--rw-rw-rw-   0        0        0    17650 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cddl.txt
--rw-rw-rw-   0        0        0     1527 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cecill-c-header.txt
--rw-rw-rw-   0        0        0    22380 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/cecill-c.txt
--rw-rw-rw-   0        0        0    11840 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/epl.txt
--rw-rw-rw-   0        0        0    18173 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/gpl2.txt
--rw-rw-rw-   0        0        0      720 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/gpl3-header.txt
--rw-rw-rw-   0        0        0    35864 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/gpl3.txt
--rw-rw-rw-   0        0        0     6426 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/inra_license_agreement.txt
--rw-rw-rw-   0        0        0      778 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/isc.txt
--rw-rw-rw-   0        0        0     7777 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/lgpl.txt
--rw-rw-rw-   0        0        0     1103 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/mit.txt
--rw-rw-rw-   0        0        0      196 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/mpl-header.txt
--rw-rw-rw-   0        0        0    16078 2017-05-18 09:15:38.000000 pkglts-6.5.0/src/pkglts/option/license/templates/mpl.txt
--rw-rw-rw-   0        0        0     9475 2020-04-14 06:55:23.000000 pkglts-6.5.0/src/pkglts/option/license/templates/private.txt
--rw-rw-rw-   0        0        0     1235 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/unlicense.txt
--rw-rw-rw-   0        0        0      301 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/wtfpl-header-warranty.txt
--rw-rw-rw-   0        0        0      301 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/wtfpl-header.txt
--rw-rw-rw-   0        0        0      515 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/wtfpl.txt
--rw-rw-rw-   0        0        0     1444 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/x11.txt
--rw-rw-rw-   0        0        0      919 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/license/templates/zlib.txt
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.048215 pkglts-6.5.0/src/pkglts/option/notebook/
--rw-rw-rw-   0        0        0       23 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/notebook/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.413489 pkglts-6.5.0/src/pkglts/option/notebook/example/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.072218 pkglts-6.5.0/src/pkglts/option/notebook/example/{{ notebook.src_directory }}/
--rw-rw-rw-   0        0        0    17056 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/notebook/example/{{ notebook.src_directory }}/example.ipynb
--rw-rw-rw-   0        0        0     4449 2019-10-29 06:16:57.000000 pkglts-6.5.0/src/pkglts/option/notebook/nbcompile.py
--rw-rw-rw-   0        0        0      822 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/notebook/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.104220 pkglts-6.5.0/src/pkglts/option/plugin_project/
--rw-rw-rw-   0        0        0       49 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/plugin_project/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.425494 pkglts-6.5.0/src/pkglts/option/plugin_project/example/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.425494 pkglts-6.5.0/src/pkglts/option/plugin_project/example/src/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.425494 pkglts-6.5.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.130777 pkglts-6.5.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/resource/
--rw-rw-rw-   0        0        0       83 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/resource/extra_file.txt
--rw-rw-rw-   0        0        0       92 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/resource/extra_script.py.tpl
--rw-rw-rw-   0        0        0      978 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/plugin_project/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.162780 pkglts-6.5.0/src/pkglts/option/plugin_project/resource/
--rw-rw-rw-   0        0        0      225 2019-10-29 06:16:57.000000 pkglts-6.5.0/src/pkglts/option/plugin_project/resource/setup.py.tpl
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.437538 pkglts-6.5.0/src/pkglts/option/plugin_project/resource/src/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.186777 pkglts-6.5.0/src/pkglts/option/plugin_project/resource/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0     1016 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/plugin_project/resource/src/{{ base.pkgname }}/option.py.tpl
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.220397 pkglts-6.5.0/src/pkglts/option/pypi/
--rw-rw-rw-   0        0        0       19 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/pypi/__init__.py
--rw-rw-rw-   0        0        0     2697 2023-03-13 18:21:24.000000 pkglts-6.5.0/src/pkglts/option/pypi/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.240371 pkglts-6.5.0/src/pkglts/option/pypi/resource/
--rw-rw-rw-   0        0        0      290 2020-04-15 06:02:11.000000 pkglts-6.5.0/src/pkglts/option/pypi/resource/.pypirc
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.264369 pkglts-6.5.0/src/pkglts/option/pysetup/
--rw-rw-rw-   0        0        0       22 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/pysetup/__init__.py
--rw-rw-rw-   0        0        0     2115 2023-03-13 18:21:24.000000 pkglts-6.5.0/src/pkglts/option/pysetup/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.354908 pkglts-6.5.0/src/pkglts/option/pysetup/resource/
--rw-rw-rw-   0        0        0      739 2019-10-29 06:16:57.000000 pkglts-6.5.0/src/pkglts/option/pysetup/resource/MANIFEST.in
--rw-rw-rw-   0        0        0      122 2020-02-06 18:07:27.000000 pkglts-6.5.0/src/pkglts/option/pysetup/resource/setup.cfg
--rw-rw-rw-   0        0        0     2954 2021-04-29 10:55:32.000000 pkglts-6.5.0/src/pkglts/option/pysetup/resource/setup.py.tpl
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.408937 pkglts-6.5.0/src/pkglts/option/readthedocs/
--rw-rw-rw-   0        0        0       26 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/readthedocs/__init__.py
--rw-rw-rw-   0        0        0     1615 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/readthedocs/option.py
--rw-rw-rw-   0        0        0        0 2017-01-03 08:51:05.000000 pkglts-6.5.0/src/pkglts/option/regenerate.no
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.521140 pkglts-6.5.0/src/pkglts/option/reqs/
--rw-rw-rw-   0        0        0       56 2019-10-29 06:16:57.000000 pkglts-6.5.0/src/pkglts/option/reqs/__init__.py
--rw-rw-rw-   0        0        0     2351 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/reqs/find_requirements.py
--rw-rw-rw-   0        0        0     3808 2021-12-09 14:39:11.000000 pkglts-6.5.0/src/pkglts/option/reqs/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.564933 pkglts-6.5.0/src/pkglts/option/reqs/resource/
--rw-rw-rw-   0        0        0      319 2020-04-15 06:18:47.000000 pkglts-6.5.0/src/pkglts/option/reqs/resource/requirements.txt
--rw-rw-rw-   0        0        0      136 2020-04-15 06:18:47.000000 pkglts-6.5.0/src/pkglts/option/reqs/resource/requirements_minimal.txt
--rw-rw-rw-   0        0        0     2100 2019-10-29 06:16:57.000000 pkglts-6.5.0/src/pkglts/option/reqs/stdpkgs.txt
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.611164 pkglts-6.5.0/src/pkglts/option/requires/
--rw-rw-rw-   0        0        0       23 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/requires/__init__.py
--rw-rw-rw-   0        0        0      796 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/requires/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.649406 pkglts-6.5.0/src/pkglts/option/sphinx/
--rw-rw-rw-   0        0        0       21 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/sphinx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.474557 pkglts-6.5.0/src/pkglts/option/sphinx/example/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.671588 pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.882460 pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/
--rw-rw-rw-   0        0        0      312 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/autodoc.rst
--rw-rw-rw-   0        0        0      358 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/autosummary.rst
--rw-rw-rw-   0        0        0      385 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/graphviz.rst
--rw-rw-rw-   0        0        0      468 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/ifconfig.rst
--rw-rw-rw-   0        0        0      221 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/index.rst
--rw-rw-rw-   0        0        0      823 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/inheritance.rst
--rw-rw-rw-   0        0        0      631 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/intersphinx.rst
--rw-rw-rw-   0        0        0      364 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/math.rst
--rw-rw-rw-   0        0        0      665 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/matplotlib.rst
--rw-rw-rw-   0        0        0      441 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/todo.rst
--rw-rw-rw-   0        0        0      344 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/viewcode.rst
--rw-rw-rw-   0        0        0      443 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/workflow.dot
--rw-rw-rw-   0        0        0      493 2019-10-29 06:16:57.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/index.rst
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.470535 pkglts-6.5.0/src/pkglts/option/sphinx/example/src/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.933991 pkglts-6.5.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0      742 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_doc.py.tpl
--rw-rw-rw-   0        0        0      110 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_inheritance1.py.tpl
--rw-rw-rw-   0        0        0       81 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_inheritance2.py.tpl
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.965989 pkglts-6.5.0/src/pkglts/option/sphinx/example/{{ sphinx.gallery  }}/
--rw-rw-rw-   0        0        0      109 2019-10-29 06:16:57.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/{{ sphinx.gallery  }}/README.rst
--rw-rw-rw-   0        0        0      297 2019-10-29 06:16:57.000000 pkglts-6.5.0/src/pkglts/option/sphinx/example/{{ sphinx.gallery  }}/plot_smth.py
--rw-rw-rw-   0        0        0     1447 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/sphinx/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:06.977988 pkglts-6.5.0/src/pkglts/option/sphinx/resource/
--rw-rw-rw-   0        0        0       77 2021-03-01 14:25:42.000000 pkglts-6.5.0/src/pkglts/option/sphinx/resource/{% if 'pysetup' is available %}setup{% else %}_{% endif %}.cfg
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.046046 pkglts-6.5.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/
--rw-rw-rw-   0        0        0     6967 2021-03-01 14:25:42.000000 pkglts-6.5.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/Makefile
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.046046 pkglts-6.5.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/_static/
--rw-rw-rw-   0        0        0        0 2021-03-01 14:25:42.000000 pkglts-6.5.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/_static/nonempty.txt
--rw-rw-rw-   0        0        0     5819 2021-03-01 14:25:42.000000 pkglts-6.5.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/conf.py.tpl
--rwxrwxrwx   0        0        0     6731 2021-03-01 14:25:42.000000 pkglts-6.5.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/make.bat
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.081234 pkglts-6.5.0/src/pkglts/option/src/
--rw-rw-rw-   0        0        0       58 2019-10-29 06:16:57.000000 pkglts-6.5.0/src/pkglts/option/src/__init__.py
--rw-rw-rw-   0        0        0      848 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/src/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.482534 pkglts-6.5.0/src/pkglts/option/src/resource/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.482534 pkglts-6.5.0/src/pkglts/option/src/resource/src/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.097248 pkglts-6.5.0/src/pkglts/option/src/resource/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0      109 2019-10-29 06:16:57.000000 pkglts-6.5.0/src/pkglts/option/src/resource/src/{{ base.pkgname }}/__init__.py.tpl
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.130319 pkglts-6.5.0/src/pkglts/option/test/
--rw-rw-rw-   0        0        0       19 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.490536 pkglts-6.5.0/src/pkglts/option/test/example/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.490536 pkglts-6.5.0/src/pkglts/option/test/example/src/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.150314 pkglts-6.5.0/src/pkglts/option/test/example/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0      497 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/test/example/src/{{ base.pkgname }}/example.py.tpl
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.182314 pkglts-6.5.0/src/pkglts/option/test/example/test/
--rw-rw-rw-   0        0        0      285 2018-04-08 21:39:40.000000 pkglts-6.5.0/src/pkglts/option/test/example/test/__init__.py.tpl
--rw-rw-rw-   0        0        0     1521 2018-02-15 07:33:01.000000 pkglts-6.5.0/src/pkglts/option/test/example/test/test_example.py.tpl
--rw-rw-rw-   0        0        0     1094 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/test/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.198314 pkglts-6.5.0/src/pkglts/option/test/resource/
--rw-rw-rw-   0        0        0      472 2019-10-29 06:16:57.000000 pkglts-6.5.0/src/pkglts/option/test/resource/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.226844 pkglts-6.5.0/src/pkglts/option/test/resource/test/
--rw-rw-rw-   0        0        0     1072 2020-02-24 10:07:37.000000 pkglts-6.5.0/src/pkglts/option/test/resource/test/{% if test.suite_name == 'pytest' %}conftest{% else %}_{% endif %}.py.tpl
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.258834 pkglts-6.5.0/src/pkglts/option/tox/
--rw-rw-rw-   0        0        0       18 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/tox/__init__.py
--rw-rw-rw-   0        0        0      483 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/tox/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.274834 pkglts-6.5.0/src/pkglts/option/tox/resource/
--rw-rw-rw-   0        0        0      606 2023-03-13 18:21:24.000000 pkglts-6.5.0/src/pkglts/option/tox/resource/tox.ini
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.310856 pkglts-6.5.0/src/pkglts/option/travis/
--rw-rw-rw-   0        0        0       21 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/travis/__init__.py
--rw-rw-rw-   0        0        0      758 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/travis/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.330414 pkglts-6.5.0/src/pkglts/option/travis/resource/
--rw-rw-rw-   0        0        0     1860 2023-03-13 18:21:24.000000 pkglts-6.5.0/src/pkglts/option/travis/resource/.travis.yml
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.382427 pkglts-6.5.0/src/pkglts/option/version/
--rw-rw-rw-   0        0        0       22 2018-02-27 09:14:53.000000 pkglts-6.5.0/src/pkglts/option/version/__init__.py
--rw-rw-rw-   0        0        0     1652 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/version/bump_version.py
--rw-rw-rw-   0        0        0     1068 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option/version/option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.520593 pkglts-6.5.0/src/pkglts/option/version/resource/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:01.520593 pkglts-6.5.0/src/pkglts/option/version/resource/src/
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.422448 pkglts-6.5.0/src/pkglts/option/version/resource/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0       99 2019-10-29 06:16:57.000000 pkglts-6.5.0/src/pkglts/option/version/resource/src/{{ base.pkgname }}/__init__.py.tpl
--rw-rw-rw-   0        0        0      420 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/option/version/resource/src/{{ base.pkgname }}/version.py.tpl
--rw-rw-rw-   0        0        0     2876 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/option_object.py
--rw-rw-rw-   0        0        0     1496 2021-06-30 08:49:09.000000 pkglts-6.5.0/src/pkglts/option_tools.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:07.494413 pkglts-6.5.0/src/pkglts/resource/
--rw-rw-rw-   0        0        0      395 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/resource/namespace__init__.py.tpl
--rw-rw-rw-   0        0        0     4731 2020-04-15 05:36:21.000000 pkglts-6.5.0/src/pkglts/small_tools.py
--rw-rw-rw-   0        0        0     7451 2021-04-01 16:35:51.000000 pkglts-6.5.0/src/pkglts/templating.py
--rw-rw-rw-   0        0        0     1710 2019-10-29 22:35:37.000000 pkglts-6.5.0/src/pkglts/tree_ascii_fmt.py
--rw-rw-rw-   0        0        0      310 2023-03-13 18:21:24.000000 pkglts-6.5.0/src/pkglts/version.py
--rw-rw-rw-   0        0        0     2169 2021-07-07 13:18:45.000000 pkglts-6.5.0/src/pkglts/version_management.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:03.220752 pkglts-6.5.0/src/pkglts.egg-info/
--rw-rw-rw-   0        0        0     4782 2023-03-13 19:10:00.000000 pkglts-6.5.0/src/pkglts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    16447 2023-03-13 19:10:01.000000 pkglts-6.5.0/src/pkglts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 19:10:00.000000 pkglts-6.5.0/src/pkglts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1424 2023-03-13 19:10:00.000000 pkglts-6.5.0/src/pkglts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2017-12-07 14:17:38.000000 pkglts-6.5.0/src/pkglts.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2023-03-13 19:10:00.000000 pkglts-6.5.0/src/pkglts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-13 19:10:00.000000 pkglts-6.5.0/src/pkglts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.042608 pkglts-6.5.0/test/
--rw-rw-rw-   0        0        0        0 2018-12-13 12:11:43.000000 pkglts-6.5.0/test/__init__.py
--rw-rw-rw-   0        0        0      970 2023-03-13 18:15:33.000000 pkglts-6.5.0/test/conftest.py
--rw-rw-rw-   0        0        0        0 2017-01-03 08:51:05.000000 pkglts-6.5.0/test/info.rst
--rw-rw-rw-   0        0        0        0 2017-01-03 08:51:05.000000 pkglts-6.5.0/test/regenerate.no
--rw-rw-rw-   0        0        0     3421 2020-04-15 05:45:06.000000 pkglts-6.5.0/test/test_config_management.py
--rw-rw-rw-   0        0        0     4791 2019-10-29 06:16:57.000000 pkglts-6.5.0/test/test_dependency.py
--rw-rw-rw-   0        0        0      340 2019-10-29 06:16:57.000000 pkglts-6.5.0/test/test_file_management.py
--rw-rw-rw-   0        0        0     1956 2019-10-29 22:35:37.000000 pkglts-6.5.0/test/test_hash_management.py
--rw-rw-rw-   0        0        0      731 2019-10-29 22:35:37.000000 pkglts-6.5.0/test/test_local.py
--rw-rw-rw-   0        0        0      315 2018-02-15 07:33:01.000000 pkglts-6.5.0/test/test_manage.py
--rw-rw-rw-   0        0        0     3051 2019-10-29 22:35:37.000000 pkglts-6.5.0/test/test_manage_cfg.py
--rw-rw-rw-   0        0        0     1787 2019-10-29 22:35:37.000000 pkglts-6.5.0/test/test_manage_clean.py
--rw-rw-rw-   0        0        0     2774 2019-10-29 22:35:37.000000 pkglts-6.5.0/test/test_manage_example.py
--rw-rw-rw-   0        0        0     4454 2020-02-06 18:02:24.000000 pkglts-6.5.0/test/test_manage_regenerate.py
--rw-rw-rw-   0        0        0     1848 2020-10-22 13:45:14.000000 pkglts-6.5.0/test/test_manage_reset.py
--rw-rw-rw-   0        0        0      299 2019-10-29 06:16:57.000000 pkglts-6.5.0/test/test_manage_tools_check_option_parameters.py
--rw-rw-rw-   0        0        0     5217 2019-10-29 22:35:37.000000 pkglts-6.5.0/test/test_manage_tools_regenerate.py
--rw-rw-rw-   0        0        0     2126 2020-02-06 18:02:24.000000 pkglts-6.5.0/test/test_manage_tools_update_option.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.064805 pkglts-6.5.0/test/test_option/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.108835 pkglts-6.5.0/test/test_option/test_appveyor/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_appveyor/__init__.py
--rw-rw-rw-   0        0        0      714 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_appveyor/test_config.py
--rw-rw-rw-   0        0        0      318 2018-02-15 07:33:01.000000 pkglts-6.5.0/test/test_option/test_appveyor/test_handlers.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.132825 pkglts-6.5.0/test/test_option/test_base/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_base/__init__.py
--rw-rw-rw-   0        0        0     1338 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_base/test_config.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.164406 pkglts-6.5.0/test/test_option/test_conda/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_conda/__init__.py
--rw-rw-rw-   0        0        0     1074 2023-01-19 13:13:37.000000 pkglts-6.5.0/test/test_option/test_conda/test_config.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.192389 pkglts-6.5.0/test/test_option/test_coverage/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_coverage/__init__.py
--rw-rw-rw-   0        0        0      620 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_coverage/test_config.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.240002 pkglts-6.5.0/test/test_option/test_coveralls/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_coveralls/__init__.py
--rw-rw-rw-   0        0        0      458 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_coveralls/test_config.py
--rw-rw-rw-   0        0        0      304 2018-02-15 07:33:01.000000 pkglts-6.5.0/test/test_option/test_coveralls/test_handlers.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.262555 pkglts-6.5.0/test/test_option/test_data/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_data/__init__.py
--rw-rw-rw-   0        0        0      547 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_data/test_config.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.310585 pkglts-6.5.0/test/test_option/test_doc/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_doc/__init__.py
--rw-rw-rw-   0        0        0     1431 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_doc/test_config.py
--rw-rw-rw-   0        0        0      481 2019-10-29 06:16:57.000000 pkglts-6.5.0/test/test_option/test_doc/test_fmt_badge.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.336641 pkglts-6.5.0/test/test_option/test_flake8/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_flake8/__init__.py
--rw-rw-rw-   0        0        0      446 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_flake8/test_config.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.504579 pkglts-6.5.0/test/test_option/test_git/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_git/__init__.py
--rw-rw-rw-   0        0        0      646 2022-03-25 13:56:41.000000 pkglts-6.5.0/test/test_option/test_git/test_config.py
--rw-rw-rw-   0        0        0      673 2020-02-06 18:02:24.000000 pkglts-6.5.0/test/test_option/test_git/test_handlers.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.576572 pkglts-6.5.0/test/test_option/test_github/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_github/__init__.py
--rw-rw-rw-   0        0        0      718 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_github/test_config.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.620570 pkglts-6.5.0/test/test_option/test_gitlab/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_gitlab/__init__.py
--rw-rw-rw-   0        0        0      732 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_gitlab/test_config.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.670797 pkglts-6.5.0/test/test_option/test_landscape/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_landscape/__init__.py
--rw-rw-rw-   0        0        0      458 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_landscape/test_config.py
--rw-rw-rw-   0        0        0      304 2018-02-15 07:33:01.000000 pkglts-6.5.0/test/test_option/test_landscape/test_handlers.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.753152 pkglts-6.5.0/test/test_option/test_lgtm/
--rw-rw-rw-   0        0        0        0 2019-10-30 07:39:24.000000 pkglts-6.5.0/test/test_option/test_lgtm/__init__.py
--rw-rw-rw-   0        0        0      438 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_lgtm/test_config.py
--rw-rw-rw-   0        0        0      294 2019-10-30 07:39:24.000000 pkglts-6.5.0/test/test_option/test_lgtm/test_handlers.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.837154 pkglts-6.5.0/test/test_option/test_license/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_license/__init__.py
--rw-rw-rw-   0        0        0      950 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_license/test_config.py
--rw-rw-rw-   0        0        0      590 2017-07-15 20:09:55.000000 pkglts-6.5.0/test/test_option/test_license/test_handlers.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.881572 pkglts-6.5.0/test/test_option/test_notebook/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_notebook/__init__.py
--rw-rw-rw-   0        0        0     1063 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_notebook/test_config.py
--rw-rw-rw-   0        0        0     2059 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_option_common.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.909557 pkglts-6.5.0/test/test_option/test_plugin_project/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_plugin_project/__init__.py
--rw-rw-rw-   0        0        0     1002 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_plugin_project/test_config.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:08.971772 pkglts-6.5.0/test/test_option/test_pypi/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_pypi/__init__.py
--rw-rw-rw-   0        0        0      692 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_pypi/test_config.py
--rw-rw-rw-   0        0        0     1139 2023-03-13 18:21:24.000000 pkglts-6.5.0/test/test_option/test_pypi/test_handlers.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:09.036182 pkglts-6.5.0/test/test_option/test_pysetup/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_pysetup/__init__.py
--rw-rw-rw-   0        0        0      730 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_pysetup/test_config.py
--rw-rw-rw-   0        0        0     1751 2023-03-13 18:21:24.000000 pkglts-6.5.0/test/test_option/test_pysetup/test_handlers.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:09.090377 pkglts-6.5.0/test/test_option/test_readthedocs/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_readthedocs/__init__.py
--rw-rw-rw-   0        0        0      744 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_readthedocs/test_config.py
--rw-rw-rw-   0        0        0      235 2018-02-15 07:33:01.000000 pkglts-6.5.0/test/test_option/test_readthedocs/test_handlers.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:09.172505 pkglts-6.5.0/test/test_option/test_reqs/
--rw-rw-rw-   0        0        0        0 2019-10-29 06:16:57.000000 pkglts-6.5.0/test/test_option/test_reqs/__init__.py
--rw-rw-rw-   0        0        0     2231 2021-12-09 14:39:11.000000 pkglts-6.5.0/test/test_option/test_reqs/test_config.py
--rw-rw-rw-   0        0        0     1849 2019-10-29 22:35:37.000000 pkglts-6.5.0/test/test_option/test_reqs/test_find_requirements.py
--rw-rw-rw-   0        0        0      529 2019-10-29 22:35:37.000000 pkglts-6.5.0/test/test_option/test_reqs/test_handlers.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:09.220508 pkglts-6.5.0/test/test_option/test_requires/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_requires/__init__.py
--rw-rw-rw-   0        0        0      454 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_requires/test_config.py
--rw-rw-rw-   0        0        0      302 2018-02-15 07:33:01.000000 pkglts-6.5.0/test/test_option/test_requires/test_handlers.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:09.240772 pkglts-6.5.0/test/test_option/test_sphinx/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_sphinx/__init__.py
--rw-rw-rw-   0        0        0     1197 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_sphinx/test_config.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:09.316759 pkglts-6.5.0/test/test_option/test_src/
--rw-rw-rw-   0        0        0        0 2019-10-29 06:16:57.000000 pkglts-6.5.0/test/test_option/test_src/__init__.py
--rw-rw-rw-   0        0        0      690 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_src/test_config.py
--rw-rw-rw-   0        0        0      284 2019-10-29 06:16:57.000000 pkglts-6.5.0/test/test_option/test_src/test_handlers.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:09.348758 pkglts-6.5.0/test/test_option/test_test/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_test/__init__.py
--rw-rw-rw-   0        0        0      842 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_test/test_config.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:09.383016 pkglts-6.5.0/test/test_option/test_tox/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_tox/__init__.py
--rw-rw-rw-   0        0        0      434 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_tox/test_config.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:09.441235 pkglts-6.5.0/test/test_option/test_travis/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_travis/__init__.py
--rw-rw-rw-   0        0        0      446 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_travis/test_config.py
--rw-rw-rw-   0        0        0      298 2018-02-15 07:33:01.000000 pkglts-6.5.0/test/test_option/test_travis/test_handlers.py
-drwxrwxrwx   0        0        0        0 2023-03-13 19:10:09.503529 pkglts-6.5.0/test/test_option/test_version/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.5.0/test/test_option/test_version/__init__.py
--rw-rw-rw-   0        0        0     1335 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_option/test_version/test_config.py
--rw-rw-rw-   0        0        0      527 2020-02-06 18:02:24.000000 pkglts-6.5.0/test/test_option/test_version/test_handlers.py
--rw-rw-rw-   0        0        0     2527 2020-02-06 18:02:24.000000 pkglts-6.5.0/test/test_option_tools.py
--rw-rw-rw-   0        0        0     2694 2018-06-09 22:55:54.000000 pkglts-6.5.0/test/test_templating.py
--rw-rw-rw-   0        0        0     2110 2021-07-07 13:18:45.000000 pkglts-6.5.0/test/test_version_management.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.474955 pkglts-6.6.0/
+-rw-rw-rw-   0        0        0      460 2023-04-17 12:40:54.000000 pkglts-6.6.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3937 2023-04-17 12:40:54.000000 pkglts-6.6.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      167 2023-04-17 12:40:54.000000 pkglts-6.6.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    22406 2023-04-17 12:40:54.000000 pkglts-6.6.0/LICENSE
+-rw-rw-rw-   0        0        0      434 2023-04-17 12:40:54.000000 pkglts-6.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4782 2023-04-17 13:16:04.474955 pkglts-6.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3741 2023-04-17 12:40:54.000000 pkglts-6.6.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.768807 pkglts-6.6.0/doc/
+-rw-rw-rw-   0        0        0     6967 2023-04-17 12:40:54.000000 pkglts-6.6.0/doc/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.776779 pkglts-6.6.0/doc/_notebook/
+-rw-rw-rw-   0        0        0      754 2018-08-05 08:23:37.000000 pkglts-6.6.0/doc/_notebook/example.rst
+-rw-rw-rw-   0        0        0       97 2018-08-05 07:42:43.000000 pkglts-6.6.0/doc/_notebook/index.rst
+-rw-rw-rw-   0        0        0       29 2017-08-08 14:05:32.000000 pkglts-6.6.0/doc/authors.rst
+-rw-rw-rw-   0        0        0     4272 2023-04-17 13:15:22.000000 pkglts-6.6.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2017-08-08 14:05:32.000000 pkglts-6.6.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2017-08-08 14:05:32.000000 pkglts-6.6.0/doc/history.rst
+-rw-rw-rw-   0        0        0      420 2018-02-15 07:33:01.000000 pkglts-6.6.0/doc/index.rst
+-rw-rw-rw-   0        0        0      726 2018-02-15 09:25:07.000000 pkglts-6.6.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2023-04-17 12:40:54.000000 pkglts-6.6.0/doc/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.471795 pkglts-6.6.0/doc/option/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.780771 pkglts-6.6.0/doc/option/base/
+-rw-rw-rw-   0        0        0     1778 2018-02-27 09:14:53.000000 pkglts-6.6.0/doc/option/base/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.784821 pkglts-6.6.0/doc/option/conda/
+-rw-rw-rw-   0        0        0      621 2018-08-01 07:30:08.000000 pkglts-6.6.0/doc/option/conda/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.788774 pkglts-6.6.0/doc/option/coverage/
+-rw-rw-rw-   0        0        0     2177 2018-02-27 09:14:53.000000 pkglts-6.6.0/doc/option/coverage/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.796773 pkglts-6.6.0/doc/option/coveralls/
+-rw-rw-rw-   0        0        0     1766 2017-01-03 08:51:05.000000 pkglts-6.6.0/doc/option/coveralls/coveralls_tutorial.rst
+-rw-rw-rw-   0        0        0      972 2018-02-27 09:14:53.000000 pkglts-6.6.0/doc/option/coveralls/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.804779 pkglts-6.6.0/doc/option/data/
+-rw-rw-rw-   0        0        0     1150 2018-02-27 09:14:53.000000 pkglts-6.6.0/doc/option/data/data_tutorial.rst
+-rw-rw-rw-   0        0        0      329 2017-01-03 08:51:05.000000 pkglts-6.6.0/doc/option/data/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.808780 pkglts-6.6.0/doc/option/doc/
+-rw-rw-rw-   0        0        0      533 2018-02-27 09:14:53.000000 pkglts-6.6.0/doc/option/doc/history.rst
+-rw-rw-rw-   0        0        0     2053 2018-02-27 09:14:53.000000 pkglts-6.6.0/doc/option/doc/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.812778 pkglts-6.6.0/doc/option/flake8/
+-rw-rw-rw-   0        0        0      474 2018-02-27 09:14:53.000000 pkglts-6.6.0/doc/option/flake8/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.820773 pkglts-6.6.0/doc/option/git/
+-rw-rw-rw-   0        0        0      400 2018-02-15 07:33:01.000000 pkglts-6.6.0/doc/option/git/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.828772 pkglts-6.6.0/doc/option/github/
+-rw-rw-rw-   0        0        0     2785 2017-01-03 08:51:05.000000 pkglts-6.6.0/doc/option/github/github_tutorial.rst
+-rw-rw-rw-   0        0        0      451 2018-02-15 07:33:01.000000 pkglts-6.6.0/doc/option/github/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.838303 pkglts-6.6.0/doc/option/gitlab/
+-rw-rw-rw-   0        0        0     2627 2018-02-15 07:33:01.000000 pkglts-6.6.0/doc/option/gitlab/gitlab_tutorial.rst
+-rw-rw-rw-   0        0        0      402 2018-02-15 07:33:01.000000 pkglts-6.6.0/doc/option/gitlab/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.842308 pkglts-6.6.0/doc/option/landscape/
+-rw-rw-rw-   0        0        0     1207 2017-01-03 08:51:05.000000 pkglts-6.6.0/doc/option/landscape/landscape_tutorial.rst
+-rw-rw-rw-   0        0        0     1006 2018-02-27 09:14:53.000000 pkglts-6.6.0/doc/option/landscape/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.846325 pkglts-6.6.0/doc/option/lgtm/
+-rw-rw-rw-   0        0        0      557 2019-10-30 07:39:24.000000 pkglts-6.6.0/doc/option/lgtm/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.854303 pkglts-6.6.0/doc/option/license/
+-rw-rw-rw-   0        0        0     7038 2019-10-29 19:00:47.000000 pkglts-6.6.0/doc/option/license/license_list.rst
+-rw-rw-rw-   0        0        0      932 2018-02-27 09:14:53.000000 pkglts-6.6.0/doc/option/license/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.862306 pkglts-6.6.0/doc/option/notebook/
+-rw-rw-rw-   0        0        0      906 2018-04-06 16:07:32.000000 pkglts-6.6.0/doc/option/notebook/main.rst
+-rw-rw-rw-   0        0        0      854 2018-04-06 16:07:32.000000 pkglts-6.6.0/doc/option/notebook/nbcompile.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.870348 pkglts-6.6.0/doc/option/plugin/
+-rw-rw-rw-   0        0        0      642 2017-01-03 08:51:05.000000 pkglts-6.6.0/doc/option/plugin/main.rst
+-rw-rw-rw-   0        0        0      148 2017-01-03 08:51:05.000000 pkglts-6.6.0/doc/option/plugin/plugin_tutorial.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.874307 pkglts-6.6.0/doc/option/plugin_project/
+-rw-rw-rw-   0        0        0     1080 2017-07-15 20:09:55.000000 pkglts-6.6.0/doc/option/plugin_project/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.882306 pkglts-6.6.0/doc/option/pypi/
+-rw-rw-rw-   0        0        0      343 2018-02-27 09:14:53.000000 pkglts-6.6.0/doc/option/pypi/main.rst
+-rw-rw-rw-   0        0        0     3660 2017-01-03 08:51:05.000000 pkglts-6.6.0/doc/option/pypi/pypi_tutorial.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.890306 pkglts-6.6.0/doc/option/pysetup/
+-rw-rw-rw-   0        0        0     1122 2018-08-05 08:23:37.000000 pkglts-6.6.0/doc/option/pysetup/main.rst
+-rw-rw-rw-   0        0        0      355 2018-08-05 08:23:37.000000 pkglts-6.6.0/doc/option/pysetup/reqs.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.898308 pkglts-6.6.0/doc/option/readthedocs/
+-rw-rw-rw-   0        0        0      723 2018-02-27 09:14:53.000000 pkglts-6.6.0/doc/option/readthedocs/main.rst
+-rw-rw-rw-   0        0        0     2666 2017-01-03 08:51:05.000000 pkglts-6.6.0/doc/option/readthedocs/readthedocs_tutorial.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.906321 pkglts-6.6.0/doc/option/requires/
+-rw-rw-rw-   0        0        0      743 2018-02-27 09:14:53.000000 pkglts-6.6.0/doc/option/requires/main.rst
+-rw-rw-rw-   0        0        0     1117 2018-02-15 07:33:01.000000 pkglts-6.6.0/doc/option/requires/requires_tutorial.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.910304 pkglts-6.6.0/doc/option/sphinx/
+-rw-rw-rw-   0        0        0     1460 2018-04-06 16:07:32.000000 pkglts-6.6.0/doc/option/sphinx/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.914307 pkglts-6.6.0/doc/option/test/
+-rw-rw-rw-   0        0        0     1179 2018-02-27 09:14:53.000000 pkglts-6.6.0/doc/option/test/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.918342 pkglts-6.6.0/doc/option/tox/
+-rw-rw-rw-   0        0        0      698 2018-02-27 09:14:53.000000 pkglts-6.6.0/doc/option/tox/main.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.930302 pkglts-6.6.0/doc/option/travis/
+-rw-rw-rw-   0        0        0      519 2021-05-27 13:53:46.000000 pkglts-6.6.0/doc/option/travis/main.rst
+-rw-rw-rw-   0        0        0     2089 2021-05-27 13:53:46.000000 pkglts-6.6.0/doc/option/travis/travis_tutorial.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.948890 pkglts-6.6.0/doc/option/version/
+-rw-rw-rw-   0        0        0      421 2018-08-05 08:23:37.000000 pkglts-6.6.0/doc/option/version/bump.rst
+-rw-rw-rw-   0        0        0      556 2018-02-27 09:14:53.000000 pkglts-6.6.0/doc/option/version/main.rst
+-rw-rw-rw-   0        0        0     2192 2018-02-15 07:33:01.000000 pkglts-6.6.0/doc/option_list.rst
+-rw-rw-rw-   0        0        0     5879 2019-03-14 16:09:18.000000 pkglts-6.6.0/doc/readme.rst
+-rw-rw-rw-   0        0        0      318 2018-08-05 08:23:37.000000 pkglts-6.6.0/doc/tool_list.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.976898 pkglts-6.6.0/doc/tutorial/
+-rw-rw-rw-   0        0        0      668 2017-01-03 08:51:05.000000 pkglts-6.6.0/doc/tutorial/dvlpt_env.rst
+-rw-rw-rw-   0        0        0      468 2017-01-03 08:51:05.000000 pkglts-6.6.0/doc/tutorial/migration.rst
+-rw-rw-rw-   0        0        0     1145 2018-10-31 18:23:46.000000 pkglts-6.6.0/doc/tutorial/pypi.rst
+-rw-rw-rw-   0        0        0      635 2017-01-03 08:51:05.000000 pkglts-6.6.0/doc/tutorial/web_tools.rst
+-rw-rw-rw-   0        0        0      773 2018-02-15 07:33:01.000000 pkglts-6.6.0/doc/tutorials.rst
+-rw-rw-rw-   0        0        0     1117 2017-08-08 14:05:32.000000 pkglts-6.6.0/doc/usage.rst
+-rw-rw-rw-   0        0        0      323 2023-04-17 12:40:54.000000 pkglts-6.6.0/requirements.txt
+-rw-rw-rw-   0        0        0       66 2023-04-17 12:40:54.000000 pkglts-6.6.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0      236 2023-04-17 13:16:04.478920 pkglts-6.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     3937 2023-04-17 13:15:22.000000 pkglts-6.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.475795 pkglts-6.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.058447 pkglts-6.6.0/src/pkglts/
+-rw-rw-rw-   0        0        0      183 2023-04-17 12:40:54.000000 pkglts-6.6.0/src/pkglts/__init__.py
+-rw-rw-rw-   0        0        0      202 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/config.py
+-rw-rw-rw-   0        0        0    12875 2023-03-13 18:21:24.000000 pkglts-6.6.0/src/pkglts/config_management.py
+-rw-rw-rw-   0        0        0     5526 2019-10-29 06:16:57.000000 pkglts-6.6.0/src/pkglts/dependency.py
+-rw-rw-rw-   0        0        0      407 2019-08-27 13:00:03.000000 pkglts-6.6.0/src/pkglts/file_management.py
+-rw-rw-rw-   0        0        0     2754 2019-11-13 12:35:41.000000 pkglts-6.6.0/src/pkglts/hash_management.py
+-rw-rw-rw-   0        0        0     1427 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/local.py
+-rw-rw-rw-   0        0        0     1634 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/logging_tools.py
+-rw-rw-rw-   0        0        0     9009 2021-03-03 16:14:09.000000 pkglts-6.6.0/src/pkglts/manage.py
+-rw-rw-rw-   0        0        0     7395 2020-10-22 13:45:14.000000 pkglts-6.6.0/src/pkglts/manage_script.py
+-rw-rw-rw-   0        0        0     4113 2021-07-07 13:18:45.000000 pkglts-6.6.0/src/pkglts/manage_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.094433 pkglts-6.6.0/src/pkglts/option/
+-rw-rw-rw-   0        0        0       45 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.102491 pkglts-6.6.0/src/pkglts/option/appveyor/
+-rw-rw-rw-   0        0        0       23 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/appveyor/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-03-16 10:29:48.000000 pkglts-6.6.0/src/pkglts/option/appveyor/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.106437 pkglts-6.6.0/src/pkglts/option/appveyor/resource/
+-rw-rw-rw-   0        0        0     1117 2023-04-17 13:15:22.000000 pkglts-6.6.0/src/pkglts/option/appveyor/resource/appveyor.yml
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.114441 pkglts-6.6.0/src/pkglts/option/base/
+-rw-rw-rw-   0        0        0       19 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/base/__init__.py
+-rw-rw-rw-   0        0        0     1310 2023-03-16 10:21:50.000000 pkglts-6.6.0/src/pkglts/option/base/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.130443 pkglts-6.6.0/src/pkglts/option/conda/
+-rw-rw-rw-   0        0        0       20 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/conda/__init__.py
+-rw-rw-rw-   0        0        0     1121 2023-03-16 10:29:48.000000 pkglts-6.6.0/src/pkglts/option/conda/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.483809 pkglts-6.6.0/src/pkglts/option/conda/resource/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.140571 pkglts-6.6.0/src/pkglts/option/conda/resource/conda/
+-rw-rw-rw-   0        0        0     1083 2021-12-15 17:52:05.000000 pkglts-6.6.0/src/pkglts/option/conda/resource/conda/meta.yaml
+-rw-rw-rw-   0        0        0      848 2023-03-13 18:21:24.000000 pkglts-6.6.0/src/pkglts/option/conda/resource/conda/requirements.yml
+-rw-rw-rw-   0        0        0      682 2023-03-13 18:21:24.000000 pkglts-6.6.0/src/pkglts/option/conda/resource/conda/requirements_minimal.yml
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.152612 pkglts-6.6.0/src/pkglts/option/coverage/
+-rw-rw-rw-   0        0        0       23 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/coverage/__init__.py
+-rw-rw-rw-   0        0        0      616 2023-03-16 10:29:48.000000 pkglts-6.6.0/src/pkglts/option/coverage/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.156568 pkglts-6.6.0/src/pkglts/option/coverage/resource/
+-rw-rw-rw-   0        0        0      367 2018-06-06 09:43:05.000000 pkglts-6.6.0/src/pkglts/option/coverage/resource/.coveragerc
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.164572 pkglts-6.6.0/src/pkglts/option/coveralls/
+-rw-rw-rw-   0        0        0       24 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/coveralls/__init__.py
+-rw-rw-rw-   0        0        0      985 2023-03-16 10:29:48.000000 pkglts-6.6.0/src/pkglts/option/coveralls/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.172565 pkglts-6.6.0/src/pkglts/option/data/
+-rw-rw-rw-   0        0        0       19 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.510096 pkglts-6.6.0/src/pkglts/option/data/example/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.508013 pkglts-6.6.0/src/pkglts/option/data/example/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.188572 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/
+-rw-rw-rw-   0        0        0   342163 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.png
+-rw-rw-rw-   0        0        0       13 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.txt
+-rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.ui
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.204626 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/
+-rw-rw-rw-   0        0        0   342163 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.png
+-rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.txt
+-rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.ui
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.220565 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/
+-rw-rw-rw-   0        0        0   342163 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.png
+-rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.txt
+-rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.ui
+-rw-rw-rw-   0        0        0      365 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/list_data.py.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.238618 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/
+-rw-rw-rw-   0        0        0        0 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/__init__.py.tpl
+-rw-rw-rw-   0        0        0   342163 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.png
+-rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.txt
+-rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.ui
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.242605 pkglts-6.6.0/src/pkglts/option/data/example/test/
+-rw-rw-rw-   0        0        0      538 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/test/{% if data.use_ext_dir %}test_data{% else %}_{% endif %}.py.tpl
+-rw-rw-rw-   0        0        0      296 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/example/test/{% if not data.use_ext_dir %}test_data{% else %}_{% endif %}.py.tpl
+-rw-rw-rw-   0        0        0      608 2023-03-16 10:29:48.000000 pkglts-6.6.0/src/pkglts/option/data/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.514065 pkglts-6.6.0/src/pkglts/option/data/resource/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.518076 pkglts-6.6.0/src/pkglts/option/data/resource/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.246607 pkglts-6.6.0/src/pkglts/option/data/resource/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/
+-rw-rw-rw-   0        0        0        0 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/data/resource/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/__init__.py.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.250603 pkglts-6.6.0/src/pkglts/option/data/resource/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0     1500 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/data/resource/src/{{ base.pkgname }}/{% if data.use_ext_dir %}data_access{% else %}_{% endif %}.py.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.262604 pkglts-6.6.0/src/pkglts/option/doc/
+-rw-rw-rw-   0        0        0      796 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/doc/__init__.py
+-rw-rw-rw-   0        0        0     5564 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/doc/history.py
+-rw-rw-rw-   0        0        0     1775 2023-03-16 10:29:49.000000 pkglts-6.6.0/src/pkglts/option/doc/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.294602 pkglts-6.6.0/src/pkglts/option/doc/resource/
+-rw-rw-rw-   0        0        0      411 2020-04-15 06:18:47.000000 pkglts-6.6.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}AUTHORS{% else %}_{% endif %}.md
+-rw-rw-rw-   0        0        0     4505 2021-07-07 13:18:45.000000 pkglts-6.6.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}CONTRIBUTING{% else %}_{% endif %}.md
+-rw-rw-rw-   0        0        0       70 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}HISTORY{% else %}_{% endif %}.md
+-rw-rw-rw-   0        0        0      158 2020-04-15 06:18:47.000000 pkglts-6.6.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}README{% else %}_{% endif %}.md
+-rw-rw-rw-   0        0        0      377 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}mkdocs{% else %}_{% endif %}.yml
+-rw-rw-rw-   0        0        0      424 2020-04-15 06:04:23.000000 pkglts-6.6.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}AUTHORS{% else %}_{% endif %}.rst
+-rw-rw-rw-   0        0        0     4706 2023-03-13 18:21:24.000000 pkglts-6.6.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}CONTRIBUTING{% else %}_{% endif %}.rst
+-rw-rw-rw-   0        0        0      109 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}HISTORY{% else %}_{% endif %}.rst
+-rw-rw-rw-   0        0        0      192 2020-04-15 06:18:47.000000 pkglts-6.6.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}README{% else %}_{% endif %}.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.302605 pkglts-6.6.0/src/pkglts/option/flake8/
+-rw-rw-rw-   0        0        0       21 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/flake8/__init__.py
+-rw-rw-rw-   0        0        0      520 2023-03-16 10:29:48.000000 pkglts-6.6.0/src/pkglts/option/flake8/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.306604 pkglts-6.6.0/src/pkglts/option/flake8/resource/
+-rw-rw-rw-   0        0        0      173 2019-10-29 06:16:57.000000 pkglts-6.6.0/src/pkglts/option/flake8/resource/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.314604 pkglts-6.6.0/src/pkglts/option/git/
+-rw-rw-rw-   0        0        0       18 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/git/__init__.py
+-rw-rw-rw-   0        0        0     1447 2023-03-16 10:29:48.000000 pkglts-6.6.0/src/pkglts/option/git/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.322604 pkglts-6.6.0/src/pkglts/option/git/resource/
+-rw-rw-rw-   0        0        0     1580 2021-03-03 16:14:09.000000 pkglts-6.6.0/src/pkglts/option/git/resource/.gitignore
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.330611 pkglts-6.6.0/src/pkglts/option/github/
+-rw-rw-rw-   0        0        0       21 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/github/__init__.py
+-rw-rw-rw-   0        0        0      905 2023-03-16 10:29:48.000000 pkglts-6.6.0/src/pkglts/option/github/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.340719 pkglts-6.6.0/src/pkglts/option/gitlab/
+-rw-rw-rw-   0        0        0       21 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/gitlab/__init__.py
+-rw-rw-rw-   0        0        0      950 2023-03-16 10:29:47.000000 pkglts-6.6.0/src/pkglts/option/gitlab/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.348708 pkglts-6.6.0/src/pkglts/option/landscape/
+-rw-rw-rw-   0        0        0       24 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/landscape/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-03-16 10:29:48.000000 pkglts-6.6.0/src/pkglts/option/landscape/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.356710 pkglts-6.6.0/src/pkglts/option/landscape/resource/
+-rw-rw-rw-   0        0        0      323 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/landscape/resource/.landscape.yml
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.360717 pkglts-6.6.0/src/pkglts/option/lgtm/
+-rw-rw-rw-   0        0        0       19 2019-10-30 07:39:24.000000 pkglts-6.6.0/src/pkglts/option/lgtm/__init__.py
+-rw-rw-rw-   0        0        0      864 2023-03-16 10:29:46.000000 pkglts-6.6.0/src/pkglts/option/lgtm/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.372746 pkglts-6.6.0/src/pkglts/option/license/
+-rw-rw-rw-   0        0        0       22 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/license/__init__.py
+-rw-rw-rw-   0        0        0     1879 2023-03-16 10:29:48.000000 pkglts-6.6.0/src/pkglts/option/license/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.376732 pkglts-6.6.0/src/pkglts/option/license/resource/
+-rw-rw-rw-   0        0        0       49 2020-03-17 18:25:54.000000 pkglts-6.6.0/src/pkglts/option/license/resource/LICENSE.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.617226 pkglts-6.6.0/src/pkglts/option/license/templates/
+-rw-rw-rw-   0        0        0      741 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/agpl3-header.txt
+-rw-rw-rw-   0        0        0    35211 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/agpl3.txt
+-rw-rw-rw-   0        0        0      596 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/apache-header.txt
+-rw-rw-rw-   0        0        0    11131 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/apache.txt
+-rw-rw-rw-   0        0        0     1373 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/bsd2.txt
+-rw-rw-rw-   0        0        0     1585 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/bsd3.txt
+-rw-rw-rw-   0        0        0      389 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cc0-header.txt
+-rw-rw-rw-   0        0        0     7169 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cc0.txt
+-rw-rw-rw-   0        0        0      316 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cc_by-header.txt
+-rw-rw-rw-   0        0        0    19785 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cc_by.txt
+-rw-rw-rw-   0        0        0      333 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cc_by_nc-header.txt
+-rw-rw-rw-   0        0        0    20812 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cc_by_nc.txt
+-rw-rw-rw-   0        0        0      345 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cc_by_nc_nd-header.txt
+-rw-rw-rw-   0        0        0    18957 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cc_by_nc_nd.txt
+-rw-rw-rw-   0        0        0      347 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cc_by_nc_sa-header.txt
+-rw-rw-rw-   0        0        0    22669 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cc_by_nc_sa.txt
+-rw-rw-rw-   0        0        0      328 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cc_by_nd-header.txt
+-rw-rw-rw-   0        0        0    17942 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cc_by_nd.txt
+-rw-rw-rw-   0        0        0      330 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cc_by_sa-header.txt
+-rw-rw-rw-   0        0        0    22597 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cc_by_sa.txt
+-rw-rw-rw-   0        0        0    17650 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cddl.txt
+-rw-rw-rw-   0        0        0     1527 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cecill-c-header.txt
+-rw-rw-rw-   0        0        0    22380 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/cecill-c.txt
+-rw-rw-rw-   0        0        0    11840 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/epl.txt
+-rw-rw-rw-   0        0        0    18173 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/gpl2.txt
+-rw-rw-rw-   0        0        0      720 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/gpl3-header.txt
+-rw-rw-rw-   0        0        0    35864 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/gpl3.txt
+-rw-rw-rw-   0        0        0     6426 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/inra_license_agreement.txt
+-rw-rw-rw-   0        0        0      778 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/isc.txt
+-rw-rw-rw-   0        0        0     7777 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/lgpl.txt
+-rw-rw-rw-   0        0        0     1103 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/mit.txt
+-rw-rw-rw-   0        0        0      196 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/mpl-header.txt
+-rw-rw-rw-   0        0        0    16078 2017-05-18 09:15:38.000000 pkglts-6.6.0/src/pkglts/option/license/templates/mpl.txt
+-rw-rw-rw-   0        0        0     9475 2020-04-14 06:55:23.000000 pkglts-6.6.0/src/pkglts/option/license/templates/private.txt
+-rw-rw-rw-   0        0        0     1235 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/unlicense.txt
+-rw-rw-rw-   0        0        0      301 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/wtfpl-header-warranty.txt
+-rw-rw-rw-   0        0        0      301 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/wtfpl-header.txt
+-rw-rw-rw-   0        0        0      515 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/wtfpl.txt
+-rw-rw-rw-   0        0        0     1444 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/x11.txt
+-rw-rw-rw-   0        0        0      919 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/license/templates/zlib.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.633224 pkglts-6.6.0/src/pkglts/option/notebook/
+-rw-rw-rw-   0        0        0       23 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/notebook/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.548647 pkglts-6.6.0/src/pkglts/option/notebook/example/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.640202 pkglts-6.6.0/src/pkglts/option/notebook/example/{{ notebook.src_directory }}/
+-rw-rw-rw-   0        0        0    17056 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/notebook/example/{{ notebook.src_directory }}/example.ipynb
+-rw-rw-rw-   0        0        0     4449 2019-10-29 06:16:57.000000 pkglts-6.6.0/src/pkglts/option/notebook/nbcompile.py
+-rw-rw-rw-   0        0        0      933 2023-03-16 10:29:47.000000 pkglts-6.6.0/src/pkglts/option/notebook/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.645224 pkglts-6.6.0/src/pkglts/option/plugin_project/
+-rw-rw-rw-   0        0        0       49 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/plugin_project/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.556660 pkglts-6.6.0/src/pkglts/option/plugin_project/example/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.560648 pkglts-6.6.0/src/pkglts/option/plugin_project/example/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.560648 pkglts-6.6.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.657228 pkglts-6.6.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/resource/
+-rw-rw-rw-   0        0        0       83 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/resource/extra_file.txt
+-rw-rw-rw-   0        0        0       92 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/resource/extra_script.py.tpl
+-rw-rw-rw-   0        0        0     1091 2023-03-16 10:29:49.000000 pkglts-6.6.0/src/pkglts/option/plugin_project/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.661224 pkglts-6.6.0/src/pkglts/option/plugin_project/resource/
+-rw-rw-rw-   0        0        0      225 2019-10-29 06:16:57.000000 pkglts-6.6.0/src/pkglts/option/plugin_project/resource/setup.py.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.560648 pkglts-6.6.0/src/pkglts/option/plugin_project/resource/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.665230 pkglts-6.6.0/src/pkglts/option/plugin_project/resource/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0     1016 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/plugin_project/resource/src/{{ base.pkgname }}/option.py.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.673246 pkglts-6.6.0/src/pkglts/option/pypi/
+-rw-rw-rw-   0        0        0       19 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/pypi/__init__.py
+-rw-rw-rw-   0        0        0     2810 2023-03-16 10:29:48.000000 pkglts-6.6.0/src/pkglts/option/pypi/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.677235 pkglts-6.6.0/src/pkglts/option/pypi/resource/
+-rw-rw-rw-   0        0        0      290 2020-04-15 06:02:11.000000 pkglts-6.6.0/src/pkglts/option/pypi/resource/.pypirc
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.685232 pkglts-6.6.0/src/pkglts/option/pysetup/
+-rw-rw-rw-   0        0        0       22 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/pysetup/__init__.py
+-rw-rw-rw-   0        0        0     2288 2023-04-17 13:15:22.000000 pkglts-6.6.0/src/pkglts/option/pysetup/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.699535 pkglts-6.6.0/src/pkglts/option/pysetup/resource/
+-rw-rw-rw-   0        0        0      739 2019-10-29 06:16:57.000000 pkglts-6.6.0/src/pkglts/option/pysetup/resource/MANIFEST.in
+-rw-rw-rw-   0        0        0      122 2020-02-06 18:07:27.000000 pkglts-6.6.0/src/pkglts/option/pysetup/resource/setup.cfg
+-rw-rw-rw-   0        0        0     2954 2021-04-29 10:55:32.000000 pkglts-6.6.0/src/pkglts/option/pysetup/resource/setup.py.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.707508 pkglts-6.6.0/src/pkglts/option/readthedocs/
+-rw-rw-rw-   0        0        0       26 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/readthedocs/__init__.py
+-rw-rw-rw-   0        0        0     1728 2023-03-16 10:29:49.000000 pkglts-6.6.0/src/pkglts/option/readthedocs/option.py
+-rw-rw-rw-   0        0        0        0 2017-01-03 08:51:05.000000 pkglts-6.6.0/src/pkglts/option/regenerate.no
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.726557 pkglts-6.6.0/src/pkglts/option/reqs/
+-rw-rw-rw-   0        0        0       56 2019-10-29 06:16:57.000000 pkglts-6.6.0/src/pkglts/option/reqs/__init__.py
+-rw-rw-rw-   0        0        0     2351 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/reqs/find_requirements.py
+-rw-rw-rw-   0        0        0     3919 2023-03-16 10:29:49.000000 pkglts-6.6.0/src/pkglts/option/reqs/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.730552 pkglts-6.6.0/src/pkglts/option/reqs/resource/
+-rw-rw-rw-   0        0        0      319 2020-04-15 06:18:47.000000 pkglts-6.6.0/src/pkglts/option/reqs/resource/requirements.txt
+-rw-rw-rw-   0        0        0      136 2020-04-15 06:18:47.000000 pkglts-6.6.0/src/pkglts/option/reqs/resource/requirements_minimal.txt
+-rw-rw-rw-   0        0        0     2100 2019-10-29 06:16:57.000000 pkglts-6.6.0/src/pkglts/option/reqs/stdpkgs.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.754572 pkglts-6.6.0/src/pkglts/option/requires/
+-rw-rw-rw-   0        0        0       23 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/requires/__init__.py
+-rw-rw-rw-   0        0        0      852 2023-03-16 10:29:49.000000 pkglts-6.6.0/src/pkglts/option/requires/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.762549 pkglts-6.6.0/src/pkglts/option/sphinx/
+-rw-rw-rw-   0        0        0       21 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/sphinx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.592668 pkglts-6.6.0/src/pkglts/option/sphinx/example/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.766550 pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.823594 pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/
+-rw-rw-rw-   0        0        0      312 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/autodoc.rst
+-rw-rw-rw-   0        0        0      358 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/autosummary.rst
+-rw-rw-rw-   0        0        0      385 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/graphviz.rst
+-rw-rw-rw-   0        0        0      468 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/ifconfig.rst
+-rw-rw-rw-   0        0        0      221 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/index.rst
+-rw-rw-rw-   0        0        0      823 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/inheritance.rst
+-rw-rw-rw-   0        0        0      631 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/intersphinx.rst
+-rw-rw-rw-   0        0        0      364 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/math.rst
+-rw-rw-rw-   0        0        0      665 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/matplotlib.rst
+-rw-rw-rw-   0        0        0      441 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/todo.rst
+-rw-rw-rw-   0        0        0      344 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/viewcode.rst
+-rw-rw-rw-   0        0        0      443 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/workflow.dot
+-rw-rw-rw-   0        0        0      493 2019-10-29 06:16:57.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/index.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.592668 pkglts-6.6.0/src/pkglts/option/sphinx/example/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.831597 pkglts-6.6.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0      742 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_doc.py.tpl
+-rw-rw-rw-   0        0        0      110 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_inheritance1.py.tpl
+-rw-rw-rw-   0        0        0       81 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_inheritance2.py.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.839634 pkglts-6.6.0/src/pkglts/option/sphinx/example/{{ sphinx.gallery  }}/
+-rw-rw-rw-   0        0        0      109 2019-10-29 06:16:57.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/{{ sphinx.gallery  }}/README.rst
+-rw-rw-rw-   0        0        0      297 2019-10-29 06:16:57.000000 pkglts-6.6.0/src/pkglts/option/sphinx/example/{{ sphinx.gallery  }}/plot_smth.py
+-rw-rw-rw-   0        0        0     1560 2023-03-16 10:29:47.000000 pkglts-6.6.0/src/pkglts/option/sphinx/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.843591 pkglts-6.6.0/src/pkglts/option/sphinx/resource/
+-rw-rw-rw-   0        0        0       77 2021-03-01 14:25:42.000000 pkglts-6.6.0/src/pkglts/option/sphinx/resource/{% if 'pysetup' is available %}setup{% else %}_{% endif %}.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.851591 pkglts-6.6.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/
+-rw-rw-rw-   0        0        0     6967 2021-03-01 14:25:42.000000 pkglts-6.6.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.855599 pkglts-6.6.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/_static/
+-rw-rw-rw-   0        0        0        0 2021-03-01 14:25:42.000000 pkglts-6.6.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/_static/nonempty.txt
+-rw-rw-rw-   0        0        0     5819 2021-03-01 14:25:42.000000 pkglts-6.6.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/conf.py.tpl
+-rwxrwxrwx   0        0        0     6731 2021-03-01 14:25:42.000000 pkglts-6.6.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.863591 pkglts-6.6.0/src/pkglts/option/src/
+-rw-rw-rw-   0        0        0       58 2019-10-29 06:16:57.000000 pkglts-6.6.0/src/pkglts/option/src/__init__.py
+-rw-rw-rw-   0        0        0      961 2023-03-16 10:29:48.000000 pkglts-6.6.0/src/pkglts/option/src/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.608665 pkglts-6.6.0/src/pkglts/option/src/resource/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.608665 pkglts-6.6.0/src/pkglts/option/src/resource/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.867590 pkglts-6.6.0/src/pkglts/option/src/resource/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0      109 2019-10-29 06:16:57.000000 pkglts-6.6.0/src/pkglts/option/src/resource/src/{{ base.pkgname }}/__init__.py.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.875592 pkglts-6.6.0/src/pkglts/option/test/
+-rw-rw-rw-   0        0        0       19 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.612644 pkglts-6.6.0/src/pkglts/option/test/example/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.612644 pkglts-6.6.0/src/pkglts/option/test/example/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.883594 pkglts-6.6.0/src/pkglts/option/test/example/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0      497 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/test/example/src/{{ base.pkgname }}/example.py.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.895612 pkglts-6.6.0/src/pkglts/option/test/example/test/
+-rw-rw-rw-   0        0        0      285 2018-04-08 21:39:40.000000 pkglts-6.6.0/src/pkglts/option/test/example/test/__init__.py.tpl
+-rw-rw-rw-   0        0        0     1521 2018-02-15 07:33:01.000000 pkglts-6.6.0/src/pkglts/option/test/example/test/test_example.py.tpl
+-rw-rw-rw-   0        0        0     1207 2023-03-16 10:29:49.000000 pkglts-6.6.0/src/pkglts/option/test/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.899595 pkglts-6.6.0/src/pkglts/option/test/resource/
+-rw-rw-rw-   0        0        0      546 2023-04-17 13:15:22.000000 pkglts-6.6.0/src/pkglts/option/test/resource/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.907637 pkglts-6.6.0/src/pkglts/option/test/resource/test/
+-rw-rw-rw-   0        0        0     1086 2023-04-17 13:15:22.000000 pkglts-6.6.0/src/pkglts/option/test/resource/test/{% if test.suite_name == 'pytest' %}conftest{% else %}_{% endif %}.py.tpl
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.915624 pkglts-6.6.0/src/pkglts/option/tox/
+-rw-rw-rw-   0        0        0       18 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/tox/__init__.py
+-rw-rw-rw-   0        0        0      539 2023-03-16 10:29:47.000000 pkglts-6.6.0/src/pkglts/option/tox/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.919592 pkglts-6.6.0/src/pkglts/option/tox/resource/
+-rw-rw-rw-   0        0        0      606 2023-03-13 18:21:24.000000 pkglts-6.6.0/src/pkglts/option/tox/resource/tox.ini
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.934634 pkglts-6.6.0/src/pkglts/option/travis/
+-rw-rw-rw-   0        0        0       21 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/travis/__init__.py
+-rw-rw-rw-   0        0        0      814 2023-03-16 10:29:47.000000 pkglts-6.6.0/src/pkglts/option/travis/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.942634 pkglts-6.6.0/src/pkglts/option/travis/resource/
+-rw-rw-rw-   0        0        0     1746 2023-04-17 13:15:22.000000 pkglts-6.6.0/src/pkglts/option/travis/resource/.travis.yml
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.958635 pkglts-6.6.0/src/pkglts/option/version/
+-rw-rw-rw-   0        0        0       22 2018-02-27 09:14:53.000000 pkglts-6.6.0/src/pkglts/option/version/__init__.py
+-rw-rw-rw-   0        0        0     1652 2021-07-07 13:18:45.000000 pkglts-6.6.0/src/pkglts/option/version/bump_version.py
+-rw-rw-rw-   0        0        0     1179 2023-03-16 10:29:50.000000 pkglts-6.6.0/src/pkglts/option/version/option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.628646 pkglts-6.6.0/src/pkglts/option/version/resource/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:02.630181 pkglts-6.6.0/src/pkglts/option/version/resource/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.966637 pkglts-6.6.0/src/pkglts/option/version/resource/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0       99 2019-10-29 06:16:57.000000 pkglts-6.6.0/src/pkglts/option/version/resource/src/{{ base.pkgname }}/__init__.py.tpl
+-rw-rw-rw-   0        0        0      420 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/option/version/resource/src/{{ base.pkgname }}/version.py.tpl
+-rw-rw-rw-   0        0        0     2876 2021-07-07 13:18:45.000000 pkglts-6.6.0/src/pkglts/option_object.py
+-rw-rw-rw-   0        0        0     1496 2021-06-30 08:49:09.000000 pkglts-6.6.0/src/pkglts/option_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.974694 pkglts-6.6.0/src/pkglts/resource/
+-rw-rw-rw-   0        0        0      395 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/resource/namespace__init__.py.tpl
+-rw-rw-rw-   0        0        0     4731 2020-04-15 05:36:21.000000 pkglts-6.6.0/src/pkglts/small_tools.py
+-rw-rw-rw-   0        0        0     7451 2021-04-01 16:35:51.000000 pkglts-6.6.0/src/pkglts/templating.py
+-rw-rw-rw-   0        0        0     1710 2019-10-29 22:35:37.000000 pkglts-6.6.0/src/pkglts/tree_ascii_fmt.py
+-rw-rw-rw-   0        0        0      310 2023-04-17 13:15:22.000000 pkglts-6.6.0/src/pkglts/version.py
+-rw-rw-rw-   0        0        0     2169 2021-07-07 13:18:45.000000 pkglts-6.6.0/src/pkglts/version_management.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:03.086468 pkglts-6.6.0/src/pkglts.egg-info/
+-rw-rw-rw-   0        0        0     4782 2023-04-17 13:16:01.000000 pkglts-6.6.0/src/pkglts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    16447 2023-04-17 13:16:02.000000 pkglts-6.6.0/src/pkglts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 13:16:01.000000 pkglts-6.6.0/src/pkglts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1424 2023-04-17 13:16:01.000000 pkglts-6.6.0/src/pkglts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2017-12-07 14:17:38.000000 pkglts-6.6.0/src/pkglts.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-04-17 13:16:01.000000 pkglts-6.6.0/src/pkglts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 13:16:01.000000 pkglts-6.6.0/src/pkglts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.083706 pkglts-6.6.0/test/
+-rw-rw-rw-   0        0        0        0 2018-12-13 12:11:43.000000 pkglts-6.6.0/test/__init__.py
+-rw-rw-rw-   0        0        0      982 2023-04-17 13:15:22.000000 pkglts-6.6.0/test/conftest.py
+-rw-rw-rw-   0        0        0        0 2017-01-03 08:51:05.000000 pkglts-6.6.0/test/info.rst
+-rw-rw-rw-   0        0        0        0 2017-01-03 08:51:05.000000 pkglts-6.6.0/test/regenerate.no
+-rw-rw-rw-   0        0        0     3421 2020-04-15 05:45:06.000000 pkglts-6.6.0/test/test_config_management.py
+-rw-rw-rw-   0        0        0     4791 2019-10-29 06:16:57.000000 pkglts-6.6.0/test/test_dependency.py
+-rw-rw-rw-   0        0        0      340 2019-10-29 06:16:57.000000 pkglts-6.6.0/test/test_file_management.py
+-rw-rw-rw-   0        0        0     1956 2019-10-29 22:35:37.000000 pkglts-6.6.0/test/test_hash_management.py
+-rw-rw-rw-   0        0        0      731 2019-10-29 22:35:37.000000 pkglts-6.6.0/test/test_local.py
+-rw-rw-rw-   0        0        0      315 2018-02-15 07:33:01.000000 pkglts-6.6.0/test/test_manage.py
+-rw-rw-rw-   0        0        0     3051 2019-10-29 22:35:37.000000 pkglts-6.6.0/test/test_manage_cfg.py
+-rw-rw-rw-   0        0        0     1787 2019-10-29 22:35:37.000000 pkglts-6.6.0/test/test_manage_clean.py
+-rw-rw-rw-   0        0        0     2774 2019-10-29 22:35:37.000000 pkglts-6.6.0/test/test_manage_example.py
+-rw-rw-rw-   0        0        0     4454 2020-02-06 18:02:24.000000 pkglts-6.6.0/test/test_manage_regenerate.py
+-rw-rw-rw-   0        0        0     1848 2020-10-22 13:45:14.000000 pkglts-6.6.0/test/test_manage_reset.py
+-rw-rw-rw-   0        0        0      299 2019-10-29 06:16:57.000000 pkglts-6.6.0/test/test_manage_tools_check_option_parameters.py
+-rw-rw-rw-   0        0        0     5217 2019-10-29 22:35:37.000000 pkglts-6.6.0/test/test_manage_tools_regenerate.py
+-rw-rw-rw-   0        0        0     2126 2020-02-06 18:02:24.000000 pkglts-6.6.0/test/test_manage_tools_update_option.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.095706 pkglts-6.6.0/test/test_option/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.107750 pkglts-6.6.0/test/test_option/test_appveyor/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_appveyor/__init__.py
+-rw-rw-rw-   0        0        0      714 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_appveyor/test_config.py
+-rw-rw-rw-   0        0        0      318 2018-02-15 07:33:01.000000 pkglts-6.6.0/test/test_option/test_appveyor/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.115727 pkglts-6.6.0/test/test_option/test_base/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_base/__init__.py
+-rw-rw-rw-   0        0        0     1338 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_base/test_config.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.127715 pkglts-6.6.0/test/test_option/test_conda/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_conda/__init__.py
+-rw-rw-rw-   0        0        0     1074 2023-01-19 13:13:37.000000 pkglts-6.6.0/test/test_option/test_conda/test_config.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.139787 pkglts-6.6.0/test/test_option/test_coverage/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_coverage/__init__.py
+-rw-rw-rw-   0        0        0      620 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_coverage/test_config.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.159707 pkglts-6.6.0/test/test_option/test_coveralls/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_coveralls/__init__.py
+-rw-rw-rw-   0        0        0      458 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_coveralls/test_config.py
+-rw-rw-rw-   0        0        0      304 2018-02-15 07:33:01.000000 pkglts-6.6.0/test/test_option/test_coveralls/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.167840 pkglts-6.6.0/test/test_option/test_data/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_data/__init__.py
+-rw-rw-rw-   0        0        0      547 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_data/test_config.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.181880 pkglts-6.6.0/test/test_option/test_doc/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_doc/__init__.py
+-rw-rw-rw-   0        0        0     1431 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_doc/test_config.py
+-rw-rw-rw-   0        0        0      481 2019-10-29 06:16:57.000000 pkglts-6.6.0/test/test_option/test_doc/test_fmt_badge.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.196070 pkglts-6.6.0/test/test_option/test_flake8/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_flake8/__init__.py
+-rw-rw-rw-   0        0        0      446 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_flake8/test_config.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.212068 pkglts-6.6.0/test/test_option/test_git/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_git/__init__.py
+-rw-rw-rw-   0        0        0      646 2022-03-25 13:56:41.000000 pkglts-6.6.0/test/test_option/test_git/test_config.py
+-rw-rw-rw-   0        0        0      673 2020-02-06 18:02:24.000000 pkglts-6.6.0/test/test_option/test_git/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.220069 pkglts-6.6.0/test/test_option/test_github/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_github/__init__.py
+-rw-rw-rw-   0        0        0      718 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_github/test_config.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.232070 pkglts-6.6.0/test/test_option/test_gitlab/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_gitlab/__init__.py
+-rw-rw-rw-   0        0        0      732 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_gitlab/test_config.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.248186 pkglts-6.6.0/test/test_option/test_landscape/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_landscape/__init__.py
+-rw-rw-rw-   0        0        0      458 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_landscape/test_config.py
+-rw-rw-rw-   0        0        0      304 2018-02-15 07:33:01.000000 pkglts-6.6.0/test/test_option/test_landscape/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.262225 pkglts-6.6.0/test/test_option/test_lgtm/
+-rw-rw-rw-   0        0        0        0 2019-10-30 07:39:24.000000 pkglts-6.6.0/test/test_option/test_lgtm/__init__.py
+-rw-rw-rw-   0        0        0      438 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_lgtm/test_config.py
+-rw-rw-rw-   0        0        0      294 2019-10-30 07:39:24.000000 pkglts-6.6.0/test/test_option/test_lgtm/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.276368 pkglts-6.6.0/test/test_option/test_license/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_license/__init__.py
+-rw-rw-rw-   0        0        0      950 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_license/test_config.py
+-rw-rw-rw-   0        0        0      590 2017-07-15 20:09:55.000000 pkglts-6.6.0/test/test_option/test_license/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.280353 pkglts-6.6.0/test/test_option/test_notebook/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_notebook/__init__.py
+-rw-rw-rw-   0        0        0     1063 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_notebook/test_config.py
+-rw-rw-rw-   0        0        0     2059 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_option_common.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.296354 pkglts-6.6.0/test/test_option/test_plugin_project/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_plugin_project/__init__.py
+-rw-rw-rw-   0        0        0     1002 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_plugin_project/test_config.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.308380 pkglts-6.6.0/test/test_option/test_pypi/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_pypi/__init__.py
+-rw-rw-rw-   0        0        0      692 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_pypi/test_config.py
+-rw-rw-rw-   0        0        0     1139 2023-03-13 18:21:24.000000 pkglts-6.6.0/test/test_option/test_pypi/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.328485 pkglts-6.6.0/test/test_option/test_pysetup/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_pysetup/__init__.py
+-rw-rw-rw-   0        0        0      730 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_pysetup/test_config.py
+-rw-rw-rw-   0        0        0     2418 2023-04-17 13:15:22.000000 pkglts-6.6.0/test/test_option/test_pysetup/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.346512 pkglts-6.6.0/test/test_option/test_readthedocs/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_readthedocs/__init__.py
+-rw-rw-rw-   0        0        0      744 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_readthedocs/test_config.py
+-rw-rw-rw-   0        0        0      235 2018-02-15 07:33:01.000000 pkglts-6.6.0/test/test_option/test_readthedocs/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.366516 pkglts-6.6.0/test/test_option/test_reqs/
+-rw-rw-rw-   0        0        0        0 2019-10-29 06:16:57.000000 pkglts-6.6.0/test/test_option/test_reqs/__init__.py
+-rw-rw-rw-   0        0        0     2231 2021-12-09 14:39:11.000000 pkglts-6.6.0/test/test_option/test_reqs/test_config.py
+-rw-rw-rw-   0        0        0     1849 2019-10-29 22:35:37.000000 pkglts-6.6.0/test/test_option/test_reqs/test_find_requirements.py
+-rw-rw-rw-   0        0        0      529 2019-10-29 22:35:37.000000 pkglts-6.6.0/test/test_option/test_reqs/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.378517 pkglts-6.6.0/test/test_option/test_requires/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_requires/__init__.py
+-rw-rw-rw-   0        0        0      454 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_requires/test_config.py
+-rw-rw-rw-   0        0        0      302 2018-02-15 07:33:01.000000 pkglts-6.6.0/test/test_option/test_requires/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.386512 pkglts-6.6.0/test/test_option/test_sphinx/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_sphinx/__init__.py
+-rw-rw-rw-   0        0        0     1197 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_sphinx/test_config.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.400742 pkglts-6.6.0/test/test_option/test_src/
+-rw-rw-rw-   0        0        0        0 2019-10-29 06:16:57.000000 pkglts-6.6.0/test/test_option/test_src/__init__.py
+-rw-rw-rw-   0        0        0      690 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_src/test_config.py
+-rw-rw-rw-   0        0        0      284 2019-10-29 06:16:57.000000 pkglts-6.6.0/test/test_option/test_src/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.412737 pkglts-6.6.0/test/test_option/test_test/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_test/__init__.py
+-rw-rw-rw-   0        0        0      842 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_test/test_config.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.424727 pkglts-6.6.0/test/test_option/test_tox/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_tox/__init__.py
+-rw-rw-rw-   0        0        0      434 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_tox/test_config.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.448724 pkglts-6.6.0/test/test_option/test_travis/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_travis/__init__.py
+-rw-rw-rw-   0        0        0      446 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_travis/test_config.py
+-rw-rw-rw-   0        0        0      298 2018-02-15 07:33:01.000000 pkglts-6.6.0/test/test_option/test_travis/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:16:04.470903 pkglts-6.6.0/test/test_option/test_version/
+-rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-6.6.0/test/test_option/test_version/__init__.py
+-rw-rw-rw-   0        0        0     1335 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_option/test_version/test_config.py
+-rw-rw-rw-   0        0        0      527 2020-02-06 18:02:24.000000 pkglts-6.6.0/test/test_option/test_version/test_handlers.py
+-rw-rw-rw-   0        0        0     2527 2020-02-06 18:02:24.000000 pkglts-6.6.0/test/test_option_tools.py
+-rw-rw-rw-   0        0        0     2694 2018-06-09 22:55:54.000000 pkglts-6.6.0/test/test_templating.py
+-rw-rw-rw-   0        0        0     2110 2021-07-07 13:18:45.000000 pkglts-6.6.0/test/test_version_management.py
```

### Comparing `pkglts-6.5.0/CONTRIBUTING.rst` & `pkglts-6.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/LICENSE` & `pkglts-6.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/PKG-INFO` & `pkglts-6.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkglts
-Version: 6.5.0
+Version: 6.6.0
 Summary: Building packages with long term support
 Home-page: https://github.com/revesansparole/pkglts
 Author: revesansparole
 Author-email: revesansparole@gmail.com
 License: CeCILL-C
 Keywords: packaging,package builder
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pkglts-6.5.0/README.rst` & `pkglts-6.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/Makefile` & `pkglts-6.6.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/_notebook/example.rst` & `pkglts-6.6.0/doc/_notebook/example.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/conf.py` & `pkglts-6.6.0/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,17 +75,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "6.5.0"
+version = "6.6.0"
 # The full version, including alpha/beta/rc tags.
-release = "6.5.0"
+release = "6.6.0"
 
 
 exclude_patterns = ['build', 'dist']
 
 pygments_style = 'sphinx'
 
 # -- Options for HTML output -------------------------------------------
```

### Comparing `pkglts-6.5.0/doc/installation.rst` & `pkglts-6.6.0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/make.bat` & `pkglts-6.6.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/base/main.rst` & `pkglts-6.6.0/doc/option/base/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/conda/main.rst` & `pkglts-6.6.0/doc/option/conda/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/coverage/main.rst` & `pkglts-6.6.0/doc/option/coverage/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/coveralls/coveralls_tutorial.rst` & `pkglts-6.6.0/doc/option/coveralls/coveralls_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/coveralls/main.rst` & `pkglts-6.6.0/doc/option/coveralls/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/data/data_tutorial.rst` & `pkglts-6.6.0/doc/option/data/data_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/doc/history.rst` & `pkglts-6.6.0/doc/option/doc/history.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/doc/main.rst` & `pkglts-6.6.0/doc/option/doc/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/github/github_tutorial.rst` & `pkglts-6.6.0/doc/option/github/github_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/gitlab/gitlab_tutorial.rst` & `pkglts-6.6.0/doc/option/gitlab/gitlab_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/landscape/landscape_tutorial.rst` & `pkglts-6.6.0/doc/option/landscape/landscape_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/landscape/main.rst` & `pkglts-6.6.0/doc/option/landscape/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/lgtm/main.rst` & `pkglts-6.6.0/doc/option/lgtm/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/license/license_list.rst` & `pkglts-6.6.0/doc/option/license/license_list.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/license/main.rst` & `pkglts-6.6.0/doc/option/license/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/notebook/main.rst` & `pkglts-6.6.0/doc/option/notebook/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/notebook/nbcompile.rst` & `pkglts-6.6.0/doc/option/notebook/nbcompile.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/plugin/main.rst` & `pkglts-6.6.0/doc/option/plugin/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/plugin_project/main.rst` & `pkglts-6.6.0/doc/option/plugin_project/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/pypi/pypi_tutorial.rst` & `pkglts-6.6.0/doc/option/pypi/pypi_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/pysetup/main.rst` & `pkglts-6.6.0/doc/option/pysetup/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/readthedocs/main.rst` & `pkglts-6.6.0/doc/option/readthedocs/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/readthedocs/readthedocs_tutorial.rst` & `pkglts-6.6.0/doc/option/readthedocs/readthedocs_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/requires/main.rst` & `pkglts-6.6.0/doc/option/requires/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/requires/requires_tutorial.rst` & `pkglts-6.6.0/doc/option/requires/requires_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/sphinx/main.rst` & `pkglts-6.6.0/doc/option/sphinx/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/test/main.rst` & `pkglts-6.6.0/doc/option/test/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/tox/main.rst` & `pkglts-6.6.0/doc/option/tox/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/travis/main.rst` & `pkglts-6.6.0/doc/option/travis/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/travis/travis_tutorial.rst` & `pkglts-6.6.0/doc/option/travis/travis_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option/version/main.rst` & `pkglts-6.6.0/doc/option/version/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/option_list.rst` & `pkglts-6.6.0/doc/option_list.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/readme.rst` & `pkglts-6.6.0/doc/readme.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/tutorial/dvlpt_env.rst` & `pkglts-6.6.0/doc/tutorial/dvlpt_env.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/tutorial/pypi.rst` & `pkglts-6.6.0/doc/tutorial/pypi.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/tutorial/web_tools.rst` & `pkglts-6.6.0/doc/tutorial/web_tools.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/tutorials.rst` & `pkglts-6.6.0/doc/tutorials.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/doc/usage.rst` & `pkglts-6.6.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/setup.py` & `pkglts-6.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         if pth.suffix in ['', '.bat', '.cfg', '.json', '.md', '.in', '.ini', '.png', '.ps1', '.rst', '.sh', '.tpl', '.txt', '.yaml', '.yml']:
             data_files.append(str(pth.relative_to(src_dir)))
 
 pkg_data = {'pkglts': data_files}
 
 setup_kwds = dict(
     name='pkglts',
-    version="6.5.0",
+    version="6.6.0",
     description=short_descr,
     long_description=readme + '\n\n' + history,
     author="revesansparole",
     author_email="revesansparole@gmail.com",
     url='https://github.com/revesansparole/pkglts',
     license='CeCILL-C',
     zip_safe=False,
```

### Comparing `pkglts-6.5.0/src/pkglts/config_management.py` & `pkglts-6.6.0/src/pkglts/config_management.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/dependency.py` & `pkglts-6.6.0/src/pkglts/dependency.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/hash_management.py` & `pkglts-6.6.0/src/pkglts/hash_management.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/local.py` & `pkglts-6.6.0/src/pkglts/local.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/logging_tools.py` & `pkglts-6.6.0/src/pkglts/logging_tools.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/manage.py` & `pkglts-6.6.0/src/pkglts/manage.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/manage_script.py` & `pkglts-6.6.0/src/pkglts/manage_script.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/manage_tools.py` & `pkglts-6.6.0/src/pkglts/manage_tools.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/appveyor/option.py` & `pkglts-6.6.0/src/pkglts/option/requires/option.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,30 @@
+import logging
 from pathlib import Path
 
 from pkglts.option.doc import fmt_badge
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
 
-class OptionAppveyor(Option):
+
+class OptionRequires(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
-    def update_parameters(self, cfg):
-        sec = dict(
-            token=""
-        )
-        cfg[self._name] = sec
-
     def require_option(self, cfg):
-        return ['doc', 'pysetup', 'github']
+        return ['doc', 'github']
 
     def environment_extensions(self, cfg):
         owner = cfg['github']['owner']
-        project = cfg['github']['project'].replace("_", "-")
-        token = cfg[self._name]['token']
+        project = cfg['github']['project']
 
-        url = f"ci.appveyor.com/project/{owner}/{project}/branch/master"
-        img = f"ci.appveyor.com/api/projects/status/{token}/branch/master?svg=true"
-        badge = fmt_badge(img, url, "Appveyor build status", cfg['doc']['fmt'])
+        base_url = f"requires.io/github/{owner}/{project}/"
+        url = f"{base_url}requirements/?branch=master"
+        img = f"{base_url}requirements.svg?branch=master"
+        badge = fmt_badge(img, url, "Requirements status", cfg['doc']['fmt'])
 
         return {"badge": badge}
```

### Comparing `pkglts-6.5.0/src/pkglts/option/appveyor/resource/appveyor.yml` & `pkglts-6.6.0/src/pkglts/option/appveyor/resource/appveyor.yml`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     - CONDA: "C:\\Miniconda3-x64\\Scripts"
 
 install:
   - "%CONDA%\\conda config --set always_yes yes --set changeps1 no"
   # useful for debugging any issues with conda
   - "%CONDA%\\conda info -a"
   # create environment
-  - "%CONDA%\\conda create -n ci python"
+  - "%CONDA%\\conda create -n ci python={{ pysetup.py_max_ver }}"
   - "%CONDA%\\activate ci"
 
 build: false
 
 build_script:
   # install dependencies
   {% if reqs.conda_reqs(['install', 'test', 'doc', 'dvlpt']) != "" -%}
@@ -29,9 +29,9 @@
   {% if reqs.pip_reqs(['install', 'test', 'doc', 'dvlpt']) != "" -%}
   - {{ reqs.pip_reqs(['install', 'test', 'doc', 'dvlpt']) }}
   {%- endif %}
 
   # install package
   - pip install .
   # test
-  - pytest --cov={{ base.pkg_full_name }}
+  - pytest
 # #}
```

### Comparing `pkglts-6.5.0/src/pkglts/option/base/option.py` & `pkglts-6.6.0/src/pkglts/option/base/option.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import logging
 from pathlib import Path
 
 from pkglts.local import pkg_full_name
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionBase(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         sec = dict(
             pkgname=Path.cwd().name,
             namespace=None,
             url=None,
             authors=[("moi", "moi@email.com")]
         )
         cfg[self._name] = sec
```

### Comparing `pkglts-6.5.0/src/pkglts/option/conda/option.py` & `pkglts-6.6.0/src/pkglts/option/conda/option.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import logging
 from pathlib import Path
 
 from pkglts.option.reqs.option import requirements
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionConda(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         sec = dict(
             env_name="{{ base.pkgname }}",
         )
         cfg[self._name] = sec
 
     def check(self, cfg):
         invalids = []
```

### Comparing `pkglts-6.5.0/src/pkglts/option/conda/resource/conda/meta.yaml` & `pkglts-6.6.0/src/pkglts/option/conda/resource/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/conda/resource/conda/requirements.yml` & `pkglts-6.6.0/src/pkglts/option/conda/resource/conda/requirements.yml`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/conda/resource/conda/requirements_minimal.yml` & `pkglts-6.6.0/src/pkglts/option/conda/resource/conda/requirements_minimal.yml`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/coverage/option.py` & `pkglts-6.6.0/src/pkglts/option/coverage/option.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import logging
 from pathlib import Path
 
 from pkglts.dependency import Dependency
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionCoverage(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
```

### Comparing `pkglts-6.5.0/src/pkglts/option/coveralls/option.py` & `pkglts-6.6.0/src/pkglts/option/coveralls/option.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import logging
 from pathlib import Path
 
 from pkglts.dependency import Dependency
 from pkglts.option.doc import fmt_badge
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionCoveralls(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
```

### Comparing `pkglts-6.5.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.png` & `pkglts-6.6.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.png`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.png` & `pkglts-6.6.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.png`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.png` & `pkglts-6.6.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.png`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.png` & `pkglts-6.6.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.png`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/data/example/test/{% if data.use_ext_dir %}test_data{% else %}_{% endif %}.py.tpl` & `pkglts-6.6.0/src/pkglts/option/data/example/test/{% if data.use_ext_dir %}test_data{% else %}_{% endif %}.py.tpl`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/data/resource/src/{{ base.pkgname }}/{% if data.use_ext_dir %}data_access{% else %}_{% endif %}.py.tpl` & `pkglts-6.6.0/src/pkglts/option/data/resource/src/{{ base.pkgname }}/{% if data.use_ext_dir %}data_access{% else %}_{% endif %}.py.tpl`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/doc/__init__.py` & `pkglts-6.6.0/src/pkglts/option/doc/__init__.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/doc/history.py` & `pkglts-6.6.0/src/pkglts/option/doc/history.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/doc/option.py` & `pkglts-6.6.0/src/pkglts/option/doc/option.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+import logging
 from pathlib import Path
 
 from pkglts.dependency import Dependency
 from pkglts.option_object import Option
 from pkglts.option_tools import available_options
 from pkglts.version import __version__
-
 from . import history
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionDoc(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         sec = dict(
             description="belle petite description",
             fmt="rst",
             keywords=[]
         )
         cfg[self._name] = sec
```

### Comparing `pkglts-6.5.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}CONTRIBUTING{% else %}_{% endif %}.md` & `pkglts-6.6.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}CONTRIBUTING{% else %}_{% endif %}.md`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}CONTRIBUTING{% else %}_{% endif %}.rst` & `pkglts-6.6.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}CONTRIBUTING{% else %}_{% endif %}.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/git/option.py` & `pkglts-6.6.0/src/pkglts/option/git/option.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import logging
 import re
 import subprocess
 from pathlib import Path
 
+from unidecode import unidecode
+
 from pkglts.option_object import Option
 from pkglts.version import __version__
-from unidecode import unidecode
 
 LOGGER = logging.getLogger(__name__)
 
 
 class OptionGit(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         sec = dict(
             permanent_branches=[],
         )
         cfg[self._name] = sec
 
     def require_option(self, cfg):
         return ['base']
```

### Comparing `pkglts-6.5.0/src/pkglts/option/git/resource/.gitignore` & `pkglts-6.6.0/src/pkglts/option/git/resource/.gitignore`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/github/option.py` & `pkglts-6.6.0/src/pkglts/option/data/option.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,26 @@
+import logging
 from pathlib import Path
 
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
 
-class OptionGithub(Option):
+
+class OptionData(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         sec = dict(
-            owner="{{ base.authors[0][0] }}",
-            project="{{ base.pkgname }}",
-            url="https://github.com/{{ github.owner }}/{{ github.project }}"
+            filetype=[".json", ".ini"],
+            use_ext_dir=False
         )
         cfg[self._name] = sec
 
-    def check(self, cfg):
-        invalids = []
-        project = cfg[self._name]['project']
-
-        if not project:
-            invalids.append('github.project')
-
-        return invalids
-
     def require_option(self, cfg):
-        return ['git']
+        return ['src']
```

### Comparing `pkglts-6.5.0/src/pkglts/option/gitlab/option.py` & `pkglts-6.6.0/src/pkglts/option/github/option.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,36 @@
+import logging
 from pathlib import Path
 
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
 
-class OptionGitlab(Option):
+
+class OptionGithub(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         sec = dict(
             owner="{{ base.authors[0][0] }}",
             project="{{ base.pkgname }}",
-            server="framagit.org",
-            url="https://{{ gitlab.server }}/{{ gitlab.owner }}/{{ gitlab.project }}"
+            url="https://github.com/{{ github.owner }}/{{ github.project }}"
         )
         cfg[self._name] = sec
 
     def check(self, cfg):
         invalids = []
         project = cfg[self._name]['project']
 
         if not project:
-            invalids.append('gitlab.project')
+            invalids.append('github.project')
 
         return invalids
 
     def require_option(self, cfg):
         return ['git']
```

### Comparing `pkglts-6.5.0/src/pkglts/option/landscape/option.py` & `pkglts-6.6.0/src/pkglts/option/landscape/option.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import logging
 from pathlib import Path
 
 from pkglts.option.doc import fmt_badge
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionLandscape(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
```

### Comparing `pkglts-6.5.0/src/pkglts/option/lgtm/option.py` & `pkglts-6.6.0/src/pkglts/option/lgtm/option.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import logging
 from pathlib import Path
 
 from pkglts.option.doc import fmt_badge
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionLgtm(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
```

### Comparing `pkglts-6.5.0/src/pkglts/option/license/option.py` & `pkglts-6.6.0/src/pkglts/option/license/option.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         sec = dict(
             name="cecill-c",
             year=datetime.now().year,
             organization="organization",
             project="{{ base.pkgname }}"
         )
         cfg[self._name] = sec
```

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/agpl3-header.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/agpl3-header.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/agpl3.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/agpl3.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/apache-header.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/apache-header.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/apache.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/apache.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/bsd2.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/bsd2.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/bsd3.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/bsd3.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/cc0.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/cc0.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/cc_by.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/cc_by.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/cc_by_nc.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/cc_by_nc.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/cc_by_nc_nd.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/cc_by_nc_nd.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/cc_by_nc_sa.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/cc_by_nc_sa.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/cc_by_nd.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/cc_by_nd.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/cc_by_sa.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/cc_by_sa.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/cddl.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/cddl.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/cecill-c-header.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/cecill-c-header.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/cecill-c.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/cecill-c.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/epl.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/epl.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/gpl2.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/gpl2.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/gpl3-header.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/gpl3-header.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/gpl3.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/gpl3.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/inra_license_agreement.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/inra_license_agreement.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/isc.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/isc.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/lgpl.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/lgpl.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/mit.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/mit.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/mpl.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/mpl.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/private.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/private.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/unlicense.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/unlicense.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/wtfpl.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/wtfpl.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/x11.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/x11.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/license/templates/zlib.txt` & `pkglts-6.6.0/src/pkglts/option/license/templates/zlib.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/notebook/example/{{ notebook.src_directory }}/example.ipynb` & `pkglts-6.6.0/src/pkglts/option/notebook/example/{{ notebook.src_directory }}/example.ipynb`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/notebook/nbcompile.py` & `pkglts-6.6.0/src/pkglts/option/notebook/nbcompile.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/notebook/option.py` & `pkglts-6.6.0/src/pkglts/option/notebook/option.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import logging
 from pathlib import Path
 
 from pkglts.option_object import Option
 from pkglts.version import __version__
-
 from . import nbcompile
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionNotebook(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         sec = dict(
             src_directory="example"
         )
         cfg[self._name] = sec
 
     def check(self, cfg):
         invalids = []
```

### Comparing `pkglts-6.5.0/src/pkglts/option/plugin_project/option.py` & `pkglts-6.6.0/src/pkglts/option/plugin_project/option.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import logging
 from pathlib import Path
 
 from pkglts.dependency import Dependency
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionPluginProject(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         cfg[self._name] = {
             "plugin_name": "{{ base.pkgname }}"
         }
 
     def check(self, cfg):
         invalids = []
         plugin_name = cfg[self._name]['plugin_name']
```

### Comparing `pkglts-6.5.0/src/pkglts/option/plugin_project/resource/src/{{ base.pkgname }}/option.py.tpl` & `pkglts-6.6.0/src/pkglts/option/plugin_project/resource/src/{{ base.pkgname }}/option.py.tpl`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/pypi/option.py` & `pkglts-6.6.0/src/pkglts/option/pypi/option.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+import logging
 from pathlib import Path
 
 from pkglts.dependency import Dependency
 from pkglts.local import pkg_full_name
 from pkglts.option.doc import fmt_badge
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionPypi(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         sec = dict(
             classifiers=[
                 "Development Status :: 2 - Pre-Alpha",
                 "Intended Audience :: Developers",
                 "License :: OSI Approved :: BSD License",
                 "Natural Language :: English"
             ],
```

### Comparing `pkglts-6.5.0/src/pkglts/option/pysetup/option.py` & `pkglts-6.6.0/src/pkglts/option/pysetup/option.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import logging
 from pathlib import Path
 
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionPysetup(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         sec = dict(
             intended_versions=["3.10"],
         )
         cfg[self._name] = sec
 
     def check(self, cfg):
         invalids = []
@@ -26,21 +30,22 @@
 
         return invalids
 
     def require_option(self, cfg):
         return ['src', 'doc', 'license', 'version', 'reqs']
 
     def environment_extensions(self, cfg):
-        py_min_ver = sorted([int(v) for v in ver.split(".")] for ver in cfg[self._name]['intended_versions'])[0]
+        py_vers = sorted([int(v) for v in ver.split(".")] for ver in cfg[self._name]['intended_versions'])
 
         universal = len(set(ver.split(".")[0] for ver in cfg[self._name]['intended_versions'])) > 1
 
         return {
             "pkg_url": pkg_url(cfg),
-            "py_min_ver": ".".join(str(v) for v in py_min_ver),
+            "py_max_ver": ".".join(str(v) for v in py_vers[-1]),
+            "py_min_ver": ".".join(str(v) for v in py_vers[0]),
             "universal": universal
         }
 
 
 def pkg_url(cfg):
     """Extract a valid url from all config sections.
```

### Comparing `pkglts-6.5.0/src/pkglts/option/pysetup/resource/MANIFEST.in` & `pkglts-6.6.0/src/pkglts/option/pysetup/resource/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/pysetup/resource/setup.py.tpl` & `pkglts-6.6.0/src/pkglts/option/pysetup/resource/setup.py.tpl`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/readthedocs/option.py` & `pkglts-6.6.0/src/pkglts/option/readthedocs/option.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import logging
 from pathlib import Path
 
 from pkglts.option.doc import fmt_badge
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionReadthedocs(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         if 'gitlab' in cfg:
             prj_name = "{{ gitlab.project }}"
         elif 'github' in cfg:
             prj_name = "{{ github.project }}"
         else:
             raise NotImplementedError("not supposed to happen")
```

### Comparing `pkglts-6.5.0/src/pkglts/option/reqs/find_requirements.py` & `pkglts-6.6.0/src/pkglts/option/reqs/find_requirements.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/reqs/option.py` & `pkglts-6.6.0/src/pkglts/option/reqs/option.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+import logging
 from pathlib import Path
 
 from pkglts.dependency import Dependency
 from pkglts.option_object import Option
 from pkglts.option_tools import available_options
 from pkglts.version import __version__
-
 from . import find_requirements
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionReqs(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         sec = dict(
             require=[]
         )
         cfg[self._name] = sec
 
     def check(self, cfg):
         invalids = []
```

### Comparing `pkglts-6.5.0/src/pkglts/option/reqs/stdpkgs.txt` & `pkglts-6.6.0/src/pkglts/option/reqs/stdpkgs.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/requires/option.py` & `pkglts-6.6.0/src/pkglts/option/gitlab/option.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,37 @@
+import logging
 from pathlib import Path
 
-from pkglts.option.doc import fmt_badge
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
 
-class OptionRequires(Option):
+
+class OptionGitlab(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
-    def require_option(self, cfg):
-        return ['doc', 'github']
+    def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
+        sec = dict(
+            owner="{{ base.authors[0][0] }}",
+            project="{{ base.pkgname }}",
+            server="framagit.org",
+            url="https://{{ gitlab.server }}/{{ gitlab.owner }}/{{ gitlab.project }}"
+        )
+        cfg[self._name] = sec
+
+    def check(self, cfg):
+        invalids = []
+        project = cfg[self._name]['project']
 
-    def environment_extensions(self, cfg):
-        owner = cfg['github']['owner']
-        project = cfg['github']['project']
-
-        base_url = f"requires.io/github/{owner}/{project}/"
-        url = f"{base_url}requirements/?branch=master"
-        img = f"{base_url}requirements.svg?branch=master"
-        badge = fmt_badge(img, url, "Requirements status", cfg['doc']['fmt'])
+        if not project:
+            invalids.append('gitlab.project')
 
-        return {"badge": badge}
+        return invalids
+
+    def require_option(self, cfg):
+        return ['git']
```

### Comparing `pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/inheritance.rst` & `pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/inheritance.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/intersphinx.rst` & `pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/intersphinx.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/sphinx/example/doc/docexamples/matplotlib.rst` & `pkglts-6.6.0/src/pkglts/option/sphinx/example/doc/docexamples/matplotlib.rst`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_doc.py.tpl` & `pkglts-6.6.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_doc.py.tpl`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/sphinx/option.py` & `pkglts-6.6.0/src/pkglts/option/sphinx/option.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+import logging
 from pathlib import Path
 
 from pkglts.dependency import Dependency
 from pkglts.option_object import Option
 from pkglts.small_tools import is_pathname_valid
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionSphinx(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         sec = dict(
             theme="default",
             autodoc_dvlpt=True,
             build_dir="build/sphinx",
             doc_dir="doc",
             gallery="",
         )
```

### Comparing `pkglts-6.5.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/Makefile` & `pkglts-6.6.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/Makefile`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/conf.py.tpl` & `pkglts-6.6.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/conf.py.tpl`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/make.bat` & `pkglts-6.6.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/make.bat`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/test/example/test/test_example.py.tpl` & `pkglts-6.6.0/src/pkglts/option/test/example/test/test_example.py.tpl`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/test/option.py` & `pkglts-6.6.0/src/pkglts/option/test/option.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import logging
 from pathlib import Path
 
 from pkglts.dependency import Dependency
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionTest(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         sec = dict(
             suite_name="pytest",
         )
         cfg[self._name] = sec
 
     def check(self, cfg):
         invalids = []
```

### Comparing `pkglts-6.5.0/src/pkglts/option/test/resource/test/{% if test.suite_name == 'pytest' %}conftest{% else %}_{% endif %}.py.tpl` & `pkglts-6.6.0/src/pkglts/option/test/resource/test/{% if test.suite_name == 'pytest' %}conftest{% else %}_{% endif %}.py.tpl`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    {%- if 'coverage' is available %}
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov={{ base.pkg_full_name }}")
-    {%- else %}
-    pass
-    {%- endif %}
+# def pytest_cmdline_preparse(args):
+#     {%- if 'coverage' is available %}
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov={{ base.pkg_full_name }}")
+#     {%- else %}
+#     pass
+#     {%- endif %}
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

### Comparing `pkglts-6.5.0/src/pkglts/option/tox/resource/tox.ini` & `pkglts-6.6.0/src/pkglts/option/tox/resource/tox.ini`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/travis/option.py` & `pkglts-6.6.0/src/pkglts/option/travis/option.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import logging
 from pathlib import Path
 
 from pkglts.option.doc import fmt_badge
 from pkglts.option_object import Option
 from pkglts.version import __version__
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionTravis(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
```

### Comparing `pkglts-6.5.0/src/pkglts/option/travis/resource/.travis.yml` & `pkglts-6.6.0/src/pkglts/option/travis/resource/.travis.yml`

 * *Files 10% similar despite different names*

```diff
@@ -50,20 +50,16 @@
 
 script:
 # {# pkglts, travis.script
   {% if 'test' is available -%}
   {%- if test.suite_name == 'nose' -%}
   - nosetests
   {%- elif test.suite_name == 'pytest' -%}
-  {%- if 'coverage' is available -%}
-  - pytest --cov={{ base.pkg_full_name }}
-  {%- else -%}
   - pytest
   {%- endif -%}
-  {%- endif -%}
   {%- endif %}
 # #}
 
 after_success:
 # {# pkglts, travis.after
   {% if 'coveralls' is available -%}
   - coveralls
```

### Comparing `pkglts-6.5.0/src/pkglts/option/version/bump_version.py` & `pkglts-6.6.0/src/pkglts/option/version/bump_version.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option/version/option.py` & `pkglts-6.6.0/src/pkglts/option/version/option.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import logging
 from pathlib import Path
 
 from pkglts.option_object import Option
 from pkglts.version import __version__
-
 from . import bump_version
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OptionVersion(Option):
     def version(self):
         return __version__
 
     def root_dir(self):
         return Path(__file__).parent
 
     def update_parameters(self, cfg):
+        LOGGER.info("update parameters %s", self._name)
         sec = dict(
             major=0,
             minor=0,
             post=1,
         )
         cfg[self._name] = sec
```

### Comparing `pkglts-6.5.0/src/pkglts/option_object.py` & `pkglts-6.6.0/src/pkglts/option_object.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/option_tools.py` & `pkglts-6.6.0/src/pkglts/option_tools.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/small_tools.py` & `pkglts-6.6.0/src/pkglts/small_tools.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/templating.py` & `pkglts-6.6.0/src/pkglts/templating.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/tree_ascii_fmt.py` & `pkglts-6.6.0/src/pkglts/tree_ascii_fmt.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts/version_management.py` & `pkglts-6.6.0/src/pkglts/version_management.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts.egg-info/PKG-INFO` & `pkglts-6.6.0/src/pkglts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkglts
-Version: 6.5.0
+Version: 6.6.0
 Summary: Building packages with long term support
 Home-page: https://github.com/revesansparole/pkglts
 Author: revesansparole
 Author-email: revesansparole@gmail.com
 License: CeCILL-C
 Keywords: packaging,package builder
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pkglts-6.5.0/src/pkglts.egg-info/SOURCES.txt` & `pkglts-6.6.0/src/pkglts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/src/pkglts.egg-info/entry_points.txt` & `pkglts-6.6.0/src/pkglts.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/conftest.py` & `pkglts-6.6.0/test/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=pkglts")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=pkglts")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

### Comparing `pkglts-6.5.0/test/test_config_management.py` & `pkglts-6.6.0/test/test_config_management.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_dependency.py` & `pkglts-6.6.0/test/test_dependency.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_hash_management.py` & `pkglts-6.6.0/test/test_hash_management.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_local.py` & `pkglts-6.6.0/test/test_local.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_manage_cfg.py` & `pkglts-6.6.0/test/test_manage_cfg.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_manage_clean.py` & `pkglts-6.6.0/test/test_manage_clean.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_manage_example.py` & `pkglts-6.6.0/test/test_manage_example.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_manage_regenerate.py` & `pkglts-6.6.0/test/test_manage_regenerate.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_manage_reset.py` & `pkglts-6.6.0/test/test_manage_reset.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_manage_tools_regenerate.py` & `pkglts-6.6.0/test/test_manage_tools_regenerate.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_manage_tools_update_option.py` & `pkglts-6.6.0/test/test_manage_tools_update_option.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_appveyor/test_config.py` & `pkglts-6.6.0/test/test_option/test_appveyor/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_base/test_config.py` & `pkglts-6.6.0/test/test_option/test_base/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_conda/test_config.py` & `pkglts-6.6.0/test/test_option/test_conda/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_coverage/test_config.py` & `pkglts-6.6.0/test/test_option/test_coverage/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_data/test_config.py` & `pkglts-6.6.0/test/test_option/test_data/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_doc/test_config.py` & `pkglts-6.6.0/test/test_option/test_doc/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_git/test_config.py` & `pkglts-6.6.0/test/test_option/test_git/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_git/test_handlers.py` & `pkglts-6.6.0/test/test_option/test_git/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_github/test_config.py` & `pkglts-6.6.0/test/test_option/test_github/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_gitlab/test_config.py` & `pkglts-6.6.0/test/test_option/test_gitlab/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_license/test_config.py` & `pkglts-6.6.0/test/test_option/test_license/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_license/test_handlers.py` & `pkglts-6.6.0/test/test_option/test_license/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_notebook/test_config.py` & `pkglts-6.6.0/test/test_option/test_notebook/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_option_common.py` & `pkglts-6.6.0/test/test_option/test_option_common.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_plugin_project/test_config.py` & `pkglts-6.6.0/test/test_option/test_plugin_project/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_pypi/test_config.py` & `pkglts-6.6.0/test/test_option/test_pypi/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_pypi/test_handlers.py` & `pkglts-6.6.0/test/test_option/test_pypi/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_pysetup/test_config.py` & `pkglts-6.6.0/test/test_option/test_pysetup/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_pysetup/test_handlers.py` & `pkglts-6.6.0/test/test_option/test_pysetup/test_handlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,14 +22,32 @@
         loc_cfg = deepcopy(tpl_cfg)
         loc_cfg[name]['url'] = name
         cfg = Config(loc_cfg)
         cfg.load_extra()
         assert cfg._env.globals['pysetup'].pkg_url == name
 
 
+def test_py_max_ver_uses_max_intended_version():
+    cfg = Config(dict(pysetup={"intended_versions": ["2.7"]}))
+    cfg.load_extra()
+    assert cfg._env.globals['pysetup'].py_max_ver == "2.7"
+
+    cfg = Config(dict(pysetup={"intended_versions": ["2.7", "3.6"]}))
+    cfg.load_extra()
+    assert cfg._env.globals['pysetup'].py_max_ver == "3.6"
+
+    cfg = Config(dict(pysetup={"intended_versions": ["3.7", "3.6"]}))
+    cfg.load_extra()
+    assert cfg._env.globals['pysetup'].py_max_ver == "3.7"
+
+    cfg = Config(dict(pysetup={"intended_versions": ["3.10", "3.9"]}))
+    cfg.load_extra()
+    assert cfg._env.globals['pysetup'].py_max_ver == "3.10"
+
+
 def test_py_min_ver_uses_min_intended_version():
     cfg = Config(dict(pysetup={"intended_versions": ["2.7"]}))
     cfg.load_extra()
     assert cfg._env.globals['pysetup'].py_min_ver == "2.7"
 
     cfg = Config(dict(pysetup={"intended_versions": ["2.7", "3.6"]}))
     cfg.load_extra()
```

### Comparing `pkglts-6.5.0/test/test_option/test_readthedocs/test_config.py` & `pkglts-6.6.0/test/test_option/test_readthedocs/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_reqs/test_config.py` & `pkglts-6.6.0/test/test_option/test_reqs/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_reqs/test_find_requirements.py` & `pkglts-6.6.0/test/test_option/test_reqs/test_find_requirements.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_reqs/test_handlers.py` & `pkglts-6.6.0/test/test_option/test_reqs/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_sphinx/test_config.py` & `pkglts-6.6.0/test/test_option/test_sphinx/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_src/test_config.py` & `pkglts-6.6.0/test/test_option/test_src/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_test/test_config.py` & `pkglts-6.6.0/test/test_option/test_test/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_version/test_config.py` & `pkglts-6.6.0/test/test_option/test_version/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option/test_version/test_handlers.py` & `pkglts-6.6.0/test/test_option/test_version/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_option_tools.py` & `pkglts-6.6.0/test/test_option_tools.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_templating.py` & `pkglts-6.6.0/test/test_templating.py`

 * *Files identical despite different names*

### Comparing `pkglts-6.5.0/test/test_version_management.py` & `pkglts-6.6.0/test/test_version_management.py`

 * *Files identical despite different names*

