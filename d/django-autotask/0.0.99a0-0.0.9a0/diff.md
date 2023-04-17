# Comparing `tmp/django-autotask-0.0.99a0.tar.gz` & `tmp/django-autotask-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-autotask-0.0.99a0.tar", last modified: Mon Nov 23 19:00:17 2020, max compression
+gzip compressed data, was "dist/django-autotask-0.0.9a0.tar", last modified: Tue Oct  8 23:20:54 2019, max compression
```

## Comparing `django-autotask-0.0.99a0.tar` & `django-autotask-0.0.9a0.tar`

### file list

```diff
@@ -1,280 +1,96 @@
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-11-23 19:00:17.000000 django-autotask-0.0.99a0/
--rw-rw-r--   0 sam       (1000) sam       (1000)       82 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/MANIFEST.in
--rw-rw-r--   0 sam       (1000) sam       (1000)       38 2020-11-23 19:00:17.000000 django-autotask-0.0.99a0/setup.cfg
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-11-23 19:00:17.000000 django-autotask-0.0.99a0/djautotask/
--rw-rw-r--   0 sam       (1000) sam       (1000)       99 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/apps.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-11-23 19:00:17.000000 django-autotask-0.0.99a0/djautotask/__pycache__/
--rw-rw-r--   0 sam       (1000) sam       (1000)    46098 2020-11-23 19:00:08.000000 django-autotask-0.0.99a0/djautotask/__pycache__/sync.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      704 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/__pycache__/utils.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      345 2020-11-23 19:00:15.000000 django-autotask-0.0.99a0/djautotask/__pycache__/urls.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     7315 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/__pycache__/api.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     2766 2020-11-23 19:00:15.000000 django-autotask-0.0.99a0/djautotask/__pycache__/views.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    42899 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/__pycache__/models.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      305 2020-11-23 19:00:04.000000 django-autotask-0.0.99a0/djautotask/__pycache__/__init__.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    56185 2020-10-29 16:32:56.000000 django-autotask-0.0.99a0/djautotask/sync.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    10232 2020-10-29 16:22:17.000000 django-autotask-0.0.99a0/djautotask/admin.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-11-23 19:00:17.000000 django-autotask-0.0.99a0/djautotask/management/
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-11-23 19:00:17.000000 django-autotask-0.0.99a0/djautotask/management/__pycache__/
--rw-rw-r--   0 sam       (1000) sam       (1000)      153 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/management/__pycache__/__init__.cpython-36.pyc
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-11-23 19:00:17.000000 django-autotask-0.0.99a0/djautotask/management/commands/
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-11-23 19:00:17.000000 django-autotask-0.0.99a0/djautotask/management/commands/__pycache__/
--rw-rw-r--   0 sam       (1000) sam       (1000)     6321 2020-11-23 19:00:09.000000 django-autotask-0.0.99a0/djautotask/management/commands/__pycache__/atsync.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     8397 2020-11-23 18:59:59.000000 django-autotask-0.0.99a0/djautotask/management/commands/atsync.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1637 2020-11-23 18:59:59.000000 django-autotask-0.0.99a0/djautotask/management/commands/clearoldsyncjobs.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      492 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/management/commands/list_users.py
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/management/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2788 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/views.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    35150 2020-10-29 16:22:17.000000 django-autotask-0.0.99a0/djautotask/models.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-11-23 19:00:17.000000 django-autotask-0.0.99a0/djautotask/tests/
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-11-23 19:00:17.000000 django-autotask-0.0.99a0/djautotask/tests/__pycache__/
--rw-rw-r--   0 sam       (1000) sam       (1000)    11718 2020-11-23 19:00:08.000000 django-autotask-0.0.99a0/djautotask/tests/__pycache__/fixtures.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    19234 2020-11-23 19:00:08.000000 django-autotask-0.0.99a0/djautotask/tests/__pycache__/test_commands.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     2338 2020-11-23 19:00:09.000000 django-autotask-0.0.99a0/djautotask/tests/__pycache__/test_views.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     2458 2020-11-23 19:00:08.000000 django-autotask-0.0.99a0/djautotask/tests/__pycache__/mocks.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    56076 2020-11-23 19:00:09.000000 django-autotask-0.0.99a0/djautotask/tests/__pycache__/test_sync.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      294 2020-11-23 19:00:15.000000 django-autotask-0.0.99a0/djautotask/tests/__pycache__/urls.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    13907 2020-11-23 19:00:08.000000 django-autotask-0.0.99a0/djautotask/tests/__pycache__/fixture_utils.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     3332 2020-11-23 19:00:09.000000 django-autotask-0.0.99a0/djautotask/tests/__pycache__/test_model.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      148 2020-11-23 19:00:08.000000 django-autotask-0.0.99a0/djautotask/tests/__pycache__/__init__.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)   174033 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/tests/atws.wsdl
--rw-rw-r--   0 sam       (1000) sam       (1000)    58570 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/tests/test_sync.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2957 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/tests/test_model.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2202 2020-10-29 16:22:17.000000 django-autotask-0.0.99a0/djautotask/tests/mocks.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2109 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/tests/test_views.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    19138 2020-10-29 16:22:17.000000 django-autotask-0.0.99a0/djautotask/tests/test_commands.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    15718 2020-10-29 16:22:17.000000 django-autotask-0.0.99a0/djautotask/tests/fixture_utils.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      140 2020-11-23 18:59:59.000000 django-autotask-0.0.99a0/djautotask/tests/urls.py
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/tests/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    23888 2020-10-29 16:22:17.000000 django-autotask-0.0.99a0/djautotask/tests/fixtures.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-11-23 19:00:17.000000 django-autotask-0.0.99a0/djautotask/templates/
--rw-rw-r--   0 sam       (1000) sam       (1000)      112 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/templates/change_form.html
--rw-rw-r--   0 sam       (1000) sam       (1000)      216 2020-11-23 18:59:59.000000 django-autotask-0.0.99a0/djautotask/urls.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-11-23 19:00:17.000000 django-autotask-0.0.99a0/djautotask/migrations/
--rw-rw-r--   0 sam       (1000) sam       (1000)      280 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0021_merge_20191031_1259.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      446 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0013_auto_20190923_1439.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      281 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0041_merge_20200204_1546.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      398 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0029_phase_last_activity_date.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1861 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0076_auto_20200923_0953.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     3582 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0024_auto_20191122_1516.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      644 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0040_auto_20200204_1538.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     4027 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0038_notetype_tasknote_ticketnote.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1723 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0006_auto_20190916_1645.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1552 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0018_auto_20191029_1634.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      337 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0005_remove_ticketstatus_value.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-11-23 19:00:17.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/
--rw-rw-r--   0 sam       (1000) sam       (1000)     1397 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0005_auto_20190916_1549.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      553 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0011_auto_20190923_1157.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1237 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0042_auto_20200205_1455.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      771 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0055_auto_20200325_0928.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      537 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0005_remove_ticketstatus_value.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     5541 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0080_accountphysicallocationtracker_accounttracker_accounttypetracker_allocationcodetracker_contracttrack.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      898 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0051_contract.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      711 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0028_task_secondary_resources.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      498 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0041_merge_20200204_1546.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      947 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0076_auto_20200925_1326.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      504 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0006_merge_20190920_1450.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      524 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0050_remove_ticket_role.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1493 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0028_phase.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      609 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0002_ticket_ticket_number.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      698 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0030_task_phase.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     2608 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0009_auto_20190918_1525.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      911 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0064_auto_20200511_1124.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      744 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0064_servicecall_location.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      498 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0033_merge_20191204_1022.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      730 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0072_account_parent_account.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      717 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0053_timeentry_contract.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1595 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0082_auto_20201020_1617.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      558 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0009_auto_20190920_1648.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     3491 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0059_auto_20200414_1242.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      791 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0077_auto_20200924_1512.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     2100 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0038_notetype_tasknote_ticketnote.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      495 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0031_merge_20191202_1119.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      806 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0010_auto_20190923_0930.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      864 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0060_auto_20200414_1522.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      654 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0083_ticketudftracker.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      617 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0038_auto_20200130_1218.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      780 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0047_auto_20200207_1126.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      800 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0017_auto_20191021_1028.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      498 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0040_merge_20200131_1627.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      497 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0056_merge_20200327_1045.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1442 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0015_auto_20191001_0847.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1583 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0001_initial.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      855 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0067_auto_20200519_1100.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      591 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0079_auto_20201003_1125.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      718 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0034_auto_20191210_1518.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      745 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0047_task_assigned_resource_role.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1498 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0006_auto_20190916_1645.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      749 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0048_auto_20200211_1037.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1105 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0018_auto_20191029_1621.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      818 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0046_auto_20200207_1002.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      497 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0021_merge_20191031_1259.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      611 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0070_auto_20200714_0807.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      740 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0043_timeentry_allocation_code.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     2205 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0024_auto_20191122_1516.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      716 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0062_task_department.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      497 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0010_merge_20190923_1155.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1248 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0075_taskpredecessor.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1058 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0016_auto_20191021_0958.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1031 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0031_auto_20191129_1454.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      497 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0078_merge_20201001_1657.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      799 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0069_auto_20200602_1419.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      777 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0058_auto_20200408_1022.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1323 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0004_auto_20190913_1425.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1406 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0018_auto_20191029_1634.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1223 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0045_resourceroledepartment_resourceservicedeskrole.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      498 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0068_merge_20200521_1615.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      524 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0020_auto_20191030_0916.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1389 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0055_auto_20200325_1335.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      699 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0065_auto_20200512_1224.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      661 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0085_auto_20201022_1822.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      648 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0066_auto_20200512_1420.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      559 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0026_auto_20191125_0952.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      507 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0039_merge_20200131_1022.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      497 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0054_merge_20200323_1511.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1490 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0003_auto_20190913_0941.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      499 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0022_merge_20191031_1620.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      563 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0013_auto_20190923_1439.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1559 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0008_auto_20190917_1454.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1402 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0039_auto_20200131_1134.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      496 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0044_merge_20200205_1651.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      940 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0063_accountphysicallocation.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      754 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0032_auto_20191129_1501.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1658 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0042_auto_20200205_1057.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      498 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0008_merge_20190920_1644.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      766 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0046_ticket_assigned_resource_role.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      153 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/__init__.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      779 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0043_department.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      819 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0036_auto_20200127_1157.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      506 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0049_merge_20200227_1701.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1438 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0007_auto_20190917_1009.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      499 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0067_merge_20200514_1713.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      607 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0061_auto_20200416_1241.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      804 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0081_project_department.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      667 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0052_contract_status.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      643 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0074_auto_20200827_1818.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      734 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0037_subissuetype_parent_value.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      793 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0051_auto_20200315_1819.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      783 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0057_auto_20200406_1620.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      607 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0023_auto_20191119_0923.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      636 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0019_auto_20191030_0905.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      700 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0040_auto_20200204_1538.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      600 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0029_phase_last_activity_date.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      597 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0073_syncjob_skipped.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      497 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0021_merge_20191031_0858.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      776 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0084_projectudftracker_taskudftracker.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      552 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0025_auto_20191125_0939.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1646 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0035_timeentry.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      990 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0076_auto_20200923_0953.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      622 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0071_project_status_detail.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     2525 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0014_auto_20190930_1548.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      559 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0027_auto_20191125_1103.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      497 2020-11-23 19:00:05.000000 django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0012_merge_20190923_1439.cpython-36.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      445 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0052_contract_status.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      505 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0034_auto_20191210_1518.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      346 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0020_auto_20191030_0916.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     8223 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0059_auto_20200414_1242.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      697 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0043_department.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      360 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0011_auto_20190923_1157.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      281 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0033_merge_20191204_1022.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      401 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0073_syncjob_skipped.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1330 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0064_auto_20200511_1124.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      881 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0032_auto_20191129_1501.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     4964 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0009_auto_20190918_1525.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      366 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0026_auto_20191125_0952.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      501 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0028_task_secondary_resources.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1519 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0039_auto_20200131_1134.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      279 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0044_merge_20200205_1651.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1640 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0007_auto_20190917_1009.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      331 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0050_remove_ticket_role.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      777 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0069_auto_20200602_1419.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      643 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0065_auto_20200512_1224.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      416 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0038_auto_20200130_1218.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      740 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0055_auto_20200325_0928.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2395 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0042_auto_20200205_1057.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2114 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0035_timeentry.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      441 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0009_auto_20190920_1648.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      523 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0047_task_assigned_resource_role.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      375 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0027_auto_20191125_1103.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      542 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0046_ticket_assigned_resource_role.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      280 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0021_merge_20191031_0858.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      421 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0071_project_status_detail.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      728 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0057_auto_20200406_1620.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      289 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0049_merge_20200227_1701.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      513 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0072_account_parent_account.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2211 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0001_initial.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1423 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0017_auto_20191021_1028.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     3176 2020-10-29 16:22:17.000000 django-autotask-0.0.99a0/djautotask/migrations/0082_auto_20201020_1617.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2205 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0016_auto_20191021_0958.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1680 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0031_auto_20191129_1454.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      280 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0012_merge_20190923_1439.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     6182 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0014_auto_20190930_1548.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      407 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0002_ticket_ticket_number.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      575 2020-10-29 16:22:17.000000 django-autotask-0.0.99a0/djautotask/migrations/0083_ticketudftracker.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1763 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0028_phase.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1583 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0015_auto_20191001_0847.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      514 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0037_subissuetype_parent_value.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1385 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0075_taskpredecessor.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      590 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0081_project_department.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      391 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0079_auto_20201003_1125.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      281 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0040_merge_20200131_1627.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      451 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0019_auto_20191030_0905.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      281 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0068_merge_20200521_1615.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      437 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0074_auto_20200827_1818.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1036 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0010_auto_20190923_0930.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1647 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0045_resourceroledepartment_resourceservicedeskrole.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1715 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0003_auto_20190913_0941.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      506 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0062_task_department.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1456 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0036_auto_20200127_1157.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      754 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0051_auto_20200315_1819.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1506 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0055_auto_20200325_1335.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      280 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0056_merge_20200327_1045.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      410 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0061_auto_20200416_1241.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      279 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0078_merge_20201001_1657.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      362 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0025_auto_20191125_0939.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      717 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0058_auto_20200408_1022.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      504 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0053_timeentry_contract.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1517 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0005_auto_20190916_1549.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      401 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0023_auto_20191119_0923.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      412 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0070_auto_20200714_0807.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    14818 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0080_accountphysicallocationtracker_accounttracker_accounttypetracker_allocationcodetracker_contracttrack.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      282 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0022_merge_20191031_1620.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      757 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0077_auto_20200924_1512.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      835 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0067_auto_20200519_1100.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      290 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0039_merge_20200131_1022.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1304 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0042_auto_20200205_1455.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      281 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0008_merge_20190920_1644.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1430 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0004_auto_20190913_1425.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      773 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0046_auto_20200207_1002.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      917 2020-10-29 16:22:17.000000 django-autotask-0.0.99a0/djautotask/migrations/0084_projectudftracker_taskudftracker.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      529 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0064_servicecall_location.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      280 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0054_merge_20200323_1511.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      282 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0067_merge_20200514_1713.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      589 2020-10-29 16:22:17.000000 django-autotask-0.0.99a0/djautotask/migrations/0085_auto_20201022_1822.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      779 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0051_contract.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      853 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0048_auto_20200211_1037.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1843 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0008_auto_20190917_1454.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      520 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0043_timeentry_allocation_code.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      762 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0047_auto_20200207_1126.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      442 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0066_auto_20200512_1420.py
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      850 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0060_auto_20200414_1522.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      278 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0031_merge_20191202_1119.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      822 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0063_accountphysicallocation.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1697 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0018_auto_20191029_1621.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      982 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0076_auto_20200925_1326.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      490 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0030_task_phase.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      280 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0010_merge_20190923_1155.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      287 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/migrations/0006_merge_20190920_1450.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     8087 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/api.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      227 2020-11-23 18:59:59.000000 django-autotask-0.0.99a0/djautotask/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      460 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/djautotask/utils.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2318 2020-11-23 19:00:17.000000 django-autotask-0.0.99a0/PKG-INFO
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2020-11-23 19:00:17.000000 django-autotask-0.0.99a0/django_autotask.egg-info/
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2020-11-23 19:00:04.000000 django-autotask-0.0.99a0/django_autotask.egg-info/not-zip-safe
--rw-rw-r--   0 sam       (1000) sam       (1000)     2318 2020-11-23 19:00:16.000000 django-autotask-0.0.99a0/django_autotask.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)       11 2020-11-23 19:00:16.000000 django-autotask-0.0.99a0/django_autotask.egg-info/top_level.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)    15184 2020-11-23 19:00:16.000000 django-autotask-0.0.99a0/django_autotask.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2020-11-23 19:00:16.000000 django-autotask-0.0.99a0/django_autotask.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       97 2020-11-23 19:00:16.000000 django-autotask-0.0.99a0/django_autotask.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)      885 2020-11-23 18:59:59.000000 django-autotask-0.0.99a0/README.md
--rw-rw-r--   0 sam       (1000) sam       (1000)     1797 2020-10-16 19:30:59.000000 django-autotask-0.0.99a0/setup.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/
+-rw-rw-r--   0 sam       (1000) sam       (1000)       99 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/apps.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/migrations/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      280 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0010_merge_20190923_1155.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1430 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0004_auto_20190913_1425.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1843 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0008_auto_20190917_1454.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2211 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0001_initial.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1583 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/migrations/0015_auto_20191001_0847.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     6182 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/migrations/0014_auto_20190930_1548.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      601 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0009_auto_20190920_1648.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3229 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0014_auto_20190930_1548.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)      552 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0006_merge_20190920_1450.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)      547 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0008_merge_20190920_1644.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)      545 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0010_merge_20190923_1155.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1718 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0008_auto_20190917_1454.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1537 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0005_auto_20190916_1549.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)      545 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0012_merge_20190923_1439.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1774 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0001_initial.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1663 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0003_auto_20190913_0941.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)      589 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0011_auto_20190923_1157.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)      591 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0005_remove_ticketstatus_value.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)      917 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0010_auto_20190923_0930.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)      153 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1582 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0015_auto_20191001_0847.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1612 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0007_auto_20190917_1009.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1470 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0004_auto_20190913_1425.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)      627 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0013_auto_20190923_1439.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)      668 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0002_ticket_ticket_number.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3136 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0009_auto_20190918_1525.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1649 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0006_auto_20190916_1645.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)      337 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0005_remove_ticketstatus_value.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      360 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0011_auto_20190923_1157.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2019-09-05 17:26:40.000000 django-autotask-0.0.9a0/djautotask/migrations/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1640 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0007_auto_20190917_1009.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      441 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0009_auto_20190920_1648.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4964 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0009_auto_20190918_1525.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      287 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0006_merge_20190920_1450.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1036 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0010_auto_20190923_0930.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1723 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0006_auto_20190916_1645.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      446 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0013_auto_20190923_1439.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      280 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0012_merge_20190923_1439.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      281 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0008_merge_20190920_1644.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1715 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0003_auto_20190913_0941.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1517 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0005_auto_20190916_1549.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      407 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0002_ticket_ticket_number.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/__pycache__/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     8811 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/__pycache__/models.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2949 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/__pycache__/api.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)      683 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/__pycache__/utils.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)      332 2019-10-08 23:20:52.000000 django-autotask-0.0.9a0/djautotask/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)    16255 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/__pycache__/sync.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     6563 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/models.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      226 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/__init__.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/tests/
+-rw-rw-r--   0 sam       (1000) sam       (1000)    11643 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/tests/fixtures.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)   174033 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/tests/atws.wsdl
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/
+-rw-rw-r--   0 sam       (1000) sam       (1000)    10185 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/test_commands.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     7853 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/fixture_utils.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     7163 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/fixtures.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)    18302 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/test_sync.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1836 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/mocks.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)      363 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/test_model.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)      148 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)       72 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/tests/test_model.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     8875 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/tests/test_commands.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2019-09-05 17:26:40.000000 django-autotask-0.0.9a0/djautotask/tests/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1516 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/tests/mocks.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    15091 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/tests/test_sync.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     7839 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/tests/fixture_utils.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3236 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/admin.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    16965 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/sync.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/management/
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/management/__pycache__/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      153 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/management/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/management/__init__.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/management/commands/
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/management/commands/__pycache__/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     4469 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/management/commands/__pycache__/atsync.cpython-35.pyc
+-rw-rw-r--   0 sam       (1000) sam       (1000)     5350 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/management/commands/atsync.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      384 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/utils.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3005 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/api.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1797 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/setup.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)       38 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/setup.cfg
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2385 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/PKG-INFO
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/django_autotask.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3978 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/django_autotask.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/django_autotask.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2385 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/django_autotask.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)       97 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/django_autotask.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       11 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/django_autotask.egg-info/top_level.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/django_autotask.egg-info/not-zip-safe
+-rw-rw-r--   0 sam       (1000) sam       (1000)      945 2019-09-05 17:26:40.000000 django-autotask-0.0.9a0/README.md
+-rw-rw-r--   0 sam       (1000) sam       (1000)       82 2019-09-05 17:26:40.000000 django-autotask-0.0.9a0/MANIFEST.in
```

### Comparing `django-autotask-0.0.99a0/djautotask/tests/atws.wsdl` & `django-autotask-0.0.9a0/djautotask/tests/atws.wsdl`

 * *Files 0% similar despite different names*

#### Comparing `django-autotask-0.0.99a0/djautotask/tests/atws.wsdl` & `django-autotask-0.0.9a0/djautotask/tests/atws.wsdl`

```diff
@@ -104,15 +104,15 @@
           <s:element minOccurs="0" maxOccurs="1" name="Description" type="s:string"/>
           <s:element minOccurs="1" maxOccurs="1" name="IsRequired" type="s:boolean"/>
           <s:element minOccurs="1" maxOccurs="1" name="IsReadOnly" type="s:boolean"/>
           <s:element minOccurs="1" maxOccurs="1" name="IsQueryable" type="s:boolean"/>
           <s:element minOccurs="1" maxOccurs="1" name="IsReference" type="s:boolean"/>
           <s:element minOccurs="0" maxOccurs="1" name="ReferenceEntityType" type="s:string"/>
           <s:element minOccurs="1" maxOccurs="1" name="IsPickList" type="s:boolean"/>
