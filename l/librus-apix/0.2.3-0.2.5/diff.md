# Comparing `tmp/librus_apix-0.2.3.tar.gz` & `tmp/librus_apix-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-0.2.3.tar", last modified: Sun Apr  2 22:28:11 2023, max compression
+gzip compressed data, was "librus_apix-0.2.5.tar", last modified: Mon Apr 17 21:11:32 2023, max compression
```

## Comparing `librus_apix-0.2.3.tar` & `librus_apix-0.2.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-02 22:28:11.422038 librus_apix-0.2.3/
--rw-r--r--   0 poro      (1000) poro      (1000)     1722 2022-09-08 20:51:34.000000 librus_apix-0.2.3/LICENSE
--rw-r--r--   0 poro      (1000) poro      (1000)     1722 2022-09-08 20:51:34.000000 librus_apix-0.2.3/LICENSE.orig
--rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-04-02 22:28:11.422038 librus_apix-0.2.3/PKG-INFO
--rw-r--r--   0 poro      (1000) poro      (1000)     2376 2023-04-02 22:22:28.000000 librus_apix-0.2.3/README.md
-drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-02 22:28:11.418704 librus_apix-0.2.3/librus_apix/
--rw-r--r--   0 poro      (1000) poro      (1000)      346 2022-09-08 20:51:34.000000 librus_apix-0.2.3/librus_apix/__init__.py
--rw-r--r--   0 poro      (1000) poro      (1000)     1156 2022-09-08 20:51:34.000000 librus_apix-0.2.3/librus_apix/announcements.py
--rw-r--r--   0 poro      (1000) poro      (1000)     3038 2023-04-02 21:48:01.000000 librus_apix-0.2.3/librus_apix/attendance.py
--rw-r--r--   0 poro      (1000) poro      (1000)      210 2022-09-08 20:51:34.000000 librus_apix-0.2.3/librus_apix/exceptions.py
--rw-r--r--   0 poro      (1000) poro      (1000)     2367 2022-09-08 20:51:34.000000 librus_apix-0.2.3/librus_apix/get_token.py
--rw-r--r--   0 poro      (1000) poro      (1000)     4346 2023-04-02 08:57:21.000000 librus_apix-0.2.3/librus_apix/grades.py
--rw-r--r--   0 poro      (1000) poro      (1000)      287 2022-12-30 11:55:28.000000 librus_apix-0.2.3/librus_apix/helpers.py
--rw-r--r--   0 poro      (1000) poro      (1000)     2175 2022-09-08 20:51:34.000000 librus_apix-0.2.3/librus_apix/homework.py
--rw-r--r--   0 poro      (1000) poro      (1000)     2108 2023-01-12 19:56:33.000000 librus_apix-0.2.3/librus_apix/messages.py
--rw-r--r--   0 poro      (1000) poro      (1000)     3053 2022-12-15 18:59:11.000000 librus_apix-0.2.3/librus_apix/schedule.py
--rw-r--r--   0 poro      (1000) poro      (1000)     3098 2022-12-14 21:45:32.000000 librus_apix-0.2.3/librus_apix/timetable.py
--rw-r--r--   0 poro      (1000) poro      (1000)      422 2022-09-08 20:51:34.000000 librus_apix-0.2.3/librus_apix/urls.py
-drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-02 22:28:11.422038 librus_apix-0.2.3/librus_apix.egg-info/
--rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-04-02 22:28:11.000000 librus_apix-0.2.3/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 poro      (1000) poro      (1000)      530 2023-04-02 22:28:11.000000 librus_apix-0.2.3/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 poro      (1000) poro      (1000)        1 2023-04-02 22:28:11.000000 librus_apix-0.2.3/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 poro      (1000) poro      (1000)       18 2023-04-02 22:28:11.000000 librus_apix-0.2.3/librus_apix.egg-info/requires.txt
--rw-r--r--   0 poro      (1000) poro      (1000)       12 2023-04-02 22:28:11.000000 librus_apix-0.2.3/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 poro      (1000) poro      (1000)       89 2022-09-08 20:51:34.000000 librus_apix-0.2.3/pyproject.toml
--rw-r--r--   0 poro      (1000) poro      (1000)      589 2023-04-02 22:28:11.425371 librus_apix-0.2.3/setup.cfg
--rw-r--r--   0 poro      (1000) poro      (1000)       37 2022-09-08 20:51:34.000000 librus_apix-0.2.3/setup.py
+drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-17 21:11:32.350315 librus_apix-0.2.5/
+-rw-r--r--   0 poro      (1000) poro      (1000)     1722 2023-04-17 20:43:54.000000 librus_apix-0.2.5/LICENSE
+-rw-r--r--   0 poro      (1000) poro      (1000)     1722 2023-04-17 20:43:54.000000 librus_apix-0.2.5/LICENSE.orig
+-rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-04-17 21:11:32.350315 librus_apix-0.2.5/PKG-INFO
+-rw-r--r--   0 poro      (1000) poro      (1000)     2427 2023-04-17 21:01:31.000000 librus_apix-0.2.5/README.md
+drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-17 21:11:32.350315 librus_apix-0.2.5/librus_apix/
+-rw-r--r--   0 poro      (1000) poro      (1000)      346 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/__init__.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     1156 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/announcements.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     3038 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/attendance.py
+-rw-r--r--   0 poro      (1000) poro      (1000)      210 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/exceptions.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2367 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/get_token.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     4680 2023-04-17 20:49:54.000000 librus_apix-0.2.5/librus_apix/grades.py
+-rw-r--r--   0 poro      (1000) poro      (1000)      287 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/helpers.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2175 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/homework.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2108 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/messages.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     3053 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/schedule.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     3098 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/timetable.py
+-rw-r--r--   0 poro      (1000) poro      (1000)      422 2023-04-17 20:43:54.000000 librus_apix-0.2.5/librus_apix/urls.py
+drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-17 21:11:32.350315 librus_apix-0.2.5/librus_apix.egg-info/
+-rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-04-17 21:11:32.000000 librus_apix-0.2.5/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 poro      (1000) poro      (1000)      530 2023-04-17 21:11:32.000000 librus_apix-0.2.5/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)        1 2023-04-17 21:11:32.000000 librus_apix-0.2.5/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)       18 2023-04-17 21:11:32.000000 librus_apix-0.2.5/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)       12 2023-04-17 21:11:32.000000 librus_apix-0.2.5/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)       89 2023-04-17 20:43:54.000000 librus_apix-0.2.5/pyproject.toml
+-rw-r--r--   0 poro      (1000) poro      (1000)      589 2023-04-17 21:11:32.353649 librus_apix-0.2.5/setup.cfg
+-rw-r--r--   0 poro      (1000) poro      (1000)       37 2023-04-17 20:43:54.000000 librus_apix-0.2.5/setup.py
```

### Comparing `librus_apix-0.2.3/LICENSE` & `librus_apix-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.3/LICENSE.orig` & `librus_apix-0.2.5/LICENSE.orig`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.3/README.md` & `librus_apix-0.2.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,54 +5,56 @@
 ```sh
 pip install librus-apix
 ```
 
 ## Quick Start
 
 ## Getting the Token
-from librus-apix.get_token import get_token
+```py
+from librus_apix.get_token import get_token
 
 token = get_token("Username", "Password")
