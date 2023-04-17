# Comparing `tmp/nbproject-0.8.4.tar.gz` & `tmp/nbproject-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbproject-0.8.4.tar", last modified: Mon Apr 10 18:53:31 2023, max compression
+gzip compressed data, was "nbproject-0.8.5.tar", last modified: Mon Apr 17 13:01:13 2023, max compression
```

## Comparing `nbproject-0.8.4.tar` & `nbproject-0.8.5.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     2571 2023-02-08 13:39:58.283208 nbproject-0.8.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      135 2022-06-23 16:31:28.344875 nbproject-0.8.4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      622 2022-06-23 16:31:28.344875 nbproject-0.8.4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     2018 2022-07-10 09:55:57.247165 nbproject-0.8.4/.gitignore
--rw-r--r--   0        0        0     1704 2022-08-29 09:37:35.667895 nbproject-0.8.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      766 2022-10-30 08:56:16.956519 nbproject-0.8.4/CITATION.cff
--rw-r--r--   0        0        0    11558 2022-06-23 16:31:28.364832 nbproject-0.8.4/LICENSE
--rw-r--r--   0        0        0      656 2022-10-30 08:56:16.972155 nbproject-0.8.4/README.md
--rw-r--r--   0        0        0       56 2022-06-23 16:31:28.376708 nbproject-0.8.4/docs/api.md
--rw-r--r--   0        0        0    19632 2023-04-10 18:52:58.083315 nbproject-0.8.4/docs/changelog.md
--rw-r--r--   0        0        0     1962 2022-11-14 08:41:14.596281 nbproject-0.8.4/docs/faq/example-after-init-set-filename.ipynb
--rw-r--r--   0        0        0     1568 2022-10-22 11:48:44.237635 nbproject-0.8.4/docs/faq/example-project-uninitialized/2022-07-13-my-task-x.ipynb
--rw-r--r--   0        0        0      133 2022-09-06 12:59:34.191307 nbproject-0.8.4/docs/faq/example-project-uninitialized/index.md
--rw-r--r--   0        0        0     1971 2022-11-14 08:41:14.611876 nbproject-0.8.4/docs/faq/example-project/2022-05-13-my-task-x.ipynb
--rw-r--r--   0        0        0     1756 2022-11-14 08:41:14.611876 nbproject-0.8.4/docs/faq/example-project/2022-07-18-my-task-y.ipynb
--rw-r--r--   0        0        0      111 2022-09-06 12:59:34.206452 nbproject-0.8.4/docs/faq/example-project/index.md
--rw-r--r--   0        0        0      381 2022-11-14 08:41:14.627499 nbproject-0.8.4/docs/faq/example-project/nbproject_metadata.yml
--rw-r--r--   0        0        0     1964 2022-11-14 08:41:14.627499 nbproject-0.8.4/docs/faq/header-author-field.ipynb
--rw-r--r--   0        0        0     1603 2022-11-14 08:41:14.643126 nbproject-0.8.4/docs/faq/inconsistent-packages-parents-no-store.ipynb
--rw-r--r--   0        0        0     2462 2022-11-14 08:41:14.643126 nbproject-0.8.4/docs/faq/inconsistent-packages-parents-store.ipynb
--rw-r--r--   0        0        0     1145 2022-10-10 13:46:37.108668 nbproject-0.8.4/docs/faq/index.md
--rw-r--r--   0        0        0     1384 2022-10-22 11:48:44.284507 nbproject-0.8.4/docs/faq/initialize-set-env.ipynb
--rw-r--r--   0        0        0     2122 2022-10-22 11:48:44.284507 nbproject-0.8.4/docs/faq/initialize.ipynb
--rw-r--r--   0        0        0     4294 2022-11-14 08:41:14.665256 nbproject-0.8.4/docs/faq/internal-functions.ipynb
--rw-r--r--   0        0        0     2843 2022-10-22 11:48:44.300131 nbproject-0.8.4/docs/faq/not-initialized.ipynb
--rw-r--r--   0        0        0     1893 2022-11-14 08:41:14.665256 nbproject-0.8.4/docs/faq/publish-not-last-cell.ipynb
--rw-r--r--   0        0        0     1470 2022-11-14 08:41:14.680891 nbproject-0.8.4/docs/faq/publish-set-version.ipynb
--rw-r--r--   0        0        0     1903 2022-11-14 08:41:14.680891 nbproject-0.8.4/docs/faq/publish-without-saving.ipynb
--rw-r--r--   0        0        0     1874 2022-11-14 08:41:14.696516 nbproject-0.8.4/docs/faq/publish-without-title.ipynb
--rw-r--r--   0        0        0     1732 2022-11-14 08:41:14.696516 nbproject-0.8.4/docs/faq/publish-wrapper.ipynb
--rw-r--r--   0        0        0     1660 2022-10-22 11:48:44.337899 nbproject-0.8.4/docs/faq/set-env-via-environment-var.ipynb
--rw-r--r--   0        0        0      710 2022-10-10 13:46:37.118666 nbproject-0.8.4/docs/faq/setup.md
--rw-r--r--   0        0        0     1425 2022-10-22 11:48:44.337899 nbproject-0.8.4/docs/faq/trigger-exit-upon-init.ipynb
--rw-r--r--   0        0        0     2787 2022-11-14 08:41:14.712141 nbproject-0.8.4/docs/guide/basic-metadata.ipynb
--rw-r--r--   0        0        0     2758 2022-09-06 12:59:34.286056 nbproject-0.8.4/docs/guide/cli.md
--rw-r--r--   0        0        0      356 2022-09-06 12:59:34.296244 nbproject-0.8.4/docs/guide/index.md
--rw-r--r--   0        0        0     4864 2023-04-10 17:14:17.109831 nbproject-0.8.4/docs/guide/meta.ipynb
--rw-r--r--   0        0        0     1721 2022-11-14 08:41:14.727766 nbproject-0.8.4/docs/guide/received.ipynb
--rw-r--r--   0        0        0     3107 2022-11-14 08:41:14.743391 nbproject-0.8.4/docs/guide/update-metadata.ipynb
--rw-r--r--   0        0        0     1218 2022-12-08 16:23:43.566826 nbproject-0.8.4/docs/index.md
--rw-r--r--   0        0        0     2877 2022-11-14 08:41:14.743391 nbproject-0.8.4/docs/quickstart.ipynb
--rw-r--r--   0        0        0      142 2022-06-23 16:31:28.434840 nbproject-0.8.4/lamin-project.yaml
--rw-r--r--   0        0        0      658 2023-04-10 18:52:59.031553 nbproject-0.8.4/nbproject/__init__.py
--rw-r--r--   0        0        0     1686 2022-08-07 09:27:50.928574 nbproject-0.8.4/nbproject/__main__.py
--rw-r--r--   0        0        0     5293 2022-11-14 08:41:14.765536 nbproject-0.8.4/nbproject/_cli.py
--rw-r--r--   0        0        0     5880 2023-04-10 17:14:17.125543 nbproject-0.8.4/nbproject/_header.py
--rw-r--r--   0        0        0      291 2022-11-14 08:41:14.781172 nbproject-0.8.4/nbproject/_is_run_from_ipython.py
--rw-r--r--   0        0        0       49 2022-07-23 16:04:31.881411 nbproject-0.8.4/nbproject/_logger.py
--rw-r--r--   0        0        0     3181 2022-10-10 13:46:37.136666 nbproject-0.8.4/nbproject/_meta.py
--rw-r--r--   0        0        0     4055 2022-11-14 08:41:14.781172 nbproject-0.8.4/nbproject/_publish.py
--rw-r--r--   0        0        0     4137 2022-11-14 08:41:14.796798 nbproject-0.8.4/nbproject/_schemas.py
--rw-r--r--   0        0        0      979 2022-09-30 15:22:07.715496 nbproject-0.8.4/nbproject/dev/__init__.py
--rw-r--r--   0        0        0      611 2022-09-30 15:44:26.199043 nbproject-0.8.4/nbproject/dev/_check_last_cell.py
--rw-r--r--   0        0        0      708 2023-02-18 10:37:08.724548 nbproject-0.8.4/nbproject/dev/_classic_nb_commands.py
--rw-r--r--   0        0        0     1522 2022-08-28 12:58:31.551377 nbproject-0.8.4/nbproject/dev/_consecutiveness.py
--rw-r--r--   0        0        0      545 2022-08-16 17:29:41.764018 nbproject-0.8.4/nbproject/dev/_frontend_commands.py
--rw-r--r--   0        0        0     1745 2023-04-09 15:55:22.348445 nbproject-0.8.4/nbproject/dev/_initialize.py
--rw-r--r--   0        0        0     5751 2023-02-18 10:37:08.740183 nbproject-0.8.4/nbproject/dev/_jupyter_communicate.py
--rw-r--r--   0        0        0      867 2022-11-14 08:55:56.709932 nbproject-0.8.4/nbproject/dev/_jupyter_lab_commands.py
--rw-r--r--   0        0        0      355 2023-02-18 10:37:17.396767 nbproject-0.8.4/nbproject/dev/_lamin_communicate.py
--rw-r--r--   0        0        0     3757 2022-10-12 08:12:35.746640 nbproject-0.8.4/nbproject/dev/_meta_live.py
--rw-r--r--   0        0        0     4685 2022-11-14 08:41:14.812422 nbproject-0.8.4/nbproject/dev/_meta_store.py
--rw-r--r--   0        0        0     5562 2022-11-14 08:41:14.828046 nbproject-0.8.4/nbproject/dev/_metadata_display.py
--rw-r--r--   0        0        0      961 2022-07-15 19:42:53.037973 nbproject-0.8.4/nbproject/dev/_notebook.py
--rw-r--r--   0        0        0     4042 2022-07-23 14:58:07.898575 nbproject-0.8.4/nbproject/dev/_pypackage.py
--rw-r--r--   0        0        0      599 2022-11-14 08:41:14.828046 nbproject-0.8.4/nbproject/dev/_set_version.py
--rw-r--r--   0        0        0      736 2022-07-17 18:42:44.854639 nbproject-0.8.4/noxfile.py
--rw-r--r--   0        0        0     1195 2022-09-06 12:59:34.336281 nbproject-0.8.4/pyproject.toml
--rw-r--r--   0        0        0      949 2022-09-06 12:59:34.346054 nbproject-0.8.4/tests/conftest.py
--rw-r--r--   0        0        0     2506 2022-09-06 12:59:34.356032 nbproject-0.8.4/tests/test_cli.py
--rw-r--r--   0        0        0     1530 2023-02-10 14:17:38.727097 nbproject-0.8.4/tests/test_jupyter.py
--rw-r--r--   0        0        0      334 2022-08-29 09:37:35.723898 nbproject-0.8.4/tests/test_notebooks.py
--rw-r--r--   0        0        0      312 2022-11-14 08:41:14.843671 nbproject-0.8.4/tests/test_set_version.py
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 nbproject-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     2574 2023-04-17 07:11:01.411035 nbproject-0.8.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-06-10 19:50:58.313927 nbproject-0.8.5/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-06-10 19:50:58.314964 nbproject-0.8.5/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1880 2022-07-10 12:10:29.382368 nbproject-0.8.5/.gitignore
+-rw-r--r--   0        0        0     1645 2022-08-29 09:33:05.135542 nbproject-0.8.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      740 2022-10-24 12:29:45.346974 nbproject-0.8.5/CITATION.cff
+-rw-r--r--   0        0        0    11357 2022-04-18 20:46:44.681265 nbproject-0.8.5/LICENSE
+-rw-r--r--   0        0        0     1404 2023-04-17 07:11:01.411511 nbproject-0.8.5/README.md
+-rw-r--r--   0        0        0    19810 2023-04-17 13:00:39.473943 nbproject-0.8.5/docs/changelog.md
+-rw-r--r--   0        0        0     1874 2022-11-12 18:33:53.213819 nbproject-0.8.5/docs/faq/example-after-init-set-filename.ipynb
+-rw-r--r--   0        0        0     1481 2022-10-07 21:00:12.845099 nbproject-0.8.5/docs/faq/example-project-uninitialized/2022-07-13-my-task-x.ipynb
+-rw-r--r--   0        0        0      123 2022-09-06 11:40:41.171382 nbproject-0.8.5/docs/faq/example-project-uninitialized/index.md
+-rw-r--r--   0        0        0     1874 2022-11-12 18:33:53.214012 nbproject-0.8.5/docs/faq/example-project/2022-05-13-my-task-x.ipynb
+-rw-r--r--   0        0        0     1661 2022-11-12 18:33:53.214173 nbproject-0.8.5/docs/faq/example-project/2022-07-18-my-task-y.ipynb
+-rw-r--r--   0        0        0      101 2022-09-06 11:40:41.171829 nbproject-0.8.5/docs/faq/example-project/index.md
+-rw-r--r--   0        0        0      364 2022-11-12 18:33:53.214429 nbproject-0.8.5/docs/faq/example-project/nbproject_metadata.yml
+-rw-r--r--   0        0        0     1873 2022-11-12 18:33:53.214599 nbproject-0.8.5/docs/faq/header-author-field.ipynb
+-rw-r--r--   0        0        0     1520 2022-11-12 18:33:53.214757 nbproject-0.8.5/docs/faq/inconsistent-packages-parents-no-store.ipynb
+-rw-r--r--   0        0        0     2330 2022-11-12 18:33:53.214908 nbproject-0.8.5/docs/faq/inconsistent-packages-parents-store.ipynb
+-rw-r--r--   0        0        0     1096 2022-10-10 12:03:49.454347 nbproject-0.8.5/docs/faq/index.md
+-rw-r--r--   0        0        0     1311 2022-09-06 11:40:41.172354 nbproject-0.8.5/docs/faq/initialize-set-env.ipynb
+-rw-r--r--   0        0        0     2049 2022-09-06 11:40:41.172505 nbproject-0.8.5/docs/faq/initialize.ipynb
+-rw-r--r--   0        0        0     4086 2022-11-12 18:33:53.215053 nbproject-0.8.5/docs/faq/internal-functions.ipynb
+-rw-r--r--   0        0        0     2708 2022-09-06 11:40:41.172679 nbproject-0.8.5/docs/faq/not-initialized.ipynb
+-rw-r--r--   0        0        0     1803 2022-11-12 18:33:53.215192 nbproject-0.8.5/docs/faq/publish-not-last-cell.ipynb
+-rw-r--r--   0        0        0     1399 2022-11-12 18:33:53.215339 nbproject-0.8.5/docs/faq/publish-set-version.ipynb
+-rw-r--r--   0        0        0     1818 2022-11-12 18:33:53.215489 nbproject-0.8.5/docs/faq/publish-without-saving.ipynb
+-rw-r--r--   0        0        0     1787 2022-11-12 18:33:53.215632 nbproject-0.8.5/docs/faq/publish-without-title.ipynb
+-rw-r--r--   0        0        0     1653 2022-11-12 18:33:53.215765 nbproject-0.8.5/docs/faq/publish-wrapper.ipynb
+-rw-r--r--   0        0        0     1577 2022-10-07 21:00:16.804143 nbproject-0.8.5/docs/faq/set-env-via-environment-var.ipynb
+-rw-r--r--   0        0        0      679 2022-10-10 14:54:28.366976 nbproject-0.8.5/docs/faq/setup.md
+-rw-r--r--   0        0        0     1357 2022-09-06 11:40:41.173529 nbproject-0.8.5/docs/faq/trigger-exit-upon-init.ipynb
+-rw-r--r--   0        0        0     2694 2022-11-12 18:33:53.215926 nbproject-0.8.5/docs/guide/basic-metadata.ipynb
+-rw-r--r--   0        0        0     2675 2022-09-06 11:40:41.173736 nbproject-0.8.5/docs/guide/cli.md
+-rw-r--r--   0        0        0      328 2022-09-06 11:40:41.173880 nbproject-0.8.5/docs/guide/index.md
+-rw-r--r--   0        0        0     4639 2023-04-17 07:11:01.412769 nbproject-0.8.5/docs/guide/meta.ipynb
+-rw-r--r--   0        0        0     1637 2022-11-12 18:33:53.216221 nbproject-0.8.5/docs/guide/received.ipynb
+-rw-r--r--   0        0        0     2964 2022-11-12 18:33:53.216369 nbproject-0.8.5/docs/guide/update-metadata.ipynb
+-rw-r--r--   0        0        0      142 2023-04-17 07:11:01.413339 nbproject-0.8.5/docs/index.md
+-rw-r--r--   0        0        0     2755 2022-11-12 18:33:53.216521 nbproject-0.8.5/docs/quickstart.ipynb
+-rw-r--r--   0        0        0       57 2023-04-17 07:11:01.413670 nbproject-0.8.5/docs/reference.md
+-rw-r--r--   0        0        0      137 2022-06-01 14:27:38.468097 nbproject-0.8.5/lamin-project.yaml
+-rw-r--r--   0        0        0      658 2023-04-17 12:59:28.739410 nbproject-0.8.5/nbproject/__init__.py
+-rw-r--r--   0        0        0     1631 2022-08-17 11:48:35.494040 nbproject-0.8.5/nbproject/__main__.py
+-rw-r--r--   0        0        0     5121 2022-11-12 18:33:53.216715 nbproject-0.8.5/nbproject/_cli.py
+-rw-r--r--   0        0        0     5720 2023-04-17 07:11:01.414277 nbproject-0.8.5/nbproject/_header.py
+-rw-r--r--   0        0        0      285 2022-11-13 23:00:04.437788 nbproject-0.8.5/nbproject/_is_run_from_ipython.py
+-rw-r--r--   0        0        0       48 2022-07-23 18:45:14.093130 nbproject-0.8.5/nbproject/_logger.py
+-rw-r--r--   0        0        0     3080 2022-10-10 12:03:49.455892 nbproject-0.8.5/nbproject/_meta.py
+-rw-r--r--   0        0        0     3943 2022-11-12 18:52:44.680900 nbproject-0.8.5/nbproject/_publish.py
+-rw-r--r--   0        0        0     4007 2022-11-12 18:33:53.217134 nbproject-0.8.5/nbproject/_schemas.py
+-rw-r--r--   0        0        0      924 2022-09-26 22:11:29.434198 nbproject-0.8.5/nbproject/dev/__init__.py
+-rw-r--r--   0        0        0      590 2022-10-07 21:00:16.805272 nbproject-0.8.5/nbproject/dev/_check_last_cell.py
+-rw-r--r--   0        0        0      681 2022-08-17 11:48:35.496655 nbproject-0.8.5/nbproject/dev/_classic_nb_commands.py
+-rw-r--r--   0        0        0     1471 2022-08-27 06:14:49.459673 nbproject-0.8.5/nbproject/dev/_consecutiveness.py
+-rw-r--r--   0        0        0      525 2022-08-17 11:48:35.496751 nbproject-0.8.5/nbproject/dev/_frontend_commands.py
+-rw-r--r--   0        0        0     1693 2022-10-10 18:44:26.046062 nbproject-0.8.5/nbproject/dev/_initialize.py
+-rw-r--r--   0        0        0     5136 2023-04-17 12:58:56.403151 nbproject-0.8.5/nbproject/dev/_jupyter_communicate.py
+-rw-r--r--   0        0        0      822 2023-04-17 07:11:01.415333 nbproject-0.8.5/nbproject/dev/_jupyter_lab_commands.py
+-rw-r--r--   0        0        0      343 2023-04-17 07:11:01.415771 nbproject-0.8.5/nbproject/dev/_lamin_communicate.py
+-rw-r--r--   0        0        0     3642 2022-10-10 18:44:26.046429 nbproject-0.8.5/nbproject/dev/_meta_live.py
+-rw-r--r--   0        0        0     4541 2022-11-12 18:33:53.217570 nbproject-0.8.5/nbproject/dev/_meta_store.py
+-rw-r--r--   0        0        0     5385 2022-11-12 18:33:53.217735 nbproject-0.8.5/nbproject/dev/_metadata_display.py
+-rw-r--r--   0        0        0      922 2022-07-15 19:53:53.061564 nbproject-0.8.5/nbproject/dev/_notebook.py
+-rw-r--r--   0        0        0     3900 2022-07-23 14:31:43.204220 nbproject-0.8.5/nbproject/dev/_pypackage.py
+-rw-r--r--   0        0        0      575 2022-11-12 18:52:44.681103 nbproject-0.8.5/nbproject/dev/_set_version.py
+-rw-r--r--   0        0        0      575 2023-04-17 07:11:01.416205 nbproject-0.8.5/noxfile.py
+-rw-r--r--   0        0        0     1091 2023-04-17 07:11:01.416607 nbproject-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0      920 2022-09-06 11:40:41.175303 nbproject-0.8.5/tests/conftest.py
+-rw-r--r--   0        0        0     2428 2022-09-06 11:40:41.175526 nbproject-0.8.5/tests/test_cli.py
+-rw-r--r--   0        0        0     1472 2023-04-17 07:11:01.416978 nbproject-0.8.5/tests/test_jupyter.py
+-rw-r--r--   0        0        0      322 2022-08-29 09:33:05.137063 nbproject-0.8.5/tests/test_notebooks.py
+-rw-r--r--   0        0        0      303 2022-11-12 18:52:44.681259 nbproject-0.8.5/tests/test_set_version.py
+-rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 nbproject-0.8.5/PKG-INFO
```

### Comparing `nbproject-0.8.4/.gitignore` & `nbproject-0.8.5/.gitignore`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-.DS_Store
-
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-pip-wheel-metadata/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-.python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# Lamin
-_build
-docs/nbproject.*
-lamin_sphinx
-docs/conf.py
-_docs_tmp*
+.DS_Store
+
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+pip-wheel-metadata/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+.python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# Lamin
+_build
+docs/nbproject.*
+lamin_sphinx
+docs/conf.py
+_docs_tmp*
```

