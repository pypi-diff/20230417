# Comparing `tmp/najia-1.2.2.tar.gz` & `tmp/najia-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/najia-1.2.2.tar", last modified: Mon Jan 13 09:30:46 2020, max compression
+gzip compressed data, was "najia-1.2.3.tar", last modified: Wed Jul 27 16:06:24 2022, max compression
```

## Comparing `najia-1.2.2.tar` & `najia-1.2.3.tar`

### file list

```diff
@@ -1,45 +1,51 @@
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2020-01-13 09:30:46.000000 najia-1.2.2/
--rw-r--r--   0 bopo       (501) staff       (20)     2669 2020-01-13 09:30:46.000000 najia-1.2.2/PKG-INFO
--rw-r--r--   0 bopo       (501) staff       (20)     1064 2019-12-31 14:51:23.000000 najia-1.2.2/LICENSE
--rw-r--r--   0 bopo       (501) staff       (20)     3477 2019-12-31 14:51:23.000000 najia-1.2.2/CONTRIBUTING.rst
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2020-01-13 09:30:46.000000 najia-1.2.2/tests/
--rw-r--r--   0 bopo       (501) staff       (20)      224 2019-12-31 14:51:23.000000 najia-1.2.2/tests/test_mark.py
--rw-r--r--   0 bopo       (501) staff       (20)     1095 2020-01-03 07:08:12.000000 najia-1.2.2/tests/test_gua.py
--rw-r--r--   0 bopo       (501) staff       (20)       90 2020-01-10 08:27:55.000000 najia-1.2.2/tests/test_qin6.py
--rw-r--r--   0 bopo       (501) staff       (20)       60 2019-12-31 14:51:23.000000 najia-1.2.2/tests/__init__.py
--rw-r--r--   0 bopo       (501) staff       (20)      148 2019-12-31 14:51:23.000000 najia-1.2.2/tests/test_gong.py
--rw-r--r--   0 bopo       (501) staff       (20)      126 2019-12-31 14:51:23.000000 najia-1.2.2/tests/test_xkong.py
--rw-r--r--   0 bopo       (501) staff       (20)       90 2019-12-31 14:51:23.000000 najia-1.2.2/tests/test_god6.py
--rw-r--r--   0 bopo       (501) staff       (20)      128 2019-12-31 14:51:23.000000 najia-1.2.2/tests/test_compile.py
--rw-r--r--   0 bopo       (501) staff       (20)      147 2019-12-31 14:51:23.000000 najia-1.2.2/tests/test_najia.py
--rw-r--r--   0 bopo       (501) staff       (20)      262 2020-01-01 14:13:08.000000 najia-1.2.2/MANIFEST.in
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2020-01-13 09:30:46.000000 najia-1.2.2/docs/
--rw-r--r--   0 bopo       (501) staff       (20)      302 2019-12-31 14:51:23.000000 najia-1.2.2/docs/index.rst
--rw-r--r--   0 bopo       (501) staff       (20)       33 2019-12-31 14:51:23.000000 najia-1.2.2/docs/contributing.rst
--rw-r--r--   0 bopo       (501) staff       (20)      606 2019-12-31 14:51:23.000000 najia-1.2.2/docs/Makefile
--rwxr-xr-x   0 bopo       (501) staff       (20)     4761 2019-12-31 14:51:23.000000 najia-1.2.2/docs/conf.py
--rw-r--r--   0 bopo       (501) staff       (20)       65 2019-12-31 14:51:23.000000 najia-1.2.2/docs/usage.rst
--rw-r--r--   0 bopo       (501) staff       (20)      767 2019-12-31 14:51:23.000000 najia-1.2.2/docs/make.bat
--rw-r--r--   0 bopo       (501) staff       (20)       28 2019-12-31 14:51:23.000000 najia-1.2.2/docs/history.rst
--rw-r--r--   0 bopo       (501) staff       (20)     1082 2019-12-31 14:51:23.000000 najia-1.2.2/docs/installation.rst
--rw-r--r--   0 bopo       (501) staff       (20)       28 2019-12-31 14:51:23.000000 najia-1.2.2/docs/authors.rst
--rw-r--r--   0 bopo       (501) staff       (20)       27 2019-12-31 14:51:23.000000 najia-1.2.2/docs/readme.rst
--rw-r--r--   0 bopo       (501) staff       (20)     1560 2020-01-13 09:30:31.000000 najia-1.2.2/setup.py
--rw-r--r--   0 bopo       (501) staff       (20)       89 2019-12-31 14:51:23.000000 najia-1.2.2/HISTORY.rst
--rw-r--r--   0 bopo       (501) staff       (20)      144 2019-12-31 14:51:23.000000 najia-1.2.2/AUTHORS.rst
--rw-r--r--   0 bopo       (501) staff       (20)      447 2020-01-13 09:30:46.000000 najia-1.2.2/setup.cfg
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2020-01-13 09:30:46.000000 najia-1.2.2/najia.egg-info/
--rw-r--r--   0 bopo       (501) staff       (20)     2669 2020-01-13 09:30:45.000000 najia-1.2.2/najia.egg-info/PKG-INFO
--rw-r--r--   0 bopo       (501) staff       (20)        1 2020-01-13 09:30:45.000000 najia-1.2.2/najia.egg-info/not-zip-safe
--rw-r--r--   0 bopo       (501) staff       (20)      714 2020-01-13 09:30:45.000000 najia-1.2.2/najia.egg-info/SOURCES.txt
--rw-r--r--   0 bopo       (501) staff       (20)       47 2020-01-13 09:30:45.000000 najia-1.2.2/najia.egg-info/entry_points.txt
--rw-r--r--   0 bopo       (501) staff       (20)       25 2020-01-13 09:30:45.000000 najia-1.2.2/najia.egg-info/requires.txt
--rw-r--r--   0 bopo       (501) staff       (20)        6 2020-01-13 09:30:45.000000 najia-1.2.2/najia.egg-info/top_level.txt
--rw-r--r--   0 bopo       (501) staff       (20)        1 2020-01-13 09:30:45.000000 najia-1.2.2/najia.egg-info/dependency_links.txt
--rw-r--r--   0 bopo       (501) staff       (20)     1342 2020-01-01 14:13:08.000000 najia-1.2.2/README.rst
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2020-01-13 09:30:46.000000 najia-1.2.2/najia/
--rw-r--r--   0 bopo       (501) staff       (20)     7905 2020-01-13 09:30:31.000000 najia-1.2.2/najia/najia.py
--rw-r--r--   0 bopo       (501) staff       (20)      103 2020-01-13 09:30:31.000000 najia-1.2.2/najia/__init__.py
--rw-r--r--   0 bopo       (501) staff       (20)     4921 2020-01-13 09:30:31.000000 najia-1.2.2/najia/utils.py
--rw-r--r--   0 bopo       (501) staff       (20)      984 2020-01-10 08:27:55.000000 najia-1.2.2/najia/__main__.py
--rw-r--r--   0 bopo       (501) staff       (20)     4216 2019-12-31 14:54:02.000000 najia-1.2.2/najia/const.py
+drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-07-27 16:06:24.307246 najia-1.2.3/
+-rw-r--r--   0 bopo       (501) staff       (20)      144 2022-07-27 13:53:11.000000 najia-1.2.3/AUTHORS.rst
+-rw-r--r--   0 bopo       (501) staff       (20)     3477 2022-07-27 13:53:11.000000 najia-1.2.3/CONTRIBUTING.rst
+-rw-r--r--   0 bopo       (501) staff       (20)       89 2022-07-27 13:53:11.000000 najia-1.2.3/HISTORY.rst
+-rw-r--r--   0 bopo       (501) staff       (20)     1064 2022-07-27 13:53:11.000000 najia-1.2.3/LICENSE
+-rw-r--r--   0 bopo       (501) staff       (20)      293 2022-07-27 13:53:11.000000 najia-1.2.3/MANIFEST.in
+-rw-r--r--   0 bopo       (501) staff       (20)     2150 2022-07-27 16:06:24.307314 najia-1.2.3/PKG-INFO
+-rw-r--r--   0 bopo       (501) staff       (20)     1342 2022-07-27 13:53:11.000000 najia-1.2.3/README.rst
+drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-07-27 16:06:24.302542 najia-1.2.3/docs/
+-rw-r--r--   0 bopo       (501) staff       (20)      606 2022-07-27 13:53:11.000000 najia-1.2.3/docs/Makefile
+-rw-r--r--   0 bopo       (501) staff       (20)       28 2022-07-27 13:53:11.000000 najia-1.2.3/docs/authors.rst
+-rwxr-xr-x   0 bopo       (501) staff       (20)     4761 2022-07-27 13:53:11.000000 najia-1.2.3/docs/conf.py
+-rw-r--r--   0 bopo       (501) staff       (20)       33 2022-07-27 13:53:11.000000 najia-1.2.3/docs/contributing.rst
+-rw-r--r--   0 bopo       (501) staff       (20)       28 2022-07-27 13:53:11.000000 najia-1.2.3/docs/history.rst
+-rw-r--r--   0 bopo       (501) staff       (20)      302 2022-07-27 13:53:11.000000 najia-1.2.3/docs/index.rst
+-rw-r--r--   0 bopo       (501) staff       (20)     1082 2022-07-27 13:53:11.000000 najia-1.2.3/docs/installation.rst
+-rw-r--r--   0 bopo       (501) staff       (20)      767 2022-07-27 13:53:11.000000 najia-1.2.3/docs/make.bat
+-rw-r--r--   0 bopo       (501) staff       (20)       27 2022-07-27 13:53:11.000000 najia-1.2.3/docs/readme.rst
+-rw-r--r--   0 bopo       (501) staff       (20)       65 2022-07-27 13:53:11.000000 najia-1.2.3/docs/usage.rst
+drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-07-27 16:06:24.303346 najia-1.2.3/najia/
+-rw-r--r--   0 bopo       (501) staff       (20)      103 2022-07-27 16:04:59.000000 najia-1.2.3/najia/__init__.py
+-rw-r--r--   0 bopo       (501) staff       (20)      984 2022-07-27 13:53:11.000000 najia-1.2.3/najia/__main__.py
+-rw-r--r--   0 bopo       (501) staff       (20)     4172 2022-07-27 14:04:54.000000 najia-1.2.3/najia/const.py
+drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-07-27 16:06:24.305793 najia-1.2.3/najia/data/
+-rw-r--r--   0 bopo       (501) staff       (20)   125961 2022-07-27 13:53:11.000000 najia-1.2.3/najia/data/dc.json
+-rw-r--r--   0 bopo       (501) staff       (20)   116616 2022-07-27 13:53:11.000000 najia-1.2.3/najia/data/dd.json
+-rw-r--r--   0 bopo       (501) staff       (20)    58818 2022-07-27 13:53:11.000000 najia-1.2.3/najia/data/guaci.txt
+-rw-r--r--   0 bopo       (501) staff       (20)      954 2022-07-27 13:53:11.000000 najia-1.2.3/najia/data/simple.tpl
+-rw-r--r--   0 bopo       (501) staff       (20)      954 2022-07-27 13:53:11.000000 najia-1.2.3/najia/data/standard.tpl
+-rw-r--r--   0 bopo       (501) staff       (20)     8190 2022-07-27 14:07:17.000000 najia-1.2.3/najia/najia.py
+-rw-r--r--   0 bopo       (501) staff       (20)     5070 2022-07-27 15:29:15.000000 najia-1.2.3/najia/utils.py
+drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-07-27 16:06:24.304144 najia-1.2.3/najia.egg-info/
+-rw-r--r--   0 bopo       (501) staff       (20)     2150 2022-07-27 16:06:24.000000 najia-1.2.3/najia.egg-info/PKG-INFO
+-rw-r--r--   0 bopo       (501) staff       (20)      819 2022-07-27 16:06:24.000000 najia-1.2.3/najia.egg-info/SOURCES.txt
+-rw-r--r--   0 bopo       (501) staff       (20)        1 2022-07-27 16:06:24.000000 najia-1.2.3/najia.egg-info/dependency_links.txt
+-rw-r--r--   0 bopo       (501) staff       (20)       46 2022-07-27 16:06:24.000000 najia-1.2.3/najia.egg-info/entry_points.txt
+-rw-r--r--   0 bopo       (501) staff       (20)        1 2022-07-27 16:06:24.000000 najia-1.2.3/najia.egg-info/not-zip-safe
+-rw-r--r--   0 bopo       (501) staff       (20)       27 2022-07-27 16:06:24.000000 najia-1.2.3/najia.egg-info/requires.txt
+-rw-r--r--   0 bopo       (501) staff       (20)        6 2022-07-27 16:06:24.000000 najia-1.2.3/najia.egg-info/top_level.txt
+-rw-r--r--   0 bopo       (501) staff       (20)      347 2022-07-27 16:06:24.307637 najia-1.2.3/setup.cfg
+-rw-r--r--   0 bopo       (501) staff       (20)     1562 2022-07-27 13:53:11.000000 najia-1.2.3/setup.py
+drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-07-27 16:06:24.307040 najia-1.2.3/tests/
+-rw-r--r--   0 bopo       (501) staff       (20)       60 2022-07-27 13:53:11.000000 najia-1.2.3/tests/__init__.py
+-rw-r--r--   0 bopo       (501) staff       (20)      128 2022-07-27 13:53:11.000000 najia-1.2.3/tests/test_compile.py
+-rw-r--r--   0 bopo       (501) staff       (20)      709 2022-07-27 15:29:29.000000 najia-1.2.3/tests/test_god6.py
+-rw-r--r--   0 bopo       (501) staff       (20)      148 2022-07-27 13:53:11.000000 najia-1.2.3/tests/test_gong.py
+-rw-r--r--   0 bopo       (501) staff       (20)     1095 2022-07-27 13:53:11.000000 najia-1.2.3/tests/test_gua.py
+-rw-r--r--   0 bopo       (501) staff       (20)      224 2022-07-27 13:53:11.000000 najia-1.2.3/tests/test_mark.py
+-rw-r--r--   0 bopo       (501) staff       (20)      147 2022-07-27 13:53:11.000000 najia-1.2.3/tests/test_najia.py
+-rw-r--r--   0 bopo       (501) staff       (20)      389 2022-07-27 15:32:57.000000 najia-1.2.3/tests/test_qin6.py
+-rw-r--r--   0 bopo       (501) staff       (20)      399 2022-07-27 15:40:25.000000 najia-1.2.3/tests/test_xkong.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `najia-1.2.2/LICENSE` & `najia-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `najia-1.2.2/CONTRIBUTING.rst` & `najia-1.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `najia-1.2.2/tests/test_gua.py` & `najia-1.2.3/tests/test_gua.py`

 * *Files identical despite different names*