-          <s:element minOccurs="1" maxOccurs="1" name="PicklistValues" type="tns:ArrayOfPickListValue"/>
+          <s:element minOccurs="0" maxOccurs="1" name="PicklistValues" type="tns:ArrayOfPickListValue"/>
           <s:element minOccurs="0" maxOccurs="1" name="PicklistParentValueField" type="s:string"/>
           <s:element minOccurs="0" maxOccurs="1" name="DefaultValue" type="s:string"/>
         </s:sequence>
       </s:complexType>
       <s:complexType name="ArrayOfPickListValue">
         <s:sequence>
           <s:element minOccurs="0" maxOccurs="unbounded" name="PickListValue" nillable="true" type="tns:PickListValue"/>
```

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/0024_auto_20191122_1516.py` & `django-autotask-0.0.9a0/djautotask/migrations/0009_auto_20190918_1525.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,92 @@
-# Generated by Django 2.1.14 on 2019-11-22 15:16
+# Generated by Django 2.1.11 on 2019-09-18 15:25
 
 from django.db import migrations, models
 import django.db.models.deletion
 import django_extensions.db.fields
 
 
 class Migration(migrations.Migration):
-    atomic = False
+
     dependencies = [
-        ('djautotask', '0023_auto_20191119_0923'),
+        ('djautotask', '0008_auto_20190917_1454'),
     ]
 
     operations = [
-        migrations.RenameModel(
-            old_name='TicketStatus',
-            new_name='Status',
-        ),
-        migrations.AlterModelOptions(
-            name='status',
-            options={'verbose_name_plural': 'Statuses'},
-        ),
         migrations.CreateModel(
-            name='Task',
+            name='Project',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created', django_extensions.db.fields.CreationDateTimeField(auto_now_add=True, verbose_name='created')),
                 ('modified', django_extensions.db.fields.ModificationDateTimeField(auto_now=True, verbose_name='modified')),
-                ('title', models.CharField(blank=True, max_length=255, null=True)),
-                ('number', models.CharField(blank=True, max_length=50, null=True)),
-                ('description', models.CharField(blank=True, max_length=8000, null=True)),
-                ('completed_date', models.DateTimeField(blank=True, null=True)),
-                ('create_date', models.DateTimeField(blank=True, null=True)),
-                ('start_date', models.DateTimeField(blank=True, null=True)),
-                ('end_date', models.DateTimeField(blank=True, null=True)),
-                ('estimated_hours', models.PositiveIntegerField(default=0)),
-                ('remaining_hours', models.PositiveIntegerField(default=0)),
-                ('last_activity_date', models.DateTimeField(blank=True, null=True)),
-                ('assigned_resource', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.Resource')),
-                ('priority_label', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.TicketPriority')),
-                ('project', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.Project')),
+                ('name', models.CharField(max_length=100)),
+                ('number', models.CharField(max_length=50, null=True)),
+                ('description', models.CharField(max_length=2000)),
+                ('actual_hours', models.DecimalField(decimal_places=2, max_digits=9, null=True)),
+                ('completed_date_time', models.DateTimeField(null=True)),
+                ('completed_percentage', models.PositiveSmallIntegerField(default=0)),
+                ('duration', models.PositiveSmallIntegerField(default=0)),
+                ('start_date_time', models.DateTimeField(null=True)),
+                ('end_date_time', models.DateTimeField(null=True)),
+                ('estimated_time', models.DecimalField(decimal_places=2, max_digits=9, null=True)),
+                ('last_activity_date_time', models.DateTimeField(null=True)),
+                ('account', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.Account')),
+                ('project_lead_resource', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.Resource')),
             ],
             options={
                 'ordering': ('-modified', '-created'),
                 'get_latest_by': 'modified',
                 'abstract': False,
             },
         ),
         migrations.CreateModel(
-            name='TaskSecondaryResource',
+            name='ProjectStatus',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created', django_extensions.db.fields.CreationDateTimeField(auto_now_add=True, verbose_name='created')),
                 ('modified', django_extensions.db.fields.ModificationDateTimeField(auto_now=True, verbose_name='modified')),
-                ('resource', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.Resource')),
-                ('task', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.Task')),
+                ('value', models.CharField(blank=True, max_length=50, null=True)),
+                ('label', models.CharField(blank=True, max_length=50, null=True)),
+                ('is_default_value', models.BooleanField(default=False)),
+                ('sort_order', models.PositiveSmallIntegerField(blank=True, null=True)),
+                ('parent_value', models.CharField(blank=True, max_length=20, null=True)),
+                ('is_active', models.BooleanField(default=False)),
+                ('is_system', models.BooleanField(default=False)),
+            ],
+            options={
+                'verbose_name_plural': 'Project statuses',
+            },
+        ),
+        migrations.CreateModel(
+            name='ProjectType',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('created', django_extensions.db.fields.CreationDateTimeField(auto_now_add=True, verbose_name='created')),
+                ('modified', django_extensions.db.fields.ModificationDateTimeField(auto_now=True, verbose_name='modified')),
+                ('value', models.CharField(blank=True, max_length=50, null=True)),
+                ('label', models.CharField(blank=True, max_length=50, null=True)),
+                ('is_default_value', models.BooleanField(default=False)),
+                ('sort_order', models.PositiveSmallIntegerField(blank=True, null=True)),
+                ('parent_value', models.CharField(blank=True, max_length=20, null=True)),
+                ('is_active', models.BooleanField(default=False)),
+                ('is_system', models.BooleanField(default=False)),
             ],
             options={
-                'ordering': ('-modified', '-created'),
-                'get_latest_by': 'modified',
                 'abstract': False,
             },
         ),
         migrations.AddField(
-            model_name='task',
+            model_name='project',
             name='status',
-            field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.Status'),
+            field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.ProjectStatus'),
+        ),
+        migrations.AddField(
+            model_name='project',
+            name='type',
+            field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.ProjectType'),
+        ),
+        migrations.AddField(
+            model_name='ticket',
+            name='project',
+            field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.Project'),
         ),
     ]
```

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/0006_auto_20190916_1645.py` & `django-autotask-0.0.9a0/djautotask/migrations/0006_auto_20190916_1645.py`

 * *Files identical despite different names*

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/0018_auto_20191029_1634.py` & `django-autotask-0.0.9a0/djautotask/migrations/0015_auto_20191001_0847.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# Generated by Django 2.1.11 on 2019-10-29 16:34
+# Generated by Django 2.1.11 on 2019-10-01 08:47
 
 from django.db import migrations, models
 import django.db.models.deletion
 import django_extensions.db.fields
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('djautotask', '0017_auto_20191021_1028'),
+        ('djautotask', '0014_auto_20190930_1548'),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='LicenseType',
+            name='DisplayColor',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created', django_extensions.db.fields.CreationDateTimeField(auto_now_add=True, verbose_name='created')),
                 ('modified', django_extensions.db.fields.ModificationDateTimeField(auto_now=True, verbose_name='modified')),
                 ('label', models.CharField(blank=True, max_length=50, null=True)),
                 ('is_default_value', models.BooleanField(default=False)),
                 ('sort_order', models.PositiveSmallIntegerField(blank=True, null=True)),
                 ('parent_value', models.CharField(blank=True, max_length=20, null=True)),
                 ('is_active', models.BooleanField(default=False)),
                 ('is_system', models.BooleanField(default=False)),
             ],
             options={
-                'abstract': False,
+                'verbose_name_plural': 'Display colors',
             },
         ),
         migrations.AddField(
-            model_name='resource',
-            name='license_type',
-            field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.LicenseType'),
+            model_name='ticketcategory',
+            name='display_color',
+            field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.DisplayColor'),
         ),
     ]
```

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0011_auto_20190923_1157.cpython-36.pyc` & `django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0012_merge_20190923_1439.cpython-35.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-00000000: 330d 0d0a f3f4 895f 6801 0000 e300 0000  3......_h.......
+00000000: 160d 0d0a 81dc 935d 1801 0000 e300 0000  .......]........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2200 0000 6400 6401 6c00 6d01 5a01  .s"...d.d.l.m.Z.
-00000030: 0100 4700 6402 6403 8400 6403 6501 6a02  ..G.d.d...d.e.j.
-00000040: 8303 5a02 6404 5300 2905 e900 0000 0029  ..Z.d.S.)......)
-00000050: 01da 0a6d 6967 7261 7469 6f6e 7363 0000  ...migrationsc..
-00000060: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
-00000070: 0000 7326 0000 0065 005a 0164 005a 0264  ..s&...e.Z.d.Z.d
-00000080: 0867 015a 0365 046a 0564 0364 0464 0569  .g.Z.e.j.d.d.d.i
-00000090: 0164 068d 0267 015a 0664 0753 0029 09da  .d...g.Z.d.S.)..
-000000a0: 094d 6967 7261 7469 6f6e da0a 646a 6175  .Migration..djau
-000000b0: 746f 7461 736b da18 3030 3130 5f6d 6572  totask..0010_mer
-000000c0: 6765 5f32 3031 3930 3932 335f 3131 3535  ge_20190923_1155
-000000d0: da05 7175 6575 65da 1376 6572 626f 7365  ..queue..verbose
-000000e0: 5f6e 616d 655f 706c 7572 616c da06 5175  _name_plural..Qu
-000000f0: 6575 6573 2902 da04 6e61 6d65 da07 6f70  eues)...name..op
-00000100: 7469 6f6e 734e 2902 7204 0000 0072 0500  tionsN).r....r..
-00000110: 0000 2907 da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
-00000120: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000130: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
-00000140: 656e 6369 6573 7202 0000 00da 1141 6c74  enciesr......Alt
-00000150: 6572 4d6f 6465 6c4f 7074 696f 6e73 da0a  erModelOptions..
-00000160: 6f70 6572 6174 696f 6e73 a900 7211 0000  operations..r...
-00000170: 0072 1100 0000 fa55 2f68 6f6d 652f 7361  .r.....U/home/sa
-00000180: 6d2f 6769 742f 4b61 6e62 616e 2f64 6a61  m/git/Kanban/dja
-00000190: 6e67 6f2d 6175 746f 7461 736b 2f64 6a61  ngo-autotask/dja
-000001a0: 7574 6f74 6173 6b2f 6d69 6772 6174 696f  utotask/migratio
-000001b0: 6e73 2f30 3031 315f 6175 746f 5f32 3031  ns/0011_auto_201
-000001c0: 3930 3932 335f 3131 3537 2e70 7972 0300  90923_1157.pyr..
-000001d0: 0000 0600 0000 7308 0000 0008 0306 0404  ......s.........
-000001e0: 0102 0172 0300 0000 4e29 03da 0964 6a61  ...r....N)...dja
-000001f0: 6e67 6f2e 6462 7202 0000 0072 0300 0000  ngo.dbr....r....
-00000200: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00000210: 1200 0000 da08 3c6d 6f64 756c 653e 0300  ......<module>..
-00000220: 0000 7302 0000 000c 03                   ..s......
+00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
+00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
+00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
+00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
+00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
+00000070: 0000 0000 0003 0000 0040 0000 0073 2200  .........@...s".
+00000080: 0000 6500 005a 0100 6400 005a 0200 6405  ..e..Z..d..Z..d.
+00000090: 0064 0600 6702 005a 0300 6700 005a 0400  .d..g..Z..g..Z..
+000000a0: 6404 0053 2907 da09 4d69 6772 6174 696f  d..S)...Migratio
+000000b0: 6eda 0a64 6a61 7574 6f74 6173 6bda 1730  n..djautotask..0
+000000c0: 3031 305f 6175 746f 5f32 3031 3930 3932  010_auto_2019092
+000000d0: 335f 3039 3330 da17 3030 3131 5f61 7574  3_0930..0011_aut
+000000e0: 6f5f 3230 3139 3039 3233 5f31 3135 374e  o_20190923_1157N
+000000f0: 2902 fa0a 646a 6175 746f 7461 736b 7205  )...djautotaskr.
+00000100: 0000 0029 0272 0700 0000 7a17 3030 3131  ...).r....z.0011
+00000110: 5f61 7574 6f5f 3230 3139 3039 3233 5f31  _auto_20190923_1
+00000120: 3135 3729 05da 085f 5f6e 616d 655f 5fda  157)...__name__.
+00000130: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000140: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
+00000150: 6465 6e63 6965 73da 0a6f 7065 7261 7469  dencies..operati
+00000160: 6f6e 73a9 0072 0d00 0000 720d 0000 00fa  ons..r....r.....
+00000170: 562f 686f 6d65 2f73 616d 2f67 6974 2f4b  V/home/sam/git/K
+00000180: 616e 6261 6e2f 646a 616e 676f 2d61 7574  anban/django-aut
+00000190: 6f74 6173 6b2f 646a 6175 746f 7461 736b  otask/djautotask
+000001a0: 2f6d 6967 7261 7469 6f6e 732f 3030 3132  /migrations/0012
+000001b0: 5f6d 6572 6765 5f32 3031 3930 3932 335f  _merge_20190923_
+000001c0: 3134 3339 2e70 7972 0300 0000 0600 0000  1439.pyr........
+000001d0: 7306 0000 000c 0303 0109 0372 0300 0000  s..........r....
+000001e0: 4e29 03da 0964 6a61 6e67 6f2e 6462 7202  N)...django.dbr.
+000001f0: 0000 0072 0300 0000 720d 0000 0072 0d00  ...r....r....r..
+00000200: 0000 720d 0000 0072 0e00 0000 da08 3c6d  ..r....r......<m
+00000210: 6f64 756c 653e 0300 0000 7302 0000 0010  odule>....s.....
+00000220: 03                                       .
```

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0076_auto_20200925_1326.cpython-36.pyc` & `django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0002_ticket_ticket_number.cpython-35.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,42 @@
-00000000: 330d 0d0a f3f4 895f d603 0000 e300 0000  3......_........
+00000000: 160d 0d0a 81dc 935d 9701 0000 e300 0000  .......]........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2e00 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
-00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 4700  m.Z...d.d.l.Z.G.
-00000040: 6403 6404 8400 6404 6501 6a05 8303 5a05  d.d...d.e.j...Z.
-00000050: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
-00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
-00000070: 734e 6300 0000 0000 0000 0000 0000 000c  sNc.............
-00000080: 0000 0040 0000 0073 7200 0000 6500 5a01  ...@...sr...e.Z.
-00000090: 6400 5a02 6410 6701 5a03 6504 6a05 6403  d.Z.d.g.Z.e.j.d.
-000000a0: 6404 6411 6901 6406 8d02 6504 6a06 6403  d.d.i.d...e.j.d.
-000000b0: 6407 6507 6a08 6408 6408 6509 6a0a 6a07  d.e.j.d.d.e.j.j.
-000000c0: 6a0b 6a0c 6409 640a 640b 8d05 640c 8d03  j.j.d.d.d...d...
-000000d0: 6504 6a06 6403 640d 6507 6a08 6408 6408  e.j.d.d.e.j.d.d.
-000000e0: 6509 6a0a 6a07 6a0b 6a0c 640e 640a 640b  e.j.j.j.j.d.d.d.
-000000f0: 8d05 640c 8d03 6703 5a0d 640f 5300 2912  ..d...g.Z.d.S.).
-00000100: da09 4d69 6772 6174 696f 6eda 0a64 6a61  ..Migration..dja
-00000110: 7574 6f74 6173 6bda 1430 3037 355f 7461  utotask..0075_ta
-00000120: 736b 7072 6564 6563 6573 736f 725a 0f74  skpredecessorZ.t
-00000130: 6173 6b70 7265 6465 6365 7373 6f72 da08  askpredecessor..
-00000140: 6f72 6465 7269 6e67 da17 7072 6564 6563  ordering..predec
-00000150: 6573 736f 725f 7461 736b 5f5f 7469 746c  essor_task__titl
-00000160: 6529 02da 046e 616d 65da 076f 7074 696f  e)...name..optio
-00000170: 6e73 da10 7072 6564 6563 6573 736f 725f  ns..predecessor_
-00000180: 7461 736b 54da 1470 7265 6465 6365 7373  taskT..predecess
-00000190: 6f72 5f74 6173 6b5f 7365 747a 0f64 6a61  or_task_setz.dja
-000001a0: 7574 6f74 6173 6b2e 5461 736b 2905 da05  utotask.Task)...
-000001b0: 626c 616e 6bda 046e 756c 6cda 096f 6e5f  blank..null..on_
-000001c0: 6465 6c65 7465 da0c 7265 6c61 7465 645f  delete..related_
-000001d0: 6e61 6d65 da02 746f 2903 da0a 6d6f 6465  name..to)...mode
-000001e0: 6c5f 6e61 6d65 7209 0000 00da 0566 6965  l_namer......fie
-000001f0: 6c64 da0e 7375 6363 6573 736f 725f 7461  ld..successor_ta
-00000200: 736b da12 7375 6363 6573 736f 725f 7461  sk..successor_ta
-00000210: 736b 5f73 6574 4e29 0272 0500 0000 7206  sk_setN).r....r.
-00000220: 0000 0029 0172 0800 0000 290e da08 5f5f  ...).r....)...__
-00000230: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000240: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000250: da0c 6465 7065 6e64 656e 6369 6573 7202  ..dependenciesr.
-00000260: 0000 00da 1141 6c74 6572 4d6f 6465 6c4f  .....AlterModelO
-00000270: 7074 696f 6e73 da0a 416c 7465 7246 6965  ptions..AlterFie
-00000280: 6c64 7203 0000 00da 0a46 6f72 6569 676e  ldr......Foreign
-00000290: 4b65 79da 0664 6a61 6e67 6fda 0264 62da  Key..django..db.
-000002a0: 0864 656c 6574 696f 6eda 0743 4153 4341  .deletion..CASCA
-000002b0: 4445 da0a 6f70 6572 6174 696f 6e73 a900  DE..operations..
-000002c0: 7222 0000 0072 2200 0000 fa55 2f68 6f6d  r"...r"....U/hom
-000002d0: 652f 7361 6d2f 6769 742f 4b61 6e62 616e  e/sam/git/Kanban
-000002e0: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
-000002f0: 2f64 6a61 7574 6f74 6173 6b2f 6d69 6772  /djautotask/migr
-00000300: 6174 696f 6e73 2f30 3037 365f 6175 746f  ations/0076_auto
-00000310: 5f32 3032 3030 3932 355f 3133 3236 2e70  _20200925_1326.p
-00000320: 7972 0400 0000 0700 0000 7318 0000 0008  yr........s.....
-00000330: 0306 0404 0102 010a 0204 0102 0102 011e  ................
-00000340: 0204 0102 0102 0172 0400 0000 2906 da09  .......r....)...
-00000350: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
-00000360: 0000 00da 1964 6a61 6e67 6f2e 6462 2e6d  .....django.db.m
-00000370: 6f64 656c 732e 6465 6c65 7469 6f6e 721d  odels.deletionr.
-00000380: 0000 0072 0400 0000 7222 0000 0072 2200  ...r....r"...r".
-00000390: 0000 7222 0000 0072 2300 0000 da08 3c6d  ..r"...r#.....<m
-000003a0: 6f64 756c 653e 0300 0000 7304 0000 0010  odule>....s.....
-000003b0: 0108 03                                  ...
+00000020: 0073 3300 0000 6400 0064 0100 6c00 006d  .s3...d..d..l..m
+00000030: 0100 5a01 006d 0200 5a02 0001 4764 0200  ..Z..m..Z...Gd..
+00000040: 6403 0084 0000 6403 0065 0100 6a03 0083  d.....d..e..j...
+00000050: 0300 5a03 0064 0400 5329 05e9 0000 0000  ..Z..d..S)......
+00000060: 2902 da0a 6d69 6772 6174 696f 6e73 da06  )...migrations..
+00000070: 6d6f 6465 6c73 6300 0000 0000 0000 0000  modelsc.........
+00000080: 0000 000d 0000 0040 0000 0073 5200 0000  .......@...sR...
+00000090: 6500 005a 0100 6400 005a 0200 640e 0067  e..Z..d..Z..d..g
+000000a0: 0100 5a03 0065 0400 6a05 0064 0300 6404  ..Z..e..j..d..d.
+000000b0: 0064 0500 6406 0064 0700 6506 006a 0700  .d..d..d..e..j..
+000000c0: 6408 0064 0900 640a 0064 0b00 640c 0064  d..d..d..d..d..d
+000000d0: 0900 8300 0383 0003 6701 005a 0800 640d  ........g..Z..d.
+000000e0: 0053 290f da09 4d69 6772 6174 696f 6eda  .S)...Migration.
+000000f0: 0a64 6a61 7574 6f74 6173 6bda 0c30 3030  .djautotask..000
+00000100: 315f 696e 6974 6961 6cda 0a6d 6f64 656c  1_initial..model
+00000110: 5f6e 616d 65da 0674 6963 6b65 74da 046e  _name..ticket..n
+00000120: 616d 65da 0d74 6963 6b65 745f 6e75 6d62  ame..ticket_numb
+00000130: 6572 da05 6669 656c 64da 0562 6c61 6e6b  er..field..blank
+00000140: 54da 0a6d 6178 5f6c 656e 6774 68e9 3200  T..max_length.2.
+00000150: 0000 da04 6e75 6c6c 4e29 027a 0a64 6a61  ....nullN).z.dja
+00000160: 7574 6f74 6173 6b7a 0c30 3030 315f 696e  utotaskz.0001_in
+00000170: 6974 6961 6c29 09da 085f 5f6e 616d 655f  itial)...__name_
+00000180: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000190: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
+000001a0: 656e 6465 6e63 6965 7372 0200 0000 da08  endenciesr......
+000001b0: 4164 6446 6965 6c64 7203 0000 00da 0943  AddFieldr......C
+000001c0: 6861 7246 6965 6c64 da0a 6f70 6572 6174  harField..operat
+000001d0: 696f 6e73 a900 7217 0000 0072 1700 0000  ions..r....r....
+000001e0: fa57 2f68 6f6d 652f 7361 6d2f 6769 742f  .W/home/sam/git/
+000001f0: 4b61 6e62 616e 2f64 6a61 6e67 6f2d 6175  Kanban/django-au
+00000200: 746f 7461 736b 2f64 6a61 7574 6f74 6173  totask/djautotas
+00000210: 6b2f 6d69 6772 6174 696f 6e73 2f30 3030  k/migrations/000
+00000220: 325f 7469 636b 6574 5f74 6963 6b65 745f  2_ticket_ticket_
+00000230: 6e75 6d62 6572 2e70 7972 0400 0000 0600  number.pyr......
+00000240: 0000 730a 0000 000c 0309 0409 0106 0106  ..s.............
+00000250: 0172 0400 0000 4e29 04da 0964 6a61 6e67  .r....N)...djang
+00000260: 6f2e 6462 7202 0000 0072 0300 0000 7204  o.dbr....r....r.
+00000270: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
+00000280: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000290: 3e03 0000 0073 0200 0000 1603            >....s......
```

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0050_remove_ticket_role.cpython-36.pyc` & `django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0008_merge_20190920_1644.cpython-35.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-00000000: 330d 0d0a f3f4 895f 4b01 0000 e300 0000  3......_K.......
+00000000: 160d 0d0a 81dc 935d 1901 0000 e300 0000  .......]........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2200 0000 6400 6401 6c00 6d01 5a01  .s"...d.d.l.m.Z.
-00000030: 0100 4700 6402 6403 8400 6403 6501 6a02  ..G.d.d...d.e.j.
-00000040: 8303 5a02 6404 5300 2905 e900 0000 0029  ..Z.d.S.)......)
-00000050: 01da 0a6d 6967 7261 7469 6f6e 7363 0000  ...migrationsc..
-00000060: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
-00000070: 0000 7322 0000 0065 005a 0164 005a 0264  ..s"...e.Z.d.Z.d
-00000080: 0767 015a 0365 046a 0564 0364 0464 058d  .g.Z.e.j.d.d.d..
-00000090: 0267 015a 0664 0653 0029 08da 094d 6967  .g.Z.d.S.)...Mig
-000000a0: 7261 7469 6f6e da0a 646a 6175 746f 7461  ration..djautota
-000000b0: 736b da18 3030 3439 5f6d 6572 6765 5f32  sk..0049_merge_2
-000000c0: 3032 3030 3232 375f 3137 3031 da06 7469  0200227_1701..ti
-000000d0: 636b 6574 da04 726f 6c65 2902 da0a 6d6f  cket..role)...mo
-000000e0: 6465 6c5f 6e61 6d65 da04 6e61 6d65 4e29  del_name..nameN)
-000000f0: 0272 0400 0000 7205 0000 0029 07da 085f  .r....r....)..._
-00000100: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000110: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000120: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
-00000130: 0200 0000 da0b 5265 6d6f 7665 4669 656c  ......RemoveFiel
-00000140: 64da 0a6f 7065 7261 7469 6f6e 73a9 0072  d..operations..r
-00000150: 1000 0000 7210 0000 00fa 552f 686f 6d65  ....r.....U/home
-00000160: 2f73 616d 2f67 6974 2f4b 616e 6261 6e2f  /sam/git/Kanban/
-00000170: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
-00000180: 646a 6175 746f 7461 736b 2f6d 6967 7261  djautotask/migra
-00000190: 7469 6f6e 732f 3030 3530 5f72 656d 6f76  tions/0050_remov
-000001a0: 655f 7469 636b 6574 5f72 6f6c 652e 7079  e_ticket_role.py
-000001b0: 7203 0000 0006 0000 0073 0800 0000 0803  r........s......
-000001c0: 0604 0401 0201 7203 0000 004e 2903 da09  ......r....N)...
-000001d0: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
-000001e0: 0000 0072 1000 0000 7210 0000 0072 1000  ...r....r....r..
-000001f0: 0000 7211 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000200: 3e03 0000 0073 0200 0000 0c03            >....s......
+00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
+00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
+00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
+00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
+00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
+00000070: 0000 0000 0003 0000 0040 0000 0073 2200  .........@...s".
+00000080: 0000 6500 005a 0100 6400 005a 0200 6405  ..e..Z..d..Z..d.
+00000090: 0064 0600 6702 005a 0300 6700 005a 0400  .d..g..Z..g..Z..
+000000a0: 6404 0053 2907 da09 4d69 6772 6174 696f  d..S)...Migratio
+000000b0: 6eda 0a64 6a61 7574 6f74 6173 6bda 1730  n..djautotask..0
+000000c0: 3030 375f 6175 746f 5f32 3031 3930 3931  007_auto_2019091
+000000d0: 375f 3130 3039 da18 3030 3036 5f6d 6572  7_1009..0006_mer
+000000e0: 6765 5f32 3031 3930 3932 305f 3134 3530  ge_20190920_1450
+000000f0: 4e29 02fa 0a64 6a61 7574 6f74 6173 6b72  N)...djautotaskr
+00000100: 0500 0000 2902 7207 0000 007a 1830 3030  ....).r....z.000
+00000110: 365f 6d65 7267 655f 3230 3139 3039 3230  6_merge_20190920
+00000120: 5f31 3435 3029 05da 085f 5f6e 616d 655f  _1450)...__name_
+00000130: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000140: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
+00000150: 656e 6465 6e63 6965 73da 0a6f 7065 7261  endencies..opera
+00000160: 7469 6f6e 73a9 0072 0d00 0000 720d 0000  tions..r....r...
+00000170: 00fa 562f 686f 6d65 2f73 616d 2f67 6974  ..V/home/sam/git
+00000180: 2f4b 616e 6261 6e2f 646a 616e 676f 2d61  /Kanban/django-a
+00000190: 7574 6f74 6173 6b2f 646a 6175 746f 7461  utotask/djautota
+000001a0: 736b 2f6d 6967 7261 7469 6f6e 732f 3030  sk/migrations/00
+000001b0: 3038 5f6d 6572 6765 5f32 3031 3930 3932  08_merge_2019092
+000001c0: 305f 3136 3434 2e70 7972 0300 0000 0600  0_1644.pyr......
+000001d0: 0000 7306 0000 000c 0303 0109 0372 0300  ..s..........r..
+000001e0: 0000 4e29 03da 0964 6a61 6e67 6f2e 6462  ..N)...django.db
+000001f0: 7202 0000 0072 0300 0000 720d 0000 0072  r....r....r....r
+00000200: 0d00 0000 720d 0000 0072 0e00 0000 da08  ....r....r......
+00000210: 3c6d 6f64 756c 653e 0300 0000 7302 0000  <module>....s...
+00000220: 0010 03                                  ...
```

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0009_auto_20190920_1648.cpython-36.pyc` & `django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0009_auto_20190920_1648.cpython-35.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-00000000: 330d 0d0a f3f4 895f b901 0000 e300 0000  3......_........
+00000000: 160d 0d0a 81dc 935d b901 0000 e300 0000  .......]........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2200 0000 6400 6401 6c00 6d01 5a01  .s"...d.d.l.m.Z.
-00000030: 0100 4700 6402 6403 8400 6403 6501 6a02  ..G.d.d...d.e.j.
-00000040: 8303 5a02 6404 5300 2905 e900 0000 0029  ..Z.d.S.)......)
-00000050: 01da 0a6d 6967 7261 7469 6f6e 7363 0000  ...migrationsc..
-00000060: 0000 0000 0000 0000 0000 0500 0000 4000  ..............@.
-00000070: 0000 732e 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00000080: 0867 015a 0365 046a 0564 0364 0464 058d  .g.Z.e.j.d.d.d..
-00000090: 0265 046a 0564 0664 0464 058d 0267 025a  .e.j.d.d.d...g.Z
-000000a0: 0664 0753 0029 09da 094d 6967 7261 7469  .d.S.)...Migrati
-000000b0: 6f6e da0a 646a 6175 746f 7461 736b da18  on..djautotask..
-000000c0: 3030 3038 5f6d 6572 6765 5f32 3031 3930  0008_merge_20190
-000000d0: 3932 305f 3136 3434 da05 7175 6575 65da  920_1644..queue.
-000000e0: 0576 616c 7565 2902 da0a 6d6f 6465 6c5f  .value)...model_
-000000f0: 6e61 6d65 da04 6e61 6d65 da0e 7469 636b  name..name..tick
-00000100: 6574 7072 696f 7269 7479 4e29 0272 0400  etpriorityN).r..
-00000110: 0000 7205 0000 0029 07da 085f 5f6e 616d  ..r....)...__nam
-00000120: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000130: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
-00000140: 6570 656e 6465 6e63 6965 7372 0200 0000  ependenciesr....
-00000150: da0b 5265 6d6f 7665 4669 656c 64da 0a6f  ..RemoveField..o
-00000160: 7065 7261 7469 6f6e 73a9 0072 1100 0000  perations..r....
-00000170: 7211 0000 00fa 552f 686f 6d65 2f73 616d  r.....U/home/sam
-00000180: 2f67 6974 2f4b 616e 6261 6e2f 646a 616e  /git/Kanban/djan
-00000190: 676f 2d61 7574 6f74 6173 6b2f 646a 6175  go-autotask/djau
-000001a0: 746f 7461 736b 2f6d 6967 7261 7469 6f6e  totask/migration
-000001b0: 732f 3030 3039 5f61 7574 6f5f 3230 3139  s/0009_auto_2019
-000001c0: 3039 3230 5f31 3634 382e 7079 7203 0000  0920_1648.pyr...
-000001d0: 0006 0000 0073 0e00 0000 0803 0604 0401  .....s..........
-000001e0: 0201 0602 0401 0201 7203 0000 004e 2903  ........r....N).
-000001f0: da09 646a 616e 676f 2e64 6272 0200 0000  ..django.dbr....
-00000200: 7203 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00000210: 1100 0000 7212 0000 00da 083c 6d6f 6475  ....r......<modu
-00000220: 6c65 3e03 0000 0073 0200 0000 0c03       le>....s......
+00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
+00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
+00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
+00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
+00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
+00000070: 0000 0000 0006 0000 0040 0000 0073 4900  .........@...sI.
+00000080: 0000 6500 005a 0100 6400 005a 0200 6409  ..e..Z..d..Z..d.
+00000090: 0067 0100 5a03 0065 0400 6a05 0064 0300  .g..Z..e..j..d..
+000000a0: 6404 0064 0500 6406 0083 0002 6504 006a  d..d..d.....e..j
+000000b0: 0500 6403 0064 0700 6405 0064 0600 8300  ..d..d..d..d....
+000000c0: 0267 0200 5a06 0064 0800 5329 0ada 094d  .g..Z..d..S)...M
+000000d0: 6967 7261 7469 6f6e da0a 646a 6175 746f  igration..djauto
+000000e0: 7461 736b da18 3030 3038 5f6d 6572 6765  task..0008_merge
+000000f0: 5f32 3031 3930 3932 305f 3136 3434 da0a  _20190920_1644..
+00000100: 6d6f 6465 6c5f 6e61 6d65 da05 7175 6575  model_name..queu
+00000110: 65da 046e 616d 65da 0576 616c 7565 5a0e  e..name..valueZ.
+00000120: 7469 636b 6574 7072 696f 7269 7479 4e29  ticketpriorityN)
+00000130: 027a 0a64 6a61 7574 6f74 6173 6b72 0500  .z.djautotaskr..
+00000140: 0000 2907 da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+00000150: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000160: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
+00000170: 656e 6369 6573 7202 0000 00da 0b52 656d  enciesr......Rem
+00000180: 6f76 6546 6965 6c64 da0a 6f70 6572 6174  oveField..operat
+00000190: 696f 6e73 a900 7210 0000 0072 1000 0000  ions..r....r....
+000001a0: fa55 2f68 6f6d 652f 7361 6d2f 6769 742f  .U/home/sam/git/
+000001b0: 4b61 6e62 616e 2f64 6a61 6e67 6f2d 6175  Kanban/django-au
+000001c0: 746f 7461 736b 2f64 6a61 7574 6f74 6173  totask/djautotas
+000001d0: 6b2f 6d69 6772 6174 696f 6e73 2f30 3030  k/migrations/000
+000001e0: 395f 6175 746f 5f32 3031 3930 3932 305f  9_auto_20190920_
+000001f0: 3136 3438 2e70 7972 0300 0000 0600 0000  1648.pyr........
+00000200: 730e 0000 000c 0309 0409 0106 0106 0209  s...............
+00000210: 0106 0172 0300 0000 4e29 03da 0964 6a61  ...r....N)...dja
+00000220: 6e67 6f2e 6462 7202 0000 0072 0300 0000  ngo.dbr....r....
+00000230: 7210 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
+00000240: 1100 0000 da08 3c6d 6f64 756c 653e 0300  ......<module>..
+00000250: 0000 7302 0000 0010 03                   ..s......
```

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0075_taskpredecessor.cpython-36.pyc` & `django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0015_auto_20191001_0847.cpython-35.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,99 @@
-00000000: 330d 0d0a f3f4 895f 6905 0000 e300 0000  3......_i.......
+00000000: 160d 0d0a c519 9d5d 2f06 0000 e300 0000  .......]/.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3600 0000 6400 6401 6c00 6d01 5a01  .s6...d.d.l.m.Z.
-00000030: 6d02 5a02 0100 6400 6402 6c03 5a04 6400  m.Z...d.d.l.Z.d.
-00000040: 6402 6c05 5a06 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
-00000050: 6501 6a07 8303 5a07 6402 5300 2905 e900  e.j...Z.d.S.)...
-00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
-00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
-00000080: 0000 0000 0000 000f 0000 0040 0000 0073  ...........@...s
-00000090: b400 0000 6500 5a01 6400 5a02 6418 6701  ....e.Z.d.Z.d.g.
-000000a0: 5a03 6504 6a05 6403 6404 6506 6a07 6405  Z.e.j.d.d.e.j.d.
-000000b0: 6405 6406 6407 6408 8d04 6602 6409 6508  d.d.d.d...f.d.e.
-000000c0: 6a09 6a0a 6a0b 6405 6409 640a 8d02 6602  j.j.j.d.d.d...f.
-000000d0: 640b 6508 6a09 6a0a 6a0c 6405 640b 640c  d.e.j.j.j.d.d.d.
-000000e0: 8d02 6602 640d 6506 6a0d 6405 6405 640e  ..f.d.e.j.d.d.d.
-000000f0: 8d02 6602 640f 6506 6a0e 6405 6405 650f  ..f.d.e.j.d.d.e.
-00000100: 6a09 6a06 6a10 6a11 640f 6410 6411 8d05  j.j.j.j.d.d.d...
-00000110: 6602 6412 6506 6a0e 6405 6405 650f 6a09  f.d.e.j.d.d.e.j.
-00000120: 6a06 6a10 6a11 6412 6410 6411 8d05 6602  j.j.j.d.d.d...f.
-00000130: 6706 6419 640b 6406 6415 9c03 6416 8d03  g.d.d.d.d...d...
-00000140: 6701 5a12 6417 5300 291a da09 4d69 6772  g.Z.d.S.)...Migr
-00000150: 6174 696f 6eda 0a64 6a61 7574 6f74 6173  ation..djautotas
-00000160: 6bda 1730 3037 345f 6175 746f 5f32 3032  k..0074_auto_202
-00000170: 3030 3832 375f 3138 3138 da0f 5461 736b  00827_1818..Task
-00000180: 5072 6564 6563 6573 736f 72da 0269 6454  Predecessor..idT
-00000190: 46da 0249 4429 04da 0c61 7574 6f5f 6372  F..ID)...auto_cr
-000001a0: 6561 7465 64da 0b70 7269 6d61 7279 5f6b  eated..primary_k
-000001b0: 6579 da09 7365 7269 616c 697a 65da 0c76  ey..serialize..v
-000001c0: 6572 626f 7365 5f6e 616d 65da 0763 7265  erbose_name..cre
-000001d0: 6174 6564 2902 da0c 6175 746f 5f6e 6f77  ated)...auto_now
-000001e0: 5f61 6464 720d 0000 00da 086d 6f64 6966  _addr......modif
-000001f0: 6965 6429 02da 0861 7574 6f5f 6e6f 7772  ied)...auto_nowr
-00000200: 0d00 0000 da08 6c61 675f 6461 7973 2902  ......lag_days).
-00000210: da05 626c 616e 6bda 046e 756c 6cda 1070  ..blank..null..p
-00000220: 7265 6465 6365 7373 6f72 5f74 6173 6b7a  redecessor_taskz
-00000230: 0f64 6a61 7574 6f74 6173 6b2e 5461 736b  .djautotask.Task
-00000240: 2905 7213 0000 0072 1400 0000 da09 6f6e  ).r....r......on
-00000250: 5f64 656c 6574 65da 0c72 656c 6174 6564  _delete..related
-00000260: 5f6e 616d 65da 0274 6fda 0e73 7563 6365  _name..to..succe
-00000270: 7373 6f72 5f74 6173 6bfa 092d 6d6f 6469  ssor_task..-modi
-00000280: 6669 6564 fa08 2d63 7265 6174 6564 2903  fied..-created).
-00000290: da08 6f72 6465 7269 6e67 da0d 6765 745f  ..ordering..get_
-000002a0: 6c61 7465 7374 5f62 79da 0861 6273 7472  latest_by..abstr
-000002b0: 6163 7429 03da 046e 616d 65da 0666 6965  act)...name..fie
-000002c0: 6c64 73da 076f 7074 696f 6e73 4e29 0272  lds..optionsN).r
-000002d0: 0500 0000 7206 0000 0029 0272 1a00 0000  ....r....).r....
-000002e0: 721b 0000 0029 13da 085f 5f6e 616d 655f  r....)...__name_
-000002f0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000300: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
-00000310: 656e 6465 6e63 6965 7372 0200 0000 da0b  endenciesr......
-00000320: 4372 6561 7465 4d6f 6465 6c72 0300 0000  CreateModelr....
-00000330: da09 4175 746f 4669 656c 64da 1164 6a61  ..AutoField..dja
-00000340: 6e67 6f5f 6578 7465 6e73 696f 6e73 da02  ngo_extensions..
-00000350: 6462 7220 0000 00da 1543 7265 6174 696f  dbr .....Creatio
-00000360: 6e44 6174 6554 696d 6546 6965 6c64 da19  nDateTimeField..
-00000370: 4d6f 6469 6669 6361 7469 6f6e 4461 7465  ModificationDate
-00000380: 5469 6d65 4669 656c 64da 0c49 6e74 6567  TimeField..Integ
-00000390: 6572 4669 656c 64da 0a46 6f72 6569 676e  erField..Foreign
-000003a0: 4b65 79da 0664 6a61 6e67 6fda 0864 656c  Key..django..del
-000003b0: 6574 696f 6eda 0743 4153 4341 4445 da0a  etion..CASCADE..
-000003c0: 6f70 6572 6174 696f 6e73 a900 7232 0000  operations..r2..
-000003d0: 0072 3200 0000 fa52 2f68 6f6d 652f 7361  .r2....R/home/sa
-000003e0: 6d2f 6769 742f 4b61 6e62 616e 2f64 6a61  m/git/Kanban/dja
-000003f0: 6e67 6f2d 6175 746f 7461 736b 2f64 6a61  ngo-autotask/dja
-00000400: 7574 6f74 6173 6b2f 6d69 6772 6174 696f  utotask/migratio
-00000410: 6e73 2f30 3037 355f 7461 736b 7072 6564  ns/0075_taskpred
-00000420: 6563 6573 736f 722e 7079 7204 0000 0008  ecessor.pyr.....
-00000430: 0000 0073 1800 0000 0803 0604 0401 0202  ...s............
-00000440: 1401 1401 1401 1001 1e01 2003 0201 0201  .......... .....
-00000450: 7204 0000 0029 08da 0964 6a61 6e67 6f2e  r....)...django.
-00000460: 6462 7202 0000 0072 0300 0000 da19 646a  dbr....r......dj
-00000470: 616e 676f 2e64 622e 6d6f 6465 6c73 2e64  ango.db.models.d
-00000480: 656c 6574 696f 6e72 2e00 0000 da1b 646a  eletionr......dj
-00000490: 616e 676f 5f65 7874 656e 7369 6f6e 732e  ango_extensions.
-000004a0: 6462 2e66 6965 6c64 7372 2800 0000 7204  db.fieldsr(...r.
-000004b0: 0000 0072 3200 0000 7232 0000 0072 3200  ...r2...r2...r2.
-000004c0: 0000 7233 0000 00da 083c 6d6f 6475 6c65  ..r3.....<module
-000004d0: 3e03 0000 0073 0600 0000 1001 0801 0803  >....s..........
+00000020: 0073 4b00 0000 6400 0064 0100 6c00 006d  .sK...d..d..l..m
+00000030: 0100 5a01 006d 0200 5a02 0001 6400 0064  ..Z..m..Z...d..d
+00000040: 0200 6c03 005a 0400 6400 0064 0200 6c05  ..l..Z..d..d..l.
+00000050: 005a 0600 4764 0300 6404 0084 0000 6404  .Z..Gd..d.....d.
+00000060: 0065 0100 6a07 0083 0300 5a07 0064 0200  .e..j.....Z..d..
+00000070: 5329 05e9 0000 0000 2902 da0a 6d69 6772  S)......)...migr
+00000080: 6174 696f 6e73 da06 6d6f 6465 6c73 4e63  ations..modelsNc
+00000090: 0000 0000 0000 0000 0000 0000 1200 0000  ................
+000000a0: 4000 0000 7384 0100 0065 0000 5a01 0064  @...s....e..Z..d
+000000b0: 0000 5a02 0064 2900 6701 005a 0300 6504  ..Z..d).g..Z..e.
+000000c0: 006a 0500 6403 0064 0400 6405 0064 0600  .j..d..d..d..d..
+000000d0: 6506 006a 0700 6407 0064 0800 6409 0064  e..j..d..d..d..d
+000000e0: 0800 640a 0064 0b00 640c 0064 0d00 8300  ..d..d..d..d....
+000000f0: 0466 0200 640e 0065 0800 6a09 006a 0a00  .f..d..e..j..j..
+00000100: 6a0b 0064 0f00 6408 0064 0c00 640e 0083  j..d..d..d..d...
+00000110: 0002 6602 0064 1000 6508 006a 0900 6a0a  ..f..d..e..j..j.
+00000120: 006a 0c00 6411 0064 0800 640c 0064 1000  .j..d..d..d..d..
+00000130: 8300 0266 0200 6412 0065 0600 6a0d 0064  ...f..d..e..j..d
+00000140: 1300 6408 0064 1400 6415 0064 1600 6408  ..d..d..d..d..d.
+00000150: 0083 0003 6602 0064 1700 6506 006a 0e00  ....f..d..e..j..
+00000160: 6418 0064 0b00 8300 0166 0200 6419 0065  d..d.....f..d..e
+00000170: 0600 6a0f 0064 1300 6408 0064 1600 6408  ..j..d..d..d..d.
+00000180: 0083 0002 6602 0064 1a00 6506 006a 0d00  ....f..d..e..j..
+00000190: 6413 0064 0800 6414 0064 1b00 6416 0064  d..d..d..d..d..d
+000001a0: 0800 8300 0366 0200 641c 0065 0600 6a0e  .....f..d..e..j.
+000001b0: 0064 1800 640b 0083 0001 6602 0064 1d00  .d..d.....f..d..
+000001c0: 6506 006a 0e00 6418 0064 0b00 8300 0166  e..j..d..d.....f
+000001d0: 0200 6709 0064 1e00 641f 0064 2000 6901  ..g..d..d..d .i.
+000001e0: 0083 0003 6504 006a 1000 6421 0064 2200  ....e..j..d!.d".
+000001f0: 6403 0064 2300 6424 0065 0600 6a11 0064  d..d#.d$.e..j..d
+00000200: 1600 6408 0064 2500 6512 006a 0900 6a06  ..d..d%.e..j..j.
+00000210: 006a 1300 6a14 0064 2600 6427 0083 0003  .j..j..d&.d'....
+00000220: 8300 0367 0200 5a15 0064 2800 5329 2ada  ...g..Z..d(.S)*.
+00000230: 094d 6967 7261 7469 6f6e da0a 646a 6175  .Migration..djau
+00000240: 746f 7461 736b da17 3030 3134 5f61 7574  totask..0014_aut
+00000250: 6f5f 3230 3139 3039 3330 5f31 3534 38da  o_20190930_1548.
+00000260: 046e 616d 65da 0c44 6973 706c 6179 436f  .name..DisplayCo
+00000270: 6c6f 72da 0666 6965 6c64 73da 0269 64da  lor..fields..id.
+00000280: 0c61 7574 6f5f 6372 6561 7465 6454 da0b  .auto_createdT..
+00000290: 7072 696d 6172 795f 6b65 79da 0973 6572  primary_key..ser
+000002a0: 6961 6c69 7a65 46da 0c76 6572 626f 7365  ializeF..verbose
+000002b0: 5f6e 616d 65da 0249 44da 0763 7265 6174  _name..ID..creat
+000002c0: 6564 da0c 6175 746f 5f6e 6f77 5f61 6464  ed..auto_now_add
+000002d0: da08 6d6f 6469 6669 6564 da08 6175 746f  ..modified..auto
+000002e0: 5f6e 6f77 da05 6c61 6265 6cda 0562 6c61  _now..label..bla
+000002f0: 6e6b da0a 6d61 785f 6c65 6e67 7468 e932  nk..max_length.2
+00000300: 0000 00da 046e 756c 6cda 1069 735f 6465  .....null..is_de
+00000310: 6661 756c 745f 7661 6c75 65da 0764 6566  fault_value..def
+00000320: 6175 6c74 da0a 736f 7274 5f6f 7264 6572  ault..sort_order
+00000330: da0c 7061 7265 6e74 5f76 616c 7565 e914  ..parent_value..
+00000340: 0000 00da 0969 735f 6163 7469 7665 da09  .....is_active..
+00000350: 6973 5f73 7973 7465 6dda 076f 7074 696f  is_system..optio
+00000360: 6e73 da13 7665 7262 6f73 655f 6e61 6d65  ns..verbose_name
+00000370: 5f70 6c75 7261 6c7a 0e44 6973 706c 6179  _pluralz.Display
+00000380: 2063 6f6c 6f72 73da 0a6d 6f64 656c 5f6e   colors..model_n
+00000390: 616d 655a 0e74 6963 6b65 7463 6174 6567  ameZ.ticketcateg
+000003a0: 6f72 79da 0d64 6973 706c 6179 5f63 6f6c  ory..display_col
+000003b0: 6f72 da05 6669 656c 64da 096f 6e5f 6465  or..field..on_de
+000003c0: 6c65 7465 da02 746f 7a17 646a 6175 746f  lete..toz.djauto
+000003d0: 7461 736b 2e44 6973 706c 6179 436f 6c6f  task.DisplayColo
+000003e0: 724e 2902 7a0a 646a 6175 746f 7461 736b  rN).z.djautotask
+000003f0: 7206 0000 0029 16da 085f 5f6e 616d 655f  r....)...__name_
+00000400: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000410: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
+00000420: 656e 6465 6e63 6965 7372 0200 0000 da0b  endenciesr......
+00000430: 4372 6561 7465 4d6f 6465 6c72 0300 0000  CreateModelr....
+00000440: da09 4175 746f 4669 656c 64da 1164 6a61  ..AutoField..dja
+00000450: 6e67 6f5f 6578 7465 6e73 696f 6e73 da02  ngo_extensions..
+00000460: 6462 7209 0000 00da 1543 7265 6174 696f  dbr......Creatio
+00000470: 6e44 6174 6554 696d 6546 6965 6c64 da19  nDateTimeField..
+00000480: 4d6f 6469 6669 6361 7469 6f6e 4461 7465  ModificationDate
+00000490: 5469 6d65 4669 656c 64da 0943 6861 7246  TimeField..CharF
+000004a0: 6965 6c64 da0c 426f 6f6c 6561 6e46 6965  ield..BooleanFie
+000004b0: 6c64 da19 506f 7369 7469 7665 536d 616c  ld..PositiveSmal
+000004c0: 6c49 6e74 6567 6572 4669 656c 64da 0841  lIntegerField..A
+000004d0: 6464 4669 656c 64da 0a46 6f72 6569 676e  ddField..Foreign
+000004e0: 4b65 79da 0664 6a61 6e67 6fda 0864 656c  Key..django..del
+000004f0: 6574 696f 6eda 0853 4554 5f4e 554c 4cda  etion..SET_NULL.
+00000500: 0a6f 7065 7261 7469 6f6e 73a9 0072 3a00  .operations..r:.
+00000510: 0000 723a 0000 00fa 552f 686f 6d65 2f73  ..r:....U/home/s
+00000520: 616d 2f67 6974 2f4b 616e 6261 6e2f 646a  am/git/Kanban/dj
+00000530: 616e 676f 2d61 7574 6f74 6173 6b2f 646a  ango-autotask/dj
+00000540: 6175 746f 7461 736b 2f6d 6967 7261 7469  autotask/migrati
+00000550: 6f6e 732f 3030 3135 5f61 7574 6f5f 3230  ons/0015_auto_20
+00000560: 3139 3130 3031 5f30 3834 372e 7079 7204  191001_0847.pyr.
+00000570: 0000 0008 0000 0073 2200 0000 0c03 0904  .......s".......
+00000580: 0901 0602 2701 2101 2101 2101 1501 1b01  ....'.!.!.!.....
+00000590: 2101 1501 1b03 0c03 0901 0601 0601 7204  !.............r.
+000005a0: 0000 0029 08da 0964 6a61 6e67 6f2e 6462  ...)...django.db
+000005b0: 7202 0000 0072 0300 0000 da19 646a 616e  r....r......djan
+000005c0: 676f 2e64 622e 6d6f 6465 6c73 2e64 656c  go.db.models.del
+000005d0: 6574 696f 6e72 3600 0000 da1b 646a 616e  etionr6.....djan
+000005e0: 676f 5f65 7874 656e 7369 6f6e 732e 6462  go_extensions.db
+000005f0: 2e66 6965 6c64 7372 2d00 0000 7204 0000  .fieldsr-...r...
+00000600: 0072 3a00 0000 723a 0000 0072 3a00 0000  .r:...r:...r:...
+00000610: 723b 0000 00da 083c 6d6f 6475 6c65 3e03  r;.....<module>.
+00000620: 0000 0073 0600 0000 1601 0c01 0c03       ...s..........
```

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0023_auto_20191119_0923.cpython-36.pyc` & `django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0011_auto_20190923_1157.cpython-35.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-00000000: 330d 0d0a f3f4 895f 9101 0000 e300 0000  3......_........
+00000000: 160d 0d0a 81dc 935d 6801 0000 e300 0000  .......]h.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2600 0000 6400 6401 6c00 6d01 5a01  .s&...d.d.l.m.Z.
-00000030: 6d02 5a02 0100 4700 6402 6403 8400 6403  m.Z...G.d.d...d.
-00000040: 6501 6a03 8303 5a03 6404 5300 2905 e900  e.j...Z.d.S.)...
-00000050: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
-00000060: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
-00000070: 0000 0000 0000 0600 0000 4000 0000 732c  ..........@...s,
-00000080: 0000 0065 005a 0164 005a 0264 0967 015a  ...e.Z.d.Z.d.g.Z
-00000090: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
-000000a0: 068d 0164 078d 0367 015a 0864 0853 0029  ...d...g.Z.d.S.)
-000000b0: 0ada 094d 6967 7261 7469 6f6e da0a 646a  ...Migration..dj
-000000c0: 6175 746f 7461 736b da18 3030 3232 5f6d  autotask..0022_m
-000000d0: 6572 6765 5f32 3031 3931 3033 315f 3136  erge_20191031_16
-000000e0: 3230 da07 7072 6f6a 6563 74da 0864 7572  20..project..dur
-000000f0: 6174 696f 6e72 0100 0000 2901 da07 6465  ationr....)...de
-00000100: 6661 756c 7429 03da 0a6d 6f64 656c 5f6e  fault)...model_n
-00000110: 616d 65da 046e 616d 65da 0566 6965 6c64  ame..name..field
-00000120: 4e29 0272 0500 0000 7206 0000 0029 09da  N).r....r....)..
-00000130: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000140: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000150: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
-00000160: 7372 0200 0000 da0a 416c 7465 7246 6965  sr......AlterFie
-00000170: 6c64 7203 0000 00da 1450 6f73 6974 6976  ldr......Positiv
-00000180: 6549 6e74 6567 6572 4669 656c 64da 0a6f  eIntegerField..o
-00000190: 7065 7261 7469 6f6e 73a9 0072 1400 0000  perations..r....
-000001a0: 7214 0000 00fa 552f 686f 6d65 2f73 616d  r.....U/home/sam
-000001b0: 2f67 6974 2f4b 616e 6261 6e2f 646a 616e  /git/Kanban/djan
-000001c0: 676f 2d61 7574 6f74 6173 6b2f 646a 6175  go-autotask/djau
-000001d0: 746f 7461 736b 2f6d 6967 7261 7469 6f6e  totask/migration
-000001e0: 732f 3030 3233 5f61 7574 6f5f 3230 3139  s/0023_auto_2019
-000001f0: 3131 3139 5f30 3932 332e 7079 7204 0000  1119_0923.pyr...
-00000200: 0006 0000 0073 0a00 0000 0803 0604 0401  .....s..........
-00000210: 0201 0201 7204 0000 004e 2904 da09 646a  ....r....N)...dj
-00000220: 616e 676f 2e64 6272 0200 0000 7203 0000  ango.dbr....r...
-00000230: 0072 0400 0000 7214 0000 0072 1400 0000  .r....r....r....
-00000240: 7214 0000 0072 1500 0000 da08 3c6d 6f64  r....r......<mod
-00000250: 756c 653e 0300 0000 7302 0000 0010 03    ule>....s......
+00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
+00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
+00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
+00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
+00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
+00000070: 0000 0000 0006 0000 0040 0000 0073 3a00  .........@...s:.
+00000080: 0000 6500 005a 0100 6400 005a 0200 6409  ..e..Z..d..Z..d.
+00000090: 0067 0100 5a03 0065 0400 6a05 0064 0300  .g..Z..e..j..d..
+000000a0: 6404 0064 0500 6406 0064 0700 6901 0083  d..d..d..d..i...
+000000b0: 0002 6701 005a 0600 6408 0053 290a da09  ..g..Z..d..S)...
+000000c0: 4d69 6772 6174 696f 6eda 0a64 6a61 7574  Migration..djaut
+000000d0: 6f74 6173 6bda 1830 3031 305f 6d65 7267  otask..0010_merg
+000000e0: 655f 3230 3139 3039 3233 5f31 3135 35da  e_20190923_1155.
+000000f0: 046e 616d 65da 0571 7565 7565 da07 6f70  .name..queue..op
+00000100: 7469 6f6e 73da 1376 6572 626f 7365 5f6e  tions..verbose_n
+00000110: 616d 655f 706c 7572 616c da06 5175 6575  ame_plural..Queu
+00000120: 6573 4e29 027a 0a64 6a61 7574 6f74 6173  esN).z.djautotas
+00000130: 6b72 0500 0000 2907 da08 5f5f 6e61 6d65  kr....)...__name
+00000140: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000150: 5f5f 7175 616c 6e61 6d65 5f5f da0c 6465  __qualname__..de
+00000160: 7065 6e64 656e 6369 6573 7202 0000 00da  pendenciesr.....
+00000170: 1141 6c74 6572 4d6f 6465 6c4f 7074 696f  .AlterModelOptio
+00000180: 6e73 da0a 6f70 6572 6174 696f 6e73 a900  ns..operations..
+00000190: 7211 0000 0072 1100 0000 fa55 2f68 6f6d  r....r.....U/hom
+000001a0: 652f 7361 6d2f 6769 742f 4b61 6e62 616e  e/sam/git/Kanban
+000001b0: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
+000001c0: 2f64 6a61 7574 6f74 6173 6b2f 6d69 6772  /djautotask/migr
+000001d0: 6174 696f 6e73 2f30 3031 315f 6175 746f  ations/0011_auto
+000001e0: 5f32 3031 3930 3932 335f 3131 3537 2e70  _20190923_1157.p
+000001f0: 7972 0300 0000 0600 0000 7308 0000 000c  yr........s.....
+00000200: 0309 0409 0106 0172 0300 0000 4e29 03da  .......r....N)..
+00000210: 0964 6a61 6e67 6f2e 6462 7202 0000 0072  .django.dbr....r
+00000220: 0300 0000 7211 0000 0072 1100 0000 7211  ....r....r....r.
+00000230: 0000 0072 1200 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000240: 653e 0300 0000 7302 0000 0010 03         e>....s......
```

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/__pycache__/0071_project_status_detail.cpython-36.pyc` & `django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0013_auto_20190923_1439.cpython-35.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-00000000: 330d 0d0a f3f4 895f a501 0000 e300 0000  3......_........
+00000000: 160d 0d0a 81dc 935d be01 0000 e300 0000  .......]........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2600 0000 6400 6401 6c00 6d01 5a01  .s&...d.d.l.m.Z.
-00000030: 6d02 5a02 0100 4700 6402 6403 8400 6403  m.Z...G.d.d...d.
-00000040: 6501 6a03 8303 5a03 6404 5300 2905 e900  e.j...Z.d.S.)...
-00000050: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
-00000060: 73da 066d 6f64 656c 7363 0000 0000 0000  s..modelsc......
-00000070: 0000 0000 0000 0800 0000 4000 0000 7330  ..........@...s0
-00000080: 0000 0065 005a 0164 005a 0264 0a67 015a  ...e.Z.d.Z.d.g.Z
-00000090: 0365 046a 0564 0364 0465 066a 0764 0564  .e.j.d.d.e.j.d.d
-000000a0: 0664 0564 078d 0364 088d 0367 015a 0864  .d.d...d...g.Z.d
-000000b0: 0953 0029 0bda 094d 6967 7261 7469 6f6e  .S.)...Migration
-000000c0: da0a 646a 6175 746f 7461 736b da17 3030  ..djautotask..00
-000000d0: 3730 5f61 7574 6f5f 3230 3230 3037 3134  70_auto_20200714
-000000e0: 5f30 3830 37da 0770 726f 6a65 6374 da0d  _0807..project..
-000000f0: 7374 6174 7573 5f64 6574 6169 6c54 69d0  status_detailTi.
-00000100: 0700 0029 03da 0562 6c61 6e6b da0a 6d61  ...)...blank..ma
-00000110: 785f 6c65 6e67 7468 da04 6e75 6c6c 2903  x_length..null).
-00000120: da0a 6d6f 6465 6c5f 6e61 6d65 da04 6e61  ..model_name..na
-00000130: 6d65 da05 6669 656c 644e 2902 7205 0000  me..fieldN).r...
-00000140: 0072 0600 0000 2909 da08 5f5f 6e61 6d65  .r....)...__name
-00000150: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00000160: 5f5f 7175 616c 6e61 6d65 5f5f da0c 6465  __qualname__..de
-00000170: 7065 6e64 656e 6369 6573 7202 0000 00da  pendenciesr.....
-00000180: 0841 6464 4669 656c 6472 0300 0000 da09  .AddFieldr......
-00000190: 4368 6172 4669 656c 64da 0a6f 7065 7261  CharField..opera
-000001a0: 7469 6f6e 73a9 0072 1600 0000 7216 0000  tions..r....r...
-000001b0: 00fa 582f 686f 6d65 2f73 616d 2f67 6974  ..X/home/sam/git
-000001c0: 2f4b 616e 6261 6e2f 646a 616e 676f 2d61  /Kanban/django-a
-000001d0: 7574 6f74 6173 6b2f 646a 6175 746f 7461  utotask/djautota
-000001e0: 736b 2f6d 6967 7261 7469 6f6e 732f 3030  sk/migrations/00
-000001f0: 3731 5f70 726f 6a65 6374 5f73 7461 7475  71_project_statu
-00000200: 735f 6465 7461 696c 2e70 7972 0400 0000  s_detail.pyr....
-00000210: 0600 0000 730a 0000 0008 0306 0404 0102  ....s...........
-00000220: 0102 0172 0400 0000 4e29 04da 0964 6a61  ...r....N)...dja
-00000230: 6e67 6f2e 6462 7202 0000 0072 0300 0000  ngo.dbr....r....
-00000240: 7204 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00000250: 1600 0000 7217 0000 00da 083c 6d6f 6475  ....r......<modu
-00000260: 6c65 3e03 0000 0073 0200 0000 1003       le>....s......
+00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
+00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
+00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
+00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
+00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
+00000070: 0000 0000 0006 0000 0040 0000 0073 4900  .........@...sI.
+00000080: 0000 6500 005a 0100 6400 005a 0200 6409  ..e..Z..d..Z..d.
+00000090: 0067 0100 5a03 0065 0400 6a05 0064 0300  .g..Z..e..j..d..
+000000a0: 6404 0064 0500 6406 0083 0002 6504 006a  d..d..d.....e..j
+000000b0: 0500 6403 0064 0700 6405 0064 0600 8300  ..d..d..d..d....
+000000c0: 0267 0200 5a06 0064 0800 5329 0ada 094d  .g..Z..d..S)...M
+000000d0: 6967 7261 7469 6f6e da0a 646a 6175 746f  igration..djauto
+000000e0: 7461 736b da18 3030 3132 5f6d 6572 6765  task..0012_merge
+000000f0: 5f32 3031 3930 3932 335f 3134 3339 da0a  _20190923_1439..
+00000100: 6d6f 6465 6c5f 6e61 6d65 5a0d 7072 6f6a  model_nameZ.proj
+00000110: 6563 7473 7461 7475 73da 046e 616d 65da  ectstatus..name.
+00000120: 0576 616c 7565 5a0b 7072 6f6a 6563 7474  .valueZ.projectt
+00000130: 7970 654e 2902 7a0a 646a 6175 746f 7461  ypeN).z.djautota
+00000140: 736b 7a18 3030 3132 5f6d 6572 6765 5f32  skz.0012_merge_2
+00000150: 3031 3930 3932 335f 3134 3339 2907 da08  0190923_1439)...
+00000160: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000170: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000180: 5f5f da0c 6465 7065 6e64 656e 6369 6573  __..dependencies
+00000190: 7202 0000 00da 0b52 656d 6f76 6546 6965  r......RemoveFie
+000001a0: 6c64 da0a 6f70 6572 6174 696f 6e73 a900  ld..operations..
+000001b0: 720f 0000 0072 0f00 0000 fa55 2f68 6f6d  r....r.....U/hom
+000001c0: 652f 7361 6d2f 6769 742f 4b61 6e62 616e  e/sam/git/Kanban
+000001d0: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
+000001e0: 2f64 6a61 7574 6f74 6173 6b2f 6d69 6772  /djautotask/migr
+000001f0: 6174 696f 6e73 2f30 3031 335f 6175 746f  ations/0013_auto
+00000200: 5f32 3031 3930 3932 335f 3134 3339 2e70  _20190923_1439.p
+00000210: 7972 0300 0000 0600 0000 730e 0000 000c  yr........s.....
+00000220: 0309 0409 0106 0106 0209 0106 0172 0300  .............r..
+00000230: 0000 4e29 03da 0964 6a61 6e67 6f2e 6462  ..N)...django.db
+00000240: 7202 0000 0072 0300 0000 720f 0000 0072  r....r....r....r
+00000250: 0f00 0000 720f 0000 0072 1000 0000 da08  ....r....r......
+00000260: 3c6d 6f64 756c 653e 0300 0000 7302 0000  <module>....s...
+00000270: 0010 03                                  ...
```

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/0064_auto_20200511_1124.py` & `django-autotask-0.0.9a0/djautotask/migrations/0010_auto_20190923_0930.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,40 @@
-# Generated by Django 2.1.14 on 2020-05-11 11:24
+# Generated by Django 2.1.11 on 2019-09-23 09:30
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('djautotask', '0063_accountphysicallocation'),
+        ('djautotask', '0009_auto_20190918_1525'),
     ]
 
     operations = [
-        migrations.AddField(
-            model_name='ticket',
-            name='first_response_date_time',
-            field=models.DateTimeField(blank=True, null=True),
+        migrations.RemoveField(
+            model_name='project',
+            name='completed_date_time',
         ),
-        migrations.AddField(
-            model_name='ticket',
-            name='first_response_due_date_time',
-            field=models.DateTimeField(blank=True, null=True),
+        migrations.RemoveField(
+            model_name='project',
+            name='end_date_time',
         ),
-        migrations.AddField(
-            model_name='ticket',
-            name='resolution_plan_date_time',
-            field=models.DateTimeField(blank=True, null=True),
+        migrations.RemoveField(
+            model_name='project',
+            name='start_date_time',
         ),
         migrations.AddField(
-            model_name='ticket',
-            name='resolution_plan_due_date_time',
-            field=models.DateTimeField(blank=True, null=True),
+            model_name='project',
+            name='completed_date',
+            field=models.DateField(null=True),
         ),
         migrations.AddField(
-            model_name='ticket',
-            name='resolved_date_time',
-            field=models.DateTimeField(blank=True, null=True),
+            model_name='project',
+            name='end_date',
+            field=models.DateField(null=True),
         ),
         migrations.AddField(
-            model_name='ticket',
-            name='resolved_due_date_time',
-            field=models.DateTimeField(blank=True, null=True),
+            model_name='project',
+            name='start_date',
+            field=models.DateField(null=True),
         ),
     ]
```

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/0039_auto_20200131_1134.py` & `django-autotask-0.0.9a0/djautotask/migrations/0003_auto_20190913_0941.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-# Generated by Django 2.1.14 on 2020-01-31 11:34
+# Generated by Django 2.1.11 on 2019-09-13 09:41
 
 from django.db import migrations, models
 import django.db.models.deletion
 import django_extensions.db.fields
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('djautotask', '0038_notetype_tasknote_ticketnote'),
+        ('djautotask', '0002_ticket_ticket_number'),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='TaskTypeLink',
+            name='TicketStatus',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created', django_extensions.db.fields.CreationDateTimeField(auto_now_add=True, verbose_name='created')),
                 ('modified', django_extensions.db.fields.ModificationDateTimeField(auto_now=True, verbose_name='modified')),