### Comparing `nbproject-0.8.4/CITATION.cff` & `nbproject-0.8.5/CITATION.cff`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-cff-version: 1.2.0
-title: "nbproject: Manage Jupyter notebooks"
-authors:
-- family-names: Rybakov
-  given-names: Sergei
-  orcid: https://orcid.org/0000-0002-4944-6586
-- family-names: Wolf
-  given-names: Alex
-  orcid: https://orcid.org/0000-0002-8760-7838
-url: https://github.com/laminlabs/nbproject
-preferred-citation:
-  type: article
-  title: "nbproject: Manage Jupyter notebooks"
-  authors:
-  - family-names: Rybakov
-    given-names: Sergei
-    orcid: https://orcid.org/0000-0002-4944-6586
-  - family-names: Heumos
-    given-names: Lukas
-    orcid: https://orcid.org/0000-0002-8937-3457
-  - family-names: Wolf
-    given-names: Alex
-    orcid: https://orcid.org/0000-0002-8760-7838
-  doi: 10.56528/nbp
-  journal: Lamin Reports
-  year: 2022
+cff-version: 1.2.0
+title: "nbproject: Manage Jupyter notebooks"
+authors:
+- family-names: Rybakov
+  given-names: Sergei
+  orcid: https://orcid.org/0000-0002-4944-6586
+- family-names: Wolf
+  given-names: Alex
+  orcid: https://orcid.org/0000-0002-8760-7838
+url: https://github.com/laminlabs/nbproject
+preferred-citation:
+  type: article
+  title: "nbproject: Manage Jupyter notebooks"
+  authors:
+  - family-names: Rybakov
+    given-names: Sergei
+    orcid: https://orcid.org/0000-0002-4944-6586
+  - family-names: Heumos
+    given-names: Lukas
+    orcid: https://orcid.org/0000-0002-8937-3457
+  - family-names: Wolf
+    given-names: Alex
+    orcid: https://orcid.org/0000-0002-8760-7838
+  doi: 10.56528/nbp
+  journal: Lamin Reports
+  year: 2022
```

### Comparing `nbproject-0.8.4/LICENSE` & `nbproject-0.8.5/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `nbproject-0.8.4/docs/changelog.md` & `nbproject-0.8.5/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-♻️ Replace display with metadata_only option in header | [257](https://github.com/laminlabs/nbproject/pull/257) | [Koncopd](https://github.com/Koncopd) | 2023-04-10 | 0.8.4
+🐛 Fix VS Code integration for recent VS Code versions | [260](https://github.com/laminlabs/nbproject/pull/260) | [Koncopd](https://github.com/Koncopd) | 2023-04-17 | 0.8.5
+♻️ Replace `display` with `metadata_only` arg in `header` | [257](https://github.com/laminlabs/nbproject/pull/257) | [Koncopd](https://github.com/Koncopd) | 2023-04-10 | 0.8.4
 🚸 Allow to not display metadata | [255](https://github.com/laminlabs/nbproject/pull/255) | [falexwolf](https://github.com/falexwolf) | 2023-03-12 | 0.8.3
 ⬆️ Observe `lndb-setup` rename to `lndb` | [253](https://github.com/laminlabs/nbproject/pull/253) | [bpenteado](https://github.com/bpenteado) | 2023-02-16 | 0.8.2
 ✨ Safer notebook path inference and more ways to do it | [251](https://github.com/laminlabs/nbproject/pull/251) | [Koncopd](https://github.com/Koncopd) | 2023-02-10 |
 🐛 Check keys before accessing in `notebook_path` | [250](https://github.com/laminlabs/nbproject/pull/250) | [Koncopd](https://github.com/Koncopd) | 2023-02-08 |
 :zap: Do nothing with ipylab when not in ipython | [247](https://github.com/laminlabs/nbproject/pull/247) | [Koncopd](https://github.com/Koncopd) | 2022-11-14 |
 🚸 Only init `JupyterFrontEnd` if run within ipython | [246](https://github.com/laminlabs/nbproject/pull/246) | [falexwolf](https://github.com/falexwolf) | 2022-11-13 | 0.8.1
 🚸 Do no longer auto-bump `version` upon `publish()` <span class="badge badge-warning">Breaking</span> | [244](https://github.com/laminlabs/nbproject/pull/244) | [falexwolf](https://github.com/falexwolf) | 2022-11-12 | 0.8.0
```

