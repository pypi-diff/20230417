# Comparing `tmp/HawaData-0.2.9.tar.gz` & `tmp/HawaData-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.2.9.tar", last modified: Thu Apr 13 07:04:42 2023, max compression
+gzip compressed data, was "HawaData-0.3.0.tar", last modified: Mon Apr 17 08:29:53 2023, max compression
```

## Comparing `HawaData-0.2.9.tar` & `HawaData-0.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.486831 HawaData-0.2.9/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.473830 HawaData-0.2.9/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     1922 2023-04-13 07:04:42.000000 HawaData-0.2.9/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      765 2023-04-13 07:04:42.000000 HawaData-0.2.9/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-04-13 07:04:42.000000 HawaData-0.2.9/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)      257 2023-04-13 07:04:42.000000 HawaData-0.2.9/HawaData.egg-info/requires.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)       10 2023-04-13 07:04:42.000000 HawaData-0.2.9/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     1922 2023-04-13 07:04:42.486584 HawaData-0.2.9/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.2.9/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.474329 HawaData-0.2.9/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.2.9/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.476401 HawaData-0.2.9/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.2.9/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2842 2022-12-11 02:48:15.000000 HawaData-0.2.9/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.2.9/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.2.9/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.478699 HawaData-0.2.9/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.2.9/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     8762 2023-04-13 06:33:34.000000 HawaData-0.2.9/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     4582 2023-03-31 06:23:45.000000 HawaData-0.2.9/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2691 2022-12-01 05:37:32.000000 HawaData-0.2.9/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.2.9/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.479985 HawaData-0.2.9/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.2.9/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.2.9/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.2.9/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.480982 HawaData-0.2.9/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.2.9/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    22989 2023-04-13 07:01:46.000000 HawaData-0.2.9/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5252 2022-12-08 10:47:44.000000 HawaData-0.2.9/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-04-13 07:04:42.486909 HawaData-0.2.9/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      875 2022-12-02 07:10:09.000000 HawaData-0.2.9/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.482765 HawaData-0.2.9/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2022-12-01 08:54:31.000000 HawaData-0.2.9/test/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      654 2022-12-02 04:24:16.000000 HawaData-0.2.9/test/mock.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.483602 HawaData-0.2.9/test/test_common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:19.000000 HawaData-0.2.9/test/test_common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      770 2023-04-13 03:56:08.000000 HawaData-0.2.9/test/test_common/test_common_data.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.484603 HawaData-0.2.9/test/test_data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:40.000000 HawaData-0.2.9/test/test_data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1582 2023-04-13 03:55:31.000000 HawaData-0.2.9/test/test_data/test_school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.485967 HawaData-0.2.9/test/test_paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:31.000000 HawaData-0.2.9/test/test_paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      681 2023-03-29 04:15:57.000000 HawaData-0.2.9/test/test_paper/test_health_data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      491 2022-12-02 09:56:11.000000 HawaData-0.2.9/test/test_paper/test_mht_data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.2.9/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.557623 HawaData-0.3.0/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.547461 HawaData-0.3.0/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1964 2023-04-17 08:29:53.000000 HawaData-0.3.0/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      765 2023-04-17 08:29:53.000000 HawaData-0.3.0/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-04-17 08:29:53.000000 HawaData-0.3.0/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)      257 2023-04-17 08:29:53.000000 HawaData-0.3.0/HawaData.egg-info/requires.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)       10 2023-04-17 08:29:53.000000 HawaData-0.3.0/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1964 2023-04-17 08:29:53.557365 HawaData-0.3.0/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.3.0/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.547853 HawaData-0.3.0/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.3.0/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.549631 HawaData-0.3.0/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.3.0/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2842 2022-12-11 02:48:15.000000 HawaData-0.3.0/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.3.0/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.3.0/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.550923 HawaData-0.3.0/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.3.0/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     8767 2023-04-17 08:29:21.000000 HawaData-0.3.0/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     4455 2023-04-17 08:27:12.000000 HawaData-0.3.0/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2691 2022-12-01 05:37:32.000000 HawaData-0.3.0/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.3.0/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.551828 HawaData-0.3.0/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.3.0/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.3.0/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.3.0/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.552916 HawaData-0.3.0/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.3.0/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    22989 2023-04-13 07:01:46.000000 HawaData-0.3.0/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5252 2022-12-08 10:47:44.000000 HawaData-0.3.0/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-04-17 08:29:53.557703 HawaData-0.3.0/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      875 2022-12-02 07:10:09.000000 HawaData-0.3.0/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.554271 HawaData-0.3.0/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2022-12-01 08:54:31.000000 HawaData-0.3.0/test/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      654 2022-12-02 04:24:16.000000 HawaData-0.3.0/test/mock.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.554971 HawaData-0.3.0/test/test_common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:19.000000 HawaData-0.3.0/test/test_common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      770 2023-04-13 03:56:08.000000 HawaData-0.3.0/test/test_common/test_common_data.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.555807 HawaData-0.3.0/test/test_data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:40.000000 HawaData-0.3.0/test/test_data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1622 2023-04-17 08:15:54.000000 HawaData-0.3.0/test/test_data/test_school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.556750 HawaData-0.3.0/test/test_paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:31.000000 HawaData-0.3.0/test/test_paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      681 2023-03-29 04:15:57.000000 HawaData-0.3.0/test/test_paper/test_health_data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      491 2022-12-02 09:56:11.000000 HawaData-0.3.0/test/test_paper/test_mht_data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.3.0/test/test_query.py
```

### Comparing `HawaData-0.2.9/HawaData.egg-info/PKG-INFO` & `HawaData-0.3.0/HawaData.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.2.9
+Version: 0.3.0
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -70,7 +70,8 @@
 - 0.2.3 Fix cache year data
 - 0.2.4 Filter users when length id <18
 - 0.2.5 Filter users when length id <18 true
 - 0.2.6 Fix rank dis
 - 0.2.7 Fix miss grade
 - 0.2.8 Fix miss grade all
 - 0.2.9 Fix miss grade again