+                ('value', models.CharField(blank=True, max_length=50, null=True)),
                 ('label', models.CharField(blank=True, max_length=50, null=True)),
                 ('is_default_value', models.BooleanField(default=False)),
                 ('sort_order', models.PositiveSmallIntegerField(blank=True, null=True)),
+                ('parent_value', models.CharField(blank=True, max_length=20, null=True)),
                 ('is_active', models.BooleanField(default=False)),
                 ('is_system', models.BooleanField(default=False)),
             ],
             options={
-                'ordering': ('label',),
-                'abstract': False,
+                'verbose_name': 'Ticket status',
+                'verbose_name_plural': 'Ticket statuses',
             },
         ),
         migrations.AddField(
-            model_name='timeentry',
-            name='type',
-            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.TaskTypeLink'),
+            model_name='ticket',
+            name='status',
+            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.TicketStatus'),
         ),
     ]
```

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/0007_auto_20190917_1009.py` & `django-autotask-0.0.9a0/djautotask/migrations/0007_auto_20190917_1009.py`

 * *Files identical despite different names*

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/0042_auto_20200205_1057.py` & `django-autotask-0.0.9a0/djautotask/migrations/0004_auto_20190913_1425.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,36 @@
-# Generated by Django 2.1.14 on 2020-02-05 10:57
+# Generated by Django 2.1.11 on 2019-09-13 14:25
 
 from django.db import migrations, models
 import django.db.models.deletion
 import django_extensions.db.fields
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('djautotask', '0041_merge_20200204_1546'),
+        ('djautotask', '0003_auto_20190913_0941'),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='AllocationCode',
+            name='Resource',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created', django_extensions.db.fields.CreationDateTimeField(auto_now_add=True, verbose_name='created')),
                 ('modified', django_extensions.db.fields.ModificationDateTimeField(auto_now=True, verbose_name='modified')),
