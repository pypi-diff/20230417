# Comparing `tmp/django_rq_scheduler-2023.5.0b3.tar.gz` & `tmp/django_rq_scheduler-2023.5.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rq_scheduler-2023.5.0b3.tar", max compression
+gzip compressed data, was "django_rq_scheduler-2023.5.0b4.tar", max compression
```

## Comparing `django_rq_scheduler-2023.5.0b3.tar` & `django_rq_scheduler-2023.5.0b4.tar`

### file list

```diff
@@ -1,68 +1,69 @@
--rw-r--r--   0        0        0     1107 2023-04-11 19:00:13.252306 django_rq_scheduler-2023.5.0b3/LICENSE
--rw-r--r--   0        0        0     1704 2023-04-11 19:00:13.252306 django_rq_scheduler-2023.5.0b3/README.md
--rw-r--r--   0        0        0     1741 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/pyproject.toml
--rw-r--r--   0        0        0      134 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/__init__.py
--rw-r--r--   0        0        0      147 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/admin/__init__.py
--rw-r--r--   0        0        0     5668 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/admin/job.py
--rw-r--r--   0        0        0     1646 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/admin/redis_models.py
--rw-r--r--   0        0        0      481 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/apps.py
--rw-r--r--   0        0        0     1147 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/decorators.py
--rw-r--r--   0        0        0        0 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/commands/__init__.py
--rw-r--r--   0        0        0     1189 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/commands/delete_failed_executions.py
--rw-r--r--   0        0        0     1908 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/commands/export.py
--rw-r--r--   0        0        0     3417 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/commands/import.py
--rw-r--r--   0        0        0     3602 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/commands/rqstats.py
--rw-r--r--   0        0        0     2962 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/commands/rqworker.py
--rw-r--r--   0        0        0     1374 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/management/commands/run_job.py
--rw-r--r--   0        0        0     7162 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
--rw-r--r--   0        0        0      898 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
--rw-r--r--   0        0        0     4196 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0003_auto_20220329_2107.py
--rw-r--r--   0        0        0      791 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0      896 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0     1051 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0006_auto_20230118_1640.py
--rw-r--r--   0        0        0     1302 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0007_add_result_ttl.py
--rw-r--r--   0        0        0     1982 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
--rw-r--r--   0        0        0     1362 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
--rw-r--r--   0        0        0      661 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0010_queue.py
--rw-r--r--   0        0        0     7643 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
--rw-r--r--   0        0        0        0 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/migrations/__init__.py
--rw-r--r--   0        0        0      187 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/models/__init__.py
--rw-r--r--   0        0        0     3102 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/models/args.py
--rw-r--r--   0        0        0      364 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/models/queue.py
--rw-r--r--   0        0        0    15168 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/models/scheduled_job.py
--rw-r--r--   0        0        0      366 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/models/worker.py
--rw-r--r--   0        0        0        0 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/py.typed
--rw-r--r--   0        0        0     5406 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/queues.py
--rw-r--r--   0        0        0     5151 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/rq_classes.py
--rw-r--r--   0        0        0      822 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/settings.py
--rw-r--r--   0        0        0      163 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/change_form.html
--rw-r--r--   0        0        0      127 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/change_list.html
--rw-r--r--   0        0        0     1559 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/confirm_action.html
--rw-r--r--   0        0        0     1282 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/delete_job.html
--rw-r--r--   0        0        0     7124 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/job_detail.html
--rw-r--r--   0        0        0     2574 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/jobs-list.partial.html
--rw-r--r--   0        0        0     6285 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/jobs.html
--rw-r--r--   0        0        0     1055 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/queue_workers.html
--rw-r--r--   0        0        0      568 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/scheduler_base.html
--rw-r--r--   0        0        0     4120 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/stats.html
--rw-r--r--   0        0        0     3032 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/worker_details.html
--rw-r--r--   0        0        0     1875 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/workers-list.partial.html
--rw-r--r--   0        0        0      935 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/workers.html
--rw-r--r--   0        0        0        0 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templatetags/__init__.py
--rw-r--r--   0        0        0      628 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/templatetags/scheduler_tags.py
--rw-r--r--   0        0        0        0 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/__init__.py
--rw-r--r--   0        0        0      535 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/jobs.py
--rw-r--r--   0        0        0      668 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_internals.py
--rw-r--r--   0        0        0     5887 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_job_arg_models.py
--rw-r--r--   0        0        0     4304 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_mgmt_cmds.py
--rw-r--r--   0        0        0    27451 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_models.py
--rw-r--r--   0        0        0      807 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_redis_models.py
--rw-r--r--   0        0        0     2204 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_settings.py
--rw-r--r--   0        0        0    15014 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_views.py
--rw-r--r--   0        0        0     1183 2023-04-11 19:00:13.256306 django_rq_scheduler-2023.5.0b3/scheduler/tests/test_worker.py
--rw-r--r--   0        0        0     3323 2023-04-11 19:00:13.260306 django_rq_scheduler-2023.5.0b3/scheduler/tests/testtools.py
--rw-r--r--   0        0        0     3399 2023-04-11 19:00:13.260306 django_rq_scheduler-2023.5.0b3/scheduler/tools.py
--rw-r--r--   0        0        0     1736 2023-04-11 19:00:13.260306 django_rq_scheduler-2023.5.0b3/scheduler/urls.py
--rw-r--r--   0        0        0    16289 2023-04-11 19:00:13.260306 django_rq_scheduler-2023.5.0b3/scheduler/views.py
--rw-r--r--   0        0        0     3452 1970-01-01 00:00:00.000000 django_rq_scheduler-2023.5.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1107 2023-04-17 16:42:06.746785 django_rq_scheduler-2023.5.0b4/LICENSE
+-rw-r--r--   0        0        0     1704 2023-04-17 16:42:06.746785 django_rq_scheduler-2023.5.0b4/README.md
+-rw-r--r--   0        0        0     1741 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/__init__.py
+-rw-r--r--   0        0        0      147 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/admin/__init__.py
+-rw-r--r--   0        0        0     5661 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/admin/job.py
+-rw-r--r--   0        0        0     1641 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/admin/redis_models.py
+-rw-r--r--   0        0        0      355 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/apps.py
+-rw-r--r--   0        0        0     1207 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/decorators.py
+-rw-r--r--   0        0        0        0 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/commands/__init__.py
+-rw-r--r--   0        0        0     1189 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/commands/delete_failed_executions.py
+-rw-r--r--   0        0        0     1908 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/commands/export.py
+-rw-r--r--   0        0        0     3417 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/commands/import.py
+-rw-r--r--   0        0        0     3602 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/commands/rqstats.py
+-rw-r--r--   0        0        0     2962 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/commands/rqworker.py
+-rw-r--r--   0        0        0     1374 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/management/commands/run_job.py
+-rw-r--r--   0        0        0     7162 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
+-rw-r--r--   0        0        0      898 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
+-rw-r--r--   0        0        0     4196 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0003_auto_20220329_2107.py
+-rw-r--r--   0        0        0      791 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0      896 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0     1051 2023-04-17 16:42:06.750785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0006_auto_20230118_1640.py
+-rw-r--r--   0        0        0     1302 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0007_add_result_ttl.py
+-rw-r--r--   0        0        0     1982 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
+-rw-r--r--   0        0        0     1362 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
+-rw-r--r--   0        0        0      661 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0010_queue.py
+-rw-r--r--   0        0        0     7643 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
+-rw-r--r--   0        0        0        0 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/migrations/__init__.py
+-rw-r--r--   0        0        0      187 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/models/__init__.py
+-rw-r--r--   0        0        0     3102 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/models/args.py
+-rw-r--r--   0        0        0      364 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/models/queue.py
+-rw-r--r--   0        0        0    15140 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/models/scheduled_job.py
+-rw-r--r--   0        0        0      366 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/models/worker.py
+-rw-r--r--   0        0        0        0 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/py.typed
+-rw-r--r--   0        0        0     4858 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/queues.py
+-rw-r--r--   0        0        0     7780 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/rq_classes.py
+-rw-r--r--   0        0        0      932 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/settings.py
+-rw-r--r--   0        0        0      163 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/change_form.html
+-rw-r--r--   0        0        0      127 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/change_list.html
+-rw-r--r--   0        0        0     1559 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/confirm_action.html
+-rw-r--r--   0        0        0     1282 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/delete_job.html
+-rw-r--r--   0        0        0     7124 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/job_detail.html
+-rw-r--r--   0        0        0     2697 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/jobs-list.partial.html
+-rw-r--r--   0        0        0     6285 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/jobs.html
+-rw-r--r--   0        0        0     1055 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/queue_workers.html
+-rw-r--r--   0        0        0      568 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/scheduler_base.html
+-rw-r--r--   0        0        0     4120 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/stats.html
+-rw-r--r--   0        0        0     3032 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/worker_details.html
+-rw-r--r--   0        0        0     1875 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/workers-list.partial.html
+-rw-r--r--   0        0        0      935 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/workers.html
+-rw-r--r--   0        0        0        0 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templatetags/__init__.py
+-rw-r--r--   0        0        0     1179 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/templatetags/scheduler_tags.py
+-rw-r--r--   0        0        0        0 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/__init__.py
+-rw-r--r--   0        0        0      535 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/jobs.py
+-rw-r--r--   0        0        0      668 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_internals.py
+-rw-r--r--   0        0        0     5887 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_job_arg_models.py
+-rw-r--r--   0        0        0     2349 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_job_decorator.py
+-rw-r--r--   0        0        0     4304 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_mgmt_cmds.py
+-rw-r--r--   0        0        0    27529 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_models.py
+-rw-r--r--   0        0        0      807 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_redis_models.py
+-rw-r--r--   0        0        0     2211 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_settings.py
+-rw-r--r--   0        0        0    14933 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_views.py
+-rw-r--r--   0        0        0     1577 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/test_worker.py
+-rw-r--r--   0        0        0     3311 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tests/testtools.py
+-rw-r--r--   0        0        0     2572 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/tools.py
+-rw-r--r--   0        0        0     1736 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/urls.py
+-rw-r--r--   0        0        0    16009 2023-04-17 16:42:06.754785 django_rq_scheduler-2023.5.0b4/scheduler/views.py
+-rw-r--r--   0        0        0     3452 1970-01-01 00:00:00.000000 django_rq_scheduler-2023.5.0b4/PKG-INFO
```

### Comparing `django_rq_scheduler-2023.5.0b3/LICENSE` & `django_rq_scheduler-2023.5.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/README.md` & `django_rq_scheduler-2023.5.0b4/README.md`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/pyproject.toml` & `django_rq_scheduler-2023.5.0b4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-rq-scheduler"
 packages = [
     { include = "scheduler" },
 ]
-version = "2023.5.0b3"
+version = "2023.5.0b4"
 description = "An async job scheduler for django using redis"
 readme = "README.md"
 keywords = ["redis", "django", "background-jobs", "job-queue", "task-queue", "redis-queue", "scheduled-jobs"]
 authors = [
     "Daniel Moran <daniel.maruani@gmail.com>",
 ]
 maintainers = [
```

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/admin/job.py` & `django_rq_scheduler-2023.5.0b4/scheduler/admin/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import redis
 from django.contrib import admin, messages
 from django.contrib.contenttypes.admin import GenericStackedInline
 from django.utils.translation import gettext_lazy as _
 
 from scheduler import tools
 from scheduler.models import CronJob, JobArg, JobKwarg, RepeatableJob, ScheduledJob