-
+```
 ### Getting the Math grades
 
 ```py
-from librus-apix.grades import get_grades
+from librus_apix.grades import get_grades
 
 grades, average_grades = get_grades(token)
 
-for mark in grades["Mathematics"]:
-    print(mark.grade)
+for semester in grades:
+  for mark in grades[semester]["Mathematics"]:
+      print(mark.grade)
 ```
 
 ### Getting the Announcements
 ```py
-from librus-apix.announcements import get_announcements
+from librus_apix.announcements import get_announcements
 
 announcements = get_announcements(token)
 
 for a in announcements:
   print(a.description)
 
 ```
 
 ### Getting the attendance
 ```py
-from librus-apix.attendance import get_attendance
+from librus_apix.attendance import get_attendance
 
 first_semester, second_semester = get_attendance(token)
 
 for attendance in first_semester:
   print(attendance.symbol, attendance.date)
 
 ```
 
 ### Getting the Homework
 ```py
-from librus-apix.homework import get_homework, homework_detail
+from librus_apix.homework import get_homework, homework_detail
 
 # date from-to up to 1 month 
 date_from = '2023-03-02'
 date_to = '2023-03-30'
 
 homework = get_homework(token, date_from, date_to)
 
@@ -62,45 +64,45 @@
   details = homework_detail(token, href)
   print(details)
 
 ```
 
 ### Getting the Messages
 ```py
-from librus-apix.messages import get_recieved, message_content
+from librus_apix.messages import get_recieved, message_content
 
 messages = get_recieved(token, page=1)
 for message in messages:
   print(message.title)
   href = message.href
   print(message_content(token, href))
 
 ```
 
-# Getting the Schedule
+### Getting the Schedule
 
 ```py
