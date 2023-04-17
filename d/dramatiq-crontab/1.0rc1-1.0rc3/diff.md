# Comparing `tmp/dramatiq-crontab-1.0rc1.tar.gz` & `tmp/dramatiq-crontab-1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramatiq-crontab-1.0rc1.tar", last modified: Fri Apr 14 09:57:38 2023, max compression
+gzip compressed data, was "dramatiq-crontab-1.0rc3.tar", last modified: Mon Apr 17 07:10:33 2023, max compression
```

## Comparing `dramatiq-crontab-1.0rc1.tar` & `dramatiq-crontab-1.0rc3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1497 2023-04-13 14:44:34.004395 dramatiq-crontab-1.0rc1/LICENSE
--rw-r--r--   0        0        0     1467 2023-04-14 09:56:27.984769 dramatiq-crontab-1.0rc1/README.md
--rw-r--r--   0        0        0     2562 2023-04-14 09:56:27.987248 dramatiq-crontab-1.0rc1/dramatiq_crontab/__init__.py
--rw-r--r--   0        0        0      158 2023-04-14 09:57:38.827701 dramatiq-crontab-1.0rc1/dramatiq_crontab/_version.py
--rw-r--r--   0        0        0        0 2023-04-14 09:56:27.987359 dramatiq-crontab-1.0rc1/dramatiq_crontab/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 09:56:27.987622 dramatiq-crontab-1.0rc1/dramatiq_crontab/management/commands/__init__.py
--rw-r--r--   0        0        0     2966 2023-04-14 09:56:27.987933 dramatiq-crontab-1.0rc1/dramatiq_crontab/management/commands/crontab.py
--rw-r--r--   0        0        0      157 2023-04-14 09:56:27.988203 dramatiq-crontab-1.0rc1/dramatiq_crontab/tasks.py
--rw-r--r--   0        0        0     2436 2023-04-14 09:56:27.988641 dramatiq-crontab-1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     3389 1970-01-01 00:00:00.000000 dramatiq-crontab-1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-04-17 07:10:13.287619 dramatiq-crontab-1.0rc3/LICENSE
+-rw-r--r--   0        0        0     2738 2023-04-17 07:10:13.287619 dramatiq-crontab-1.0rc3/README.md
+-rw-r--r--   0        0        0     2288 2023-04-17 07:10:13.287619 dramatiq-crontab-1.0rc3/dramatiq_crontab/__init__.py
+-rw-r--r--   0        0        0      158 2023-04-17 07:10:32.903916 dramatiq-crontab-1.0rc3/dramatiq_crontab/_version.py
+-rw-r--r--   0        0        0      255 2023-04-17 07:10:13.287619 dramatiq-crontab-1.0rc3/dramatiq_crontab/conf.py
+-rw-r--r--   0        0        0        0 2023-04-17 07:10:13.287619 dramatiq-crontab-1.0rc3/dramatiq_crontab/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 07:10:13.287619 dramatiq-crontab-1.0rc3/dramatiq_crontab/management/commands/__init__.py
+-rw-r--r--   0        0        0     2989 2023-04-17 07:10:13.287619 dramatiq-crontab-1.0rc3/dramatiq_crontab/management/commands/crontab.py
+-rw-r--r--   0        0        0      157 2023-04-17 07:10:13.287619 dramatiq-crontab-1.0rc3/dramatiq_crontab/tasks.py
+-rw-r--r--   0        0        0     2469 2023-04-17 07:10:13.287619 dramatiq-crontab-1.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     4715 1970-01-01 00:00:00.000000 dramatiq-crontab-1.0rc3/PKG-INFO
```

### Comparing `dramatiq-crontab-1.0rc1/LICENSE` & `dramatiq-crontab-1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dramatiq-crontab-1.0rc1/dramatiq_crontab/__init__.py` & `dramatiq-crontab-1.0rc3/dramatiq_crontab/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,47 +43,41 @@
 
     The monitor slug is your actor name, the schedule should be set to the same
     cron schedule as the cron decorator. The schedule type should be set to cron.
     The monitors timezone should be set to Europe/Berlin.
     """
 
     def decorator(func):
-        minute, hour, day_of_month, month, day_of_week = schedule.split(" ")
+        *_, day_of_week = schedule.split(" ")
 
-        try:
-            day_of_week = {
-                "mon": 0,
-                "tue": 1,
-                "wed": 2,
-                "thu": 3,
-                "fri": 4,
-                "sat": 5,
-                "sun": 6,
-                "*": "*",
-            }[day_of_week.lower()]
-        except KeyError as e:
+        if day_of_week.lower() not in (
+            "*",
+            "mon",
+            "tue",
+            "wed",
+            "thu",
+            "fri",
+            "sat",
+            "sun",
+        ):
             # CronTrigger uses Python's timezone dependent first weekday,
             # so in Berlin monday is 0 and sunday is 6. We use literals to avoid
             # confusion. Literals are also more readable and crontab conform.
             raise ValueError(
                 "Please use a literal day of week (Mon, Tue, Wed, Thu, Fri, Sat, Sun) or *"
-            ) from e
+            )
 
         fn = getattr(func, "send")
         if monitor is not None:
             fn = monitor(func.actor_name)(fn)
 
         scheduler.add_job(
             fn,
-            CronTrigger(
-                hour=hour,
-                minute=minute,
-                day=day_of_month,
-                month=month,
-                day_of_week=day_of_week,
+            CronTrigger.from_crontab(
+                schedule,
                 timezone=timezone.get_default_timezone(),
             ),
             name=func.actor_name,
         )
         # We don't add the Sentry monitor on the actor itself, because we only want to
         # monitor the cron job, not the actor itself, or it's direct invocations.
         return func
```

### Comparing `dramatiq-crontab-1.0rc1/pyproject.toml` & `dramatiq-crontab-1.0rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,19 @@
 dependencies = ["dramatiq", "apscheduler", "django"]
 
 [project.optional-dependencies]
 test = [
   "pytest",
   "pytest-cov",
   "pytest-django",
-  "dramatiq[redis]",
+  "dramatiq",
   "backports.zoneinfo;python_version<'3.9'"
 ]
 sentry = ["sentry-sdk"]
+redis = ["redis"]
 
 [project.urls]
 Project-URL = "https://github.com/voiio/dramatiq-crontab"
 Changelog = "https://github.com/voiio/dramatiq-crontab/releases"
 
 [tool.flit.module]
 name = "dramatiq_crontab"
@@ -74,14 +75,15 @@
 [tool.isort]
 atomic = true
 line_length = 88
 known_first_party = "dramatiq_crontab, tests"
 include_trailing_comma = true
 default_section = "THIRDPARTY"
 combine_as_imports = true
+multi_line_output = 3
 
 [tool.pydocstyle]
 add_ignore = "D1"
 
 [tool.djlint]
 profile="django"
 indent=2
```