-                ('name', models.CharField(blank=True, max_length=200, null=True)),
-                ('description', models.CharField(blank=True, max_length=500, null=True)),
+                ('user_name', models.CharField(max_length=32)),
+                ('email', models.CharField(max_length=50)),
+                ('first_name', models.CharField(max_length=50)),
+                ('last_name', models.CharField(max_length=50)),
                 ('active', models.BooleanField(default=False)),
             ],
             options={
-                'ordering': ('-modified', '-created'),
-                'get_latest_by': 'modified',
-                'abstract': False,
-            },
-        ),
-        migrations.CreateModel(
-            name='UseType',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('created', django_extensions.db.fields.CreationDateTimeField(auto_now_add=True, verbose_name='created')),
-                ('modified', django_extensions.db.fields.ModificationDateTimeField(auto_now=True, verbose_name='modified')),
-                ('label', models.CharField(blank=True, max_length=50, null=True)),
-                ('is_default_value', models.BooleanField(default=False)),
-                ('sort_order', models.PositiveSmallIntegerField(blank=True, null=True)),
-                ('is_active', models.BooleanField(default=False)),
-                ('is_system', models.BooleanField(default=False)),
-            ],
-            options={
-                'ordering': ('label',),
-                'abstract': False,
+                'ordering': ('first_name', 'last_name'),
             },
         ),
         migrations.AddField(
-            model_name='allocationcode',
-            name='use_type',
-            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.UseType'),
+            model_name='ticket',
+            name='assigned_resource',
+            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.Resource'),
         ),
     ]