### Comparing `najia-1.2.2/docs/Makefile` & `najia-1.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `najia-1.2.2/docs/conf.py` & `najia-1.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `najia-1.2.2/docs/make.bat` & `najia-1.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `najia-1.2.2/docs/installation.rst` & `najia-1.2.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `najia-1.2.2/setup.py` & `najia-1.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['click', 'sxtwl', 'jinja2', 'arrow',]
+requirements = ['click', 'sxtwl<2', 'jinja2', 'arrow',]
 
 setup_requirements = ['pytest-runner', ]
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="bopo.wang",  
     author_email='ibopo@126.com',
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
```

### Comparing `najia-1.2.2/najia.egg-info/SOURCES.txt` & `najia-1.2.3/najia.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 najia.egg-info/PKG-INFO
 najia.egg-info/SOURCES.txt
 najia.egg-info/dependency_links.txt
 najia.egg-info/entry_points.txt
 najia.egg-info/not-zip-safe
 najia.egg-info/requires.txt
 najia.egg-info/top_level.txt
+najia/data/dc.json
+najia/data/dd.json
+najia/data/guaci.txt
+najia/data/simple.tpl
+najia/data/standard.tpl
 tests/__init__.py
 tests/test_compile.py
 tests/test_god6.py
 tests/test_gong.py
 tests/test_gua.py
 tests/test_mark.py
 tests/test_najia.py