-from librus-apix.schedule import get_schedule, schedule_detail
+from librus_apix.schedule import get_schedule, schedule_detail
 month = '2'
 year = '2023'
 schedule = get_schedule(token, month, year)
 for day in schedule:
   for event in schedule[day]:
     print(event.title)
     prefix, href = event.href.split('/')
     details = schedule_detail(token, prefix, href)
     print(details)
 
 ```
 
-# Getting the Timetable
+### Getting the Timetable
 
 ```py
 from datetime import datetime
-from librus-apix.timetable import get_timetable
+from librus_apix.timetable import get_timetable
 
 monday_date = '2023-04-3'
 monday_datetime = datetime.strptime(monday_date, '%Y-%m-%d')
 t_table = get_timetable(token, monday_datetime)
 for weekday in timetable
   for period in timetable[weekday]:
     print(period.subject, period.teacher_and_classroom)
```

### Comparing `librus_apix-0.2.3/librus_apix/announcements.py` & `librus_apix-0.2.5/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.3/librus_apix/attendance.py` & `librus_apix-0.2.5/librus_apix/attendance.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.3/librus_apix/get_token.py` & `librus_apix-0.2.5/librus_apix/get_token.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.3/librus_apix/grades.py` & `librus_apix-0.2.5/librus_apix/grades.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ctypes import ArgumentError
 import re
 from datetime import datetime
 from bs4 import BeautifulSoup
 from bs4.element import NavigableString
 from librus_apix.get_token import get_token, Token
 from librus_apix.helpers import no_access_check
 from librus_apix.exceptions import TokenError, ParseError
@@ -38,34 +39,39 @@
                 self.grade[1].replace("+", ".5").replace("-", "-0.25")
             )
         else:
             grade_value = float(self.grade)
         return grade_value
 
 
-def get_grades(token: Token, sort_by: str) -> tuple[dict[int, list[Union[Grade, Gpa]]], dict[str, Gpa]]:
-
+def get_grades(token: Token, sort_by: str = 'all') -> tuple[dict[int, list[Union[Grade, Gpa]]], dict[str, Gpa]]:
     def get_desc_and_counts(a, grade, subject) -> list[str, bool]:
         desc = f"Ocena: {_grade}\nPrzedmiot: {subject}\n"
         desc += re.sub(
             r"<br*>",
             "\n",
             a.attrs["title"].replace("<br/>", "").replace("<br />", "\n"),
         )
         gpacount = re.search("Licz do średniej: [a-zA-Z]{3}", desc)
         counts = False
         if gpacount and gpacount[0].split(": ")[1] == "tak":
             counts = True
         return desc, counts
-
+    SORT = {
+        "all": 'zmiany_logowanie_wszystkie',
+        "week": 'zmiany_logowanie_tydzien',
+        "last_login": 'zmiany_logowanie'
+            }
+    if sort_by not in SORT.keys():
+        raise ArgumentError("Wrong value for sort_by it can be either all, week or last_login") 
     sem_grades: dict[int, dict[str, list[Grade]]] = {1: {}, 2: {}}
     avg_grades = defaultdict(list)
 
     tr = no_access_check(
-            BeautifulSoup(token.post(BASE_URL + "/przegladaj_oceny/uczen", data={sort_by: 1}).text, "lxml")
+            BeautifulSoup(token.post(BASE_URL + "/przegladaj_oceny/uczen", data={SORT[sort_by]: 1}).text, "lxml")
     ).find_all("tr", attrs={"class": ["line0", "line1"], "id": None})
     if len(tr) < 1:
         raise ParseError("Error in parsing grades")
     for box in tr:
         if box.select_one("td[class='center micro screen-only']") is None:
             continue
         semester_grades = box.select(
```

### Comparing `librus_apix-0.2.3/librus_apix/homework.py` & `librus_apix-0.2.5/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.3/librus_apix/messages.py` & `librus_apix-0.2.5/librus_apix/messages.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.3/librus_apix/schedule.py` & `librus_apix-0.2.5/librus_apix/schedule.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.3/librus_apix/timetable.py` & `librus_apix-0.2.5/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.3/librus_apix.egg-info/SOURCES.txt` & `librus_apix-0.2.5/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.3/setup.cfg` & `librus_apix-0.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = 0.2.3
+version = 0.2.5
 license = MIT
 description = Web Scraper for Librus Synergia
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers = 
 	License :: OSI Approved :: MIT License
```