+- 0.3.0 Fix more school when query school
```

### Comparing `HawaData-0.2.9/HawaData.egg-info/SOURCES.txt` & `HawaData-0.3.0/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.9/PKG-INFO` & `HawaData-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.2.9
+Version: 0.3.0
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -70,7 +70,8 @@
 - 0.2.3 Fix cache year data
 - 0.2.4 Filter users when length id <18
 - 0.2.5 Filter users when length id <18 true
 - 0.2.6 Fix rank dis
 - 0.2.7 Fix miss grade
 - 0.2.8 Fix miss grade all
 - 0.2.9 Fix miss grade again
+- 0.3.0 Fix more school when query school
```

### Comparing `HawaData-0.2.9/README.md` & `HawaData-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.9/hawa/base/db.py` & `HawaData-0.3.0/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.9/hawa/base/init.py` & `HawaData-0.3.0/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.9/hawa/common/data.py` & `HawaData-0.3.0/hawa/common/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         # 计算数据
         count_functions = [i for i in dir(self) if i.startswith('_to_count_')]
         for func in count_functions:
             getattr(self, func)()
 
     def _to_init_a_meta_unit(self):
-        self.meta_unit = self.query.query_unit(self.meta_unit_type, self.meta_unit_id)
+        self.meta_unit = self.query.query_unit(self.meta_unit_type, str(self.meta_unit_id))
 
     def _to_init_b_time(self):
         if not self.target_year:
             self.target_year = pendulum.now().year
         self.last_year_num = self.target_year - 1
         project.logger.info(f'target_year: {self.target_year}')
```

### Comparing `HawaData-0.2.9/hawa/common/query.py` & `HawaData-0.3.0/hawa/common/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,18 +36,14 @@
         elif len(school_ids) == 1:
             sql = f"select * from schools where id={school_ids[0]};"
         else:
             sql = f"select * from schools where id in {tuple(school_ids)};"
         return pd.read_sql(sql, self.db.conn)
 
     def query_schools_by_startwith(self, startwith: int):
-        while startwith % 10 == 0:
-            startwith = startwith // 10
-            logger.info(f"startwith: {startwith}")
-
         param_len = len(str(startwith))
         sql = f"select * from schools where left(id,{param_len})={startwith};"
         return pd.read_sql(sql, self.db.conn)
 
     def query_papers(self, test_type: str = '', test_types: list[str] = None):
         """优先 test_types"""
         if test_types:
```

### Comparing `HawaData-0.2.9/hawa/common/utils.py` & `HawaData-0.3.0/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.9/hawa/config.py` & `HawaData-0.3.0/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.9/hawa/paper/health.py` & `HawaData-0.3.0/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.9/hawa/paper/mht.py` & `HawaData-0.3.0/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.9/setup.py` & `HawaData-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.9/test/mock.py` & `HawaData-0.3.0/test/mock.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.9/test/test_common/test_common_data.py` & `HawaData-0.3.0/test/test_common/test_common_data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.9/test/test_data/test_school.py` & `HawaData-0.3.0/test/test_data/test_school.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 
 prepare_test()
 
 
 def test_health_report_run():
     rows = [
         # {"meta_unit_id": 5134010001, "target_year": 2021},
-        {"meta_unit_id": 1101089005, "target_year": 2023},
+        {"meta_unit_id": 5134310010, "target_year": 2023},
     ]
     for row in rows:
         logger.info(row)
-        SchoolHealthReportData(**row)
+        d = SchoolHealthReportData(**row)
+        print(d.case_gender_counts)
 
 
 def test_mht_web_run():
     rows = [
         {"meta_unit_id": 4107110001, "target_year": 2022},
     ]
     for row in rows:
```

### Comparing `HawaData-0.2.9/test/test_paper/test_health_data.py` & `HawaData-0.3.0/test/test_paper/test_health_data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.9/test/test_query.py` & `HawaData-0.3.0/test/test_query.py`

 * *Files identical despite different names*