```

### Comparing `najia-1.2.2/README.rst` & `najia-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `najia-1.2.2/najia/najia.py` & `najia-1.2.3/najia/najia.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
+import arrow
 import json
 import logging
 import os
-
-import arrow
 import sxtwl
 from jinja2 import Template
 
 from najia.const import GANS, GUA5, GUA64, XING5, YAOS, ZHI5, ZHIS
 from najia.utils import GZ5X, God6, Qin6, getNajia, palace, setShiYao, xkong
 
 logging.basicConfig(level='INFO')
@@ -15,18 +14,30 @@
 
 
 class Najia(object):
     bian = None  # 变卦
     hide = None  # 伏神
     data = None
 
-    def _gz(self, cal):
+    @staticmethod
+    def _gz(cal):
+        """
+        获取干支
+        :param cal:
+        :return:
+        """
         return GANS[cal.tg] + ZHIS[cal.dz]
 
-    def _cn(self, cal):
+    @staticmethod
+    def _cn(cal):
+        """
+
+        :param cal:
+        :return:
+        """
         return GANS[cal.tg] + ZHIS[cal.dz]
 
     def _daily(self, date=None):
         lunar = sxtwl.Lunar()
         daily = lunar.getDayBySolar(date.year, date.month, date.day)
         hour = lunar.getShiGz(daily.Lday2.tg, date.hour)
 
@@ -46,52 +57,59 @@
                 'month': self._gz(daily.Lmonth2),
                 'year': self._gz(daily.Lyear2),
                 'day': self._gz(daily.Lday2),
                 'hour': self._gz(hour),
             }
         }
 
-    def _hidden(self, gong=None, qins=None):
-        '''
+    @staticmethod
+    def _hidden(gong=None, qins=None):
+        """
         计算伏神卦
 
         :param gong:
         :param qins:
         :return:
-        '''
+        """
         if gong is None:
             raise Exception('')
 
         if qins is None:
             raise Exception('')
 
         if len(set(qins)) < 5:
             mark = YAOS[gong] * 2
+
             logger.debug(mark)
+
+            # 六亲
             qin6 = [(Qin6(XING5[int(GUA5[gong])], ZHI5[ZHIS.index(x[1])])) for x in getNajia(mark)]
+
+            # 干支五行
             qinx = [GZ5X(x) for x in getNajia(mark)]
             seat = [qin6.index(x) for x in list(set(qin6).difference(set(qins)))]
 
             return {
                 'name': GUA64.get(mark),
                 'mark': mark,
                 'qin6': qin6,
                 'qinx': qinx,
                 'seat': seat,
             }
 
         return None
 
-    def _transform(self, params=None):
-        '''
+    @staticmethod
+    def _transform(params=None):
+        """
         计算变卦
 
         :param params:
         :return:
-        '''
+        """
 
         if params is None:
             raise Exception('')
 
         if type(params) == str:
             params = [x for x in params]
 
@@ -106,24 +124,28 @@
 
             return {
                 'name': GUA64.get(mark),
                 'mark': mark,
                 'qin6': qin6,
                 'qinx': qinx,
             }
+
         return None
 
     def compile(self, params=None, gender=1, date=None, title=None, guaci=False):
-        '''
+        """
         根据参数编译卦
 
+        :param guaci:
+        :param title:
+        :param gender:
         :param params:
         :param date:
         :return:
-        '''
+        """
         solar = arrow.now() if date is None else arrow.get(date)
         lunar = self._daily(solar)
 
         gender = '男' if gender == 1 else '女'
 
         # 卦码
         mark = ''.join([str(int(l) % 2) for l in params])
@@ -177,18 +199,18 @@
         }
 
         logger.debug(self.data)
 
         return self
 
     def render(self):
-        '''
+        """
 
         :return:
-        '''
+        """
         tpl = '''{{gender}}测：{{title}}
 
 公历：{{solar.year}}年 {{solar.month}}月 {{solar.day}}日 {{solar.hour}}时 {{solar.minute}}分
 干支：{{lunar.gz.year}}年 {{lunar.gz.month}}月 {{lunar.gz.day}}日 {{lunar.gz.hour}}时 （旬空：{{lunar.xkong}})
 
 得「{{name}}」{% if bian.name %}之「{{bian.name}}」{% endif %}卦
 
@@ -232,27 +254,26 @@
             rows['bian'] = {
                 'qin6': [' ' for _ in range(0, 6)],
                 'mark': [' ' for _ in range(0, 6)],
             }
 
         shiy = []
 
-        for x in range(0, 7):
+        for x in range(0, 6):
             if x == self.data['shiy'][0] - 1:
                 shiy.append('世')
             elif x == self.data['shiy'][1] - 1:
                 shiy.append('应')
             else:
                 shiy.append('  ')
 
-        print(self.data['shiy'])
         rows['shiy'] = shiy
 
         if self.data['guaci']:
-            rows['guaci'] = json.load(open(os.path.join(os.getcwd(), 'najia/data/dd.json'))).get(rows['name'])
+            rows['guaci'] = json.load(open(os.path.join(os.path.dirname(__file__), 'data/dd.json'))).get(rows['name'])
             rows['guaci'] = rows['guaci'].replace('********************', "")
 
         template = Template(tpl)
         return template.render(**rows)
 
     def export(self):
         solar, params = self.data
```

