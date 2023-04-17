# Comparing `tmp/cnki_html2json-0.0.9.tar.gz` & `tmp/cnki_html2json-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnki_html2json-0.0.9.tar", last modified: Mon Apr 17 04:20:21 2023, max compression
+gzip compressed data, was "cnki_html2json-0.1.0.tar", last modified: Mon Apr 17 07:11:25 2023, max compression
```

## Comparing `cnki_html2json-0.0.9.tar` & `cnki_html2json-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:20:21.541720 cnki_html2json-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-04-17 04:20:21.541720 cnki_html2json-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:20:21.537720 cnki_html2json-0.0.9/cnki_html2json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/cnki_html2json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/cnki_html2json/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/cnki_html2json/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/cnki_html2json/html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/cnki_html2json/parse_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/cnki_html2json/recognize_slider_coordinate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:20:21.541720 cnki_html2json-0.0.9/cnki_html2json.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-04-17 04:20:21.000000 cnki_html2json-0.0.9/cnki_html2json.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-17 04:20:21.000000 cnki_html2json-0.0.9/cnki_html2json.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 04:20:21.000000 cnki_html2json-0.0.9/cnki_html2json.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 04:20:21.000000 cnki_html2json-0.0.9/cnki_html2json.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 04:20:21.000000 cnki_html2json-0.0.9/cnki_html2json.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 04:20:21.000000 cnki_html2json-0.0.9/cnki_html2json.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 04:20:21.541720 cnki_html2json-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:20:21.541720 cnki_html2json-0.0.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/test/test_html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/test/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:11:25.730840 cnki_html2json-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-04-17 07:11:25.730840 cnki_html2json-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-17 07:11:05.000000 cnki_html2json-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:11:25.730840 cnki_html2json-0.1.0/cnki_html2json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 07:11:05.000000 cnki_html2json-0.1.0/cnki_html2json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-17 07:11:05.000000 cnki_html2json-0.1.0/cnki_html2json/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-17 07:11:05.000000 cnki_html2json-0.1.0/cnki_html2json/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-04-17 07:11:05.000000 cnki_html2json-0.1.0/cnki_html2json/html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-17 07:11:05.000000 cnki_html2json-0.1.0/cnki_html2json/parse_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-17 07:11:05.000000 cnki_html2json-0.1.0/cnki_html2json/recognize_slider_coordinate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:11:25.730840 cnki_html2json-0.1.0/cnki_html2json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-04-17 07:11:25.000000 cnki_html2json-0.1.0/cnki_html2json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-17 07:11:25.000000 cnki_html2json-0.1.0/cnki_html2json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 07:11:25.000000 cnki_html2json-0.1.0/cnki_html2json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 07:11:25.000000 cnki_html2json-0.1.0/cnki_html2json.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 07:11:25.000000 cnki_html2json-0.1.0/cnki_html2json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 07:11:25.000000 cnki_html2json-0.1.0/cnki_html2json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 07:11:25.730840 cnki_html2json-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-17 07:11:05.000000 cnki_html2json-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:11:25.730840 cnki_html2json-0.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 07:11:05.000000 cnki_html2json-0.1.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-17 07:11:05.000000 cnki_html2json-0.1.0/test/test_html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-17 07:11:05.000000 cnki_html2json-0.1.0/test/test_metadata.py
```

### Comparing `cnki_html2json-0.0.9/PKG-INFO` & `cnki_html2json-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki_html2json
-Version: 0.0.9
+Version: 0.1.0
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cnki_html2json-0.0.9/README.md` & `cnki_html2json-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.0.9/cnki_html2json/cli.py` & `cnki_html2json-0.1.0/cnki_html2json/cli.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.0.9/cnki_html2json/crawl.py` & `cnki_html2json-0.1.0/cnki_html2json/crawl.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from loguru import logger
 from datetime import datetime
 
 from cnki_html2json import html2json
 from cnki_html2json import parse_metadata
 from cnki_html2json import recognize_slider_coordinate
 
