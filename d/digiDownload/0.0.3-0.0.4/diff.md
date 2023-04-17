# Comparing `tmp/digiDownload-0.0.3.tar.gz` & `tmp/digiDownload-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digiDownload-0.0.3.tar", last modified: Sat Apr 15 18:47:50 2023, max compression
+gzip compressed data, was "digiDownload-0.0.4.tar", last modified: Mon Apr 17 13:56:28 2023, max compression
```

## Comparing `digiDownload-0.0.3.tar` & `digiDownload-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-15 18:47:50.516475 digiDownload-0.0.3/
--rw-r--r--   0 notyou    (1000) notyou    (1000)      305 2023-04-15 18:47:50.516475 digiDownload-0.0.3/PKG-INFO
-drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-15 18:47:50.516475 digiDownload-0.0.3/digiDownload/
--rw-r--r--   0 notyou    (1000) notyou    (1000)      176 2023-04-15 14:38:11.000000 digiDownload-0.0.3/digiDownload/AdBlockCookiePolicy.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)     2116 2023-04-15 18:46:06.000000 digiDownload-0.0.3/digiDownload/Book.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)      628 2023-04-15 16:01:32.000000 digiDownload-0.0.3/digiDownload/LTIParser.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)     1293 2023-04-15 18:46:06.000000 digiDownload-0.0.3/digiDownload/Session.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)       29 2023-04-15 17:22:08.000000 digiDownload-0.0.3/digiDownload/__init__.py
-drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-15 18:47:50.516475 digiDownload-0.0.3/digiDownload.egg-info/
--rw-r--r--   0 notyou    (1000) notyou    (1000)      305 2023-04-15 18:47:50.000000 digiDownload-0.0.3/digiDownload.egg-info/PKG-INFO
--rw-r--r--   0 notyou    (1000) notyou    (1000)      329 2023-04-15 18:47:50.000000 digiDownload-0.0.3/digiDownload.egg-info/SOURCES.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)        1 2023-04-15 18:47:50.000000 digiDownload-0.0.3/digiDownload.egg-info/dependency_links.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)       24 2023-04-15 18:47:50.000000 digiDownload-0.0.3/digiDownload.egg-info/requires.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)       13 2023-04-15 18:47:50.000000 digiDownload-0.0.3/digiDownload.egg-info/top_level.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)       79 2023-04-15 18:47:50.516475 digiDownload-0.0.3/setup.cfg
--rw-r--r--   0 notyou    (1000) notyou    (1000)      464 2023-04-15 18:46:06.000000 digiDownload-0.0.3/setup.py
+drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-17 13:56:28.554043 digiDownload-0.0.4/
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      305 2023-04-17 13:56:28.554043 digiDownload-0.0.4/PKG-INFO
+drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-17 13:56:28.554043 digiDownload-0.0.4/digiDownload/
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      176 2023-04-15 14:38:11.000000 digiDownload-0.0.4/digiDownload/AdBlockCookiePolicy.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     2564 2023-04-17 13:53:54.000000 digiDownload-0.0.4/digiDownload/Book.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      628 2023-04-15 16:01:32.000000 digiDownload-0.0.4/digiDownload/LTIParser.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     1293 2023-04-15 18:46:06.000000 digiDownload-0.0.4/digiDownload/Session.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       29 2023-04-15 17:22:08.000000 digiDownload-0.0.4/digiDownload/__init__.py
+drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-17 13:56:28.554043 digiDownload-0.0.4/digiDownload.egg-info/
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      305 2023-04-17 13:56:28.000000 digiDownload-0.0.4/digiDownload.egg-info/PKG-INFO
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      329 2023-04-17 13:56:28.000000 digiDownload-0.0.4/digiDownload.egg-info/SOURCES.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)        1 2023-04-17 13:56:28.000000 digiDownload-0.0.4/digiDownload.egg-info/dependency_links.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       24 2023-04-17 13:56:28.000000 digiDownload-0.0.4/digiDownload.egg-info/requires.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       13 2023-04-17 13:56:28.000000 digiDownload-0.0.4/digiDownload.egg-info/top_level.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       79 2023-04-17 13:56:28.554043 digiDownload-0.0.4/setup.cfg
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      464 2023-04-17 13:56:26.000000 digiDownload-0.0.4/setup.py
```

### Comparing `digiDownload-0.0.3/digiDownload/Book.py` & `digiDownload-0.0.4/digiDownload/Book.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from .LTIParser import LTIForm
 
+from bs4 import BeautifulSoup
 from threading import Thread
 from time import sleep
 from sys import maxsize
 
 
 class Book:
     urls = {
-        "https://a.digi4school.at": "https://a.digi4school.at/ebook/{book_id}/{page}.svg",
-        "https://a.hpthek.at": "https://a.hpthek.at/ebook/{book_id}/{page}/{page}.svg"
+        "https://a.digi4school.at": "https://a.digi4school.at/ebook/{book_id}/{extra}{page}.svg",
+        "https://a.hpthek.at": "https://a.hpthek.at/ebook/{book_id}/{page}/{extra}{page}.svg"
     }
 
     def __init__(self, client, html_content):
         self.client = client
 
         self.publisher = html_content.find("span", {"class": "publisher"}).text
         self.title = html_content.find("h1").text
@@ -20,19 +21,28 @@
         self.code = html_content["data-code"]
         self.id = html_content["data-id"]
 
         resp = LTIForm(self.client.get(f"https://digi4school.at/ebook/{self.code}").content)
         first_form = LTIForm(resp.send(self.client).content)
         second_form = first_form.send(self.client)
 
-        self.url = '/'.join(second_form.url.split("/")[0:3])
+        url = '/'.join(second_form.url.split("/")[0:3])
+        assert url in Book.urls.keys(), f"Undocumented url: {url}"
+
+        self.url = Book.urls[url]
         self.content_id = first_form["resource_link_id"]
 
+        self.extra = ""
+        main_page = self.client.get(f"https://a.digi4school.at/ebook/{self.id}/").text
+        if main_page.split('\n')[0] == "<html>":
+            soup = BeautifulSoup(main_page, "html.parser")
+            self.extra = '/'.join(soup.find("a")["href"].split("/")[:-1]) + '/'
+
     def _get_page(self, page):
-        url = self.urls[self.url].format(book_id=self.content_id, page=page)
+        url = self.url.format(book_id=self.content_id, extra=self.extra, page=page)
         resp = self.client.get(url, stream=True)
 
         return resp
 
     def _get_pages(self):
         for i in range(1, maxsize):
             resp = self._get_page(i)
```

### Comparing `digiDownload-0.0.3/digiDownload/LTIParser.py` & `digiDownload-0.0.4/digiDownload/LTIParser.py`

 * *Files identical despite different names*

### Comparing `digiDownload-0.0.3/digiDownload/Session.py` & `digiDownload-0.0.4/digiDownload/Session.py`

 * *Files identical despite different names*