### Comparing `najia-1.2.2/najia/utils.py` & `najia-1.2.3/najia/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,35 @@
 from najia import const
 
 logging.basicConfig(level='INFO')
 logger = logging.getLogger(__name__)
 
 
 def GZ5X(gz=''):
+    """
+    干支五行
+    :param gz:
+    :return:
+    """
     _, z = [i for i in gz]
     zm = const.ZHIS.index(z)
+
     return gz + const.XING5[const.ZHI5[zm]]
 
 
 def mark(symbol=None):
     """
     单拆重交 转 二进制卦码
     :param symbol:
     :return:
     """
+
     res = [str(int(x) % 2) for x in symbol]
     logger.debug(res)
+
     return res
 
 
 def xkong(gz='甲子'):
     """
     计算旬空
 
@@ -55,15 +63,25 @@
     """
 
     gm, _ = [i for i in gz]
 
     if type(gm) is str:
         gm = const.GANS.index(gm)
 
-    num = math.ceil((gm + 1) / 2) - 1
+    num = math.ceil((gm + 1) / 2) - 7
+
+    if gm == 4:
+        num = -4
+
+    if gm == 5:
+        num = -3
+
+    if gm > 5:
+        num += 1
+
     return const.SHEN6[num:] + const.SHEN6[:num]
 
 
 '''
 寻世诀：
 天同二世天变五，地同四世地变初。
 本宫六世三世异，人同游魂人变归。
@@ -86,15 +104,15 @@
     :param symbol: 卦的二进制码
     :return: 世爻，应爻，所在卦宫位置
     """
     wai = symbol[3:]  # 外卦
     nei = symbol[:3]  # 内卦
 
     def shiy(shi, index=None):
-        ying = shi - 3 if shi > 3 else shi + 3
+        ying = shi - 3 if shi >= 3 else shi + 3
         index = shi if index is None else index
 
         return shi, ying, index
 
     # 天同二世天变五
     if wai[2] == nei[2]:
         if wai[1] != nei[1] and wai[0] != nei[0]:
@@ -193,18 +211,18 @@
 
     wai = symbol[3:]  # 外卦
     nei = symbol[:3]  # 内卦
 
     wai, nei = const.YAOS.index(wai), const.YAOS.index(nei)
 
     gan = const.NAJIA[nei][0][0]
-    ngz = ['{}{}'.format(gan, zhi) for zhi in const.NAJIA[nei][0][1:]]  # 排干支
+    ngz = [f'{gan}{zhi}' for zhi in const.NAJIA[nei][0][1:]]  # 排干支
 
     gan = const.NAJIA[wai][1][0]
-    wgz = ['{}{}'.format(gan, zhi) for zhi in const.NAJIA[wai][1][1:]]  # 排干支
+    wgz = [f'{gan}{zhi}' for zhi in const.NAJIA[wai][1][1:]]  # 排干支
 
     return ngz + wgz
 
 
 def Qin6(w1, w2):
     """
     两个五行判断六亲
@@ -216,10 +234,12 @@
     """
     w1 = const.XING5.index(w1) if type(w1) is str else w1
     w2 = const.XING5.index(w2) if type(w2) is str else w2
 
     ws = w1 - w2
     ws = ws + 5 if ws < 0 else ws
     q6 = const.QING6[ws]
+
     logger.debug(ws)
     logger.debug(q6)
+
     return q6
```

### Comparing `najia-1.2.2/najia/__main__.py` & `najia-1.2.3/najia/__main__.py`

 * *Files identical despite different names*

### Comparing `najia-1.2.2/najia/const.py` & `najia-1.2.3/najia/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,25 +18,27 @@
     ('庚子寅辰', '庚午申戌'),  # 震木庚子外庚午 子寅辰午申戌
     ('辛丑亥酉', '辛未巳卯'),  # 巽木辛丑外辛未 丑亥酉未巳卯
     ('戊寅辰午', '戊申戌子'),  # 坎水戊寅外戊申 寅辰午申戌子
     ('丙辰午申', '丙戌子寅'),  # 艮土丙辰外丙戌 辰午申戌子寅
     ('乙未巳卯', '癸丑亥酉'),  # 坤土乙未外癸丑 未巳卯丑亥酉
 )
 
-GUA64 = {'111111': '乾为天', '011111': '天风姤', '001111': '天山遁', '000111': '天地否', '000011': '风地观', '000001': '山地剥',
-         '000101': '火地晋', '111101': '火天大有', '110110': '兑为泽', '010110': '泽水困', '000110': '泽地萃', '001110': '泽山咸',
-         '001010': '水山蹇', '001000': '地山谦', '001100': '雷山小过', '110100': '雷泽归妹', '101101': '离为火', '001101': '火山旅',
-         '011101': '火风鼎', '010101': '火水未济', '010001': '山水蒙', '010011': '风水涣', '010111': '天水讼', '101111': '天火同人',
-         '100100': '震为雷', '000100': '雷地豫', '010100': '雷水解', '011100': '雷风恒', '011000': '地风升', '011010': '水风井',
-         '011110': '泽风大过', '100110': '泽雷随', '011011': '巽为风', '111011': '风天小畜', '101011': '风火家人', '100011': '风雷益',
-         '100111': '天雷无妄', '100101': '火雷噬嗑', '100001': '山雷颐', '011001': '山风蛊', '010010': '坎为水', '110010': '水泽节',
-         '100010': '水雷屯', '101010': '水火既济', '101110': '泽火革', '101100': '雷火丰', '101000': '地火明夷', '010000': '地水师',
-         '001001': '艮为山', '101001': '山火贲', '111001': '山天大畜', '110001': '山泽损', '110101': '火泽睽', '110111': '天泽履',
-         '110011': '风泽中孚', '001011': '风山渐', '000000': '坤为地', '100000': '地雷复', '110000': '地泽临', '111000': '地天泰',
-         '111100': '雷天大壮', '111110': '泽天夬', '111010': '水天需', '000010': '水地比'}
+GUA64 = {
+    '111111': '乾为天', '011111': '天风姤', '001111': '天山遁', '000111': '天地否', '000011': '风地观', '000001': '山地剥',
+    '000101': '火地晋', '111101': '火天大有', '110110': '兑为泽', '010110': '泽水困', '000110': '泽地萃', '001110': '泽山咸',
+    '001010': '水山蹇', '001000': '地山谦', '001100': '雷山小过', '110100': '雷泽归妹', '101101': '离为火', '001101': '火山旅',
+    '011101': '火风鼎', '010101': '火水未济', '010001': '山水蒙', '010011': '风水涣', '010111': '天水讼', '101111': '天火同人',
+    '100100': '震为雷', '000100': '雷地豫', '010100': '雷水解', '011100': '雷风恒', '011000': '地风升', '011010': '水风井',
+    '011110': '泽风大过', '100110': '泽雷随', '011011': '巽为风', '111011': '风天小畜', '101011': '风火家人', '100011': '风雷益',
+    '100111': '天雷无妄', '100101': '火雷噬嗑', '100001': '山雷颐', '011001': '山风蛊', '010010': '坎为水', '110010': '水泽节',
+    '100010': '水雷屯', '101010': '水火既济', '101110': '泽火革', '101100': '雷火丰', '101000': '地火明夷', '010000': '地水师',
+    '001001': '艮为山', '101001': '山火贲', '111001': '山天大畜', '110001': '山泽损', '110101': '火泽睽', '110111': '天泽履',
+    '110011': '风泽中孚', '001011': '风山渐', '000000': '坤为地', '100000': '地雷复', '110000': '地泽临', '111000': '地天泰',
+    '111100': '雷天大壮', '111110': '泽天夬', '111010': '水天需', '000010': '水地比'
+}
 
 # 中文数字
 NUMCN = ("零", "一", "二", "三", "四", "五", "六", "七", "八", "九", "十")
 
 # 24节气
 JIEQI = ("冬至", "小寒", "大寒", "立春", "雨水", "驚蟄", "春分", "清明", "穀雨", "立夏", "小滿",
          "芒種", "夏至", "小暑", "大暑", "立秋", "處暑", "白露", "秋分", "寒露", "霜降", "立冬",
```