### Comparing `nbproject-0.8.4/docs/faq/example-after-init-set-filename.ipynb` & `nbproject-0.8.5/docs/guide/update-metadata.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8716804453262786%*

 * *Differences: {"'cells'": "{0: {'id': '4c5d9cf8', 'source': ['# Update metadata']}, 1: {'id': "*

 * *            "'c0aad033-1af5-436d-a8f7-7f5aedba41a8', 'source': ['You can add additional packages "*

 * *            "to be tracked right at initialization:']}, 2: {'id': "*

 * *            "'0f734180-2bf1-4341-b068-7ab84764bf57', 'source': {insert: [(0, 'from nbproject "*

 * *            "import header, meta\\n'), (1, 'import pandas\\n'), (3, 'header(\\n'), (4, '    "*

 * *            'parent=[\\n\'), (5, \'        "z14KWQKD4bwE",\\n\'), (6, \'   […]*

```diff
@@ -1,69 +1,110 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "cc6c2fe6-6291-4a91-b326-b1ec6cb8d703",
+            "id": "4c5d9cf8",
             "metadata": {
                 "tags": []
             },
             "source": [
-                "# Manually specify a filepath upon init"
+                "# Update metadata"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "752e0baa-5e48-46c0-958d-f48796ff3b2f",
+            "id": "c0aad033-1af5-436d-a8f7-7f5aedba41a8",
             "metadata": {},
             "source": [
-                "Here we see how `nbproject` prints a metadata header for a notebook that has been initialized."
+                "You can add additional packages to be tracked right at initialization:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "705ac1d5-cbd9-421f-841e-d91e15faa962",
+            "id": "0f734180-2bf1-4341-b068-7ab84764bf57",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from nbproject import header\n",
+                "from nbproject import header, meta\n",
+                "import pandas\n",
                 "\n",
-                "header(filepath=\"example-after-init-set-filename.ipynb\")"
+                "header(\n",
+                "    parent=[\n",
+                "        \"z14KWQKD4bwE\",\n",
+                "        \"jhvyoIrxoeSz\",\n",
+                "    ],\n",
+                "    pypackage=\"nbformat\",  # Indirect dependencies to be tracked. Direct dependencies are automatically tracked.\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "bd7d72a2-8fcd-4414-b957-d233664d0fe1",
+            "metadata": {},
+            "source": [
+                "Use the following convenience function to update packages."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "ff350260",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "meta.store.add_pypackages([\"numpy\", \"pytest\"]).write()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "cbea77ad-82a9-4b8f-9081-c9bf3ccda0c3",
+            "metadata": {},
+            "source": [
+                "Update `parent` or any custom metadata field via: "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "861ede19-560c-4d7f-9b64-10728eef4ef6",
+            "id": "7b4166ad-907a-4153-9cb3-5f74a7d0e5d9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from nbproject import meta"
+                "meta.store.parent = [\n",
+                "    \"z14KWQKD4bwE\",\n",
+                "    \"jhvyoIrxoeSz\",\n",
+                "    \"3m2Q6UBuwgSH\",\n",
+                "]"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "2eb0ac87-8338-4a4c-bab1-d84e3c6748be",
+            "metadata": {},
+            "source": [
+                "Don't forget to write the changes from the store to the file!"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "170ff0fd-730e-4b6b-b932-d396fa2d82d2",
+            "id": "ea6238da",
             "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
+                "tags": []
             },
             "outputs": [],
             "source": [
-                "assert meta.store.id == \"KLqggebgs7Tq\"\n",
-                "assert hasattr(meta.store, \"time_init\")"
+                "meta.store.write()"
             ]
         }
     ],
     "metadata": {
-        "interpreter": {
-            "hash": "40d3a090f54c6569ab1632332b64b2c03c39dcf918b08424e98f38b5ae0af88f"
-        },
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
@@ -71,18 +112,32 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.9.12"
         },
         "nbproject": {
-            "id": "KLqggebgs7Tq",
-            "time_init": "2022-04-18T22:07:44.214819+00:00",
+            "id": "CfcLn8WBSlKt",
+            "parent": [
+                "z14KWQKD4bwE",
+                "jhvyoIrxoeSz"
+            ],
+            "pypackage": {
+                "nbformat": "5.4.0",
+                "nbproject": "0.1.6",
+                "pandas": "1.4.2"
+            },
+            "time_init": "2022-07-18T13:04:49.875497+00:00",
             "version": "0"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "2775e555cdc2d728c54aa22130c79afb1fa4da64f22f2fc6dcc2aa346c4e0672"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `nbproject-0.8.4/docs/faq/index.md` & `nbproject-0.8.5/docs/faq/index.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# FAQ
-
-Setup & installation guide:
-
-- {doc}`setup`
-
-Edges cases, warnings, and errors:
-
-- {doc}`initialize`
-- {doc}`initialize-set-env`
-- {doc}`inconsistent-packages-parents-store`
-- {doc}`inconsistent-packages-parents-no-store`
-- {doc}`example-project/index`
-- {doc}`example-project-uninitialized/index`
-- {doc}`example-after-init-set-filename`
-- {doc}`publish-set-version`
-- {doc}`publish-without-title`
-- {doc}`publish-without-saving`
-- {doc}`publish-not-last-cell`
-- {doc}`publish-wrapper`
-- {doc}`trigger-exit-upon-init`
-- {doc}`not-initialized`
-- {doc}`internal-functions`
-- {doc}`set-env-via-environment-var`
-- {doc}`header-author-field`
-
-```{toctree}
-:maxdepth: 1
-:hidden:
-
-setup
-initialize
-initialize-set-env
-inconsistent-packages-parents-store
-inconsistent-packages-parents-no-store
-example-project/index
-example-project-uninitialized/index
-example-after-init-set-filename
-publish-set-version
-publish-without-title
-publish-without-saving
-publish-not-last-cell
-publish-wrapper
-trigger-exit-upon-init
-not-initialized
-internal-functions
-set-env-via-environment-var
-header-author-field
-```
+# FAQ
+
+Setup & installation guide:
+
+- {doc}`setup`
+
+Edges cases, warnings, and errors:
+
+- {doc}`initialize`
+- {doc}`initialize-set-env`
+- {doc}`inconsistent-packages-parents-store`
+- {doc}`inconsistent-packages-parents-no-store`
+- {doc}`example-project/index`
+- {doc}`example-project-uninitialized/index`
+- {doc}`example-after-init-set-filename`
+- {doc}`publish-set-version`
+- {doc}`publish-without-title`
+- {doc}`publish-without-saving`
+- {doc}`publish-not-last-cell`
+- {doc}`publish-wrapper`
+- {doc}`trigger-exit-upon-init`
+- {doc}`not-initialized`
+- {doc}`internal-functions`
+- {doc}`set-env-via-environment-var`
+- {doc}`header-author-field`
+
+```{toctree}
+:maxdepth: 1
+:hidden:
+
+setup
+initialize
+initialize-set-env
+inconsistent-packages-parents-store
+inconsistent-packages-parents-no-store
+example-project/index
+example-project-uninitialized/index
+example-after-init-set-filename
+publish-set-version
+publish-without-title
+publish-without-saving
+publish-not-last-cell
+publish-wrapper
+trigger-exit-upon-init
+not-initialized
+internal-functions
+set-env-via-environment-var
+header-author-field
+```
```

### Comparing `nbproject-0.8.4/docs/faq/not-initialized.ipynb` & `nbproject-0.8.5/docs/quickstart.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7391098484848485%*

 * *Differences: {"'cells'": "{0: {'source': ['# Quickstart'], delete: ['id']}, 1: {'cell_type': 'markdown', "*

 * *            "'source': "*

 * *            "['![](https://lamin-site-assets.s3.amazonaws.com/NHq29ckKVrrTYsNdG0KjT-1.gif)'], "*

 * *            "delete: ['execution_count', 'id', 'outputs']}, 2: {'cell_type': 'markdown', 'source': "*

 * *            "['1. {func}`~nbproject.header` provides relevant context.\\n', '2. "*

 * *            "{func}`~nbproject.publish` prepares a notebook for sharing it with someone else.'], "*

 * *            "de […]*

```diff
@@ -1,117 +1,90 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "26e6045d-f4e7-45a9-b6fb-4641cc0d6f86",
             "metadata": {},
             "source": [
-                "# Access metadata of un-initialized notebook"
+                "# Quickstart"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "13774927-ff59-40c1-888a-abec89465244",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from nbproject import meta"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "cf19c0f9-8f4e-4451-8a09-e78a7da550c5",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "meta.store.id"
+                "![](https://lamin-site-assets.s3.amazonaws.com/NHq29ckKVrrTYsNdG0KjT-1.gif)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "2bfbbe72-70a7-45f1-80e4-79021b2dd761",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "meta.store.time_init"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "cdafba5c-226d-47cd-a79b-337928ab0d31",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "meta.store.version"
+                "1. {func}`~nbproject.header` provides relevant context.\n",
+                "2. {func}`~nbproject.publish` prepares a notebook for sharing it with someone else."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fbcc2e26-181d-4568-80e0-b6bf51dba86d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert meta.store.id == \"not initialized\"\n",
-                "assert meta.store.time_init == \"not initialized\"\n",
-                "assert meta.store.version == \"not initialized\""
+                "from nbproject import header, publish, meta\n",
+                "\n",
+                "header(parent=[\"z14KWQKD4bwE\", \"jhvyoIrxoeSz\"])  # Initializes & displays metadata."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "9ed861eb-874b-4409-b339-6516ff66d898",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "meta.live.time_run"
+                "```{note}\n",
+                "\n",
+                "- Passing `parent` to `header()` is optional. You can use it to point viewers to upstream notebooks or to build pipelines.\n",
+                "- You can also pass `pypackage` to `header()` to track secondary dependencies.\n",
+                "\n",
+                "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "cb466e13-b03f-4b86-8b1e-350596cd9734",
             "metadata": {},
             "outputs": [],
             "source": [
-                "meta.live.time_passed"
+                "import pandas  # Any imported package is automatically tracked."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "349d5652-f9bb-408f-b68f-e98caba0461c",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "meta.live.consecutive_cells"
+                "Once you're happy with the present version of your notebook:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4ce85093-6b5a-4616-8c23-d8b972707314",
             "metadata": {},
             "outputs": [],
             "source": [
-                "meta.live.pypackage"
+                "publish()  # Sets version, checks consecutiveness & title, writes current pypackages with versions."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "a6e24832-3103-4b0b-a808-0c23ef820525",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "meta.live.title"
+                "```{note}\n",
+                "\n",
+                "If you're a developer and want to build on top of nbproject, the API offers:\n",
+                "\n",
+                "- {class}`~nbproject.meta` to access metadata: {doc}`guide/meta`.\n",
+                "- {mod}`~nbproject.dev` for development utils.\n",
+                "```"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -124,12 +97,26 @@
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.9.12"
+        },
+        "nbproject": {
+            "id": "3m2Q6UBuwgSH",
+            "parent": [
+                "z14KWQKD4bwE",
+                "jhvyoIrxoeSz"
+            ],
+            "time_init": "2022-07-18T12:32:21.625107+00:00",
+            "version": "0"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "2775e555cdc2d728c54aa22130c79afb1fa4da64f22f2fc6dcc2aa346c4e0672"
+            }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 4
 }
```

### Comparing `nbproject-0.8.4/docs/faq/trigger-exit-upon-init.ipynb` & `nbproject-0.8.5/docs/faq/example-project-uninitialized/2022-07-13-my-task-x.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7682291666666666%*

 * *Differences: {"'cells'": "{0: {'source': ['# My task X'], 'id': '1db96b40'}, 3: {'source': ['df = "*

 * *            'pd.DataFrame({"a": [1, 2, 3], "b": [2, 3, 4]})\'], \'id\': \'b630b839\'}, 4: '*

 * *            "{'source': ['df'], 'id': '4e1eb065'}, 5: {'source': ['df.mean()'], 'id': '64a0102d'}, "*

 * *            "insert: [(1, OrderedDict([('cell_type', 'code'), ('execution_count', None), ('id', "*

 * *            "'0a17df65'), ('metadata', OrderedDict()), ('outputs', []), ('source', ['%%time\\n', "*

 * *            "'from nbproject import […]*

```diff
@@ -1,45 +1,69 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "1db96b40",
             "metadata": {},
             "source": [
-                "# Trigger SystemExit upon init in non-interactive editor"
+                "# My task X"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "0a17df65",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import pytest\n",
-                "from nbproject import header"
+                "%%time\n",
+                "from nbproject import header\n",
+                "\n",
+                "header()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "f5216382",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# header() this should be ignored"
+                "import pandas as pd\n",
+                "import pydantic"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "b630b839",
             "metadata": {},
             "outputs": [],
             "source": [
-                "with pytest.raises(SystemExit):\n",
-                "    header(\n",
-                "        parent=[\"z14KWQKD4bwE\", \"r4Dkcgt2HIfh\"], pypackage=\"anndata\"\n",
-                "    )  # header() triggers exit init"
+                "df = pd.DataFrame({\"a\": [1, 2, 3], \"b\": [2, 3, 4]})"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "4e1eb065",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "df"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "64a0102d",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "df.mean()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -52,17 +76,12 @@
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.9.12"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "2775e555cdc2d728c54aa22130c79afb1fa4da64f22f2fc6dcc2aa346c4e0672"
-            }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 5
 }
```

### Comparing `nbproject-0.8.4/docs/guide/cli.md` & `nbproject-0.8.5/docs/guide/cli.md`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-# Manage a collection of notebooks with the CLI
-
-Here we consider that you have a collection of existing notebooks that you'd like to become
-
-- more reproducible through pypackage tracking
-- more findable & integrated through project management metadata
-
-```{warning}
-This implementation is subject to change. We'll offer better & better ways of integrating databases and a distributed metadata store.
-```
-
-## Initialize nbproject
-
-Use the CLI to init `nbproject` for a collection of notebooks like this:
-
-```
-$ cd my_notebook_collection/
-$ nbproject init
-created my_notebook_collection/nbproject_metadata.yml
-```
-
-Now all notebooks contain the initial nbproject metadata fields.
-The `nbproject_metadata.yml` file shows you the metadata fields for each notebook, and serves as a metadata "database" for the project.
-
-You'll of course also see these metadata fields in each notebook, as usual, when calling:
-
-```
-from nbproject import header
-```
-
-## Synchronize changes
-
-If you have any changes in the metadata of the notebooks of your project, changes in location of a notebook within the project directory, additions of new notebooks, renamings etc., you can synchronize everything with `nbproject_metadata.yml` via
-
-```
-$ nbproject sync .
-synchronized my_notebook_collection/nbproject_metadata.yml
-```
-
-Passing `.` to `nbproject sync` synchronizes the whole root directory of you project.
-You can also pass a list of paths within you project to synchronize only specific notebooks.
-
-## Infer pypackages
-
-To automatically infer pypackages from the notebooks of your project, use the option `--deps` (or `-d`):
-
-```
-$ nbproject sync . --deps
-synchronized my_notebook_collection/nbproject_metadata.yml
-```
-
-This command parses the notebooks, infers all pypackages within the notebooks with their versions
-from the current python environment and writes them to metadata of the notebooks.
-
-## Pin pypackages
-
-If you want to avoid pining the pypackages versions, use the option `--no-versions` (or `-nv`):
-
-```
-$ nbproject sync . --deps --no-versions
-synchronized my_notebook_collection/nbproject_metadata.yml
-```
-
-## Publish a list of notebooks
-
-You can use CLI to publish a list of notebooks (see the publish tutorial also):
-
-```
-$ nbproject publish notebook.ipynb another_notebook.ipynb
-published 2 notebooks.
-```
-
-## Generate a requirements file
-
-To generate a `requirements.txt` for a list of notebooks of the project, run:
-
-```
-$ nbproject reqs .
-created my_notebook_collection/requirements.txt
-```
-
-Again, passing `.` means that `requirements.txt` is created for all notebooks of your project.
-To create the file only for specific notebooks, pass the list of their paths.
+# Manage a collection of notebooks with the CLI
+
+Here we consider that you have a collection of existing notebooks that you'd like to become
+
+- more reproducible through pypackage tracking
+- more findable & integrated through project management metadata
+
+```{warning}
+This implementation is subject to change. We'll offer better & better ways of integrating databases and a distributed metadata store.
+```
+
+## Initialize nbproject
+
+Use the CLI to init `nbproject` for a collection of notebooks like this:
+
+```
+$ cd my_notebook_collection/
+$ nbproject init
+created my_notebook_collection/nbproject_metadata.yml
+```
+
+Now all notebooks contain the initial nbproject metadata fields.
+The `nbproject_metadata.yml` file shows you the metadata fields for each notebook, and serves as a metadata "database" for the project.
+
+You'll of course also see these metadata fields in each notebook, as usual, when calling:
+
+```
+from nbproject import header
+```
+
+## Synchronize changes
+
+If you have any changes in the metadata of the notebooks of your project, changes in location of a notebook within the project directory, additions of new notebooks, renamings etc., you can synchronize everything with `nbproject_metadata.yml` via
+
+```
+$ nbproject sync .
+synchronized my_notebook_collection/nbproject_metadata.yml
+```
+
+Passing `.` to `nbproject sync` synchronizes the whole root directory of you project.
+You can also pass a list of paths within you project to synchronize only specific notebooks.
+
+## Infer pypackages
+
+To automatically infer pypackages from the notebooks of your project, use the option `--deps` (or `-d`):
+
+```
+$ nbproject sync . --deps
+synchronized my_notebook_collection/nbproject_metadata.yml
+```
+
+This command parses the notebooks, infers all pypackages within the notebooks with their versions
+from the current python environment and writes them to metadata of the notebooks.
+
+## Pin pypackages
+
+If you want to avoid pining the pypackages versions, use the option `--no-versions` (or `-nv`):
+
+```
+$ nbproject sync . --deps --no-versions
+synchronized my_notebook_collection/nbproject_metadata.yml
+```
+
+## Publish a list of notebooks
+
+You can use CLI to publish a list of notebooks (see the publish tutorial also):
+
+```
+$ nbproject publish notebook.ipynb another_notebook.ipynb
+published 2 notebooks.
+```
+
+## Generate a requirements file
+
+To generate a `requirements.txt` for a list of notebooks of the project, run:
+
+```
+$ nbproject reqs .
+created my_notebook_collection/requirements.txt
+```
+
+Again, passing `.` means that `requirements.txt` is created for all notebooks of your project.
+To create the file only for specific notebooks, pass the list of their paths.
```

### Comparing `nbproject-0.8.4/nbproject/__init__.py` & `nbproject-0.8.5/nbproject/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 .. autosummary::
    :toctree:
 
    meta
    dev
 
 """
-__version__ = "0.8.4"
+__version__ = "0.8.5"
 
 # init jupyter lab frontend immediately on import
 # nothing happens if this is not jupyter lab
 from .dev._jupyter_lab_commands import _init_frontend
 
 _init_frontend()
```

### Comparing `nbproject-0.8.4/nbproject/__main__.py` & `nbproject-0.8.5/nbproject/__main__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import argparse
-
-from ._cli import init, publish, reqs, sync
-
-
-def main():
-    parser = argparse.ArgumentParser(prog="nbproject")
-    subparsers = parser.add_subparsers(help="available commands:", dest="cmd")
-
-    parser_init = subparsers.add_parser("init", help="init the project")  # noqa: F841
-
-    parser_sync = subparsers.add_parser(
-        "sync", help="synchronize the notebooks of the project"
-    )
-    parser_sync.add_argument(
-        "files_dirs", nargs="+", help="which files and folders to synchronize"
-    )
-    parser_sync.add_argument(
-        "--deps",
-        "-d",
-        action="store_true",
-        help=(
-            "parse pypackages from the notebooks and pin versions from the current"
-            " environment"
-        ),
-    )
-    parser_sync.add_argument(
-        "--no-versions",
-        "-nv",
-        action="store_true",
-        help="do not pin the versions from the current environment",
-    )
-
-    parser_reqs = subparsers.add_parser("reqs", help="create requirments.txt")
-    parser_reqs.add_argument(
-        "files_dirs", nargs="+", help="create requirments.txt for these files"
-    )
-
-    parser_publish = subparsers.add_parser("publish", help="pubish the notebooks")
-    parser_publish.add_argument("files_dirs", nargs="+", help="publish these notebooks")
-
-    args = parser.parse_args()
-
-    if args.cmd == "init":
-        init()
-    elif args.cmd == "sync":
-        sync(args.files_dirs, args.deps, not args.no_versions)
-    elif args.cmd == "reqs":
-        reqs(args.files_dirs)
-    elif args.cmd == "publish":
-        publish(args.files_dirs)
-
-
-if __name__ == "__main__":
-    main()
+import argparse
+
+from ._cli import init, publish, reqs, sync
+
+
+def main():
+    parser = argparse.ArgumentParser(prog="nbproject")
+    subparsers = parser.add_subparsers(help="available commands:", dest="cmd")
+
+    parser_init = subparsers.add_parser("init", help="init the project")  # noqa: F841
+
+    parser_sync = subparsers.add_parser(
+        "sync", help="synchronize the notebooks of the project"
+    )
+    parser_sync.add_argument(
+        "files_dirs", nargs="+", help="which files and folders to synchronize"
+    )
+    parser_sync.add_argument(
+        "--deps",
+        "-d",
+        action="store_true",
+        help=(
+            "parse pypackages from the notebooks and pin versions from the current"
+            " environment"
+        ),
+    )
+    parser_sync.add_argument(
+        "--no-versions",
+        "-nv",
+        action="store_true",
+        help="do not pin the versions from the current environment",
+    )
+
+    parser_reqs = subparsers.add_parser("reqs", help="create requirments.txt")
+    parser_reqs.add_argument(
+        "files_dirs", nargs="+", help="create requirments.txt for these files"
+    )
+
+    parser_publish = subparsers.add_parser("publish", help="pubish the notebooks")
+    parser_publish.add_argument("files_dirs", nargs="+", help="publish these notebooks")
+
+    args = parser.parse_args()
+
+    if args.cmd == "init":
+        init()
+    elif args.cmd == "sync":
+        sync(args.files_dirs, args.deps, not args.no_versions)
+    elif args.cmd == "reqs":
+        reqs(args.files_dirs)
+    elif args.cmd == "publish":
+        publish(args.files_dirs)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `nbproject-0.8.4/nbproject/_cli.py` & `nbproject-0.8.5/nbproject/_cli.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-# This file contains the functions to process the cli commands.
-from itertools import chain
-from pathlib import Path
-from typing import Iterator, Union
-
-import yaml  # type: ignore
-
-from ._logger import logger
-from ._schemas import NBRecord, YAMLRecord
-from .dev._notebook import read_notebook, write_notebook
-from .dev._pypackage import infer_pypackages, resolve_versions
-
-
-def find_upwards(cwd: Path, filename: str):
-    if cwd == Path(cwd.anchor):
-        return None
-
-    fullpath = cwd / filename
-
-    return fullpath if fullpath.exists() else find_upwards(cwd.parent, filename)
-
-
-def notebooks_from_files_dirs(files_dirs: Iterator[Union[str, Path]]):
-    nbs = []
-
-    for file_dir in files_dirs:
-        file_dir = Path(file_dir)
-        if file_dir.is_dir():
-            nbs.append(file_dir.glob("**/*.ipynb"))
-        else:
-            if file_dir.suffix == ".ipynb":
-                nbs.append([file_dir])  # type: ignore
-            else:
-                logger.info(f"The file {file_dir} is not a notebook, ignoring.")
-
-    return chain(*nbs)
-
-
-def init():
-    cwd = Path.cwd()
-
-    yaml_filled = find_upwards(cwd, "nbproject_metadata.yml")
-    if yaml_filled is not None:
-        logger.info("You are already in the nbproject (sub)folder.")
-        logger.info(f"Yaml of the project is: {yaml_filled.as_posix()}.")
-        return
-
-    nbs = cwd.glob("**/*.ipynb")
-
-    init_yaml = {}
-
-    for nb_path in nbs:
-        if ".ipynb_checkpoints/" in nb_path.as_posix():
-            continue
-
-        nb_path = nb_path.relative_to(cwd)
-
-        nb = read_notebook(nb_path)
-
-        nbproj_record = NBRecord(nb)
-        nbproj_record.write(nb_path, overwrite=False)
-
-        yaml_record = YAMLRecord(nb_path, nbproj_record, init_yaml)
-        yaml_record.put_yaml()
-
-    new_file = "nbproject_metadata.yml"
-    with open(new_file, "w") as stream:
-        yaml.dump(init_yaml, stream, sort_keys=False)
-    logger.info(f"Created {cwd / new_file}.")
-
-
-def sync(
-    files_dirs: Iterator[str], parse_deps: bool = False, pin_versions: bool = False
-):
-    cwd = Path.cwd()
-    yaml_file = find_upwards(cwd, "nbproject_metadata.yml")
-
-    if yaml_file is None:
-        logger.info("You are not inside an nbproject folder, use init.")
-        return
-    else:
-        logger.info(f"Yaml of the project is: {yaml_file.as_posix()}.")
-
-    with open(yaml_file, "r") as stream:
-        yaml_proj = yaml.load(stream, Loader=yaml.FullLoader)
-
-    nbs = notebooks_from_files_dirs(files_dirs)
-    n_nbs = 0
-    for nb_path in nbs:
-        if ".ipynb_checkpoints/" in nb_path.as_posix():
-            continue
-        n_nbs += 1
-
-        nb = read_notebook(nb_path)
-
-        nbproj_record = NBRecord(nb)
-        yaml_record = YAMLRecord(nb_path, nbproj_record, yaml_proj)
-
-        if parse_deps:
-            deps = infer_pypackages(nb, pin_versions=pin_versions)
-            yaml_record.pypackage = deps  # type: ignore
-
-        yaml_record.put_metadata()
-        yaml_record.put_yaml()
-
-        nbproj_record.write(nb_path, overwrite=False)
-
-    with open(yaml_file, "w") as stream:
-        yaml.dump(yaml_proj, stream, sort_keys=False)
-    logger.info(f"Synced {n_nbs} notebooks.")
-
-
-def reqs(files_dirs: Iterator[str]):
-    # todo: check different versions and do some resolution for conflicting versions
-    gather_deps = []
-
-    nbs = notebooks_from_files_dirs(files_dirs)
-    for nb_path in nbs:
-        if ".ipynb_checkpoints/" in nb_path.as_posix():
-            continue
-
-        nb = read_notebook(nb_path)
-
-        if "nbproject" not in nb.metadata:
-            logger.info(
-                "Uninitialized or unsynced notebooks, use > nbproject init or >"
-                " nbproject sync ."
-            )
-            return
-        nbproj_metadata = nb.metadata["nbproject"]
-        if "pypackage" in nbproj_metadata:
-            gather_deps.append(nbproj_metadata["pypackage"])
-
-    deps = resolve_versions(gather_deps)
-    deps = [pkg + f"=={ver}" if ver != "" else pkg for pkg, ver in deps.items()]
-
-    requirments = "\n".join(deps)
-    with open("requirments.txt", "w") as stream:
-        stream.write(requirments)
-
-    logger.info("Created `requirements.txt`.")
-
-
-def publish(files_dirs: Iterator[str]):
-    nbs = notebooks_from_files_dirs(files_dirs)
-    n_nbs = 0
-    for nb_path in nbs:
-        if ".ipynb_checkpoints/" in nb_path.as_posix():
-            continue
-
-        nb = read_notebook(nb_path)
-
-        if "nbproject" in nb.metadata:
-            nbproject_meta = nb.metadata["nbproject"]
-            add_pkgs = None
-            if "pypackage" in nbproject_meta:
-                add_pkgs = nbproject_meta["pypackage"].keys()
-            nbproject_meta["pypackage"] = infer_pypackages(
-                nb, add_pkgs, pin_versions=True
-            )
-
-            version = "0"
-            if "version" in nbproject_meta:
-                version = nbproject_meta["version"]
-            version = "1" if version == "0" else str(int(version) + 1)
-            nbproject_meta["version"] = version
-
-            write_notebook(nb, nb_path)
-
-            n_nbs += 1
-
-        logger.info(f"Pubished {n_nbs} notebooks.")
+# This file contains the functions to process the cli commands.
+from itertools import chain
+from pathlib import Path
+from typing import Iterator, Union
+
+import yaml  # type: ignore
+
+from ._logger import logger
+from ._schemas import NBRecord, YAMLRecord
+from .dev._notebook import read_notebook, write_notebook
+from .dev._pypackage import infer_pypackages, resolve_versions
+
+
+def find_upwards(cwd: Path, filename: str):
+    if cwd == Path(cwd.anchor):
+        return None
+
+    fullpath = cwd / filename
+
+    return fullpath if fullpath.exists() else find_upwards(cwd.parent, filename)
+
+
+def notebooks_from_files_dirs(files_dirs: Iterator[Union[str, Path]]):
+    nbs = []
+
+    for file_dir in files_dirs:
+        file_dir = Path(file_dir)
+        if file_dir.is_dir():
+            nbs.append(file_dir.glob("**/*.ipynb"))
+        else:
+            if file_dir.suffix == ".ipynb":
+                nbs.append([file_dir])  # type: ignore
+            else:
+                logger.info(f"The file {file_dir} is not a notebook, ignoring.")
+
+    return chain(*nbs)
+
+
+def init():
+    cwd = Path.cwd()
+
+    yaml_filled = find_upwards(cwd, "nbproject_metadata.yml")
+    if yaml_filled is not None:
+        logger.info("You are already in the nbproject (sub)folder.")
+        logger.info(f"Yaml of the project is: {yaml_filled.as_posix()}.")
+        return
+
+    nbs = cwd.glob("**/*.ipynb")
+
+    init_yaml = {}
+
+    for nb_path in nbs:
+        if ".ipynb_checkpoints/" in nb_path.as_posix():
+            continue
+
+        nb_path = nb_path.relative_to(cwd)
+
+        nb = read_notebook(nb_path)
+
+        nbproj_record = NBRecord(nb)
+        nbproj_record.write(nb_path, overwrite=False)
+
+        yaml_record = YAMLRecord(nb_path, nbproj_record, init_yaml)
+        yaml_record.put_yaml()
+
+    new_file = "nbproject_metadata.yml"
+    with open(new_file, "w") as stream:
+        yaml.dump(init_yaml, stream, sort_keys=False)
+    logger.info(f"Created {cwd / new_file}.")
+
+
+def sync(
+    files_dirs: Iterator[str], parse_deps: bool = False, pin_versions: bool = False
+):
+    cwd = Path.cwd()
+    yaml_file = find_upwards(cwd, "nbproject_metadata.yml")
+
+    if yaml_file is None:
+        logger.info("You are not inside an nbproject folder, use init.")
+        return
+    else:
+        logger.info(f"Yaml of the project is: {yaml_file.as_posix()}.")
+
+    with open(yaml_file, "r") as stream:
+        yaml_proj = yaml.load(stream, Loader=yaml.FullLoader)
+
+    nbs = notebooks_from_files_dirs(files_dirs)
+    n_nbs = 0
+    for nb_path in nbs:
+        if ".ipynb_checkpoints/" in nb_path.as_posix():
+            continue
+        n_nbs += 1
+
+        nb = read_notebook(nb_path)
+
+        nbproj_record = NBRecord(nb)
+        yaml_record = YAMLRecord(nb_path, nbproj_record, yaml_proj)
+
+        if parse_deps:
+            deps = infer_pypackages(nb, pin_versions=pin_versions)
+            yaml_record.pypackage = deps  # type: ignore
+
+        yaml_record.put_metadata()
+        yaml_record.put_yaml()
+
+        nbproj_record.write(nb_path, overwrite=False)
+
+    with open(yaml_file, "w") as stream:
+        yaml.dump(yaml_proj, stream, sort_keys=False)
+    logger.info(f"Synced {n_nbs} notebooks.")
+
+
+def reqs(files_dirs: Iterator[str]):
+    # todo: check different versions and do some resolution for conflicting versions
+    gather_deps = []
+
+    nbs = notebooks_from_files_dirs(files_dirs)
+    for nb_path in nbs:
+        if ".ipynb_checkpoints/" in nb_path.as_posix():
+            continue
+
+        nb = read_notebook(nb_path)
+
+        if "nbproject" not in nb.metadata:
+            logger.info(
+                "Uninitialized or unsynced notebooks, use > nbproject init or >"
+                " nbproject sync ."
+            )
+            return
+        nbproj_metadata = nb.metadata["nbproject"]
+        if "pypackage" in nbproj_metadata:
+            gather_deps.append(nbproj_metadata["pypackage"])
+
+    deps = resolve_versions(gather_deps)
+    deps = [pkg + f"=={ver}" if ver != "" else pkg for pkg, ver in deps.items()]
+
+    requirments = "\n".join(deps)
+    with open("requirments.txt", "w") as stream:
+        stream.write(requirments)
+
+    logger.info("Created `requirements.txt`.")
+
+
+def publish(files_dirs: Iterator[str]):
+    nbs = notebooks_from_files_dirs(files_dirs)
+    n_nbs = 0
+    for nb_path in nbs:
+        if ".ipynb_checkpoints/" in nb_path.as_posix():
+            continue
+
+        nb = read_notebook(nb_path)
+
+        if "nbproject" in nb.metadata:
+            nbproject_meta = nb.metadata["nbproject"]
+            add_pkgs = None
+            if "pypackage" in nbproject_meta:
+                add_pkgs = nbproject_meta["pypackage"].keys()
+            nbproject_meta["pypackage"] = infer_pypackages(
+                nb, add_pkgs, pin_versions=True
+            )
+
+            version = "0"
+            if "version" in nbproject_meta:
+                version = nbproject_meta["version"]
+            version = "1" if version == "0" else str(int(version) + 1)
+            nbproject_meta["version"] = version
+
+            write_notebook(nb, nb_path)
+
+            n_nbs += 1
+
+        logger.info(f"Pubished {n_nbs} notebooks.")
```

### Comparing `nbproject-0.8.4/nbproject/_header.py` & `nbproject-0.8.5/nbproject/_header.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-import re
-from datetime import datetime, timezone
-from typing import List, Mapping, Optional, Tuple, Union
-
-from ._logger import logger
-from .dev._frontend_commands import _reload_notebook, _save_notebook
-from .dev._initialize import initialize_metadata
-from .dev._jupyter_communicate import notebook_path
-from .dev._metadata_display import display_html, table_metadata
-from .dev._notebook import Notebook, read_notebook, write_notebook
-
-_filepath = None
-_env = None
-_time_run = None
-
-
-msg_init_complete = (
-    "Init complete. Hit save & reload from disk, i.e, *discard* editor content. If you"
-    " do not want to lose editor changes, hit save *before* running `header()`."
-    " Consider using Jupyter Lab for a seamless interactive experience."
-)
-
-msg_inconsistent_parent = (
-    "Argument parent is inconsistent with store.\nPlease update"
-    " metadata, e.g.: meta.store.parent = parent; meta.store.write()"
-)
-
-
-def msg_inconsistent_pypackage(pypackage):
-    return (
-        "Argument pypackage is inconsistent with metadata store.\nPlease update"
-        f' metadata: meta.store.add_pypackages("{pypackage}").write()'
-    )
-
-
-def _output_table(notebook: Notebook, table: str):
-    out = {
-        "data": {
-            "text/html": [table],
-            "text/plain": ["<IPython.core.display.HTML object>"],
-        },
-        "metadata": {},
-        "output_type": "display_data",
-    }
-
-    header_re = re.compile(r"^[^#]*header\(", flags=re.MULTILINE)
-    ccount = 0
-    for cell in notebook.cells:
-        if cell["cell_type"] != "code":
-            continue
-        elif cell["execution_count"] is not None:
-            ccount = cell["execution_count"]
-
-        if header_re.match("".join(cell["source"])) is not None:
-            cell["outputs"] = [out]
-            cell["execution_count"] = ccount + 1
-            # update only once
-            break
-
-
-def header(
-    *,
-    parent: Union[str, List[str], None] = None,
-    pypackage: Union[str, List[str], None] = None,
-    filepath: Union[str, None] = None,
-    env: Union[str, None] = None,
-    metadata_only: bool = False,
-) -> Optional[Tuple[Mapping, bool]]:
-    """Display metadata and start tracking dependencies.
-
-    If the notebook has no nbproject metadata, initializes & writes metadata to disk.
-
-    Args:
-        parent: One or more nbproject ids of direct ancestors in a notebook pipeline.
-        pypackage: One or more python packages to track.
-        filepath: Filepath of notebook. Only needed if automatic inference fails.
-        env: Editor environment. Only needed if automatic inference fails.
-            Pass `'lab'` for jupyter lab and `'notebook'` for jupyter notebook,
-            this can help to identify the correct mechanism for interactivity
-            when automatic inference fails.
-        metadata_only: Whether or not to return only metadata
-            without writing or displaying anything.
-    """
-    filepath_env = filepath, env
-
-    if filepath is None:
-        filepath_env = notebook_path(return_env=True)
-        if filepath_env is None:
-            logger.info(
-                "Can't infer the name of the current notebook, "
-                "you are probably not inside a Jupyter notebook. "
-                "Please call `header(filepath='your-file.ipynb')`."
-            )
-            return None
-        filepath = filepath_env[0]
-
-    if env is None:
-        env = filepath_env[1]
-    # The following occurs when passing filepath manually
-    # We assume Jupyter Lab as an environment for now
-    if env is None:
-        env = "lab"
-        logger.info("Assuming editor is Jupyter Lab.")
-
-    try:
-        nb = read_notebook(filepath)  # type: ignore
-    except FileNotFoundError:
-        raise RuntimeError("Try passing the filepath manually to nbproject.Header().")
-
-    # make time_run available through API
-    time_run = datetime.now(timezone.utc)
-    global _time_run, _filepath, _env
-    _time_run, _filepath, _env = time_run, filepath, env
-
-    # initialize
-    if "nbproject" not in nb.metadata:
-        logger.info("Initializing.")
-
-        if env in ("lab", "notebook"):
-            _save_notebook(env)
-            nb = read_notebook(filepath)  # type: ignore
-
-        metadata = initialize_metadata(nb, parent=parent, pypackage=pypackage).dict()
-
-        if metadata_only:
-            # True here means that the metdata has been initialized now
-            return metadata, True
-        else:
-            nb.metadata["nbproject"] = metadata
-            _output_table(nb, table_metadata(metadata, nb, time_run))
-            write_notebook(nb, filepath)  # type: ignore
-
-            if env in ("lab", "notebook"):
-                _reload_notebook(env)
-            else:
-                raise SystemExit(msg_init_complete)
-
-    # read from ipynb metadata and add on-the-fly computed metadata
-    else:
-        metadata = nb.metadata["nbproject"]
-        table = table_metadata(metadata, nb, time_run)
-        if not metadata_only:
-            display_html(table)
-
-        # check whether updates to init are needed
-        if parent is not None:
-            if "parent" not in metadata or metadata["parent"] != parent:
-                logger.info(msg_inconsistent_parent)
-        if pypackage is not None:
-            pypackage = [pypackage] if isinstance(pypackage, str) else pypackage
-            is_empty = "pypackage" not in metadata or metadata["pypackage"] is None
-            for pkg in pypackage:
-                if is_empty or pkg not in metadata["pypackage"]:
-                    logger.info(msg_inconsistent_pypackage(pkg))
-
-        if metadata_only:
-            # False here means that the notebook has the metadata already
-            return metadata, False
-
-    return None
+import re
+from datetime import datetime, timezone
+from typing import List, Mapping, Optional, Tuple, Union
+
+from ._logger import logger
+from .dev._frontend_commands import _reload_notebook, _save_notebook
+from .dev._initialize import initialize_metadata
+from .dev._jupyter_communicate import notebook_path
+from .dev._metadata_display import display_html, table_metadata
+from .dev._notebook import Notebook, read_notebook, write_notebook
+
+_filepath = None
+_env = None
+_time_run = None
+
+
+msg_init_complete = (
+    "Init complete. Hit save & reload from disk, i.e, *discard* editor content. If you"
+    " do not want to lose editor changes, hit save *before* running `header()`."
+    " Consider using Jupyter Lab for a seamless interactive experience."
+)
+
+msg_inconsistent_parent = (
+    "Argument parent is inconsistent with store.\nPlease update"
+    " metadata, e.g.: meta.store.parent = parent; meta.store.write()"
+)
+
+
+def msg_inconsistent_pypackage(pypackage):
+    return (
+        "Argument pypackage is inconsistent with metadata store.\nPlease update"
+        f' metadata: meta.store.add_pypackages("{pypackage}").write()'
+    )
+
+
+def _output_table(notebook: Notebook, table: str):
+    out = {
+        "data": {
+            "text/html": [table],
+            "text/plain": ["<IPython.core.display.HTML object>"],
+        },
+        "metadata": {},
+        "output_type": "display_data",
+    }
+
+    header_re = re.compile(r"^[^#]*header\(", flags=re.MULTILINE)
+    ccount = 0
+    for cell in notebook.cells:
+        if cell["cell_type"] != "code":
+            continue
+        elif cell["execution_count"] is not None:
+            ccount = cell["execution_count"]
+
+        if header_re.match("".join(cell["source"])) is not None:
+            cell["outputs"] = [out]
+            cell["execution_count"] = ccount + 1
+            # update only once
+            break
+
+
+def header(
+    *,
+    parent: Union[str, List[str], None] = None,
+    pypackage: Union[str, List[str], None] = None,
+    filepath: Union[str, None] = None,
+    env: Union[str, None] = None,
+    metadata_only: bool = False,
+) -> Optional[Tuple[Mapping, bool]]:
+    """Display metadata and start tracking dependencies.
+
+    If the notebook has no nbproject metadata, initializes & writes metadata to disk.
+
+    Args:
+        parent: One or more nbproject ids of direct ancestors in a notebook pipeline.
+        pypackage: One or more python packages to track.
+        filepath: Filepath of notebook. Only needed if automatic inference fails.
+        env: Editor environment. Only needed if automatic inference fails.
+            Pass `'lab'` for jupyter lab and `'notebook'` for jupyter notebook,
+            this can help to identify the correct mechanism for interactivity
+            when automatic inference fails.
+        metadata_only: Whether or not to return only metadata
+            without writing or displaying anything.
+    """
+    filepath_env = filepath, env
+
+    if filepath is None:
+        filepath_env = notebook_path(return_env=True)
+        if filepath_env is None:
+            logger.info(
+                "Can't infer the name of the current notebook, "
+                "you are probably not inside a Jupyter notebook. "
+                "Please call `header(filepath='your-file.ipynb')`."
+            )
+            return None
+        filepath = filepath_env[0]
+
+    if env is None:
+        env = filepath_env[1]
+    # The following occurs when passing filepath manually
+    # We assume Jupyter Lab as an environment for now
+    if env is None:
+        env = "lab"
+        logger.info("Assuming editor is Jupyter Lab.")
+
+    try:
+        nb = read_notebook(filepath)  # type: ignore
+    except FileNotFoundError:
+        raise RuntimeError("Try passing the filepath manually to nbproject.Header().")
+
+    # make time_run available through API
+    time_run = datetime.now(timezone.utc)
+    global _time_run, _filepath, _env
+    _time_run, _filepath, _env = time_run, filepath, env
+
+    # initialize
+    if "nbproject" not in nb.metadata:
+        logger.info("Initializing.")
+
+        if env in ("lab", "notebook"):
+            _save_notebook(env)
+            nb = read_notebook(filepath)  # type: ignore
+
+        metadata = initialize_metadata(nb, parent=parent, pypackage=pypackage).dict()
+
+        if metadata_only:
+            # True here means that the metdata has been initialized now
+            return metadata, True
+        else:
+            nb.metadata["nbproject"] = metadata
+            _output_table(nb, table_metadata(metadata, nb, time_run))
+            write_notebook(nb, filepath)  # type: ignore
+
+            if env in ("lab", "notebook"):
+                _reload_notebook(env)
+            else:
+                raise SystemExit(msg_init_complete)
+
+    # read from ipynb metadata and add on-the-fly computed metadata
+    else:
+        metadata = nb.metadata["nbproject"]
+        table = table_metadata(metadata, nb, time_run)
+        if not metadata_only:
+            display_html(table)
+
+        # check whether updates to init are needed
+        if parent is not None:
+            if "parent" not in metadata or metadata["parent"] != parent:
+                logger.info(msg_inconsistent_parent)
+        if pypackage is not None:
+            pypackage = [pypackage] if isinstance(pypackage, str) else pypackage
+            is_empty = "pypackage" not in metadata or metadata["pypackage"] is None
+            for pkg in pypackage:
+                if is_empty or pkg not in metadata["pypackage"]:
+                    logger.info(msg_inconsistent_pypackage(pkg))
+
+        if metadata_only:
+            # False here means that the notebook has the metadata already
+            return metadata, False
+
+    return None
```

### Comparing `nbproject-0.8.4/nbproject/_meta.py` & `nbproject-0.8.5/nbproject/_meta.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-from pathlib import Path
-from typing import Union
-
-from .dev._jupyter_communicate import notebook_path
-from .dev._meta_live import MetaLive
-from .dev._meta_store import MetaContainer, MetaStore
-from .dev._notebook import read_notebook
-
-
-# https://stackoverflow.com/questions/128573/using-property-on-classmethods/64738850#64738850
-class classproperty(object):
-    def __init__(self, fget):
-        self.fget = fget
-
-    def __get__(self, owner_self, owner_cls):
-        return self.fget(owner_cls)
-
-
-# https://stackoverflow.com/questions/8955754/can-i-define-a-repr-for-a-class-rather-than-an-instance
-class MetaRepr(type):
-    def __repr__(cls):
-        return (
-            "Metadata object with .live and .store metadata fields:\n"
-            f"  .store: {cls.store}\n"
-            f"  .live: {cls.live}"
-        )
-
-
-class meta(metaclass=MetaRepr):
-    """Access `meta.store` and `meta.live`.
-
-    - `meta.store` - nbproject metadata of the ipynb file, see
-      :class:`~nbproject.dev.MetaStore`
-    - `meta.live` - execution info and properties derived from notebook content,
-      see :class:`~nbproject.dev.MetaLive`
-
-    `meta` is a static class and behaves like a module (no need to initialize it).
-    """
-
-    _filepath: Union[str, Path, None] = None
-    _env = None
-    _time_run = None
-
-    _store: Union[MetaStore, None] = None
-    _live: Union[MetaLive, None] = None
-
-    @classmethod
-    def _init_meta(cls):
-        from ._header import _env, _filepath, _time_run
-
-        env = _env
-        filepath = _filepath
-        filepath_env = _filepath, _env
-
-        if filepath is None:
-            filepath_env = notebook_path(return_env=True)
-            if filepath_env is None:
-                filepath_env = None, None
-            filepath = filepath_env[0]
-
-        if env is None:
-            env = filepath_env[1]
-
-        cls._filepath = filepath
-        cls._env = env
-        cls._time_run = _time_run
-
-        if cls._filepath is not None:
-            nb_meta = read_notebook(cls._filepath).metadata
-        else:
-            nb_meta = None
-
-        if nb_meta is not None and "nbproject" in nb_meta:
-            meta_container = MetaContainer(**nb_meta["nbproject"])
-        else:
-            empty = "not initialized"
-            meta_container = MetaContainer(id=empty, time_init=empty, version=empty)
-
-        cls._store = MetaStore(meta_container, cls._filepath, cls._env)
-        cls._live = MetaLive(cls._filepath, cls._time_run, cls._env)
-
-    @classproperty
-    def store(cls) -> MetaStore:
-        """Metadata stored in the notebook."""
-        if cls._store is None:
-            cls._init_meta()
-        return cls._store  # type: ignore
-
-    @classproperty
-    def live(cls) -> MetaLive:
-        """Contains execution info and properties of the notebook content."""
-        if cls._live is None:
-            cls._init_meta()
-        return cls._live  # type: ignore
-
-    @classproperty
-    def env(cls):
-        """Contains info about execution environment."""
-        if cls._env is None:
-            cls._init_meta()
-        return cls._env
+from pathlib import Path
+from typing import Union
+
+from .dev._jupyter_communicate import notebook_path
+from .dev._meta_live import MetaLive
+from .dev._meta_store import MetaContainer, MetaStore
+from .dev._notebook import read_notebook
+
+
+# https://stackoverflow.com/questions/128573/using-property-on-classmethods/64738850#64738850
+class classproperty(object):
+    def __init__(self, fget):
+        self.fget = fget
+
+    def __get__(self, owner_self, owner_cls):
+        return self.fget(owner_cls)
+
+
+# https://stackoverflow.com/questions/8955754/can-i-define-a-repr-for-a-class-rather-than-an-instance
+class MetaRepr(type):
+    def __repr__(cls):
+        return (
+            "Metadata object with .live and .store metadata fields:\n"
+            f"  .store: {cls.store}\n"
+            f"  .live: {cls.live}"
+        )
+
+
+class meta(metaclass=MetaRepr):
+    """Access `meta.store` and `meta.live`.
+
+    - `meta.store` - nbproject metadata of the ipynb file, see
+      :class:`~nbproject.dev.MetaStore`
+    - `meta.live` - execution info and properties derived from notebook content,
+      see :class:`~nbproject.dev.MetaLive`
+
+    `meta` is a static class and behaves like a module (no need to initialize it).
+    """
+
+    _filepath: Union[str, Path, None] = None
+    _env = None
+    _time_run = None
+
+    _store: Union[MetaStore, None] = None
+    _live: Union[MetaLive, None] = None
+
+    @classmethod
+    def _init_meta(cls):
+        from ._header import _env, _filepath, _time_run
+
+        env = _env
+        filepath = _filepath
+        filepath_env = _filepath, _env
+
+        if filepath is None:
+            filepath_env = notebook_path(return_env=True)
+            if filepath_env is None:
+                filepath_env = None, None
+            filepath = filepath_env[0]
+
+        if env is None:
+            env = filepath_env[1]
+
+        cls._filepath = filepath
+        cls._env = env
+        cls._time_run = _time_run
+
+        if cls._filepath is not None:
+            nb_meta = read_notebook(cls._filepath).metadata
+        else:
+            nb_meta = None
+
+        if nb_meta is not None and "nbproject" in nb_meta:
+            meta_container = MetaContainer(**nb_meta["nbproject"])
+        else:
+            empty = "not initialized"
+            meta_container = MetaContainer(id=empty, time_init=empty, version=empty)
+
+        cls._store = MetaStore(meta_container, cls._filepath, cls._env)
+        cls._live = MetaLive(cls._filepath, cls._time_run, cls._env)
+
+    @classproperty
+    def store(cls) -> MetaStore:
+        """Metadata stored in the notebook."""
+        if cls._store is None:
+            cls._init_meta()
+        return cls._store  # type: ignore
+
+    @classproperty
+    def live(cls) -> MetaLive:
+        """Contains execution info and properties of the notebook content."""
+        if cls._live is None:
+            cls._init_meta()
+        return cls._live  # type: ignore
+
+    @classproperty
+    def env(cls):
+        """Contains info about execution environment."""
+        if cls._env is None:
+            cls._init_meta()
+        return cls._env
```

### Comparing `nbproject-0.8.4/nbproject/_publish.py` & `nbproject-0.8.5/nbproject/_publish.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-from typing import Optional, Union
-
-from ._logger import colors, logger
-from ._meta import meta
-from .dev._check_last_cell import check_last_cell
-from .dev._consecutiveness import check_consecutiveness
-from .dev._frontend_commands import _save_notebook
-from .dev._notebook import read_notebook
-from .dev._set_version import set_version
-
-
-def run_checks_for_publish(
-    *, calling_statement: str, i_confirm_i_saved: bool = False, **kwargs
-):
-    """Runs all checks for publishing."""
-    if meta.env in ("lab", "notebook"):
-        _save_notebook(meta.env)
-    else:
-        pretend_no_test_env = (
-            kwargs["pretend_no_test_env"] if "pretend_no_test_env" in kwargs else False
-        )
-        if (
-            meta.env == "test" and not pretend_no_test_env
-        ):  # do not raise error in test environment
-            pass
-        elif not i_confirm_i_saved:
-            raise RuntimeError(
-                "Make sure you save the notebook in your editor before publishing!\n"
-                "You can avoid the need for manually saving in Jupyter Lab or Notebook,"
-                " which auto-save the buffer during publish."
-            )
-
-    notebook_title = meta.live.title
-    title_error = (
-        f"No title! Update & {colors.bold('save')} your notebook with a title '# My"
-        " title' in the first cell."
-    )
-
-    if notebook_title is None:
-        logger.error(title_error)
-        return "no-title"
-
-    nb = read_notebook(meta._filepath)  # type: ignore
-    if not check_last_cell(nb, calling_statement):
-        raise RuntimeError("Can only publish from the last code cell of the notebook.")
-
-    if not check_consecutiveness(nb):
-        if "proceed_consecutiveness" in kwargs:
-            decide = kwargs["proceed_consecutiveness"]
-        elif meta.env == "test":
-            decide = "y"
-        else:
-            decide = input("   Do you still want to proceed with publishing? (y/n) ")
-
-        if decide not in ("y", "Y", "yes", "Yes", "YES"):
-            logger.warning("Aborted!")
-            return "aborted"
-
-    return "checks-passed"
-
-
-def finalize_publish(*, calling_statement: str, version: Optional[str] = None):
-    meta.store.version = set_version(version)
-    meta.store.pypackage = meta.live.pypackage
-    meta.store.user_handle = meta.live.user_handle
-    meta.store.user_id = meta.live.user_id
-    meta.store.user_name = meta.live.user_name
-    logger.info(
-        f"Set notebook version to {colors.bold(meta.store.version)} & wrote pypackages."
-    )
-    meta.store.write(calling_statement=calling_statement)
-    return None
-
-
-def publish(
-    *,
-    version: Optional[str] = None,
-    i_confirm_i_saved: bool = False,
-    **kwargs,
-) -> Union[None, str]:
-    """Publish the notebook.
-
-    Runs these checks:
-    1. Checks consecutiveness, i.e., whether notebook cells were executed consecutively.
-    2. Checks that the notebook has a title.
-    3. Checks that the notebook is published from its last cell.
-
-    Writes these data:
-    1. Sets version.
-    2. Stores currently imported python packages with their versions.
-
-    Returns `None` upon success and an error code otherwise.
-
-    Args:
-        version: If `None`, leaves the version at its current value. Otherwise
-            sets the version to the passed version. Consider semantic versioning.
-        i_confirm_i_saved: Only relevant outside Jupyter Lab as a safeguard against
-            losing the editor buffer content because of accidentally publishing.
-    """
-    if "calling_statement" in kwargs:
-        calling_statement = kwargs.pop("calling_statement")
-    else:
-        calling_statement = "publish("
-    result = run_checks_for_publish(
-        i_confirm_i_saved=i_confirm_i_saved,
-        calling_statement=calling_statement,
-        **kwargs,
-    )
-    if result == "checks-passed":
-        return finalize_publish(version=version, calling_statement=calling_statement)
-    else:
-        return result
+from typing import Optional, Union
+
+from ._logger import colors, logger
+from ._meta import meta
+from .dev._check_last_cell import check_last_cell
+from .dev._consecutiveness import check_consecutiveness
+from .dev._frontend_commands import _save_notebook
+from .dev._notebook import read_notebook
+from .dev._set_version import set_version
+
+
+def run_checks_for_publish(
+    *, calling_statement: str, i_confirm_i_saved: bool = False, **kwargs
+):
+    """Runs all checks for publishing."""
+    if meta.env in ("lab", "notebook"):
+        _save_notebook(meta.env)
+    else:
+        pretend_no_test_env = (
+            kwargs["pretend_no_test_env"] if "pretend_no_test_env" in kwargs else False
+        )
+        if (
+            meta.env == "test" and not pretend_no_test_env
+        ):  # do not raise error in test environment
+            pass
+        elif not i_confirm_i_saved:
+            raise RuntimeError(
+                "Make sure you save the notebook in your editor before publishing!\n"
+                "You can avoid the need for manually saving in Jupyter Lab or Notebook,"
+                " which auto-save the buffer during publish."
+            )
+
+    notebook_title = meta.live.title
+    title_error = (
+        f"No title! Update & {colors.bold('save')} your notebook with a title '# My"
+        " title' in the first cell."
+    )
+
+    if notebook_title is None:
+        logger.error(title_error)
+        return "no-title"
+
+    nb = read_notebook(meta._filepath)  # type: ignore
+    if not check_last_cell(nb, calling_statement):
+        raise RuntimeError("Can only publish from the last code cell of the notebook.")
+
+    if not check_consecutiveness(nb):
+        if "proceed_consecutiveness" in kwargs:
+            decide = kwargs["proceed_consecutiveness"]
+        elif meta.env == "test":
+            decide = "y"
+        else:
+            decide = input("   Do you still want to proceed with publishing? (y/n) ")
+
+        if decide not in ("y", "Y", "yes", "Yes", "YES"):
+            logger.warning("Aborted!")
+            return "aborted"
+
+    return "checks-passed"
+
+
+def finalize_publish(*, calling_statement: str, version: Optional[str] = None):
+    meta.store.version = set_version(version)
+    meta.store.pypackage = meta.live.pypackage
+    meta.store.user_handle = meta.live.user_handle
+    meta.store.user_id = meta.live.user_id
+    meta.store.user_name = meta.live.user_name
+    logger.info(
+        f"Set notebook version to {colors.bold(meta.store.version)} & wrote pypackages."
+    )
+    meta.store.write(calling_statement=calling_statement)
+    return None
+
+
+def publish(
+    *,
+    version: Optional[str] = None,
+    i_confirm_i_saved: bool = False,
+    **kwargs,
+) -> Union[None, str]:
+    """Publish the notebook.
+
+    Runs these checks:
+    1. Checks consecutiveness, i.e., whether notebook cells were executed consecutively.
+    2. Checks that the notebook has a title.
+    3. Checks that the notebook is published from its last cell.
+
+    Writes these data:
+    1. Sets version.
+    2. Stores currently imported python packages with their versions.
+
+    Returns `None` upon success and an error code otherwise.
+
+    Args:
+        version: If `None`, leaves the version at its current value. Otherwise
+            sets the version to the passed version. Consider semantic versioning.
+        i_confirm_i_saved: Only relevant outside Jupyter Lab as a safeguard against
+            losing the editor buffer content because of accidentally publishing.
+    """
+    if "calling_statement" in kwargs:
+        calling_statement = kwargs.pop("calling_statement")
+    else:
+        calling_statement = "publish("
+    result = run_checks_for_publish(
+        i_confirm_i_saved=i_confirm_i_saved,
+        calling_statement=calling_statement,
+        **kwargs,
+    )
+    if result == "checks-passed":
+        return finalize_publish(version=version, calling_statement=calling_statement)
+    else:
+        return result
```

### Comparing `nbproject-0.8.4/nbproject/_schemas.py` & `nbproject-0.8.5/nbproject/_schemas.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-from datetime import datetime, timezone
-from pathlib import Path
-
-from .dev._initialize import nbproject_id
-from .dev._notebook import Notebook, write_notebook
-
-
-def public_fields(obj):
-    vars_props_dict = {}
-    for key in dir(obj):
-        if key[0] != "_":
-            value = getattr(obj, key)
-            if not callable(value) and value is not None:
-                vars_props_dict[key] = value
-    return vars_props_dict
-
-
-class NBRecord:
-    def __init__(self, nb: Notebook):
-        self._nb = nb
-
-        metadata = nb.metadata
-        if "nbproject" in metadata:
-            self._filled = True
-            for key, value in metadata["nbproject"].items():
-                setattr(self, "_" + key, value)
-        else:
-            self._filled = False
-
-    def check_attr(self, attr):
-        if hasattr(self, attr):
-            return getattr(self, attr)
-        else:
-            self._filled = False
-            return None
-
-    def __setattr__(self, attr_name, value):
-        if attr_name[0] != "_":
-            present_value = self.check_attr(attr_name)
-            if present_value != value:
-                self.__dict__[attr_name] = value
-                self._filled = False
-        else:
-            self.__dict__[attr_name] = value
-
-    @property
-    def id(self):
-        id = self.check_attr("_id")
-        if id is None:
-            id = nbproject_id()
-            self._id = id
-        return id
-
-    @property
-    def time_init(self):
-        time_init = self.check_attr("_time_init")
-        if time_init is None:
-            time_init = datetime.now(timezone.utc).isoformat()
-            self._time_init = time_init
-        return time_init
-
-    @property
-    def version(self):
-        version = self.check_attr("_version")
-        if version is None:
-            version = "0"
-            self._version = "0"
-        return version
-
-    @property
-    def pypackage(self):
-        if "pypackage" in self.__dict__:
-            return self.__dict__["pypackage"]
-        elif hasattr(self, "_pypackage"):
-            return self._pypackage
-        else:
-            return None
-
-    def write(self, nb_path: Path, overwrite: bool):
-        nbproj_data = public_fields(self)
-        if overwrite or not self._filled:
-            self._nb.metadata["nbproject"] = nbproj_data
-            write_notebook(self._nb, nb_path)
-            self._filled = True
-
-
-class YAMLRecord:
-    # this is for ordering and also ignore this when reading yaml fields
-    _take_keys = ("time_init", "name", "version", "location")
-
-    def __init__(self, nb_path: Path, nb_record: NBRecord, yaml_proj: dict):
-        self._yaml_proj = yaml_proj
-        self._nb_record = nb_record
-        # load fields from the notebooks' metadata
-        nb_record_fields = public_fields(nb_record)
-
-        self._id = nb_record_fields.pop("id")
-
-        for key, value in nb_record_fields.items():
-            setattr(self, key, value)
-
-        # take field from yaml, takes precedence over nb_record
-        if self._id in self._yaml_proj:
-            for key, value in self._yaml_proj[self._id].items():
-                if key not in self._take_keys:
-                    setattr(self, key, value)
-
-        # here set fields specific to yaml
-        self.time_init = datetime.fromisoformat(self.time_init)  # type: ignore
-        self.time_init = self.time_init.strftime("%Y-%m-%d %H:%M")  # type: ignore
-
-        self.location = nb_path.parent.as_posix()
-        self.name = nb_path.name
-
-    def put_metadata(self):
-        for key, value in public_fields(self).items():
-            if key not in self._take_keys:
-                setattr(self._nb_record, key, value)
-
-    def put_yaml(self):
-        yaml_project = self._yaml_proj
-
-        if self._id not in yaml_project:
-            yaml_project[self._id] = {}
-
-        yaml_record = yaml_project[self._id]
-        fields = public_fields(self)
-        for key in self._take_keys:
-            yaml_record[key] = fields.pop(key)
-        yaml_record.update(fields)
+from datetime import datetime, timezone
+from pathlib import Path
+
+from .dev._initialize import nbproject_id
+from .dev._notebook import Notebook, write_notebook
+
+
+def public_fields(obj):
+    vars_props_dict = {}
+    for key in dir(obj):
+        if key[0] != "_":
+            value = getattr(obj, key)
+            if not callable(value) and value is not None:
+                vars_props_dict[key] = value
+    return vars_props_dict
+
+
+class NBRecord:
+    def __init__(self, nb: Notebook):
+        self._nb = nb
+
+        metadata = nb.metadata
+        if "nbproject" in metadata:
+            self._filled = True
+            for key, value in metadata["nbproject"].items():
+                setattr(self, "_" + key, value)
+        else:
+            self._filled = False
+
+    def check_attr(self, attr):
+        if hasattr(self, attr):
+            return getattr(self, attr)
+        else:
+            self._filled = False
+            return None
+
+    def __setattr__(self, attr_name, value):
+        if attr_name[0] != "_":
+            present_value = self.check_attr(attr_name)
+            if present_value != value:
+                self.__dict__[attr_name] = value
+                self._filled = False
+        else:
+            self.__dict__[attr_name] = value
+
+    @property
+    def id(self):
+        id = self.check_attr("_id")
+        if id is None:
+            id = nbproject_id()
+            self._id = id
+        return id
+
+    @property
+    def time_init(self):
+        time_init = self.check_attr("_time_init")
+        if time_init is None:
+            time_init = datetime.now(timezone.utc).isoformat()
+            self._time_init = time_init
+        return time_init
+
+    @property
+    def version(self):
+        version = self.check_attr("_version")
+        if version is None:
+            version = "0"
+            self._version = "0"
+        return version
+
+    @property
+    def pypackage(self):
+        if "pypackage" in self.__dict__:
+            return self.__dict__["pypackage"]
+        elif hasattr(self, "_pypackage"):
+            return self._pypackage
+        else:
+            return None
+
+    def write(self, nb_path: Path, overwrite: bool):
+        nbproj_data = public_fields(self)
+        if overwrite or not self._filled:
+            self._nb.metadata["nbproject"] = nbproj_data
+            write_notebook(self._nb, nb_path)
+            self._filled = True
+
+
+class YAMLRecord:
+    # this is for ordering and also ignore this when reading yaml fields
+    _take_keys = ("time_init", "name", "version", "location")
+
+    def __init__(self, nb_path: Path, nb_record: NBRecord, yaml_proj: dict):
+        self._yaml_proj = yaml_proj
+        self._nb_record = nb_record
+        # load fields from the notebooks' metadata
+        nb_record_fields = public_fields(nb_record)
+
+        self._id = nb_record_fields.pop("id")
+
+        for key, value in nb_record_fields.items():
+            setattr(self, key, value)
+
+        # take field from yaml, takes precedence over nb_record
+        if self._id in self._yaml_proj:
+            for key, value in self._yaml_proj[self._id].items():
+                if key not in self._take_keys:
+                    setattr(self, key, value)
+
+        # here set fields specific to yaml
+        self.time_init = datetime.fromisoformat(self.time_init)  # type: ignore
+        self.time_init = self.time_init.strftime("%Y-%m-%d %H:%M")  # type: ignore
+
+        self.location = nb_path.parent.as_posix()
+        self.name = nb_path.name
+
+    def put_metadata(self):
+        for key, value in public_fields(self).items():
+            if key not in self._take_keys:
+                setattr(self._nb_record, key, value)
+
+    def put_yaml(self):
+        yaml_project = self._yaml_proj
+
+        if self._id not in yaml_project:
+            yaml_project[self._id] = {}
+
+        yaml_record = yaml_project[self._id]
+        fields = public_fields(self)
+        for key in self._take_keys:
+            yaml_record[key] = fields.pop(key)
+        yaml_record.update(fields)
```

### Comparing `nbproject-0.8.4/nbproject/dev/_check_last_cell.py` & `nbproject-0.8.5/nbproject/dev/_check_last_cell.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from ._notebook import Notebook
-
-
-def check_last_cell(nb: Notebook, calling_statement: str) -> bool:
-    """Check whether code has been executed in the last cell.
-
-    Args:
-        nb: Notebook content.
-        calling_statement: The statement that calls this function.
-    """
-    last_code_cell = None
-    for cell in nb.cells:
-        if cell["cell_type"] == "code" and cell["source"] != []:
-            last_code_cell = cell
-
-    if last_code_cell is not None and calling_statement in "".join(
-        last_code_cell["source"]
-    ):
-        return True
-    else:
-        return False
+from ._notebook import Notebook
+
+
+def check_last_cell(nb: Notebook, calling_statement: str) -> bool:
+    """Check whether code has been executed in the last cell.
+
+    Args:
+        nb: Notebook content.
+        calling_statement: The statement that calls this function.
+    """
+    last_code_cell = None
+    for cell in nb.cells:
+        if cell["cell_type"] == "code" and cell["source"] != []:
+            last_code_cell = cell
+
+    if last_code_cell is not None and calling_statement in "".join(
+        last_code_cell["source"]
+    ):
+        return True
+    else:
+        return False
```

### Comparing `nbproject-0.8.4/nbproject/dev/_classic_nb_commands.py` & `nbproject-0.8.5/nbproject/dev/_classic_nb_commands.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from time import sleep
-
-from .._logger import logger
-
-
-def _save_notebook():
-    try:
-        from IPython.display import Javascript, display_javascript
-    except ModuleNotFoundError:
-        logger.warning("Can not import from IPython.")
-        return None
-
-    js = Javascript("IPython.notebook.save_notebook()")
-    display_javascript(js)
-
-    sleep(1)
-
-
-def _reload_notebook():
-    try:
-        from IPython.display import Javascript, display_javascript
-    except ModuleNotFoundError:
-        logger.warning("Can not import from IPython.")
-        return None
-
-    js = Javascript("IPython.notebook.load_notebook(IPython.notebook.notebook_path)")
-    display_javascript(js)
+from time import sleep
+
+from .._logger import logger
+
+
+def _save_notebook():
+    try:
+        from IPython.display import Javascript, display_javascript
+    except ModuleNotFoundError:
+        logger.warning("Can not import from IPython.")
+        return None
+
+    js = Javascript("IPython.notebook.save_notebook()")
+    display_javascript(js)
+
+    sleep(1)
+
+
+def _reload_notebook():
+    try:
+        from IPython.display import Javascript, display_javascript
+    except ModuleNotFoundError:
+        logger.warning("Can not import from IPython.")
+        return None
+
+    js = Javascript("IPython.notebook.load_notebook(IPython.notebook.notebook_path)")
+    display_javascript(js)
```

### Comparing `nbproject-0.8.4/nbproject/dev/_consecutiveness.py` & `nbproject-0.8.5/nbproject/dev/_consecutiveness.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from loguru import logger
-
-from ._notebook import Notebook
-
-
-def check_consecutiveness(nb: Notebook, calling_statement: str = None) -> bool:
-    """Check whether code cells have been executed consecutively.
-
-    Needs to be called in the last code cell of a notebook.
-    Otherwise raises `RuntimeError`.
-
-    Returns cell transitions that violate execution at increments of 1 as a list
-    of tuples.
-
-    Args:
-        nb: Notebook content.
-        calling_statement: The statement that calls this function.
-    """
-    cells = nb.cells
-
-    violations = []
-    prev = 0
-
-    for cell in cells:
-        if cell["cell_type"] != "code" or cell["source"] == []:
-            continue
-
-        if calling_statement is not None and calling_statement in "".join(
-            cell["source"]
-        ):
-            continue
-
-        ccount = cell["execution_count"]
-        if ccount is None or prev is None or ccount - prev != 1:
-            violations.append((prev, ccount))
-
-        prev = ccount
-
-    # ignore the very last code cell of the notebook
-    # `check_consecutiveness` is being run during publish if `last_cell`` is True
-    # hence, that cell has ccount is None
-    if ccount is None:
-        violations.pop()
-
-    any_violations = len(violations) > 0
-    if any_violations:
-        logger.warning(f"Cells {violations} were not run consecutively.")
-    else:
-        logger.success("Cell numbers increase consecutively: Awesome!")
-
-    return not any_violations
+from loguru import logger
+
+from ._notebook import Notebook
+
+
+def check_consecutiveness(nb: Notebook, calling_statement: str = None) -> bool:
+    """Check whether code cells have been executed consecutively.
+
+    Needs to be called in the last code cell of a notebook.
+    Otherwise raises `RuntimeError`.
+
+    Returns cell transitions that violate execution at increments of 1 as a list
+    of tuples.
+
+    Args:
+        nb: Notebook content.
+        calling_statement: The statement that calls this function.
+    """
+    cells = nb.cells
+
+    violations = []
+    prev = 0
+
+    for cell in cells:
+        if cell["cell_type"] != "code" or cell["source"] == []:
+            continue
+
+        if calling_statement is not None and calling_statement in "".join(
+            cell["source"]
+        ):
+            continue
+
+        ccount = cell["execution_count"]
+        if ccount is None or prev is None or ccount - prev != 1:
+            violations.append((prev, ccount))
+
+        prev = ccount
+
+    # ignore the very last code cell of the notebook
+    # `check_consecutiveness` is being run during publish if `last_cell`` is True
+    # hence, that cell has ccount is None
+    if ccount is None:
+        violations.pop()
+
+    any_violations = len(violations) > 0
+    if any_violations:
+        logger.warning(f"Cells {violations} were not run consecutively.")
+    else:
+        logger.success("Cell numbers increase consecutively: Awesome!")
+
+    return not any_violations
```

### Comparing `nbproject-0.8.4/nbproject/dev/_initialize.py` & `nbproject-0.8.5/nbproject/dev/_initialize.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import secrets
-import string
-from datetime import datetime, timezone
-from typing import List, Optional, Union
-
-from ._lamin_communicate import lamin_user_settings
-from ._meta_store import MetaContainer
-from ._notebook import Notebook
-
-
-def nbproject_id():  # rename to nbproject_id also in metadata slot?
-    """A 12-character base62 string."""
-    # https://github.com/laminlabs/lamin-notes/blob/main/docs/2022/ids.ipynb
-    base62 = string.digits + string.ascii_letters.swapcase()
-    id = "".join(secrets.choice(base62) for i in range(12))
-    return id
-
-
-def initialize_metadata(
-    nb: Optional[Notebook] = None,
-    pypackage: Union[str, List[str], None] = None,
-    parent: Union[str, List[str], None] = None,
-) -> MetaContainer:
-    """Initialize nbproject metadata.
-
-    Args:
-        nb: If a notebook is provided, also infer pypackages from the notebook.
-        pypackage: One or more python packages to track.
-        parent: One or more nbproject ids of direct ancestors in a notebook pipeline.
-    """
-    meta = MetaContainer(
-        id=nbproject_id(), time_init=datetime.now(timezone.utc).isoformat()
-    )
-
-    pypackage = [pypackage] if isinstance(pypackage, str) else pypackage
-    if nb is not None and isinstance(pypackage, list):
-        from ._pypackage import infer_pypackages
-
-        meta.pypackage = infer_pypackages(nb, add_pkgs=pypackage, pin_versions=True)
-
-    if parent is not None:
-        meta.parent = parent
-
-    user = lamin_user_settings()
-    if user.handle is not None:
-        meta.user_handle = user.handle
-    if user.id is not None:
-        meta.user_id = user.id
-    if user.name is not None:
-        meta.user_name = user.name
-
-    return meta
+import secrets
+import string
+from datetime import datetime, timezone
+from typing import List, Optional, Union
+
+from ._lamin_communicate import lamin_user_settings
+from ._meta_store import MetaContainer
+from ._notebook import Notebook
+
+
+def nbproject_id():  # rename to nbproject_id also in metadata slot?
+    """A 12-character base62 string."""
+    # https://github.com/laminlabs/lamin-notes/blob/main/docs/2022/ids.ipynb
+    base62 = string.digits + string.ascii_letters.swapcase()
+    id = "".join(secrets.choice(base62) for i in range(12))
+    return id
+
+
+def initialize_metadata(
+    nb: Optional[Notebook] = None,
+    pypackage: Union[str, List[str], None] = None,
+    parent: Union[str, List[str], None] = None,
+) -> MetaContainer:
+    """Initialize nbproject metadata.
+
+    Args:
+        nb: If a notebook is provided, also infer pypackages from the notebook.
+        pypackage: One or more python packages to track.
+        parent: One or more nbproject ids of direct ancestors in a notebook pipeline.
+    """
+    meta = MetaContainer(
+        id=nbproject_id(), time_init=datetime.now(timezone.utc).isoformat()
+    )
+
+    pypackage = [pypackage] if isinstance(pypackage, str) else pypackage
+    if nb is not None and isinstance(pypackage, list):
+        from ._pypackage import infer_pypackages
+
+        meta.pypackage = infer_pypackages(nb, add_pkgs=pypackage, pin_versions=True)
+
+    if parent is not None:
+        meta.parent = parent
+
+    user = lamin_user_settings()
+    if user.handle is not None:
+        meta.user_handle = user.handle
+    if user.id is not None:
+        meta.user_id = user.id
+    if user.name is not None:
+        meta.user_name = user.name
+
+    return meta
```

### Comparing `nbproject-0.8.4/nbproject/dev/_jupyter_lab_commands.py` & `nbproject-0.8.5/nbproject/dev/_jupyter_lab_commands.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from pathlib import Path
-from time import sleep
-
-from ipylab import JupyterFrontEnd
-
-from .._is_run_from_ipython import is_run_from_ipython
-
-app = None
-
-
-def _init_frontend():
-    global app
-    if app is None and is_run_from_ipython:
-        app = JupyterFrontEnd()
-
-
-def _save_notebook():
-    _init_frontend()
-
-    if app is not None:
-        app.commands.execute("docmanager:save")
-        sleep(1)
-
-
-def _reload_notebook():
-    _init_frontend()
-
-    if app is not None:
-        app.commands.execute("docmanager:reload")
-
-
-def _lab_notebook_path():
-    _init_frontend()
-
-    if app is None:
-        return None
-
-    current_session = app.sessions.current_session
-
-    if "name" in current_session:
-        nb_path = Path.cwd() / app.sessions.current_session["name"]
-    else:
-        nb_path = None
-
-    return nb_path
+from pathlib import Path
+from time import sleep
+
+from ipylab import JupyterFrontEnd
+
+from .._is_run_from_ipython import is_run_from_ipython
+
+app = None
+
+
+def _init_frontend():
+    global app
+    if app is None and is_run_from_ipython:
+        app = JupyterFrontEnd()
+
+
+def _save_notebook():
+    _init_frontend()
+
+    if app is not None:
+        app.commands.execute("docmanager:save")
+        sleep(1)
+
+
+def _reload_notebook():
+    _init_frontend()
+
+    if app is not None:
+        app.commands.execute("docmanager:reload")
+
+
+def _lab_notebook_path():
+    _init_frontend()
+
+    if app is None:
+        return None
+
+    current_session = app.sessions.current_session
+
+    if "name" in current_session:
+        nb_path = Path.cwd() / app.sessions.current_session["name"]
+    else:
+        nb_path = None
+
+    return nb_path
```

### Comparing `nbproject-0.8.4/nbproject/dev/_meta_live.py` & `nbproject-0.8.5/nbproject/dev/_meta_live.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-from datetime import datetime, timezone
-from pathlib import Path
-from typing import Optional, Union
-
-from .._logger import logger
-from ._consecutiveness import check_consecutiveness
-from ._jupyter_lab_commands import _save_notebook
-from ._lamin_communicate import lamin_user_settings
-from ._notebook import Notebook, read_notebook
-from ._pypackage import infer_pypackages
-
-
-def get_title(nb: Notebook) -> Optional[str]:
-    """Get title of the notebook."""
-    if nb.cells[0]["cell_type"] != "markdown":
-        title = None
-    else:
-        title = nb.cells[0]["source"][0]
-        if not title.startswith("# "):
-            title = None
-        else:
-            title = title.lstrip("#").strip(" .").strip("\n")
-    return title
-
-
-class MetaLive:
-    """Live properties of the notebook.
-
-    All attributes represent either the execution information or properties inferred
-    on access from the notebook's content.
-    """
-
-    def __init__(
-        self,
-        nb_path: Union[str, Path],
-        time_run: Optional[datetime] = None,
-        env: Optional[str] = None,
-    ):
-        self._nb_path = nb_path
-        self._env = env
-        self._time_run = time_run
-
-    @property
-    def title(self) -> Optional[str]:
-        """Get the title of the notebook.
-
-        The first cell should contain markdown text formatted as a title.
-        """
-        nb = read_notebook(self._nb_path)
-        return get_title(nb)
-
-    @property
-    def pypackage(self):
-        """Infer pypackages for the notebook.
-
-        This accounts for additional pypackages in the file metadata.
-        """
-        nb = read_notebook(self._nb_path)
-        add_pkgs = None
-        if "nbproject" in nb.metadata and "pypackage" in nb.metadata["nbproject"]:
-            if nb.metadata["nbproject"]["pypackage"] is not None:
-                add_pkgs = nb.metadata["nbproject"]["pypackage"].keys()
-        return infer_pypackages(nb, add_pkgs, pin_versions=True)
-
-    @property
-    def consecutive_cells(self) -> bool:
-        """Have notebook cells been consecutively executed?
-
-        Logs cell transitions that violate execution at increments of 1
-        as a list of tuples.
-        """
-        if self._env == "lab":
-            _save_notebook()
-        elif self._env != "test":
-            logger.info("Save the notebook before checking for consecutiveness.")
-        nb = read_notebook(self._nb_path)
-        consecutiveness = check_consecutiveness(
-            nb, calling_statement=".live.consecutive_cells"
-        )
-        return consecutiveness
-
-    @property
-    def time_run(self):
-        """The time when the current session started.
-
-        To get the proper time run, you need to use `from nbproject import header`
-        at the beginning of the notebook. Otherwise, the time run is set to the time
-        of the first access to this attribute.
-        """
-        if self._time_run is None:
-            self._time_run = datetime.now(timezone.utc)
-        return self._time_run.isoformat()
-
-    @property
-    def time_passed(self):
-        """Number of seconds elapsed from `time_run`."""
-        return (datetime.now(timezone.utc) - self._time_run).total_seconds()
-
-    @property
-    def user_handle(self):
-        """User handle from lamindb."""
-        return lamin_user_settings().handle
-
-    @property
-    def user_id(self):
-        """User ID from lamindb."""
-        return lamin_user_settings().id
-
-    @property
-    def user_name(self):
-        """User name from lamindb."""
-        return lamin_user_settings().name
-
-    def __repr__(self):
-        return "Fields: " + " ".join([key for key in dir(self) if key[0] != "_"])
+from datetime import datetime, timezone
+from pathlib import Path
+from typing import Optional, Union
+
+from .._logger import logger
+from ._consecutiveness import check_consecutiveness
+from ._jupyter_lab_commands import _save_notebook
+from ._lamin_communicate import lamin_user_settings
+from ._notebook import Notebook, read_notebook
+from ._pypackage import infer_pypackages
+
+
+def get_title(nb: Notebook) -> Optional[str]:
+    """Get title of the notebook."""
+    if nb.cells[0]["cell_type"] != "markdown":
+        title = None
+    else:
+        title = nb.cells[0]["source"][0]
+        if not title.startswith("# "):
+            title = None
+        else:
+            title = title.lstrip("#").strip(" .").strip("\n")
+    return title
+
+
+class MetaLive:
+    """Live properties of the notebook.
+
+    All attributes represent either the execution information or properties inferred
+    on access from the notebook's content.
+    """
+
+    def __init__(
+        self,
+        nb_path: Union[str, Path],
+        time_run: Optional[datetime] = None,
+        env: Optional[str] = None,
+    ):
+        self._nb_path = nb_path
+        self._env = env
+        self._time_run = time_run
+
+    @property
+    def title(self) -> Optional[str]:
+        """Get the title of the notebook.
+
+        The first cell should contain markdown text formatted as a title.
+        """
+        nb = read_notebook(self._nb_path)
+        return get_title(nb)
+
+    @property
+    def pypackage(self):
+        """Infer pypackages for the notebook.
+
+        This accounts for additional pypackages in the file metadata.
+        """
+        nb = read_notebook(self._nb_path)
+        add_pkgs = None
+        if "nbproject" in nb.metadata and "pypackage" in nb.metadata["nbproject"]:
+            if nb.metadata["nbproject"]["pypackage"] is not None:
+                add_pkgs = nb.metadata["nbproject"]["pypackage"].keys()
+        return infer_pypackages(nb, add_pkgs, pin_versions=True)
+
+    @property
+    def consecutive_cells(self) -> bool:
+        """Have notebook cells been consecutively executed?
+
+        Logs cell transitions that violate execution at increments of 1
+        as a list of tuples.
+        """
+        if self._env == "lab":
+            _save_notebook()
+        elif self._env != "test":
+            logger.info("Save the notebook before checking for consecutiveness.")
+        nb = read_notebook(self._nb_path)
+        consecutiveness = check_consecutiveness(
+            nb, calling_statement=".live.consecutive_cells"
+        )
+        return consecutiveness
+
+    @property
+    def time_run(self):
+        """The time when the current session started.
+
+        To get the proper time run, you need to use `from nbproject import header`
+        at the beginning of the notebook. Otherwise, the time run is set to the time
+        of the first access to this attribute.
+        """
+        if self._time_run is None:
+            self._time_run = datetime.now(timezone.utc)
+        return self._time_run.isoformat()
+
+    @property
+    def time_passed(self):
+        """Number of seconds elapsed from `time_run`."""
+        return (datetime.now(timezone.utc) - self._time_run).total_seconds()
+
+    @property
+    def user_handle(self):
+        """User handle from lamindb."""
+        return lamin_user_settings().handle
+
+    @property
+    def user_id(self):
+        """User ID from lamindb."""
+        return lamin_user_settings().id
+
+    @property
+    def user_name(self):
+        """User name from lamindb."""
+        return lamin_user_settings().name
+
+    def __repr__(self):
+        return "Fields: " + " ".join([key for key in dir(self) if key[0] != "_"])
```

### Comparing `nbproject-0.8.4/nbproject/dev/_meta_store.py` & `nbproject-0.8.5/nbproject/dev/_meta_store.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-from pathlib import Path
-from typing import List, Mapping, Optional, Union
-
-from pydantic import BaseModel, Extra
-
-from .._logger import logger
-from ._frontend_commands import _reload_notebook, _save_notebook
-from ._metadata_display import table_metadata
-from ._notebook import Notebook, read_notebook, write_notebook
-from ._pypackage import _get_version
-
-
-def _change_display_table(metadata: Mapping, notebook: Notebook):
-    cells = notebook.cells
-
-    table_html = table_metadata(metadata, notebook)
-
-    for cell in cells:
-        if cell["cell_type"] == "code":
-            for out in cell["outputs"]:
-                if "data" in out and "text/html" in out["data"]:
-                    html = out["data"]["text/html"][0]
-                    if "<b>version</b>" in html:
-                        out["data"]["text/html"][0] = table_html
-                        break
-
-
-def _set_execution_count(calling_statement: str, notebook: Notebook):
-    cells = notebook.cells
-
-    prev = 0
-    for cell in cells:
-        if cell["cell_type"] != "code" or cell["source"] == []:
-            continue
-
-        if calling_statement in "".join(cell["source"]):
-            cell["execution_count"] = prev + 1
-
-        ccount = cell["execution_count"]
-        if ccount is not None:
-            prev = ccount
-
-
-class MetaContainer(BaseModel):
-    """The metadata stored in the notebook file."""
-
-    id: str
-    """A universal 8-digit base62 ID."""
-    version: str = "0"
-    """Published version of notebook."""
-    time_init: str
-    """Time of nbproject init in UTC. Often coincides with notebook creation."""
-    pypackage: Optional[Mapping[str, str]] = None
-    """Dictionary of notebook pypackages and their versions."""
-    parent: Union[str, List[str], None] = None
-    """One or more nbproject ids of direct ancestors in a notebook pipeline."""
-    user_handle: Optional[str] = None
-    """User handle from lamindb."""
-    user_id: Optional[str] = None
-    """User ID from lamindb."""
-    user_name: Optional[str] = None
-    """User name from lamindb."""
-
-    class Config:  # noqa
-        extra = Extra.allow
-
-
-class MetaStore:
-    """The wrapper class for metadata stored in the notebook file."""
-
-    def __init__(
-        self,
-        meta_container: MetaContainer,
-        filepath: Union[str, Path, None] = None,
-        env: Optional[str] = None,
-    ):
-        self._filepath = filepath
-        self._env = env
-
-        self._meta_container = meta_container
-
-    def __getattr__(self, attr_name):
-        return getattr(self._meta_container, attr_name)
-
-    def __setattr__(self, attr_name, value):
-        if attr_name[0] != "_":
-            setattr(self._meta_container, attr_name, value)
-        else:
-            self.__dict__[attr_name] = value
-
-    def add_pypackages(self, packages: Union[List[str], str]) -> "MetaStore":
-        """Manually add pypackages to track.
-
-        Pass a string or a list of strings representing package names.
-
-        Returns self.
-        """
-        if self._meta_container.pypackage is None:
-            self._meta_container.pypackage = {}
-
-        deps_dict = self._meta_container.pypackage
-
-        if isinstance(packages, str):
-            packages = [packages]
-
-        for dep in packages:
-            if dep not in deps_dict:
-                deps_dict[dep] = _get_version(dep)  # type: ignore
-        return self
-
-    def write(self, **kwargs):
-        """Write to file.
-
-        You can edit the nbproject metadata of the current notebook
-        by changing `.store` fields and then using this function
-        to write the changes to the file.
-
-        Outside Jupyter Lab: Save the notebook before writing.
-        """
-        if self._env in ("lab", "notebook"):
-            _save_notebook(self._env)
-
-        nb = read_notebook(self._filepath)
-
-        upd_metadata = self._meta_container.dict()
-        nb.metadata["nbproject"] = upd_metadata
-
-        _change_display_table(upd_metadata, nb)
-
-        if "calling_statement" in kwargs:
-            _set_execution_count(kwargs["calling_statement"], nb)
-
-        write_notebook(nb, self._filepath)
-
-        if self._env in ("lab", "notebook"):
-            _reload_notebook(self._env)
-        elif self._env != "test":
-            logger.info(
-                "File changed on disk! Reload the notebook if you want to continue."
-            )
-            # sys.exit(0)  # makes CI fail, need to think of a decent way of exiting
-
-    def __repr__(self):
-        return f"Wrapper object for the stored metadata:\n  {self._meta_container}"
+from pathlib import Path
+from typing import List, Mapping, Optional, Union
+
+from pydantic import BaseModel, Extra
+
+from .._logger import logger
+from ._frontend_commands import _reload_notebook, _save_notebook
+from ._metadata_display import table_metadata
+from ._notebook import Notebook, read_notebook, write_notebook
+from ._pypackage import _get_version
+
+
+def _change_display_table(metadata: Mapping, notebook: Notebook):
+    cells = notebook.cells
+
+    table_html = table_metadata(metadata, notebook)
+
+    for cell in cells:
+        if cell["cell_type"] == "code":
+            for out in cell["outputs"]:
+                if "data" in out and "text/html" in out["data"]:
+                    html = out["data"]["text/html"][0]
+                    if "<b>version</b>" in html:
+                        out["data"]["text/html"][0] = table_html
+                        break
+
+
+def _set_execution_count(calling_statement: str, notebook: Notebook):
+    cells = notebook.cells
+
+    prev = 0
+    for cell in cells:
+        if cell["cell_type"] != "code" or cell["source"] == []:
+            continue
+
+        if calling_statement in "".join(cell["source"]):
+            cell["execution_count"] = prev + 1
+
+        ccount = cell["execution_count"]
+        if ccount is not None:
+            prev = ccount
+
+
+class MetaContainer(BaseModel):
+    """The metadata stored in the notebook file."""
+
+    id: str
+    """A universal 8-digit base62 ID."""
+    version: str = "0"
+    """Published version of notebook."""
+    time_init: str
+    """Time of nbproject init in UTC. Often coincides with notebook creation."""
+    pypackage: Optional[Mapping[str, str]] = None
+    """Dictionary of notebook pypackages and their versions."""
+    parent: Union[str, List[str], None] = None
+    """One or more nbproject ids of direct ancestors in a notebook pipeline."""
+    user_handle: Optional[str] = None
+    """User handle from lamindb."""
+    user_id: Optional[str] = None
+    """User ID from lamindb."""
+    user_name: Optional[str] = None
+    """User name from lamindb."""
+
+    class Config:  # noqa
+        extra = Extra.allow
+
+
+class MetaStore:
+    """The wrapper class for metadata stored in the notebook file."""
+
+    def __init__(
+        self,
+        meta_container: MetaContainer,
+        filepath: Union[str, Path, None] = None,
+        env: Optional[str] = None,
+    ):
+        self._filepath = filepath
+        self._env = env
+
+        self._meta_container = meta_container
+
+    def __getattr__(self, attr_name):
+        return getattr(self._meta_container, attr_name)
+
+    def __setattr__(self, attr_name, value):
+        if attr_name[0] != "_":
+            setattr(self._meta_container, attr_name, value)
+        else:
+            self.__dict__[attr_name] = value
+
+    def add_pypackages(self, packages: Union[List[str], str]) -> "MetaStore":
+        """Manually add pypackages to track.
+
+        Pass a string or a list of strings representing package names.
+
+        Returns self.
+        """
+        if self._meta_container.pypackage is None:
+            self._meta_container.pypackage = {}
+
+        deps_dict = self._meta_container.pypackage
+
+        if isinstance(packages, str):
+            packages = [packages]
+
+        for dep in packages:
+            if dep not in deps_dict:
+                deps_dict[dep] = _get_version(dep)  # type: ignore
+        return self
+
+    def write(self, **kwargs):
+        """Write to file.
+
+        You can edit the nbproject metadata of the current notebook
+        by changing `.store` fields and then using this function
+        to write the changes to the file.
+
+        Outside Jupyter Lab: Save the notebook before writing.
+        """
+        if self._env in ("lab", "notebook"):
+            _save_notebook(self._env)
+
+        nb = read_notebook(self._filepath)
+
+        upd_metadata = self._meta_container.dict()
+        nb.metadata["nbproject"] = upd_metadata
+
+        _change_display_table(upd_metadata, nb)
+
+        if "calling_statement" in kwargs:
+            _set_execution_count(kwargs["calling_statement"], nb)
+
+        write_notebook(nb, self._filepath)
+
+        if self._env in ("lab", "notebook"):
+            _reload_notebook(self._env)
+        elif self._env != "test":
+            logger.info(
+                "File changed on disk! Reload the notebook if you want to continue."
+            )
+            # sys.exit(0)  # makes CI fail, need to think of a decent way of exiting
+
+    def __repr__(self):
+        return f"Wrapper object for the stored metadata:\n  {self._meta_container}"
```

### Comparing `nbproject-0.8.4/nbproject/dev/_metadata_display.py` & `nbproject-0.8.5/nbproject/dev/_metadata_display.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-from datetime import date, datetime, timezone
-from enum import Enum
-from typing import Mapping, Optional
-
-from pydantic import BaseModel
-
-from .._logger import logger
-from ._consecutiveness import check_consecutiveness
-from ._lamin_communicate import lamin_user_settings
-from ._notebook import Notebook
-from ._pypackage import infer_pypackages
-
-
-def table_html(rows: list):
-    html = "<table><tbody>"
-    for row in rows:
-        html += "<tr>"
-        html += f"<td style='text-align: left;'><b>{row.pop(0)}</b></td>"
-        for col in row:
-            html += f"<td style='text-align: left;'>{col}</td>"
-        html += "</tr>"
-    html += "</tbody></table>"
-    return html
-
-
-def display_html(html: str):
-    from IPython.display import HTML, display
-
-    display(HTML(html))
-
-
-# display configuration
-class DisplayConf(BaseModel):
-    time_init: Enum("choice", ["date", "datetime"]) = "datetime"  # type: ignore # noqa
-    time_run: Enum("choice", ["date", "datetime"]) = "datetime"  # type: ignore # noqa
-
-
-def color_id(id: str):
-    return f"{id[:4]}<span style='opacity:0.3'>{id[4:]}</span>"
-
-
-# displays fields within the ipynb metadata section and on-the-fly computed
-class DisplayMeta:
-    def __init__(self, metadata: Mapping):
-        self.metadata = metadata
-        self.conf = DisplayConf()
-
-    def id(self):
-        """Shorten ID display."""
-        id = self.metadata["id"] if "id" in self.metadata else self.metadata["uid"]
-        return color_id(id)
-
-    def version(self):
-        return self.metadata["version"]
-
-    def parent(self):
-        if "parent" in self.metadata:
-            parent = self.metadata["parent"]
-            if parent is None:
-                return None
-            if isinstance(parent, list):
-                return " ".join([color_id(id) for id in parent])
-            else:
-                return color_id(parent)
-        else:
-            return None
-
-    def time_init(self):
-        """Shorten ID display."""
-        dt = datetime.fromisoformat(self.metadata["time_init"])
-        if self.conf.time_init == "date":
-            return dt.date()
-        else:
-            return dt.strftime(
-                "%Y-%m-%d %H:%M"
-            )  # probably something more reduced is better
-
-    # this is not part of the ipynb metadata section
-    def time_run(self, dt: datetime):
-        """Shorten ID display."""
-        if self.conf.time_run == "date":
-            return dt.date()
-        else:
-            return dt.strftime(
-                "%Y-%m-%d %H:%M"
-            )  # probably something more reduced is better
-
-    def pypackage(self, deps: Optional[Mapping] = None):
-        if deps is None and "pypackage" in self.metadata:
-            deps = self.metadata["pypackage"]
-
-        if deps is None:
-            return None
-
-        deps_list = []
-        for pkg, ver in deps.items():
-            if ver != "":
-                deps_list.append(pkg + f"=={ver}")
-            else:
-                deps_list.append(pkg)
-
-        if deps_list == []:
-            return None
-        else:
-            deps_list.sort()
-            return deps_list
-
-    def author(self):
-        user_handle = self.metadata.get("user_handle", None)
-        user_id = self.metadata.get("user_id", None)
-        user_name = self.metadata.get("user_name", None)
-
-        if any((user_handle is None, user_id is None, user_name is None)):
-            user = lamin_user_settings()
-            user_handle, user_id, user_name = user.handle, user.id, user.name
-
-        # preferred display
-        if user_name is not None and user_handle is not None:
-            return f"{user_name} ({user_handle})"
-        # fallback display (only handle)
-        elif user_handle is not None:
-            return f"{user_handle}"
-
-        return None
-
-
-def table_metadata(
-    metadata: Mapping, notebook: Notebook, time_run: Optional[datetime] = None
-):
-    dm = DisplayMeta(metadata)
-
-    table = []
-
-    author = dm.author()
-    if author is not None:
-        table.append(["author", author])
-
-    table.append(["id", dm.id()])
-    version = dm.version()
-    table.append(["version", version])
-
-    table.append(["time_init", dm.time_init()])
-
-    if time_run is None:
-        time_run = datetime.now(timezone.utc)
-    table.append(["time_run", dm.time_run(time_run)])
-
-    if dm.parent() is not None:
-        table.append(["parent", dm.parent()])
-
-    if version != "0":
-        logger.disable("nbproject.dev._consecutiveness")
-        consecutiveness = check_consecutiveness(notebook)
-        logger.enable("nbproject.dev._consecutiveness")
-
-        table.append(["consecutive_cells", str(consecutiveness)])
-
-    dep_store = dm.pypackage()
-    if dep_store is not None:
-        add_pkgs = [pkg.partition("==")[0] for pkg in dep_store]
-    else:
-        add_pkgs = None
-    dep_live = dm.pypackage(infer_pypackages(notebook, add_pkgs, pin_versions=True))
-
-    # simplify display when stored & live pypackages match
-    if dep_store is not None and dep_live is not None and dep_live == dep_store:
-        table.append(["pypackage", " ".join(dep_store)])
-    else:
-        if dep_store is not None:
-            table.append(["pypackage_store", " ".join(dep_store)])
-            suffix = "_live"
-        else:
-            suffix = ""
-        if dep_live is not None:
-            table.append([f"pypackage{suffix}", " ".join(dep_live)])
-
-    return table_html(table)
+from datetime import date, datetime, timezone
+from enum import Enum
+from typing import Mapping, Optional
+
+from pydantic import BaseModel
+
+from .._logger import logger
+from ._consecutiveness import check_consecutiveness
+from ._lamin_communicate import lamin_user_settings
+from ._notebook import Notebook
+from ._pypackage import infer_pypackages
+
+
+def table_html(rows: list):
+    html = "<table><tbody>"
+    for row in rows:
+        html += "<tr>"
+        html += f"<td style='text-align: left;'><b>{row.pop(0)}</b></td>"
+        for col in row:
+            html += f"<td style='text-align: left;'>{col}</td>"
+        html += "</tr>"
+    html += "</tbody></table>"
+    return html
+
+
+def display_html(html: str):
+    from IPython.display import HTML, display
+
+    display(HTML(html))
+
+
+# display configuration
+class DisplayConf(BaseModel):
+    time_init: Enum("choice", ["date", "datetime"]) = "datetime"  # type: ignore # noqa
+    time_run: Enum("choice", ["date", "datetime"]) = "datetime"  # type: ignore # noqa
+
+
+def color_id(id: str):
+    return f"{id[:4]}<span style='opacity:0.3'>{id[4:]}</span>"
+
+
+# displays fields within the ipynb metadata section and on-the-fly computed
+class DisplayMeta:
+    def __init__(self, metadata: Mapping):
+        self.metadata = metadata
+        self.conf = DisplayConf()
+
+    def id(self):
+        """Shorten ID display."""
+        id = self.metadata["id"] if "id" in self.metadata else self.metadata["uid"]
+        return color_id(id)
+
+    def version(self):
+        return self.metadata["version"]
+
+    def parent(self):
+        if "parent" in self.metadata:
+            parent = self.metadata["parent"]
+            if parent is None:
+                return None
+            if isinstance(parent, list):
+                return " ".join([color_id(id) for id in parent])
+            else:
+                return color_id(parent)
+        else:
+            return None
+
+    def time_init(self):
+        """Shorten ID display."""
+        dt = datetime.fromisoformat(self.metadata["time_init"])
+        if self.conf.time_init == "date":
+            return dt.date()
+        else:
+            return dt.strftime(
+                "%Y-%m-%d %H:%M"
+            )  # probably something more reduced is better
+
+    # this is not part of the ipynb metadata section
+    def time_run(self, dt: datetime):
+        """Shorten ID display."""
+        if self.conf.time_run == "date":
+            return dt.date()
+        else:
+            return dt.strftime(
+                "%Y-%m-%d %H:%M"
+            )  # probably something more reduced is better
+
+    def pypackage(self, deps: Optional[Mapping] = None):
+        if deps is None and "pypackage" in self.metadata:
+            deps = self.metadata["pypackage"]
+
+        if deps is None:
+            return None
+
+        deps_list = []
+        for pkg, ver in deps.items():
+            if ver != "":
+                deps_list.append(pkg + f"=={ver}")
+            else:
+                deps_list.append(pkg)
+
+        if deps_list == []:
+            return None
+        else:
+            deps_list.sort()
+            return deps_list
+
+    def author(self):
+        user_handle = self.metadata.get("user_handle", None)
+        user_id = self.metadata.get("user_id", None)
+        user_name = self.metadata.get("user_name", None)
+
+        if any((user_handle is None, user_id is None, user_name is None)):
+            user = lamin_user_settings()
+            user_handle, user_id, user_name = user.handle, user.id, user.name
+
+        # preferred display
+        if user_name is not None and user_handle is not None:
+            return f"{user_name} ({user_handle})"
+        # fallback display (only handle)
+        elif user_handle is not None:
+            return f"{user_handle}"
+
+        return None
+
+
+def table_metadata(
+    metadata: Mapping, notebook: Notebook, time_run: Optional[datetime] = None
+):
+    dm = DisplayMeta(metadata)
+
+    table = []
+
+    author = dm.author()
+    if author is not None:
+        table.append(["author", author])
+
+    table.append(["id", dm.id()])
+    version = dm.version()
+    table.append(["version", version])
+
+    table.append(["time_init", dm.time_init()])
+
+    if time_run is None:
+        time_run = datetime.now(timezone.utc)
+    table.append(["time_run", dm.time_run(time_run)])
+
+    if dm.parent() is not None:
+        table.append(["parent", dm.parent()])
+
+    if version != "0":
+        logger.disable("nbproject.dev._consecutiveness")
+        consecutiveness = check_consecutiveness(notebook)
+        logger.enable("nbproject.dev._consecutiveness")
+
+        table.append(["consecutive_cells", str(consecutiveness)])
+
+    dep_store = dm.pypackage()
+    if dep_store is not None:
+        add_pkgs = [pkg.partition("==")[0] for pkg in dep_store]
+    else:
+        add_pkgs = None
+    dep_live = dm.pypackage(infer_pypackages(notebook, add_pkgs, pin_versions=True))
+
+    # simplify display when stored & live pypackages match
+    if dep_store is not None and dep_live is not None and dep_live == dep_store:
+        table.append(["pypackage", " ".join(dep_store)])
+    else:
+        if dep_store is not None:
+            table.append(["pypackage_store", " ".join(dep_store)])
+            suffix = "_live"
+        else:
+            suffix = ""
+        if dep_live is not None:
+            table.append([f"pypackage{suffix}", " ".join(dep_live)])
+
+    return table_html(table)
```

### Comparing `nbproject-0.8.4/nbproject/dev/_pypackage.py` & `nbproject-0.8.5/nbproject/dev/_pypackage.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-import re
-import sys
-from ast import Import, ImportFrom, parse, walk
-from typing import Iterable, List, Optional, Union  # noqa
-
-from importlib_metadata import PackageNotFoundError, packages_distributions, version
-
-from ._notebook import Notebook
-
-std_libs = None
-pkgs_dists = None
-
-
-def _load_pkgs_info():
-    global std_libs
-    global pkgs_dists
-
-    major, minor = sys.version_info[0], sys.version_info[1]
-    if major == 3 and minor > 9:
-        std_libs = sys.stdlib_module_names  # type: ignore
-    else:
-        from stdlib_list import stdlib_list
-
-        std_libs = set(stdlib_list(f"{major}.{minor}"))
-
-    pkgs_dists = packages_distributions()
-
-
-def _get_version(pkg):
-    try:
-        pkg_ver = version(pkg)
-    except PackageNotFoundError:
-        pkg_ver = ""
-    return pkg_ver
-
-
-def cell_imports(cell_source: str):
-    # based on the package https://github.com/bndr/pipreqs for python scripts
-    # parses python import statements in the code cells
-    tree = parse(cell_source)
-    for node in walk(tree):
-        if isinstance(node, Import):
-            for subnode in node.names:
-                name = subnode.name.partition(".")[0]
-                if name != "":
-                    yield name
-        elif isinstance(node, ImportFrom):
-            name = node.module.partition(".")[0]  # type: ignore
-            if name != "":
-                yield name
-
-
-def infer_pypackages(
-    content: Notebook,
-    add_pkgs: Optional[Iterable] = None,
-    pin_versions: bool = True,
-):
-    """Parse notebook object and infer all pypackages.
-
-    This does not account for additional packages in file metadata.
-
-    For the user-facing functionality,
-    see :meth:`~nbproject.dev.MetaLive.pypackage`.
-
-    Args:
-        nb: A notebook to infer pypackages from.
-        add_pkgs: Additional packages to add.
-        pin_versions: If `True`, fixes versions from the current environment.
-
-    Examples:
-        >>> pypackages = nbproject.dev.infer_pypackages(nb)
-        >>> pypackages
-        {"scanpy": "1.8.7", "pandas": "1.4.3"}
-    """
-    cells = content.cells
-
-    if std_libs is None or pkgs_dists is None:
-        _load_pkgs_info()
-
-    pkgs = set()
-    magics_re = None
-
-    for cell in cells:
-        if cell["cell_type"] != "code":
-            continue
-
-        # assuming we read the notebook with a json reader
-        cell_source = "".join(cell["source"])
-        if "import" not in cell_source:
-            continue
-        else:
-            # quick hack to ignore jupyter magics
-            if "%" in cell_source:
-                if magics_re is None:
-                    magics_re = re.compile(r"^( *)%{1,2}\w+ *", flags=re.MULTILINE)
-                cell_source = magics_re.sub(r"\1", cell_source)
-
-            for imp in cell_imports(cell_source):
-                if imp in std_libs:  # type: ignore
-                    continue
-                if imp in pkgs_dists:  # type: ignore
-                    pkgs.update(pkgs_dists[imp])  # type: ignore
-                else:
-                    pkgs.add(imp)
-
-    if add_pkgs is not None:
-        pkgs.update(add_pkgs)
-
-    pkgs = {pkg: "" for pkg in pkgs}  # type: ignore
-    if not pin_versions:
-        return pkgs
-
-    for pkg in pkgs:
-        pkgs[pkg] = _get_version(pkg)  # type: ignore
-
-    return pkgs
-
-
-def _resolve(a, b):
-    import packaging.version
-
-    parse_version = packaging.version.parse
-
-    if a == "":
-        return b
-    elif b == "":
-        return a
-    else:
-        return a if parse_version(a) > parse_version(b) else b
-
-
-def resolve_versions(notebooks_pkgs: List[dict]):
-    """Harmonize packages' versions from lists of packages."""
-    resolved = {}
-    for pkgs in notebooks_pkgs:
-        for pkg, ver in pkgs.items():
-            if pkg not in resolved:
-                resolved[pkg] = ver
-            else:
-                resolved[pkg] = _resolve(resolved[pkg], ver)
-
-    return resolved
+import re
+import sys
+from ast import Import, ImportFrom, parse, walk
+from typing import Iterable, List, Optional, Union  # noqa
+
+from importlib_metadata import PackageNotFoundError, packages_distributions, version
+
+from ._notebook import Notebook
+
+std_libs = None
+pkgs_dists = None
+
+
+def _load_pkgs_info():
+    global std_libs
+    global pkgs_dists
+
+    major, minor = sys.version_info[0], sys.version_info[1]
+    if major == 3 and minor > 9:
+        std_libs = sys.stdlib_module_names  # type: ignore
+    else:
+        from stdlib_list import stdlib_list
+
+        std_libs = set(stdlib_list(f"{major}.{minor}"))
+
+    pkgs_dists = packages_distributions()
+
+
+def _get_version(pkg):
+    try:
+        pkg_ver = version(pkg)
+    except PackageNotFoundError:
+        pkg_ver = ""
+    return pkg_ver
+
+
+def cell_imports(cell_source: str):
+    # based on the package https://github.com/bndr/pipreqs for python scripts
+    # parses python import statements in the code cells
+    tree = parse(cell_source)
+    for node in walk(tree):
+        if isinstance(node, Import):
+            for subnode in node.names:
+                name = subnode.name.partition(".")[0]
+                if name != "":
+                    yield name
+        elif isinstance(node, ImportFrom):
+            name = node.module.partition(".")[0]  # type: ignore
+            if name != "":
+                yield name
+
+
+def infer_pypackages(
+    content: Notebook,
+    add_pkgs: Optional[Iterable] = None,
+    pin_versions: bool = True,
+):
+    """Parse notebook object and infer all pypackages.
+
+    This does not account for additional packages in file metadata.
+
+    For the user-facing functionality,
+    see :meth:`~nbproject.dev.MetaLive.pypackage`.
+
+    Args:
+        nb: A notebook to infer pypackages from.
+        add_pkgs: Additional packages to add.
+        pin_versions: If `True`, fixes versions from the current environment.
+
+    Examples:
+        >>> pypackages = nbproject.dev.infer_pypackages(nb)
+        >>> pypackages
+        {"scanpy": "1.8.7", "pandas": "1.4.3"}
+    """
+    cells = content.cells
+
+    if std_libs is None or pkgs_dists is None:
+        _load_pkgs_info()
+
+    pkgs = set()
+    magics_re = None
+
+    for cell in cells:
+        if cell["cell_type"] != "code":
+            continue
+
+        # assuming we read the notebook with a json reader
+        cell_source = "".join(cell["source"])
+        if "import" not in cell_source:
+            continue
+        else:
+            # quick hack to ignore jupyter magics
+            if "%" in cell_source:
+                if magics_re is None:
+                    magics_re = re.compile(r"^( *)%{1,2}\w+ *", flags=re.MULTILINE)
+                cell_source = magics_re.sub(r"\1", cell_source)
+
+            for imp in cell_imports(cell_source):
+                if imp in std_libs:  # type: ignore
+                    continue
+                if imp in pkgs_dists:  # type: ignore
+                    pkgs.update(pkgs_dists[imp])  # type: ignore
+                else:
+                    pkgs.add(imp)
+
+    if add_pkgs is not None:
+        pkgs.update(add_pkgs)
+
+    pkgs = {pkg: "" for pkg in pkgs}  # type: ignore
+    if not pin_versions:
+        return pkgs
+
+    for pkg in pkgs:
+        pkgs[pkg] = _get_version(pkg)  # type: ignore
+
+    return pkgs
+
+
+def _resolve(a, b):
+    import packaging.version
+
+    parse_version = packaging.version.parse
+
+    if a == "":
+        return b
+    elif b == "":
+        return a
+    else:
+        return a if parse_version(a) > parse_version(b) else b
+
+
+def resolve_versions(notebooks_pkgs: List[dict]):
+    """Harmonize packages' versions from lists of packages."""
+    resolved = {}
+    for pkgs in notebooks_pkgs:
+        for pkg, ver in pkgs.items():
+            if pkg not in resolved:
+                resolved[pkg] = ver
+            else:
+                resolved[pkg] = _resolve(resolved[pkg], ver)
+
+    return resolved
```

### Comparing `nbproject-0.8.4/nbproject/dev/_set_version.py` & `nbproject-0.8.5/nbproject/dev/_set_version.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import Union
-
-from .._meta import meta
-
-
-def set_version(
-    version: Union[str, None] = None, stored_version: Union[str, None] = None
-):
-    """(Auto-) set version.
-
-    If `version` is `None`, returns the stored version.
-    Otherwise sets the version to the passed version.
-
-    Args:
-        version: Version string.
-        stored_version: Mock stored version for testing purposes.
-    """
-    if stored_version is None:
-        stored_version = meta.store.version
-
-    if version is not None:
-        return version
-    else:
-        return stored_version
+from typing import Union
+
+from .._meta import meta
+
+
+def set_version(
+    version: Union[str, None] = None, stored_version: Union[str, None] = None
+):
+    """(Auto-) set version.
+
+    If `version` is `None`, returns the stored version.
+    Otherwise sets the version to the passed version.
+
+    Args:
+        version: Version string.
+        stored_version: Mock stored version for testing purposes.
+    """
+    if stored_version is None:
+        stored_version = meta.store.version
+
+    if version is not None:
+        return version
+    else:
+        return stored_version
```

### Comparing `nbproject-0.8.4/tests/test_jupyter.py` & `nbproject-0.8.5/tests/test_jupyter.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-import os
-
-from pytest import raises
-
-from nbproject.dev import _classic_nb_commands as _clsnbk
-from nbproject.dev import _jupyter_lab_commands as _juplab
-from nbproject.dev._frontend_commands import _reload_notebook, _save_notebook
-from nbproject.dev._jupyter_communicate import (
-    notebook_path,
-    prepare_url,
-    query_server,
-    running_servers,
-)
-
-os.environ["NBPRJ_TEST_NBENV"] = "test"
-
-
-def test_jupyter_not_running():
-    assert notebook_path() is None
-    assert notebook_path(return_env=True) is None
-
-    servers_nbapp, servers_juserv = running_servers()
-    assert list(servers_nbapp) == []
-    assert list(servers_juserv) == []
-
-    server = dict(token="test", url="localhost/")
-
-    assert (
-        prepare_url(server, "/test_query")
-        == "localhost/api/sessions/test_query?token=test"  # noqa
-    )
-
-    with raises(Exception) as e_info:
-        query_server(server)
-
-    assert (
-        e_info.value.args[0]
-        == "Unable to access server;\nquerying requires either no security or token"  # noqa
-        " based security."
-    )
-
-
-def test_juplab_clsnbk_nothing_happens():
-    _juplab._save_notebook()
-    _juplab._reload_notebook()
-
-    _clsnbk._save_notebook()
-    _clsnbk._reload_notebook()
-
-    for env in ("lab", "notebook"):
-        _save_notebook(env)
-        _reload_notebook(env)
-
-    with raises(ValueError):
-        _save_notebook("nonexistent_env")
-
-    with raises(ValueError):
-        _reload_notebook("nonexistent_env")
+import os
+
+from pytest import raises
+
+from nbproject.dev import _classic_nb_commands as _clsnbk
+from nbproject.dev import _jupyter_lab_commands as _juplab
+from nbproject.dev._frontend_commands import _reload_notebook, _save_notebook
+from nbproject.dev._jupyter_communicate import (
+    notebook_path,
+    prepare_url,
+    query_server,
+    running_servers,
+)
+
+os.environ["NBPRJ_TEST_NBENV"] = "test"
+
+
+def test_jupyter_not_running():
+    assert notebook_path() is None
+    assert notebook_path(return_env=True) is None
+
+    servers_nbapp, servers_juserv = running_servers()
+    assert list(servers_nbapp) == []
+    assert list(servers_juserv) == []
+
+    server = dict(token="test", url="localhost/")
+
+    assert (
+        prepare_url(server, "/test_query")
+        == "localhost/api/sessions/test_query?token=test"  # noqa
+    )
+
+    with raises(Exception) as e_info:
+        query_server(server)
+
+    assert (
+        e_info.value.args[0]
+        == "Unable to access server;\nquerying requires either no security or token"  # noqa
+        " based security."
+    )
+
+
+def test_juplab_clsnbk_nothing_happens():
+    _juplab._save_notebook()
+    _juplab._reload_notebook()
+
+    _clsnbk._save_notebook()
+    _clsnbk._reload_notebook()
+
+    for env in ("lab", "notebook"):
+        _save_notebook(env)
+        _reload_notebook(env)
+
+    with raises(ValueError):
+        _save_notebook("nonexistent_env")
+
+    with raises(ValueError):
+        _reload_notebook("nonexistent_env")
```

