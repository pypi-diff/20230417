# Comparing `tmp/NewsArticlesScraper-0.1.7.tar.gz` & `tmp/NewsArticlesScraper-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NewsArticlesScraper-0.1.7.tar", last modified: Fri Apr 14 11:28:25 2023, max compression
+gzip compressed data, was "NewsArticlesScraper-0.2.tar", last modified: Mon Apr 17 15:31:56 2023, max compression
```

## Comparing `NewsArticlesScraper-0.1.7.tar` & `NewsArticlesScraper-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 11:28:25.935897 NewsArticlesScraper-0.1.7/
-drwxrwxrwx   0        0        0        0 2023-04-14 11:28:25.922397 NewsArticlesScraper-0.1.7/NewsArticlesScraper/
--rw-rw-rw-   0        0        0     9290 2023-04-14 11:26:33.000000 NewsArticlesScraper-0.1.7/NewsArticlesScraper/Scrapers.py
--rw-rw-rw-   0        0        0       64 2023-02-14 20:15:57.000000 NewsArticlesScraper-0.1.7/NewsArticlesScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 11:28:25.934397 NewsArticlesScraper-0.1.7/NewsArticlesScraper.egg-info/
--rw-rw-rw-   0        0        0      648 2023-04-14 11:28:25.000000 NewsArticlesScraper-0.1.7/NewsArticlesScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-04-14 11:28:25.000000 NewsArticlesScraper-0.1.7/NewsArticlesScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 11:28:25.000000 NewsArticlesScraper-0.1.7/NewsArticlesScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-14 11:28:25.000000 NewsArticlesScraper-0.1.7/NewsArticlesScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-14 11:28:25.000000 NewsArticlesScraper-0.1.7/NewsArticlesScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      648 2023-04-14 11:28:25.935397 NewsArticlesScraper-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-14 20:04:13.000000 NewsArticlesScraper-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 11:28:25.936397 NewsArticlesScraper-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      996 2023-04-14 11:26:33.000000 NewsArticlesScraper-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:31:56.670459 NewsArticlesScraper-0.2/
+drwxrwxrwx   0        0        0        0 2023-04-17 15:31:56.660459 NewsArticlesScraper-0.2/NewsArticlesScraper/
+-rw-rw-rw-   0        0        0    12860 2023-04-17 15:28:59.000000 NewsArticlesScraper-0.2/NewsArticlesScraper/Scrapers.py
+-rw-rw-rw-   0        0        0       64 2023-02-14 20:15:57.000000 NewsArticlesScraper-0.2/NewsArticlesScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:31:56.668960 NewsArticlesScraper-0.2/NewsArticlesScraper.egg-info/
+-rw-rw-rw-   0        0        0      646 2023-04-17 15:31:56.000000 NewsArticlesScraper-0.2/NewsArticlesScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-04-17 15:31:56.000000 NewsArticlesScraper-0.2/NewsArticlesScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 15:31:56.000000 NewsArticlesScraper-0.2/NewsArticlesScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-17 15:31:56.000000 NewsArticlesScraper-0.2/NewsArticlesScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-17 15:31:56.000000 NewsArticlesScraper-0.2/NewsArticlesScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      646 2023-04-17 15:31:56.669963 NewsArticlesScraper-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-02-14 20:04:13.000000 NewsArticlesScraper-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 15:31:56.670959 NewsArticlesScraper-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      994 2023-04-17 15:28:59.000000 NewsArticlesScraper-0.2/setup.py
```

### Comparing `NewsArticlesScraper-0.1.7/NewsArticlesScraper/Scrapers.py` & `NewsArticlesScraper-0.2/NewsArticlesScraper/Scrapers.py`

 * *Files 18% similar despite different names*

```diff
@@ -209,7 +209,95 @@
             "title": response.css("div h1 ::text").get(),
             "author_name": author_name,
             "body": content,
             "time": response.meta["time"],
             "url": response.url,
             "origin": "n",
         }