```

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/0035_timeentry.py` & `django-autotask-0.0.9a0/djautotask/migrations/0001_initial.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,48 @@
-# Generated by Django 2.1.14 on 2020-01-15 16:17
+# Generated by Django 2.1.11 on 2019-08-28 16:25
 
 from django.db import migrations, models
-import django.db.models.deletion
 import django_extensions.db.fields
 
 
 class Migration(migrations.Migration):
 
+    initial = True
+
     dependencies = [
-        ('djautotask', '0034_auto_20191210_1518'),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='TimeEntry',
+            name='SyncJob',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('start_time', models.DateTimeField()),
+                ('end_time', models.DateTimeField(blank=True, null=True)),
+                ('entity_name', models.CharField(max_length=100)),
+                ('added', models.PositiveIntegerField(null=True)),
+                ('updated', models.PositiveIntegerField(null=True)),
+                ('deleted', models.PositiveIntegerField(null=True)),
+                ('success', models.NullBooleanField()),
+                ('message', models.TextField(blank=True, null=True)),
+                ('sync_type', models.CharField(default='full', max_length=32)),
+            ],
+        ),
+        migrations.CreateModel(
+            name='Ticket',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created', django_extensions.db.fields.CreationDateTimeField(auto_now_add=True, verbose_name='created')),
                 ('modified', django_extensions.db.fields.ModificationDateTimeField(auto_now=True, verbose_name='modified')),
-                ('date_worked', models.DateTimeField(blank=True, null=True)),
-                ('start_date_time', models.DateTimeField(blank=True, null=True)),
-                ('end_date_time', models.DateTimeField(blank=True, null=True)),
-                ('summary_notes', models.TextField(blank=True, max_length=8000, null=True)),
-                ('internal_notes', models.TextField(blank=True, max_length=8000, null=True)),
-                ('non_billable', models.BooleanField(default=False)),
-                ('hours_worked', models.DecimalField(blank=True, decimal_places=2, max_digits=9, null=True)),
-                ('hours_to_bill', models.DecimalField(blank=True, decimal_places=2, max_digits=9, null=True)),
-                ('offset_hours', models.DecimalField(blank=True, decimal_places=2, max_digits=9, null=True)),
-                ('resource', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.CASCADE, to='djautotask.Resource')),
-                ('task', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.CASCADE, to='djautotask.Task')),
-                ('ticket', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.CASCADE, to='djautotask.Ticket')),
+                ('completed_date', models.DateTimeField(blank=True, null=True)),
+                ('create_date', models.DateTimeField(blank=True, null=True)),
+                ('description', models.TextField(blank=True, max_length=8000, null=True)),
+                ('due_date_time', models.DateTimeField()),
+                ('estimated_hours', models.DecimalField(blank=True, decimal_places=2, max_digits=6, null=True)),
+                ('last_activity_date', models.DateTimeField(blank=True, null=True)),
+                ('title', models.CharField(blank=True, max_length=255, null=True)),
             ],
             options={
-                'verbose_name_plural': 'Time entries',
+                'verbose_name': 'Ticket',
             },
         ),
     ]
```

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/0014_auto_20190930_1548.py` & `django-autotask-0.0.9a0/djautotask/migrations/0014_auto_20190930_1548.py`

 * *Files identical despite different names*

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/0015_auto_20191001_0847.py` & `django-autotask-0.0.9a0/djautotask/migrations/0008_auto_20190917_1454.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,49 @@
-# Generated by Django 2.1.11 on 2019-10-01 08:47
+# Generated by Django 2.1.11 on 2019-09-17 14:54
 
 from django.db import migrations, models
 import django.db.models.deletion
 import django_extensions.db.fields
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('djautotask', '0014_auto_20190930_1548'),
+        ('djautotask', '0007_auto_20190917_1009'),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='DisplayColor',
+            name='Account',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created', django_extensions.db.fields.CreationDateTimeField(auto_now_add=True, verbose_name='created')),
                 ('modified', django_extensions.db.fields.ModificationDateTimeField(auto_now=True, verbose_name='modified')),
-                ('label', models.CharField(blank=True, max_length=50, null=True)),
-                ('is_default_value', models.BooleanField(default=False)),
-                ('sort_order', models.PositiveSmallIntegerField(blank=True, null=True)),
-                ('parent_value', models.CharField(blank=True, max_length=20, null=True)),
-                ('is_active', models.BooleanField(default=False)),
-                ('is_system', models.BooleanField(default=False)),
+                ('name', models.CharField(max_length=100)),
+                ('number', models.CharField(max_length=50)),
+                ('active', models.BooleanField(default=True)),
+                ('last_activity_date', models.DateTimeField(blank=True, null=True)),
             ],
             options={
-                'verbose_name_plural': 'Display colors',
+                'ordering': ('-modified', '-created'),
+                'get_latest_by': 'modified',
+                'abstract': False,
             },
         ),
+        migrations.AlterModelOptions(
+            name='queue',
+            options={},
+        ),
+        migrations.AlterModelOptions(
+            name='ticketpriority',
+            options={'verbose_name_plural': 'Ticket priorities'},
+        ),
+        migrations.AlterModelOptions(
+            name='ticketstatus',
+            options={'verbose_name_plural': 'Ticket statuses'},
+        ),
         migrations.AddField(
-            model_name='ticketcategory',
-            name='display_color',
-            field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.DisplayColor'),
+            model_name='ticket',
+            name='account',
+            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.Account'),
         ),
     ]
```

