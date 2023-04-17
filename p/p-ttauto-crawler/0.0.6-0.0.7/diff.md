# Comparing `tmp/p-ttauto-crawler-0.0.6.tar.gz` & `tmp/p-ttauto-crawler-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p-ttauto-crawler-0.0.6.tar", last modified: Fri Apr 14 06:00:47 2023, max compression
+gzip compressed data, was "p-ttauto-crawler-0.0.7.tar", last modified: Mon Apr 17 01:30:41 2023, max compression
```

## Comparing `p-ttauto-crawler-0.0.6.tar` & `p-ttauto-crawler-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 06:00:47.953769 p-ttauto-crawler-0.0.6/
--rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      397 2023-04-14 06:00:47.952770 p-ttauto-crawler-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 06:00:47.934771 p-ttauto-crawler-0.0.6/p_ttauto_crawler.egg-info/
--rw-rw-rw-   0        0        0      397 2023-04-14 06:00:47.000000 p-ttauto-crawler-0.0.6/p_ttauto_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-04-14 06:00:47.000000 p-ttauto-crawler-0.0.6/p_ttauto_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 06:00:47.000000 p-ttauto-crawler-0.0.6/p_ttauto_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-14 06:00:47.000000 p-ttauto-crawler-0.0.6/p_ttauto_crawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       63 2023-04-14 06:00:47.000000 p-ttauto-crawler-0.0.6/p_ttauto_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-14 06:00:47.000000 p-ttauto-crawler-0.0.6/p_ttauto_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 06:00:47.953769 p-ttauto-crawler-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      938 2023-04-14 05:46:59.000000 p-ttauto-crawler-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 06:00:47.949771 p-ttauto-crawler-0.0.6/ttauto_crawler/
--rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.6/ttauto_crawler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 06:00:47.951770 p-ttauto-crawler-0.0.6/ttauto_crawler/bin/
--rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.6/ttauto_crawler/bin/__init__.py
--rw-rw-rw-   0        0        0    16089 2023-04-14 05:46:50.000000 p-ttauto-crawler-0.0.6/ttauto_crawler/main.py
--rw-rw-rw-   0        0        0    10719 2023-04-14 06:00:31.000000 p-ttauto-crawler-0.0.6/ttauto_crawler/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:30:41.103883 p-ttauto-crawler-0.0.7/
+-rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      397 2023-04-17 01:30:41.103883 p-ttauto-crawler-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 01:30:41.098883 p-ttauto-crawler-0.0.7/p_ttauto_crawler.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-04-17 01:30:40.000000 p-ttauto-crawler-0.0.7/p_ttauto_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-04-17 01:30:41.000000 p-ttauto-crawler-0.0.7/p_ttauto_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 01:30:40.000000 p-ttauto-crawler-0.0.7/p_ttauto_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-17 01:30:40.000000 p-ttauto-crawler-0.0.7/p_ttauto_crawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       63 2023-04-17 01:30:40.000000 p-ttauto-crawler-0.0.7/p_ttauto_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-17 01:30:40.000000 p-ttauto-crawler-0.0.7/p_ttauto_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 01:30:41.103883 p-ttauto-crawler-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      938 2023-04-17 01:30:36.000000 p-ttauto-crawler-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:30:41.100884 p-ttauto-crawler-0.0.7/ttauto_crawler/
+-rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.7/ttauto_crawler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:30:41.102883 p-ttauto-crawler-0.0.7/ttauto_crawler/bin/
+-rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.7/ttauto_crawler/bin/__init__.py
+-rw-rw-rw-   0        0        0    16746 2023-04-17 01:30:28.000000 p-ttauto-crawler-0.0.7/ttauto_crawler/main.py
+-rw-rw-rw-   0        0        0    10719 2023-04-14 06:00:31.000000 p-ttauto-crawler-0.0.7/ttauto_crawler/utils.py
```

### Comparing `p-ttauto-crawler-0.0.6/LICENSE` & `p-ttauto-crawler-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.0.6/setup.py` & `p-ttauto-crawler-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="p-ttauto-crawler",
-    version="0.0.6",
+    version="0.0.7",
     author="pengjun",
     author_email="mr_lonely@foxmail.com",
     description="template tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `p-ttauto-crawler-0.0.6/ttauto_crawler/main.py` & `p-ttauto-crawler-0.0.7/ttauto_crawler/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -269,14 +269,48 @@
             successCount+=1
     zip.close()
     ossurl = utils.ftpUpload(dist)[0]
     ### notify
     print(f"=== notifying ")
     notifyMessage(ossurl, successCount)
 