-from scheduler.queues import logger
-from scheduler.settings import SCHEDULER
+from scheduler.settings import SCHEDULER_CONFIG, logger
 from scheduler.tools import get_job_executions
 
 
 class HiddenMixin(object):
     class Media:
         js = ['admin/js/jquery.init.js', ]
 
@@ -58,21 +57,21 @@
         extra = extra_context or {}
         obj = self.get_object(request, object_id)
         try:
             execution_list = get_job_executions(obj.queue, obj)
         except redis.ConnectionError as e:
             logger.warn(f'Could not get job executions: {e}')
             execution_list = list()
-        paginator = self.get_paginator(request, execution_list, SCHEDULER['EXECUTIONS_IN_PAGE'])
+        paginator = self.get_paginator(request, execution_list, SCHEDULER_CONFIG['EXECUTIONS_IN_PAGE'])
         page_number = request.GET.get('p', 1)
         page_obj = paginator.get_page(page_number)
         page_range = paginator.get_elided_page_range(page_obj.number)
 
         extra.update({
-            "pagination_required": paginator.count > SCHEDULER['EXECUTIONS_IN_PAGE'],
+            "pagination_required": paginator.count > SCHEDULER_CONFIG['EXECUTIONS_IN_PAGE'],
             'executions': page_obj,
             'page_range': page_range,
             'page_var': 'p',
         })
 
         return super(JobAdmin, self).change_view(
             request, object_id, form_url, extra_context=extra)
```

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/admin/redis_models.py` & `django_rq_scheduler-2023.5.0b4/scheduler/admin/redis_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from django.conf import settings
+from scheduler import settings
 from django.contrib import admin
 
 from scheduler import views
 from scheduler.models import Queue
 from scheduler.models.worker import Worker
 
-QUEUES = [(key, key) for key in settings.RQ_QUEUES.keys()]
+QUEUES = [(key, key) for key in settings.QUEUES.keys()]
 
 
 class ImmutableAdmin(admin.ModelAdmin):
     def has_add_permission(self, request):
         return False  # Hide the admin "+ Add" link for Queues
 
     def has_change_permission(self, request, obj=None):
```

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/management/commands/delete_failed_executions.py` & `django_rq_scheduler-2023.5.0b4/scheduler/management/commands/delete_failed_executions.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/management/commands/export.py` & `django_rq_scheduler-2023.5.0b4/scheduler/management/commands/export.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/management/commands/import.py` & `django_rq_scheduler-2023.5.0b4/scheduler/management/commands/import.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/management/commands/rqstats.py` & `django_rq_scheduler-2023.5.0b4/scheduler/management/commands/rqstats.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/management/commands/rqworker.py` & `django_rq_scheduler-2023.5.0b4/scheduler/management/commands/rqworker.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/management/commands/run_job.py` & `django_rq_scheduler-2023.5.0b4/scheduler/management/commands/run_job.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py` & `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py` & `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0003_auto_20220329_2107.py` & `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0003_auto_20220329_2107.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py` & `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py` & `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0006_auto_20230118_1640.py` & `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0006_auto_20230118_1640.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0007_add_result_ttl.py` & `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0007_add_result_ttl.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py` & `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py` & `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0010_queue.py` & `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0010_queue.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py` & `django_rq_scheduler-2023.5.0b4/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/models/args.py` & `django_rq_scheduler-2023.5.0b4/scheduler/models/args.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/models/scheduled_job.py` & `django_rq_scheduler-2023.5.0b4/scheduler/models/scheduled_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import math
 import uuid
 from datetime import timedelta
 from typing import Dict
 
 import croniter
 from django.apps import apps
-from django.conf import settings
 from django.contrib import admin
 from django.contrib.contenttypes.fields import GenericRelation
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.templatetags.tz import utc
 from django.utils import timezone
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 from model_utils import Choices
 from model_utils.models import TimeStampedModel
 
+from scheduler import settings
 from scheduler import tools
 from scheduler.models.args import JobArg, JobKwarg
 from scheduler.queues import get_queue, logger
 from scheduler.rq_classes import DjangoQueue
 