-
 def obtain_page_papers_url(driver) -> list:
     url_list = [i.get_attribute('href') for i in driver.find_elements(By.XPATH,'//*[@id="gridTable"]/table/tbody/tr/td[2]/a')]
     return url_list
 
 def process_slider(driver):
     """判断是否进入验证码页面并进行验证"""
     recogize_count = 0
@@ -194,17 +193,17 @@
     if current_page < start_page:
         jump_page(current_page,start_page,driver)
         current_page = start_page
     logger.info(f'将从第 {start_paper_index} 篇文献开始下载')
     logger.info(f'模式设置为 {mode}')
     minutes = math.ceil(need_download_num/3)
     if minutes < 60:
-        logger.info(f'预计耗时 {minutes}分钟')
+        logger.info(f'预计耗时 {minutes} 分钟')
     else:
-        logger.info(f'预计耗时 {minutes//60}小时 {minutes%60} 分钟')
+        logger.info(f'预计耗时 {minutes//60} 小时 {minutes%60} 分钟')
     
     # 下载文献数据
     current_paper_index = start_paper_index
 
     while current_paper_index < avaiable_records_num+1:
         current_url_list = obtain_page_papers_url(driver)[current_paper_index%papers_per_page-1:]  
         for url in current_url_list:
```

### Comparing `cnki_html2json-0.0.9/cnki_html2json/html2json.py` & `cnki_html2json-0.1.0/cnki_html2json/html2json.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,22 +74,31 @@
 		self.content = resp_content
 		# self.content = resp_content.replace('<!DOCTYPE html>','').strip()
 		self.html_general = html.fromstring(self.content)
 		
 		if mode != "raw":
 			self.html_text = html.fromstring(re.sub('<citation.*?</citation>|<sup>.*?</sup>|<i>.*?</i>','',self.content,flags=re.S))
 		
-		elif mode=="raw":
-			
+		elif mode == "raw":
 			# 匹配并替换
 			pattern = r'<citation.*?>.*?</citation>'
 			content_ = self.content
-			for match in re.findall(pattern,self.content):
-				match_result = '{}'.format([int(i) for i in re.findall(r'<a class="sup">(\d+)</a>',match)])
-				content_ = content_.replace(match,match_result)
+
+			# 网页请求的源码
+			if content_.split('\n',1)[0] == '<!DOCTYPE html>': 
+				for match in re.findall(pattern, self.content,flags=re.S):
+					match_result = '{}'.format([int(i) for i in re.findall(r'<a class="sup">(\d+)</a>',match)])
+					content_ = content_.replace(match, match_result)
+			
+			# 使用driver.page_source获取的源码
+			else: 
+				for match in re.findall(pattern, self.content,flags=re.S):
+					match_result = '{}'.format([int(i) for i in re.findall(r'href="javascript:void\(0\);">(\d+)</a>',match,flags=re.S)])
+					content_ = content_.replace(match, match_result)
+				
 			self.html_text = html.fromstring(re.sub(r'<sup>.*?</sup>|<i>.*?</i>','',content_,flags=re.S))
 
 		self.error = False
 		self.annotation = False
 		self.no_structure = False
 		self.prefix = False
 		self.mode = mode
```

### Comparing `cnki_html2json-0.0.9/cnki_html2json/parse_metadata.py` & `cnki_html2json-0.1.0/cnki_html2json/parse_metadata.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.0.9/cnki_html2json/recognize_slider_coordinate.py` & `cnki_html2json-0.1.0/cnki_html2json/recognize_slider_coordinate.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.0.9/cnki_html2json.egg-info/PKG-INFO` & `cnki_html2json-0.1.0/cnki_html2json.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki-html2json
-Version: 0.0.9
+Version: 0.1.0
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cnki_html2json-0.0.9/setup.py` & `cnki_html2json-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup,find_packages
 
 setup(
     name="cnki_html2json",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.0.9",
+    version="0.1.0",
     description="A package to convert cnki html to json",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["cnki","text-structure","crawler"],
     license="MIT",
     url="https://github.com/doublessay/cnki-html2json",
     packages=find_packages(),
```

### Comparing `cnki_html2json-0.0.9/test/test_html2json.py` & `cnki_html2json-0.1.0/test/test_html2json.py`

 * *Files identical despite different names*