+def lastTaskFile():
+    thisFileDir = os.path.dirname(os.path.abspath(__file__))
+    return os.path.join(thisFileDir, "last_task.txt")
+
+def removeLastTask():
+    file = lastTaskFile()
+    if os.path.exists(file):
+        os.remove(file)
+
+def getLocalTask():
+    file = lastTaskFile()
+    data = {}
+    if os.path.exists(file):
+        with open(file, 'r', encoding='UTF-8') as f:
+            data = json.load(f)
+    return data
+
+def saveLastTask(data):
+    file = lastTaskFile()
+    with open(file, 'w') as f:
+        json.dump(data, f)
+
+def getTask():
+    data = getLocalTask()
+    if len(data) == 0:
+        s = requests.session()
+        s.headers.update({'Connection':'close'})
+        res = s.get(f"https://beta.2tianxin.com/common/admin/tta/get_task?t={random.randint(100,99999999)}", verify=False)
+        s.close()
+        if len(res.content) > 0:
+            data = json.loads(res.content)
+            saveLastTask(data)
+    return data
+
 def main():    
     global rootDir
     global curGroupId
     global allCount
     global successCount
     
     urllib3.disable_warnings()
@@ -287,40 +321,37 @@
                         datefmt='%a, %d %b %Y %H:%M:%S',
                         encoding="utf-8",
                         level=logging.DEBUG)
 
     rootDir = thisFileDir
     while(os.path.exists(os.path.join(thisFileDir, "stop.now")) == False):
         try:
-            s = requests.session()
-            s.headers.update({'Connection':'close'})
-            res = s.get(f"https://beta.2tianxin.com/common/admin/tta/get_task?t={random.randint(100,99999999)}", verify=False)
-            s.close()
-            if len(res.content) > 0:
-                clearDir()
-                data = json.loads(res.content)
-                if len(data) == 0:
-                    continue
-                curGroupId = data["id"]
-                allCount = 0
-                successCount = 0
-                start_pts = calendar.timegm(time.gmtime())
-                logging.info(f"================ begin {curGroupId} ===================")
-                logging.info(f"========== GetTask: {res.content}")
-                print(f"=== begin {curGroupId}")
-                url = data["url"].replace("\n", "").replace(";", "").replace(",", "").strip()
-                crawler_template_name = data["crawler_template_name"].replace("\n", "").replace(";", "").replace(",", "").strip()
-                if len(crawler_template_name) <= 0:
-                    crawler_template_name = "template2"
-
-                process(url, crawler_template_name)
-
-                current_pts = calendar.timegm(time.gmtime())
-                print(f"complate => {curGroupId} rst={successCount}/{allCount} duration={(current_pts - start_pts)}")
-                logging.info(f"================ end {curGroupId} rst={successCount}/{allCount} duration={(current_pts - start_pts)}===================")
+            data = getTask()
+            if len(data) == 0:
+                continue
+            curGroupId = data["id"]
+            allCount = 0
+            successCount = 0
+            start_pts = calendar.timegm(time.gmtime())
+            logging.info(f"================ begin {curGroupId} ===================")
+            logging.info(f"========== GetTask: {data}")
+            print(f"=== begin {curGroupId}")
+            url = data["url"].replace("\n", "").replace(";", "").replace(",", "").strip()
+            crawler_template_name = data["crawler_template_name"].replace("\n", "").replace(";", "").replace(",", "").strip()
+            if len(crawler_template_name) <= 0:
+                crawler_template_name = "template2"
+
+            clearDir()
+            process(url, crawler_template_name)
+            removeLastTask()
+
+            current_pts = calendar.timegm(time.gmtime())
+            print(f"complate => {curGroupId} rst={successCount}/{allCount} duration={(current_pts - start_pts)}")
+            logging.info(f"================ end {curGroupId} rst={successCount}/{allCount} duration={(current_pts - start_pts)}===================")
+            exit(-1)
         except Exception as e:
             notifyMessage(False, str(e))
             logging.error("====================== uncatch Exception ======================")
             logging.error(e)
             logging.error("======================      end      ======================")
         time.sleep(2)
     os.remove(os.path.join(thisFileDir, "stop.now"))
```

### Comparing `p-ttauto-crawler-0.0.6/ttauto_crawler/utils.py` & `p-ttauto-crawler-0.0.7/ttauto_crawler/utils.py`

 * *Files identical despite different names*