-RQ_SCHEDULER_INTERVAL = getattr(settings, "DJANGO_RQ_SCHEDULER_INTERVAL", 60)
+SCHEDULER_INTERVAL = settings.SCHEDULER_CONFIG['SCHEDULER_INTERVAL']
 
 
 def callback_save_job(job, connection, result, *args, **kwargs):
     model_name = job.meta.get('job_type', None)
     if model_name is None:
         return
     model = apps.get_model(app_label='scheduler', model_name=model_name)
     scheduled_job = model.objects.filter(job_id=job.id).first()
     if scheduled_job is not None:
         scheduled_job.unschedule()
         scheduled_job.schedule()
 
 
 class BaseJob(TimeStampedModel):
-    QUEUES = [(key, key) for key in settings.RQ_QUEUES.keys()]
+    QUEUES = [(key, key) for key in settings.QUEUES.keys()]
     JOB_TYPE = 'BaseJob'
     name = models.CharField(
         _('name'), max_length=128, unique=True,
         help_text='Name of the job.', )
     callable = models.CharField(_('callable'), max_length=2048)
     callable_args = GenericRelation(JobArg, related_query_name='args')
     callable_kwargs = GenericRelation(JobKwarg, related_query_name='kwargs')
@@ -80,18 +80,18 @@
         return tools.callable_func(self.callable)
 
     @admin.display(boolean=True, description=_('is scheduled?'))
     def is_scheduled(self) -> bool:
         """Check whether job is queued/scheduled to be executed"""
         if not self.job_id:
             return False
-        scheduled_jobs = self._get_rqueue().scheduled_job_registry.get_job_ids()
-        enqueued_jobs = self._get_rqueue().get_job_ids()
+        scheduled_jobs = self.rqueue.scheduled_job_registry.get_job_ids()
+        enqueued_jobs = self.rqueue.get_job_ids()
         res = (self.job_id in scheduled_jobs) or (self.job_id in enqueued_jobs)
-        if not res:
+        if not res:  # self.job_id is not None
             self.job_id = None
             super(BaseJob, self).save()
         return res
 
     @admin.display(description='Callable')
     def function_string(self) -> str:
         args = self.parse_args()
@@ -138,15 +138,16 @@
             res['at_front'] = self.at_front
         if self.timeout:
             res['job_timeout'] = self.timeout
         if self.result_ttl is not None:
             res['result_ttl'] = self.result_ttl
         return res
 
-    def _get_rqueue(self) -> DjangoQueue:
+    @property
+    def rqueue(self) -> DjangoQueue:
         """Returns django-queue for job
         """
         return get_queue(self.queue)
 
     def ready_for_schedule(self) -> bool:
         """Is job ready to be scheduled?
 
@@ -167,42 +168,42 @@
         """Schedule job to run.
         :returns: True if job was scheduled, False otherwise.
         """
         if not self.ready_for_schedule():
             return False
         schedule_time = self._schedule_time()
         kwargs = self._enqueue_args()
-        job = self._get_rqueue().enqueue_at(
+        job = self.rqueue.enqueue_at(
             schedule_time,
             tools.run_job,
             args=(self.JOB_TYPE, self.id),
             **kwargs, )
         self.job_id = job.id
         super(BaseJob, self).save()
         return True
 
     def enqueue_to_run(self) -> bool:
         """Enqueue job to run now.
         """
         kwargs = self._enqueue_args()
-        job = self._get_rqueue().enqueue(
+        job = self.rqueue.enqueue(
             tools.run_job,
             args=(self.JOB_TYPE, self.id),
             **kwargs,
         )
         self.job_id = job.id
         super(BaseJob, self).save()
         return True
 
     def unschedule(self) -> bool:
         """Remove job from django-queue.
 
         If job is queued to be executed or scheduled to be executed, it will remove it.
         """
-        queue = self._get_rqueue()
+        queue = self.rqueue
         if self.is_scheduled():
             queue.remove(self.job_id)
             queue.scheduled_job_registry.remove(self.job_id)
         self.job_id = None
         super(BaseJob, self).save()
         return True
 
@@ -251,15 +252,15 @@
         except Exception:
             raise ValidationError({
                 'callable': ValidationError(
                     _('Invalid callable, must be importable'), code='invalid')
             })
 
     def clean_queue(self):
-        queue_keys = settings.RQ_QUEUES.keys()
+        queue_keys = settings.QUEUES.keys()
         if self.queue not in queue_keys:
             raise ValidationError({
                 'queue': ValidationError(
                     _('Invalid queue, must be one of: {}'.format(
                         ', '.join(queue_keys))), code='invalid')
             })
 
@@ -328,25 +329,25 @@
 
     def clean(self):
         super(RepeatableJob, self).clean()
         self.clean_interval_unit()
         self.clean_result_ttl()
 
     def clean_interval_unit(self):
-        if RQ_SCHEDULER_INTERVAL > self.interval_seconds():
+        if SCHEDULER_INTERVAL > self.interval_seconds():
             raise ValidationError(
                 _("Job interval is set lower than %(queue)r queue's interval. "
                   "minimum interval is %(interval)"),
                 code='invalid',
-                params={'queue': self.queue, 'interval': RQ_SCHEDULER_INTERVAL})
-        if self.interval_seconds() % RQ_SCHEDULER_INTERVAL:
+                params={'queue': self.queue, 'interval': SCHEDULER_INTERVAL})
+        if self.interval_seconds() % SCHEDULER_INTERVAL:
             raise ValidationError(
                 _("Job interval is not a multiple of rq_scheduler's interval frequency: %(interval)ss"),
                 code='invalid',
-                params={'interval': RQ_SCHEDULER_INTERVAL})
+                params={'interval': SCHEDULER_INTERVAL})
 
     def clean_result_ttl(self) -> None:
         """
         Throws an error if there are repeats left to run and the result_ttl won't last until the next scheduled time.
         :return: None
         """
         if self.result_ttl and self.result_ttl != -1 and self.result_ttl < self.interval_seconds() and self.repeat:
```

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/queues.py` & `django_rq_scheduler-2023.5.0b4/scheduler/queues.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import logging
-from typing import List
+from typing import List, Dict
 
 import redis
 from redis.sentinel import Sentinel
 
 from .rq_classes import JobExecution, DjangoQueue, DjangoWorker
+from .settings import logger
 
-logger = logging.getLogger("scheduler")
 
-
-def _get_redis_connection(config, use_strict_redis=False):
+def _get_redis_connection(config, use_strict_redis=False, fake=False):
     """
     Returns a redis connection from a connection config
     """
     redis_cls = redis.StrictRedis if use_strict_redis else redis.Redis
     logger.debug(f'Getting connection for {config}')
     if 'URL' in config:
         if config.get('SSL') or config.get('URL').startswith('rediss://'):
@@ -59,15 +57,15 @@
 
 
 class QueueNotFoundError(Exception):
     pass
 
 
 def get_connection(name='default', use_strict_redis=False):
-    """Returns a Redis connection to use based on parameters in RQ_QUEUES
+    """Returns a Redis connection to use based on parameters in SCHEDULER_QUEUES
     """
     from .settings import QUEUES
 
     if name not in QUEUES:
         raise QueueNotFoundError(f'Queue {name} not found, queues={QUEUES.keys()}')
 
     return _get_redis_connection(QUEUES[name], use_strict_redis)
@@ -76,15 +74,15 @@
 def get_queue(
         name='default',
         default_timeout=None, is_async=None,
         autocommit=None,
         connection=None,
         **kwargs
 ) -> DjangoQueue:
-    """Returns an DjangoQueue using parameters defined in ``RQ_QUEUES``
+    """Returns an DjangoQueue using parameters defined in `SCHEDULER_QUEUES`
     """
     from .settings import QUEUES
 
     if is_async is None:
         is_async = QUEUES[name].get('ASYNC', True)
 
     if default_timeout is None:
@@ -110,61 +108,52 @@
             curr_workers = set(DjangoWorker.all(connection=connection))
             workers.update(curr_workers)
         except redis.ConnectionError as e:
             logger.error(f'Could not connect for queue {queue_name}: {e}')
     return workers
 
 
-def _filter_connection_params(queue_params):
-    """
-    Filters the queue params to keep only the connection related params.
-    """
-    CONNECTION_PARAMS = (
-        'URL',
-        'DB',
-        'USE_REDIS_CACHE',
-        'UNIX_SOCKET_PATH',
-        'HOST',
-        'PORT',
-        'PASSWORD',
-        'SENTINELS',
-        'MASTER_NAME',
-        'SOCKET_TIMEOUT',
-        'SSL',
-        'CONNECTION_KWARGS',
-    )
-
-    # return {p:v for p,v in queue_params.items() if p in CONNECTION_PARAMS}
-    # Dict comprehension compatible with python 2.6
-    return dict((p, v) for (p, v) in queue_params.items() if p in CONNECTION_PARAMS)
+_CONNECTION_PARAMS = {
+    'URL',
+    'DB',
+    'USE_REDIS_CACHE',
+    'UNIX_SOCKET_PATH',
+    'HOST',
+    'PORT',
+    'PASSWORD',
+    'SENTINELS',
+    'MASTER_NAME',
+    'SOCKET_TIMEOUT',
+    'SSL',
+    'CONNECTION_KWARGS',
+}
+
+
+def _queues_share_connection_params(q1_params: Dict, q2_params: Dict):
+    """Check that both queues share the same connection parameters
+    """
+    return all(
+        ((p not in q1_params and p not in q2_params)
+         or (q1_params.get(p, None) == q2_params.get(p, None)))
+        for p in _CONNECTION_PARAMS)
 
 
 def get_queues(*queue_names, **kwargs) -> List[DjangoQueue]:
     """
     Return queue instances from specified queue names.
     All instances must use the same Redis connection.
     """
     from .settings import QUEUES
 
-    if len(queue_names) <= 1:
-        # Return "default" queue if no queue name is specified
-        # or one queue with specified name
-        return [get_queue(*queue_names, **kwargs)]
-
     kwargs['job_class'] = JobExecution
     queue_params = QUEUES[queue_names[0]]
-    connection_params = _filter_connection_params(queue_params)
     queues = [get_queue(queue_names[0], **kwargs)]
-
     # perform consistency checks while building return list
     for name in queue_names[1:]:
-        queue = get_queue(name, **kwargs)
-        if type(queue) is not type(queues[0]):  # noqa: E721
-            raise ValueError(f'Queues must have the same class. '
-                             f'"{name}" and "{queue_names[0]}" have different classes')
-        if connection_params != _filter_connection_params(QUEUES[name]):
+        if not _queues_share_connection_params(queue_params, QUEUES[name]):
             raise ValueError(
                 f'Queues must have the same redis connection. "{name}" and'
                 f' "{queue_names[0]}" have different connections')
+        queue = get_queue(name, **kwargs)
         queues.append(queue)
 
     return queues
```

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/confirm_action.html` & `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/confirm_action.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/delete_job.html` & `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/delete_job.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/job_detail.html` & `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/job_detail.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/jobs-list.partial.html` & `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/jobs-list.partial.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,68 @@
-{% load i18n %}
-<fieldset class="module aligned {{ fieldset.classes }}">
-    <h2>Job executions</h2>
-    <div class="results">
-        <table id="result_list">
-            <thead>
-            <tr>
-                <th>ID</th>
-                <th>STATUS</th>
-                <th>Created</th>
-                <th>Scheduled</th>
-                <th>Enqueued</th>
-                <th>Started at</th>
-                <th>Ended at</th>
-                <th>Worker name</th>
-                <th>Result</th>
-            </tr>
-            </thead>
-            <tbody>
-            {% for exec in executions %}
+{% load scheduler_tags i18n %}
+{% if not add %}
+    <fieldset class="module aligned {{ fieldset.classes }}">
+        <h2>Job executions</h2>
+        <div class="results">
+            <table id="result_list">
+                <thead>
                 <tr>
-                    <td>
-                        <a href="{% url 'job_details' exec.id %}">{{ exec.id }}</a>
-                    </td>
-                    <td>
-                        {{ exec.status }}
-                    </td>
-                    <td>
-                        {{ exec.created_at|date:"Y-m-d, H:i:s"|default:"-" }}
-                    </td>
-                    <td>
-                        {{ exec.scheduled_at|date:"Y-m-d, H:i:s"|default:"-" }}
-                    </td>
-                    <td>
-                        {{ exec.enqueued_at|date:"Y-m-d, H:i:s"|default:"-" }}
-                    </td>
-                    <td>
-                        {{ exec.started_at|date:"Y-m-d, H:i:s"|default:"-" }}
-                    </td>
-                    <td>
-                        {{ exec.ended_at|date:"Y-m-d, H:i:s"|default:"-" }}
-                    </td>
-                    <td>
-                        {{ exec.worker_name|default:"-" }}
-                    </td>
-                    <td>
-                        {{ exec.latest_result|default:"-" }}
-                    </td>
+                    <th>ID</th>
+                    <th>STATUS</th>
+                    <th>Created at</th>
+                    <th>Enqueued at</th>
+                    <th>Started at</th>
+                    <th>Ran for</th>
+                    <th>Worker name</th>
+                    <th>Result</th>
                 </tr>
-            {% endfor %}
-            </tbody>
-        </table>
-    </div>
-    <p class="paginator">
-        {% if pagination_required %}
-            {% for i in page_range %}
-                {% if i == executions.paginator.ELLIPSIS %}
-                    {{ executions.paginator.ELLIPSIS }}
-                {% elif i == executions.number %}
-                    <span class="this-page">{{ i }}</span>
-                {% else %}
-                    <a href="?{{ page_var }}={{ i }}" {% if i == executions.paginator.num_pages %}
-                       class="end" {% endif %}>{{ i }}</a>
-                {% endif %}
-            {% endfor %}
-        {% endif %}
-        {{ executions.paginator.count }} {% blocktranslate count counter=executions.paginator.count %}entry
-        {% plural %}entries{% endblocktranslate %}
-    </p>
-</fieldset>
+                </thead>
+                <tbody>
+                {% for exec in executions %}
+                    <tr>
+                        <td>
+                            <a href="{% url 'job_details' exec.id %}">{{ exec.id }}</a>
+                        </td>
+                        <td>
+                            {{ exec|job_status }}
+                        </td>
+                        <td>
+                            {{ exec.created_at|date:"Y-m-d, H:i:s"|default:"-" }}
+                        </td>
+                        <td>
+                            {{ exec.enqueued_at|date:"Y-m-d, H:i:s"|default:"-" }}
+                        </td>
+                        <td>
+                            {{ exec.started_at|date:"Y-m-d, H:i:s"|default:"-" }}
+                        </td>
+                        <td>
+                            {{ exec|job_runtime }}
+                        </td>
+                        <td>
+                            {{ exec.worker_name|default:"-" }}
+                        </td>
+                        <td>
+                            {{ exec|job_result|default:"-" }}
+                        </td>
+                    </tr>
+                {% endfor %}
+                </tbody>
+            </table>
+        </div>
+        <p class="paginator">
+            {% if pagination_required %}
+                {% for i in page_range %}
+                    {% if i == executions.paginator.ELLIPSIS %}
+                        {{ executions.paginator.ELLIPSIS }}
+                    {% elif i == executions.number %}
+                        <span class="this-page">{{ i }}</span>
+                    {% else %}
+                        <a href="?{{ page_var }}={{ i }}" {% if i == executions.paginator.num_pages %}
+                           class="end" {% endif %}>{{ i }}</a>
+                    {% endif %}
+                {% endfor %}
+                {{ executions.paginator.count }} {% blocktranslate count counter=executions.paginator.count %}entry
+                {% plural %}entries{% endblocktranslate %}
+            {% endif %}
+        </p>
+    </fieldset>
+{% endif %}
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-{% load i18n %}
+{% load scheduler_tags i18n %} {% if not add %}
 ***** Job executions *****
-ID      STATUS      Created               Scheduled               Enqueued               Started at            Ended at            Worker name               Result
-{       {           {                     {                       {                      {                     {                   {                         {
-{       {           {                     {                       {                      {                     {                   {                         {
-exec.id exec.status exec.created_at|date: exec.scheduled_at|date: exec.enqueued_at|date: exec.started_at|date: exec.ended_at|date: exec.worker_name|default: exec.latest_result|default:
-}}      }}          "Y-m-d, H:i:          "Y-m-d, H:i:s"|default: "Y-m-d, H:i:           "Y-m-d, H:i:          "Y-m-d, H:i:        "-" }}                    "-" }}
-                    s"|default:"-" }}     "-" }}                  s"|default:"-" }}      s"|default:"-" }}     s"|default:"-" }}
+ID      STATUS          Created at            Enqueued at            Started at            Ran for          Worker name               Result
+{       {               {                     {                      {                     {                {                         {
+{       {               {                     {                      {                     {                {                         {
+exec.id exec|job_status exec.created_at|date: exec.enqueued_at|date: exec.started_at|date: exec|job_runtime exec.worker_name|default: exec|job_result|default:
+}}      }}              "Y-m-d, H:i:          "Y-m-d, H:i:           "Y-m-d, H:i:          }}               "-" }}                    "-" }}
+                        s"|default:"-" }}     s"|default:"-" }}      s"|default:"-" }}
 {% if pagination_required %} {% for i in page_range %} {% if i ==
 executions.paginator.ELLIPSIS %} {{ executions.paginator.ELLIPSIS }} {% elif i
 == executions.number %} {{ i }} {% else %} % if i ==
 executions.paginator.num_pages %} class="end" {% endif %}>{{ i }}
- {% endif %} {% endfor %} {% endif %} {{ executions.paginator.count }} {%
-blocktranslate count counter=executions.paginator.count %}entry {% plural
-%}entries{% endblocktranslate %}
+ {% endif %} {% endfor %} {{ executions.paginator.count }} {% blocktranslate
+count counter=executions.paginator.count %}entry {% plural %}entries{%
+endblocktranslate %} {% endif %}
+ {% endif %}
```

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/jobs.html` & `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/jobs.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/queue_workers.html` & `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/queue_workers.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/scheduler_base.html` & `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/scheduler_base.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/stats.html` & `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/stats.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/worker_details.html` & `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/worker_details.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/workers-list.partial.html` & `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/workers-list.partial.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/templates/admin/scheduler/workers.html` & `django_rq_scheduler-2023.5.0b4/scheduler/templates/admin/scheduler/workers.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/tests/jobs.py` & `django_rq_scheduler-2023.5.0b4/scheduler/tests/jobs.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/tests/test_internals.py` & `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/tests/test_job_arg_models.py` & `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_job_arg_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/tests/test_mgmt_cmds.py` & `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_mgmt_cmds.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/tests/test_models.py` & `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import zoneinfo
 from datetime import datetime, timedelta
 
-from django.conf import settings
 from django.contrib.messages import get_messages
 from django.core.exceptions import ValidationError
+from django.test import override_settings
 from django.urls import reverse
 from django.utils import timezone
 
+from scheduler import settings
 from scheduler.models import BaseJob, CronJob, JobArg, JobKwarg, RepeatableJob, ScheduledJob
 from scheduler.tools import run_job, create_worker
 from . import jobs
 from .testtools import job_factory, jobarg_factory, _get_job_from_queue, SchedulerBaseCase, _get_executions
 from ..queues import get_queue
 
 
@@ -53,36 +54,36 @@
         def test_clean_callable_invalid(self):
             job = job_factory(self.JobModelClass)
             job.callable = 'scheduler.tests.jobs.test_non_callable'
             with self.assertRaises(ValidationError):
                 job.clean_callable()
 
         def test_clean_queue(self):
-            for queue in settings.RQ_QUEUES.keys():
+            for queue in settings.QUEUES.keys():
                 job = job_factory(self.JobModelClass)
                 job.queue = queue
                 self.assertIsNone(job.clean_queue())
 
         def test_clean_queue_invalid(self):
             job = job_factory(self.JobModelClass)
             job.queue = 'xxxxxx'
             job.callable = 'scheduler.tests.jobs.test_job'
             with self.assertRaises(ValidationError):
                 job.clean()
 
         # next 2 check the above are included in job.clean() function
         def test_clean_base(self):
             job = job_factory(self.JobModelClass)
-            job.queue = list(settings.RQ_QUEUES)[0]
+            job.queue = list(settings.QUEUES)[0]
             job.callable = 'scheduler.tests.jobs.test_job'
             self.assertIsNone(job.clean())
 
         def test_clean_invalid_callable(self):
             job = job_factory(self.JobModelClass)
-            job.queue = list(settings.RQ_QUEUES)[0]
+            job.queue = list(settings.QUEUES)[0]
             job.callable = 'scheduler.tests.jobs.test_non_callable'
             with self.assertRaises(ValidationError):
                 job.clean()
 
         def test_clean_invalid_queue(self):
             job = job_factory(self.JobModelClass)
             job.queue = 'xxxxxx'
@@ -132,15 +133,15 @@
         def test_save_and_schedule(self):
             job = job_factory(self.JobModelClass, )
             self.assertIsNotNone(job.job_id)
             self.assertTrue(job.is_scheduled())
 
         def test_schedule2(self):
             job = job_factory(self.JobModelClass)
-            job.queue = list(settings.RQ_QUEUES)[0]
+            job.queue = list(settings.QUEUES)[0]
             job.enabled = False
             job.scheduled_time = timezone.now() + timedelta(minutes=1)
             self.assertFalse(job.schedule())
 
         def test_delete_and_unschedule(self):
             job = job_factory(self.JobModelClass, )
             self.assertIsNotNone(job.job_id)
@@ -169,15 +170,15 @@
         def test_timeout_passthrough(self):
             job = job_factory(self.JobModelClass, timeout=500)
             entry = _get_job_from_queue(job)
             self.assertEqual(entry.timeout, 500)
 
         def test_at_front_passthrough(self):
             job = job_factory(self.JobModelClass, at_front=True)
-            queue = job._get_rqueue()
+            queue = job.rqueue
             jobs_to_schedule = queue.scheduled_job_registry.get_job_ids()
             self.assertIn(job.job_id, jobs_to_schedule)
 
         def test_callable_result(self):
             job = job_factory(self.JobModelClass, )
             entry = _get_job_from_queue(job)
             self.assertEqual(entry.perform(), 2)
@@ -453,15 +454,15 @@
 
 
 class TestScheduledJob(BaseTestCases.TestSchedulableJob):
     JobModelClass = ScheduledJob
 
     def test_clean(self):
         job = job_factory(self.JobModelClass)
-        job.queue = list(settings.RQ_QUEUES)[0]
+        job.queue = list(settings.QUEUES)[0]
         job.callable = 'scheduler.tests.jobs.test_job'
         self.assertIsNone(job.clean())
 
     def test_unschedulable_old_job(self):
         job = job_factory(self.JobModelClass, scheduled_time=timezone.now() - timedelta(hours=1))
         self.assertFalse(job.is_scheduled())
 
@@ -476,72 +477,75 @@
     def test_schedulable_old_job_repeat_none(self):
         # If repeat is None, the job should be scheduled
         job = job_factory(self.JobModelClass, scheduled_time=timezone.now() - timedelta(hours=1), repeat=None)
         self.assertTrue(job.is_scheduled())
 
     def test_clean(self):
         job = job_factory(self.JobModelClass)
-        job.queue = list(settings.RQ_QUEUES)[0]
+        job.queue = list(settings.QUEUES)[0]
         job.callable = 'scheduler.tests.jobs.test_job'
         job.interval = 1
         job.result_ttl = -1
         self.assertIsNone(job.clean())
 
     def test_clean_seconds(self):
         job = job_factory(self.JobModelClass)
-        job.queue = list(settings.RQ_QUEUES)[0]
+        job.queue = list(settings.QUEUES)[0]
         job.callable = 'scheduler.tests.jobs.test_job'
         job.interval = 60
         job.result_ttl = -1
         job.interval_unit = 'seconds'
         self.assertIsNone(job.clean())
 
+    @override_settings(SCHEDULER_CONFIG={
+        'SCHEDULER_INTERVAL': 10,
+    })
     def test_clean_too_frequent(self):
         job = job_factory(self.JobModelClass)
-        job.queue = list(settings.RQ_QUEUES)[0]
+        job.queue = list(settings.QUEUES)[0]
         job.callable = 'scheduler.tests.jobs.test_job'
-        job.interval = 10
+        job.interval = 2  # Smaller than 10
         job.result_ttl = -1
         job.interval_unit = 'seconds'
         with self.assertRaises(ValidationError):
             job.clean_interval_unit()
 
     def test_clean_not_multiple(self):
         job = job_factory(self.JobModelClass)
-        job.queue = list(settings.RQ_QUEUES)[0]
+        job.queue = list(settings.QUEUES)[0]
         job.callable = 'scheduler.tests.jobs.test_job'
         job.interval = 121
         job.interval_unit = 'seconds'
         with self.assertRaises(ValidationError):
             job.clean_interval_unit()
 
     def test_clean_short_result_ttl(self):
         job = job_factory(self.JobModelClass)
-        job.queue = list(settings.RQ_QUEUES)[0]
+        job.queue = list(settings.QUEUES)[0]
         job.callable = 'scheduler.tests.jobs.test_job'
         job.interval = 1
         job.repeat = 1
         job.result_ttl = 3599
         job.interval_unit = 'hours'
         job.repeat = 42
         with self.assertRaises(ValidationError):
             job.clean_result_ttl()
 
     def test_clean_indefinite_result_ttl(self):
         job = job_factory(self.JobModelClass)
-        job.queue = list(settings.RQ_QUEUES)[0]
+        job.queue = list(settings.QUEUES)[0]
         job.callable = 'scheduler.tests.jobs.test_job'
         job.interval = 1
         job.result_ttl = -1
         job.interval_unit = 'hours'
         job.clean_result_ttl()
 
     def test_clean_undefined_result_ttl(self):
         job = job_factory(self.JobModelClass)
-        job.queue = list(settings.RQ_QUEUES)[0]
+        job.queue = list(settings.QUEUES)[0]
         job.callable = 'scheduler.tests.jobs.test_job'
         job.interval = 1
         job.interval_unit = 'hours'
         job.clean_result_ttl()
 
     def test_interval_seconds_weeks(self):
         job = job_factory(self.JobModelClass, interval=2, interval_unit='weeks')
@@ -602,48 +606,48 @@
         job.interval_unit = 'seconds'
         job.schedule()
         self.assertTrue(job.scheduled_time > base_time)
         self.assertTrue(job.is_scheduled())
 
     def test_check_rescheduled_after_execution(self):
         job = job_factory(self.JobModelClass, scheduled_time=timezone.now() + timedelta(seconds=1))
-        queue = job._get_rqueue()
+        queue = job.rqueue
         first_run_id = job.job_id
         entry = queue.fetch_job(first_run_id)
         queue.run_sync(entry)
         job.refresh_from_db()
         self.assertTrue(job.is_scheduled())
         self.assertNotEquals(job.job_id, first_run_id)
 
 
 class TestCronJob(BaseTestCases.TestBaseJob):
     JobModelClass = CronJob
 
     def test_clean(self):
         job = job_factory(self.JobModelClass)
         job.cron_string = '* * * * *'
-        job.queue = list(settings.RQ_QUEUES)[0]
+        job.queue = list(settings.QUEUES)[0]
         job.callable = 'scheduler.tests.jobs.test_job'
         self.assertIsNone(job.clean())
 
     def test_clean_cron_string_invalid(self):
         job = job_factory(self.JobModelClass)
         job.cron_string = 'not-a-cron-string'
-        job.queue = list(settings.RQ_QUEUES)[0]
+        job.queue = list(settings.QUEUES)[0]
         job.callable = 'scheduler.tests.jobs.test_job'
         with self.assertRaises(ValidationError):
             job.clean_cron_string()
 
     def test_repeat(self):
         job = job_factory(self.JobModelClass, repeat=10)
         entry = _get_job_from_queue(job)
         self.assertEqual(entry.meta['repeat'], 10)
 
     def test_check_rescheduled_after_execution(self):
         job = job_factory(self.JobModelClass, )
-        queue = job._get_rqueue()
+        queue = job.rqueue
         first_run_id = job.job_id
         entry = queue.fetch_job(first_run_id)
         queue.run_sync(entry)
         job.refresh_from_db()
         self.assertTrue(job.is_scheduled())
         self.assertNotEquals(job.job_id, first_run_id)
```

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/tests/test_redis_models.py` & `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_redis_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/tests/test_settings.py` & `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.conf import settings
 
 from scheduler.settings import conf_settings
 
-settings.RQ_QUEUES = {
+settings.SCHEDULER_QUEUES = {
     'default': {'HOST': 'localhost', 'PORT': 6379, 'DB': 0, 'DEFAULT_TIMEOUT': 500},
     'test': {
         'HOST': 'localhost',
         'PORT': 1,
         'DB': 1,
     },
     'sentinel': {
```

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/tests/test_views.py` & `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,15 @@
 from . import test_settings  # noqa
 from .jobs import access_self, failing_job
 from ..rq_classes import JobExecution, ExecutionStatus
 
 
 class ViewTest(TestCase):
     def setUp(self):
-        self.user = User.objects.create_user('foo', password='pass')
-        self.user.is_staff = True
-        self.user.is_active = True
-        self.user.save()
+        self.user = User.objects.create_superuser('user', password='pass')
         self.client = Client()
         self.client.login(username=self.user.username, password='pass')
         get_queue('django_rq_scheduler_test').connection.flushall()
 
     def test_jobs(self):
         """Jobs in queue are displayed properly"""
         queue = get_queue('default')
@@ -353,15 +350,15 @@
         self.assertEqual(404, response.status_code)
 
     def test_statistics_json_view(self):
         """
         Django-RQ's statistic as JSON only viewable by staff or with API_TOKEN
         """
 
-        # Override testing RQ_QUEUES
+        # Override testing SCHEDULER_QUEUES
         queues = {
             'default': {
                 'DB': 0,
                 'HOST': 'localhost',
                 'PORT': 6379,
             }
         }
```

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/tests/test_worker.py` & `django_rq_scheduler-2023.5.0b4/scheduler/tests/test_worker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import uuid
 
 from scheduler.tests.testtools import SchedulerBaseCase
 from scheduler.tools import create_worker
 from . import test_settings  # noqa
+from .. import settings
 
 
 class TestWorker(SchedulerBaseCase):
     def test_create_worker__two_workers_same_queue(self):
         worker1 = create_worker('default', 'django_rq_scheduler_test')
         worker1.register_birth()
         worker2 = create_worker('default')
@@ -25,7 +26,15 @@
         worker1 = create_worker('default', name=name)
         self.assertEqual(name, worker1.name)
 
     def test_create_worker__with_name_containing_slash(self):
         name = uuid.uuid4().hex[-4:] + '/' + uuid.uuid4().hex[-4:]
         worker1 = create_worker('default', name=name)
         self.assertEqual(name.replace('/', '.'), worker1.name)
+
+    def test_create_worker__scheduler_interval(self):
+        prev = settings.SCHEDULER_CONFIG['SCHEDULER_INTERVAL']
+        settings.SCHEDULER_CONFIG['SCHEDULER_INTERVAL'] = 1
+        worker = create_worker('default')
+        worker.work(burst=True)
+        self.assertEqual(worker.scheduler.interval, 1)
+        settings.SCHEDULER_CONFIG['SCHEDULER_INTERVAL'] = prev
```

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/tests/testtools.py` & `django_rq_scheduler-2023.5.0b4/scheduler/tests/testtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import timedelta
 
-from django.conf import settings
+from scheduler import settings
 from django.contrib.auth.models import User
 from django.contrib.contenttypes.models import ContentType
 from django.test import Client, TestCase
 from django.utils import timezone
 
 from scheduler.models import CronJob, JobKwarg, RepeatableJob, ScheduledJob
 from scheduler.queues import get_queue
@@ -20,15 +20,15 @@
 seq = sequence_gen()
 
 
 def job_factory(cls, instance_only=False, **kwargs):
     values = dict(
         name='Scheduled Job %d' % next(seq),
         job_id=None,
-        queue=list(settings.RQ_QUEUES.keys())[0],
+        queue=list(settings.QUEUES.keys())[0],
         callable='scheduler.tests.jobs.test_job',
         enabled=True,
         timeout=None)
     if cls == ScheduledJob:
         values.update(dict(
             result_ttl=None,
             scheduled_time=timezone.now() + timedelta(days=1), ))
@@ -64,15 +64,15 @@
         values['key'] = 'key%d' % next(seq),
     values.update(kwargs)
     instance = cls.objects.create(**values)
     return instance
 
 
 def _get_job_from_queue(django_job):
-    queue = django_job._get_rqueue()
+    queue = django_job.rqueue
     jobs_to_schedule = queue.scheduled_job_registry.get_job_ids()
     entry = next(i for i in jobs_to_schedule if i == django_job.job_id)
     return queue.fetch_job(entry)
 
 
 def _get_executions(django_job):
     queue = get_queue(django_job.queue)
```

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/tools.py` & `django_rq_scheduler-2023.5.0b4/scheduler/tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import importlib
 import os
 
 import croniter
 from django.apps import apps
 from django.utils import timezone
 
-from scheduler.decorators import job
 from scheduler.queues import get_queues, logger, get_queue
-from scheduler.rq_classes import DjangoWorker
-
-MODEL_NAMES = ['ScheduledJob', 'RepeatableJob', 'CronJob']
+from scheduler.rq_classes import DjangoWorker, MODEL_NAMES
 
 
 def callable_func(callable_str: str):
     path = callable_str.split('.')
     module = importlib.import_module('.'.join(path[:-1]))
     func = getattr(module, path[-1])
     if callable(func) is False:
@@ -25,26 +22,14 @@
     """Calculate the next scheduled time by creating a crontab object
     with a cron string"""
     now = timezone.now()
     itr = croniter.croniter(cron_string, now)
     return itr.get_next(timezone.datetime)
 
 
-@job
-def reschedule_all_jobs():
-    logger.debug("Rescheduling all jobs")
-    for model_name in MODEL_NAMES:
-        model = apps.get_model(app_label='scheduler', model_name=model_name)
-        enabled_jobs = model.objects.filter(enabled=True)
-        unscheduled_jobs = filter(lambda j: not j.is_scheduled(), enabled_jobs)
-        for item in unscheduled_jobs:
-            logger.debug(f"Rescheduling {str(item)}")
-            item.save()
-
-
 def get_scheduled_job(task_model: str, task_id: int):
     if task_model not in MODEL_NAMES:
         raise ValueError(f'Job Model {task_model} does not exist, choices are {MODEL_NAMES}')
     model = apps.get_model(app_label='scheduler', model_name=task_model)
     task = model.objects.filter(id=task_id).first()
     if task is None:
         raise ValueError(f'Job {task_model}:{task_id} does not exit')
@@ -86,18 +71,10 @@
     kwargs['name'] = kwargs['name'].replace('/', '.')
     worker = DjangoWorker(queues, connection=queues[0].connection, **kwargs)
     return worker
 
 
 def get_job_executions(queue_name, scheduled_job):
     queue = get_queue(queue_name)
-    res = list()
     job_list = queue.get_all_jobs()
-    res.extend(list(filter(lambda j: j.is_execution_of(scheduled_job), job_list)))
-    scheduled_job_id_list = queue.scheduled_job_registry.get_job_ids()
-
-    res.extend(list(
-        map(lambda j: j.to_json(),
-            filter(lambda j: j.is_execution_of(scheduled_job),
-                   map(queue.fetch_job, scheduled_job_id_list)
-                   ))))
+    res = list(filter(lambda j: j.is_execution_of(scheduled_job), job_list))
     return res
```

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/urls.py` & `django_rq_scheduler-2023.5.0b4/scheduler/urls.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b3/scheduler/views.py` & `django_rq_scheduler-2023.5.0b4/scheduler/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,29 +7,18 @@
 from django.http import JsonResponse
 from django.http.response import HttpResponseNotFound, Http404
 from django.shortcuts import redirect
 from django.shortcuts import render
 from django.urls import reverse
 from django.views.decorators.cache import never_cache
 from redis.exceptions import ResponseError
-from rq import requeue_job
-from rq.exceptions import NoSuchJobError
-from rq.registry import (
-    DeferredJobRegistry,
-    FailedJobRegistry,
-    FinishedJobRegistry,
-    ScheduledJobRegistry,
-    StartedJobRegistry,
-    clean_registries,
-)
-from rq.worker_registration import clean_worker_registry
 
 from .queues import get_all_workers, get_connection, logger, get_queue
 from .rq_classes import JobExecution, ExecutionStatus, DjangoWorker
-from .settings import SCHEDULER
+from .settings import SCHEDULER_CONFIG
 
 
 def get_worker_executions(worker):
     res = list()
     for queue in worker.queues:
         curr_jobs = queue.get_all_jobs()
         curr_jobs = [j for j in curr_jobs if j.worker_name == worker.name]
@@ -52,23 +41,26 @@
 
     return HttpResponseNotFound()
 
 
 def get_statistics(run_maintenance_tasks=False):
     from scheduler.settings import QUEUES
     queues = []
+    if run_maintenance_tasks:
+        workers = get_all_workers()
+        for worker in workers:
+            worker.clean_registries()
     for queue_name in QUEUES:
         try:
             queue = get_queue(queue_name)
             connection = get_connection(queue.name)
             connection_kwargs = connection.connection_pool.connection_kwargs
 
             if run_maintenance_tasks:
-                clean_registries(queue)
-                clean_worker_registry(queue)
+                queue.clean_registries()
 
             # Raw access to the first item from left of the redis list.
             # This might not be accurate since new job can be added from the left
             # with `at_front` parameters.
             # Ideally rq should supports Queue.oldest_job
 
             last_job_id = connection.lindex(queue.key, 0)
@@ -101,15 +93,15 @@
             logger.error(f'Could not connect for queue {queue_name}: {e}')
             continue
 
     return {'queues': queues}
 
 
 def _get_registry_job_list(queue, registry, page):
-    items_per_page = SCHEDULER['EXECUTIONS_IN_PAGE']
+    items_per_page = SCHEDULER_CONFIG['EXECUTIONS_IN_PAGE']
     num_jobs = len(registry)
     job_list = []
 
     if num_jobs == 0:
         return job_list, num_jobs, []
 
     last_page = int(ceil(num_jobs / items_per_page))
@@ -122,18 +114,15 @@
     if registry is not queue:
         for job_id in remove_job_ids:
             registry.remove(job_id)
 
     return valid_jobs, num_jobs, page_range
 
 
-def jobs_view(request, queue_name, registry_class, status_title):
-    queue = get_queue(queue_name)
-
-    registry = registry_class(queue.name, queue.connection) if registry_class is not None else queue
+def jobs_view(request, queue, registry, status_title):
     page = int(request.GET.get('page', 1))
     job_list, num_jobs, page_range = _get_registry_job_list(queue, registry, page)
 
     context_data = {
         **admin.site.each_context(request),
         'queue': queue,
         'jobs': job_list,
@@ -144,53 +133,60 @@
     }
     return render(request, 'admin/scheduler/jobs.html', context_data)
 
 
 @never_cache
 @staff_member_required
 def jobs(request, queue_name):
-    return jobs_view(request, queue_name, None, 'Queued')
+    queue = get_queue(queue_name)
+    return jobs_view(request, queue, queue, 'Queued')
 
 
 @never_cache
 @staff_member_required
 def finished_jobs(request, queue_name):
-    return jobs_view(request, queue_name, FinishedJobRegistry, 'Finished')
+    queue = get_queue(queue_name)
+    return jobs_view(request, queue, queue.finished_job_registry, 'Finished')
 
 
 @never_cache
 @staff_member_required
 def failed_jobs(request, queue_name):
-    return jobs_view(request, queue_name, FailedJobRegistry, 'Failed')
+    queue = get_queue(queue_name)
+    return jobs_view(request, queue, queue.failed_job_registry, 'Failed')
 
 
 @never_cache
 @staff_member_required
 def scheduled_jobs(request, queue_name):
-    return jobs_view(request, queue_name, ScheduledJobRegistry, 'Scheduled')
+    queue = get_queue(queue_name)
+    return jobs_view(request, queue, queue.scheduled_job_registry, 'Scheduled')
 
 
 @never_cache
 @staff_member_required
 def started_jobs(request, queue_name):
-    return jobs_view(request, queue_name, StartedJobRegistry, 'Started')
+    queue = get_queue(queue_name)
+    return jobs_view(request, queue, queue.started_job_registry, 'Started')
 
 
 @never_cache
 @staff_member_required
 def deferred_jobs(request, queue_name):
-    return jobs_view(request, queue_name, DeferredJobRegistry, 'Deferred')
+    queue = get_queue(queue_name)
+    return jobs_view(request, queue, queue.deferred_job_registry, 'Deferred')
 
 
 @never_cache
 @staff_member_required
 def queue_workers(request, queue_name):
     queue = get_queue(queue_name)
-    clean_worker_registry(queue)
     all_workers = DjangoWorker.all(queue.connection)
+    for w in all_workers:
+        w.clean_registries()
     worker_list = [worker for worker in all_workers if queue.name in worker.queue_names()]
 
     context_data = {
         **admin.site.each_context(request),
         'queue': queue,
         'workers': worker_list,
     }
@@ -219,15 +215,15 @@
 
     if worker is None:
         raise Http404(f"Couldn't find worker with this ID: {name}")
     # Convert microseconds to milliseconds
     worker.total_working_time = worker.total_working_time / 1000
 
     execution_list = get_worker_executions(worker)
-    paginator = Paginator(execution_list, SCHEDULER['EXECUTIONS_IN_PAGE'])
+    paginator = Paginator(execution_list, SCHEDULER_CONFIG['EXECUTIONS_IN_PAGE'])
     page_number = request.GET.get('p', 1)
     page_obj = paginator.get_page(page_number)
     page_range = paginator.get_elided_page_range(page_obj.number)
     context_data = {
         **admin.site.each_context(request),
         'queue': queue,
         'worker': worker,
@@ -248,17 +244,15 @@
     queue_index, queue, job = None, None, None
 
     for queue_name in QUEUES:
         try:
             queue = get_queue(queue_name)
             job = JobExecution.fetch(job_id, connection=queue.connection)
             break
-        except NoSuchJobError:
-            pass
-        except redis.ConnectionError:
+        except Exception:
             pass
     if job is None:
         raise Http404(f"Couldn't find job with this ID: {job_id}")
     try:
         job.func_name
         data_is_valid = True
     except Exception:
@@ -305,15 +299,15 @@
 @never_cache
 @staff_member_required
 def requeue_job_view(request, queue_name, job_id):
     queue = get_queue(queue_name)
     job = JobExecution.fetch(job_id, connection=queue.connection)
 
     if request.method == 'POST':
-        requeue_job(job_id, connection=queue.connection)
+        job.requeue()
         messages.info(request, f'You have successfully re-queued {job.id}')
         return redirect('job_details', job_id)
 
     context_data = {
         **admin.site.each_context(request),
         'job': job,
         'queue': queue,
@@ -347,34 +341,34 @@
     return render(request, 'admin/scheduler/confirm_action.html', context_data)
 
 
 @never_cache
 @staff_member_required
 def requeue_all(request, queue_name):
     queue = get_queue(queue_name)
-    registry = FailedJobRegistry(queue=queue)
     next_url = request.META.get('HTTP_REFERER') or reverse('queue_jobs', args=[queue_name])
-    job_ids = registry.get_job_ids()
+    job_ids = queue.failed_job_registry.get_job_ids()
     if request.method == 'POST':
         count = 0
         # Confirmation received
         for job_id in job_ids:
             try:
-                requeue_job(job_id, connection=queue.connection)
+                job = JobExecution.fetch(job_id, connection=queue.connection)
+                job.requeue()
                 count += 1
-            except NoSuchJobError:
+            except Exception:
                 pass
 
         messages.info(request, f'You have successfully re-queued {count} jobs!')
         return redirect('queue_jobs', queue_name)
 
     context_data = {
         **admin.site.each_context(request),
         'queue': queue,
-        'total_jobs': len(registry),
+        'total_jobs': len(queue.failed_job_registry),
         'action': 'requeue',
         'jobs': [queue.fetch_job(job_id) for job_id in job_ids],
         'next_url': next_url,
         'action_url': reverse('queue_requeue_all', args=[queue_name, ])
     }
 
     return render(request, 'admin/scheduler/confirm_action.html', context_data)
@@ -420,15 +414,16 @@
                     job = JobExecution.fetch(job_id, connection=queue.connection)
                     # Remove job id from queue and delete the actual job
                     queue.connection.lrem(queue.key, 0, job.id)
                     job.delete()
                 messages.info(request, f'You have successfully deleted {len(job_ids)} jobs!')
             elif request.POST['action'] == 'requeue':
                 for job_id in job_ids:
-                    requeue_job(job_id, connection=queue.connection)
+                    job = JobExecution.fetch(job_id, connection=queue.connection)
+                    job.requeue()
                 messages.info(request, f'You have successfully re-queued {len(job_ids)}  jobs!')
             elif request.POST['action'] == 'stop':
                 cancelled_jobs = 0
                 for job_id in job_ids:
                     try:
                         job = JobExecution.fetch(job_id, connection=queue.connection)
                         job.stop_execution(queue.connection)
@@ -450,22 +445,19 @@
     job = JobExecution.fetch(job_id, connection=queue.connection)
 
     if request.method == 'POST':
         queue.enqueue_job(job)
 
         # Remove job from correct registry if needed
         if job.get_status() == ExecutionStatus.DEFERRED:
-            registry = DeferredJobRegistry(queue.name, queue.connection)
-            registry.remove(job)
+            queue.deferred_job_registry.remove(job)
         elif job.get_status() == ExecutionStatus.FINISHED:
-            registry = FinishedJobRegistry(queue.name, queue.connection)
-            registry.remove(job)
+            queue.finished_job_registry.remove(job)
         elif job.get_status() == ExecutionStatus.SCHEDULED:
-            registry = ScheduledJobRegistry(queue.name, queue.connection)
-            registry.remove(job)
+            queue.scheduled_job_registry.remove(job)
 
         messages.info(request, 'You have successfully enqueued %s' % job.id)
         return redirect('job_details', job_id)
 
     context_data = {
         **admin.site.each_context(request),
         'job': job,
```

### Comparing `django_rq_scheduler-2023.5.0b3/PKG-INFO` & `django_rq_scheduler-2023.5.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rq-scheduler
-Version: 2023.5.0b3
+Version: 2023.5.0b4
 Summary: An async job scheduler for django using redis
 Home-page: https://github.com/dsoftwareinc/django-rq-scheduler
 License: MIT
 Keywords: redis,django,background-jobs,job-queue,task-queue,redis-queue,scheduled-jobs
 Author: Daniel Moran
 Author-email: daniel.maruani@gmail.com
 Maintainer: Daniel Moran
```