### Comparing `django-autotask-0.0.99a0/djautotask/migrations/0003_auto_20190913_0941.py` & `django-autotask-0.0.9a0/djautotask/migrations/0005_auto_20190916_1549.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-# Generated by Django 2.1.11 on 2019-09-13 09:41
+# Generated by Django 2.1.11 on 2019-09-16 15:49
 
 from django.db import migrations, models
 import django.db.models.deletion
 import django_extensions.db.fields
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('djautotask', '0002_ticket_ticket_number'),
+        ('djautotask', '0004_auto_20190913_1425'),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='TicketStatus',
+            name='TicketSecondaryResource',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created', django_extensions.db.fields.CreationDateTimeField(auto_now_add=True, verbose_name='created')),
                 ('modified', django_extensions.db.fields.ModificationDateTimeField(auto_now=True, verbose_name='modified')),
-                ('value', models.CharField(blank=True, max_length=50, null=True)),
-                ('label', models.CharField(blank=True, max_length=50, null=True)),
-                ('is_default_value', models.BooleanField(default=False)),
-                ('sort_order', models.PositiveSmallIntegerField(blank=True, null=True)),
-                ('parent_value', models.CharField(blank=True, max_length=20, null=True)),
-                ('is_active', models.BooleanField(default=False)),
-                ('is_system', models.BooleanField(default=False)),
+                ('resource', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.Resource')),
+                ('ticket', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.Ticket')),
             ],
             options={
-                'verbose_name': 'Ticket status',
-                'verbose_name_plural': 'Ticket statuses',
+                'ordering': ('-modified', '-created'),
+                'get_latest_by': 'modified',
+                'abstract': False,
             },
         ),
         migrations.AddField(
             model_name='ticket',
-            name='status',
-            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='djautotask.TicketStatus'),
+            name='secondary_resources',
+            field=models.ManyToManyField(related_name='secondary_resource_tickets', through='djautotask.TicketSecondaryResource', to='djautotask.Resource'),
         ),
     ]