+
+
+class TheGuardianSpider(scrapy.Spider):
+    """Spider to scrape The Guardian articles.
+
+    """
+    name = 'TheGuardian'
+    allowed_domains = ['theguardian.com', 'content.guardianapis.com']
+    custom_settings = {
+        'LOG_LEVEL': 'WARN',
+        'USER_AGENT': 'Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.1 (KHTML, like Gecko) Chrome/22.0.1207.1 '
+                      'Safari/537.1',
+        'ROBOTSTXT_OBEY': False,
+        'DOWNLOAD_DELAY': 1,
+        # 'JOBDIR': './News/TheGuardianJobs',
+        'REQUEST_FINGERPRINTER_IMPLEMENTATION': '2.7',
+        'DOWNLOAD_TIMEOUT': 300,
+        'DOWNLOADER_MIDDLEWARES': {
+            'scrapy.downloadermiddlewares.useragent.UserAgentMiddleware': None,
+            'scrapy_user_agents.middlewares.RandomUserAgentMiddleware': 400,
+        },
+        'RANDOM_UA_TYPE': "random",
+    }
+
+    def __init__(self, from_time: datetime.datetime, until_time: datetime.datetime, api_key="test", user_agent=None,
+                 **kwargs):
+        self.api_key = api_key
+        self.from_time = from_time
+        self.until_time = until_time
+        self.url = f"https://content.guardianapis.com/world?api-key={self.api_key}" \
+                   f"&page-size=200&use-date=first-publication" \
+                   f"&from-date={self.from_time.strftime('%Y-%m-%d')}" \
+                   f"&to-date={self.until_time.strftime('%Y-%m-%d')}&page="
+        if user_agent is not None:
+            self.custom_settings["USER_AGENT"] = user_agent
+        super().__init__(**kwargs)
+
+    def start_requests(self):
+        yield scrapy.Request(self.url + "1",
+                             callback=self.paginate)
+
+    def paginate(self, response):
+        data = response.json()["response"]
+        max_pages = data["pages"]
+        for page_number in range(1, max_pages + 1):
+            to_request_url = self.url + str(page_number) + "&x=1"
+            yield scrapy.Request(to_request_url, callback=self.parse_api)
+
+    def parse_api(self, response):
+        data = response.json()["response"]
+        articles = data["results"]
+        for article in articles:
+            yield scrapy.Request(url=article["webUrl"], callback=self.parse_article,
+                                 meta={"time": article["webPublicationDate"]})
+
+    @staticmethod
+    def parse_article(response):
+        title = response.css(".dcr-y70mar ::text").get()
+        if title is None:
+            title = response.css(".dcr-1kwg2vo ::text").get()
+        if title is None:
+            title = response.css(".dcr-18ogzt ::text").get()
+        if title is None:
+            title = response.css(".dcr-1ttbui0 ::text").get()
+        if title is None:
+            title = response.css(".dcr-1b0zxa5 ::text").get()
+        if title is None:
+            title = response.css(".dcr-1xaevyx ::text").get()
+        if title is None:
+            title = ""
+
+        author_name = response.css(".dcr-ub3a78 ::text").get()
+        if author_name is None:
+            author_name = response.css(".dcr-8gsycy a ::text").get()
+        if author_name is None:
+            author_name = ""
+
+        body = " ".join(response.css(".dcr-n6w1lc ::text").getall())
+        if body == "":
+            body = " ".join(response.css("#maincontent p ::text").getall())
+        yield {
+            "title": title,
+            "author_name": author_name,
+            "body": body,
+            "time": response.meta["time"],
+            "url": response.url,
+            "origin": "g"
+        }
```

### Comparing `NewsArticlesScraper-0.1.7/NewsArticlesScraper.egg-info/PKG-INFO` & `NewsArticlesScraper-0.2/NewsArticlesScraper.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.1.7
+Version: 0.2
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.1.7/PKG-INFO` & `NewsArticlesScraper-0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.1.7
+Version: 0.2
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.1.7/setup.py` & `NewsArticlesScraper-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.7'
+VERSION = '0.2'
 DESCRIPTION = 'Scraping news articles'
 LONG_DESCRIPTION = 'A package that allows you to scrape news articles from various news sites via scrapy.'
 
 # Setting up
 setup(
     name="NewsArticlesScraper",
     version=VERSION,
```