```

### Comparing `django-autotask-0.0.99a0/PKG-INFO` & `django-autotask-0.0.9a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: django-autotask
-Version: 0.0.99a0
+Version: 0.0.9a0
 Summary: Django app for working with Autotask. Defines models (tickets, members, companies, etc.) and callbacks.
 Home-page: https://github.com/KerkhoffTechnologies/django-autotask
 Author: Kerkhoff Technologies Inc.
 Author-email: matt@kerkhofftech.ca
 License: MIT
 Description: ## django-autotask
         
         Django app for working with Autotask. Defines models (tickets,
-        resources, accounts, etc.).
+        members, companies, etc.).
         
         ## Requirements
         
         -  Python 3.5
         -  Django 2.0
         
         Other versions may work; we haven't tried.
@@ -30,14 +30,15 @@
         
         1. Add to INSTALLED_APPS
         
             ```
             INSTALLED_APPS = [
                 ...
                 'djautotask',
+                'easy_thumbnails'  # Used for managing user pictures
                 ...
             ]
             ```
         
         
         ## Testing
```

### Comparing `django-autotask-0.0.99a0/django_autotask.egg-info/PKG-INFO` & `django-autotask-0.0.9a0/django_autotask.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: django-autotask
-Version: 0.0.99a0
+Version: 0.0.9a0
 Summary: Django app for working with Autotask. Defines models (tickets, members, companies, etc.) and callbacks.
 Home-page: https://github.com/KerkhoffTechnologies/django-autotask
 Author: Kerkhoff Technologies Inc.
 Author-email: matt@kerkhofftech.ca
 License: MIT
 Description: ## django-autotask
         
         Django app for working with Autotask. Defines models (tickets,
-        resources, accounts, etc.).
+        members, companies, etc.).
         
         ## Requirements
         
         -  Python 3.5
         -  Django 2.0
         
         Other versions may work; we haven't tried.
@@ -30,14 +30,15 @@
         
         1. Add to INSTALLED_APPS
         
             ```
             INSTALLED_APPS = [
                 ...
                 'djautotask',
+                'easy_thumbnails'  # Used for managing user pictures
                 ...
             ]
             ```
         
         
         ## Testing
```

### Comparing `django-autotask-0.0.99a0/README.md` & `django-autotask-0.0.9a0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ## django-autotask
 
 Django app for working with Autotask. Defines models (tickets,
-resources, accounts, etc.).
+members, companies, etc.).
 
 ## Requirements
 
 -  Python 3.5
 -  Django 2.0
 
 Other versions may work; we haven't tried.
@@ -22,14 +22,15 @@
 
 1. Add to INSTALLED_APPS
 
     ```
     INSTALLED_APPS = [
         ...
         'djautotask',
+        'easy_thumbnails'  # Used for managing user pictures
         ...
     ]
     ```
 
 
 ## Testing
```

### Comparing `django-autotask-0.0.99a0/setup.py` & `django-autotask-0.0.9a0/setup.py`

 * *Files identical despite different names*

