# Comparing `tmp/twitter-api-client-0.6.4.tar.gz` & `tmp/twitter-api-client-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.6.4.tar", last modified: Sat Apr 15 20:46:50 2023, max compression
+gzip compressed data, was "twitter-api-client-0.6.5.tar", last modified: Mon Apr 17 00:41:41 2023, max compression
```

## Comparing `twitter-api-client-0.6.4.tar` & `twitter-api-client-0.6.5.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 20:46:50.850656 twitter-api-client-0.6.4/
--rw-rw-r--   0 x         (1000) x         (1000)     1075 2023-04-14 02:53:18.000000 twitter-api-client-0.6.4/LICENSE
--rw-rw-r--   0 x         (1000) x         (1000)     6274 2023-04-15 20:46:50.850656 twitter-api-client-0.6.4/PKG-INFO
--rw-rw-r--   0 x         (1000) x         (1000)       38 2023-04-15 20:46:50.850656 twitter-api-client-0.6.4/setup.cfg
--rw-rw-r--   0 x         (1000) x         (1000)     7259 2023-04-15 20:45:23.000000 twitter-api-client-0.6.4/setup.py
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 20:46:50.846656 twitter-api-client-0.6.4/twitter/
--rw-rw-r--   0 x         (1000) x         (1000)        0 2023-04-14 02:53:18.000000 twitter-api-client-0.6.4/twitter/__init__.py
--rw-rw-r--   0 x         (1000) x         (1000)    26564 2023-04-15 20:45:23.000000 twitter-api-client-0.6.4/twitter/account.py
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 20:46:50.850656 twitter-api-client-0.6.4/twitter/config/
--rw-rw-r--   0 x         (1000) x         (1000)        0 2023-04-14 02:53:18.000000 twitter-api-client-0.6.4/twitter/config/__init__.py
--rw-rw-r--   0 x         (1000) x         (1000)      909 2023-04-14 02:53:18.000000 twitter-api-client-0.6.4/twitter/config/log.py
--rw-rw-r--   0 x         (1000) x         (1000)   147862 2023-04-14 21:16:39.000000 twitter-api-client-0.6.4/twitter/config/operations.py
--rw-rw-r--   0 x         (1000) x         (1000)     5859 2023-04-15 18:04:24.000000 twitter-api-client-0.6.4/twitter/config/settings.py
--rw-rw-r--   0 x         (1000) x         (1000)     2539 2023-04-14 21:53:11.000000 twitter-api-client-0.6.4/twitter/constants.py
--rw-rw-r--   0 x         (1000) x         (1000)     5242 2023-04-14 02:53:18.000000 twitter-api-client-0.6.4/twitter/login.py
--rw-rw-r--   0 x         (1000) x         (1000)    12761 2023-04-14 02:53:18.000000 twitter-api-client-0.6.4/twitter/scraper.py
--rw-rw-r--   0 x         (1000) x         (1000)     5478 2023-04-15 18:23:12.000000 twitter-api-client-0.6.4/twitter/search.py
--rw-rw-r--   0 x         (1000) x         (1000)     2235 2023-04-14 02:53:18.000000 twitter-api-client-0.6.4/twitter/utils.py
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 20:46:50.850656 twitter-api-client-0.6.4/twitter_api_client.egg-info/
--rw-rw-r--   0 x         (1000) x         (1000)     6274 2023-04-15 20:46:50.000000 twitter-api-client-0.6.4/twitter_api_client.egg-info/PKG-INFO
--rw-rw-r--   0 x         (1000) x         (1000)      461 2023-04-15 20:46:50.000000 twitter-api-client-0.6.4/twitter_api_client.egg-info/SOURCES.txt
--rw-rw-r--   0 x         (1000) x         (1000)        1 2023-04-15 20:46:50.000000 twitter-api-client-0.6.4/twitter_api_client.egg-info/dependency_links.txt
--rw-rw-r--   0 x         (1000) x         (1000)       82 2023-04-15 20:46:50.000000 twitter-api-client-0.6.4/twitter_api_client.egg-info/requires.txt
--rw-rw-r--   0 x         (1000) x         (1000)        8 2023-04-15 20:46:50.000000 twitter-api-client-0.6.4/twitter_api_client.egg-info/top_level.txt
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-17 00:41:41.387368 twitter-api-client-0.6.5/
+-rw-rw-r--   0 x         (1000) x         (1000)     1075 2023-04-14 02:53:18.000000 twitter-api-client-0.6.5/LICENSE
+-rw-rw-r--   0 x         (1000) x         (1000)     6812 2023-04-17 00:41:41.387368 twitter-api-client-0.6.5/PKG-INFO
+-rw-rw-r--   0 x         (1000) x         (1000)       38 2023-04-17 00:41:41.387368 twitter-api-client-0.6.5/setup.cfg
+-rw-rw-r--   0 x         (1000) x         (1000)     7860 2023-04-17 00:37:33.000000 twitter-api-client-0.6.5/setup.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-17 00:41:41.383368 twitter-api-client-0.6.5/twitter/
+-rw-rw-r--   0 x         (1000) x         (1000)        0 2023-04-14 02:53:18.000000 twitter-api-client-0.6.5/twitter/__init__.py
+-rw-rw-r--   0 x         (1000) x         (1000)    26566 2023-04-16 14:27:37.000000 twitter-api-client-0.6.5/twitter/account.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-17 00:41:41.387368 twitter-api-client-0.6.5/twitter/config/
+-rw-rw-r--   0 x         (1000) x         (1000)        0 2023-04-14 02:53:18.000000 twitter-api-client-0.6.5/twitter/config/__init__.py
+-rw-rw-r--   0 x         (1000) x         (1000)      909 2023-04-14 02:53:18.000000 twitter-api-client-0.6.5/twitter/config/log.py
+-rw-rw-r--   0 x         (1000) x         (1000)   147862 2023-04-14 21:16:39.000000 twitter-api-client-0.6.5/twitter/config/operations.py
+-rw-rw-r--   0 x         (1000) x         (1000)     5859 2023-04-15 18:04:24.000000 twitter-api-client-0.6.5/twitter/config/settings.py
+-rw-rw-r--   0 x         (1000) x         (1000)     2539 2023-04-14 21:53:11.000000 twitter-api-client-0.6.5/twitter/constants.py
+-rw-rw-r--   0 x         (1000) x         (1000)     5259 2023-04-17 00:28:42.000000 twitter-api-client-0.6.5/twitter/login.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-17 00:41:41.387368 twitter-api-client-0.6.5/twitter/noauth/
+-rw-rw-r--   0 x         (1000) x         (1000)        0 2023-04-16 21:57:30.000000 twitter-api-client-0.6.5/twitter/noauth/__init__.py
+-rw-rw-r--   0 x         (1000) x         (1000)     2646 2023-04-16 23:55:48.000000 twitter-api-client-0.6.5/twitter/noauth/operation.py
+-rw-rw-r--   0 x         (1000) x         (1000)     7400 2023-04-17 00:37:33.000000 twitter-api-client-0.6.5/twitter/noauth/scraper.py
+-rw-rw-r--   0 x         (1000) x         (1000)     2852 2023-04-17 00:11:45.000000 twitter-api-client-0.6.5/twitter/noauth/util.py
+-rw-rw-r--   0 x         (1000) x         (1000)    12836 2023-04-16 22:08:27.000000 twitter-api-client-0.6.5/twitter/scraper.py
+-rw-rw-r--   0 x         (1000) x         (1000)     4998 2023-04-17 00:28:42.000000 twitter-api-client-0.6.5/twitter/search.py
+-rw-rw-r--   0 x         (1000) x         (1000)     2256 2023-04-17 00:28:42.000000 twitter-api-client-0.6.5/twitter/utils.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-17 00:41:41.387368 twitter-api-client-0.6.5/twitter_api_client.egg-info/
+-rw-rw-r--   0 x         (1000) x         (1000)     6812 2023-04-17 00:41:41.000000 twitter-api-client-0.6.5/twitter_api_client.egg-info/PKG-INFO
+-rw-rw-r--   0 x         (1000) x         (1000)      565 2023-04-17 00:41:41.000000 twitter-api-client-0.6.5/twitter_api_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 x         (1000) x         (1000)        1 2023-04-17 00:41:41.000000 twitter-api-client-0.6.5/twitter_api_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 x         (1000) x         (1000)       82 2023-04-17 00:41:41.000000 twitter-api-client-0.6.5/twitter_api_client.egg-info/requires.txt
+-rw-rw-r--   0 x         (1000) x         (1000)        8 2023-04-17 00:41:41.000000 twitter-api-client-0.6.5/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.6.4/LICENSE` & `twitter-api-client-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.4/PKG-INFO` & `twitter-api-client-0.6.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.6.4
+Version: 0.6.5
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
@@ -164,15 +164,15 @@
  ```python
  from twitter.scraper import Scraper
 
  email, username, password = ..., ..., ...
  scraper = Scraper(email, username, password)  # session
 
  ####### User Data ########
- users = scraper.user_by_screen_name(['bob123', 'jim456', 'stanley789'])
+ users = scraper.user_by_screen_name(['foo', 'bar', 'baz'])
  tweets = scraper.tweets([123, 234, 345])
  likes = scraper.likes([123, 234, 345])
  tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
  media = scraper.media([123, 234, 345])
  following = scraper.following([123, 234, 345])
  followers = scraper.followers([123, 234, 345])
 
@@ -181,14 +181,33 @@
  tweets_details = scraper.tweets_details([456, 567, 678])
  retweeters = scraper.retweeters([456, 567, 678])
  favoriters = scraper.favoriters([456, 567, 678])
 
  scraper.download_media([456, 567, 678])
  ```
 
+ #### Get user/tweet data (no auth)
+
+ ```python
+ from twitter.noauth.scraper import Scraper
+
+ scraper = Scraper()
+
+ users = scraper.user(['foo', 'bar', 'baz'])
+ users = scraper.user_by_id([123, 234, 345])
+ users = scraper.users_by_ids([123, 234, 345])  # special batch query
+
+ tweets = scraper.tweet_by_id([987, 876, 765])  # condensed
+ tweets = scraper.tweet_details([987, 876, 765])
+
+ user_tweets = scraper.tweets([123, 234, 345])
+ user_tweets_replies = scraper.tweets_and_replies([123, 234, 345])
+ user_media = scraper.media([123, 234, 345])
+ ```
+
  #### Search
 
  ```python   
  from twitter.search import search
 
  search(
      '(#dogs OR #cats) min_retweets:500',
```

### Comparing `twitter-api-client-0.6.4/setup.py` & `twitter-api-client-0.6.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.6.4",
+    version="0.6.5",
     python_requires=">=3.11.0",
     description="Twitter API",
     long_description=dedent('''
     Complete implementation of the undocumented Twitter API
     
     Includes tools to **scrape**, **automate**, and **search** twitter
     
@@ -170,15 +170,15 @@
     ```python
     from twitter.scraper import Scraper
     
     email, username, password = ..., ..., ...
     scraper = Scraper(email, username, password)  # session
     
     ####### User Data ########
-    users = scraper.user_by_screen_name(['bob123', 'jim456', 'stanley789'])
+    users = scraper.user_by_screen_name(['foo', 'bar', 'baz'])
     tweets = scraper.tweets([123, 234, 345])
     likes = scraper.likes([123, 234, 345])
     tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
     media = scraper.media([123, 234, 345])
     following = scraper.following([123, 234, 345])
     followers = scraper.followers([123, 234, 345])
     
@@ -187,14 +187,33 @@
     tweets_details = scraper.tweets_details([456, 567, 678])
     retweeters = scraper.retweeters([456, 567, 678])
     favoriters = scraper.favoriters([456, 567, 678])
     
     scraper.download_media([456, 567, 678])
     ```
     
+    #### Get user/tweet data (no auth)
+    
+    ```python
+    from twitter.noauth.scraper import Scraper
+    
+    scraper = Scraper()
+    
+    users = scraper.user(['foo', 'bar', 'baz'])
+    users = scraper.user_by_id([123, 234, 345])
+    users = scraper.users_by_ids([123, 234, 345])  # special batch query
+    
+    tweets = scraper.tweet_by_id([987, 876, 765])  # condensed
+    tweets = scraper.tweet_details([987, 876, 765])
+    
+    user_tweets = scraper.tweets([123, 234, 345])
+    user_tweets_replies = scraper.tweets_and_replies([123, 234, 345])
+    user_media = scraper.media([123, 234, 345])
+    ```
+    
     #### Search
     
     ```python   
     from twitter.search import search
     
     search(
         '(#dogs OR #cats) min_retweets:500',
```

### Comparing `twitter-api-client-0.6.4/twitter/account.py` & `twitter-api-client-0.6.5/twitter/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 if 'json' in r.headers.get('content-type', ''):
                     data = r.json()
                     if data.get('errors'):
                         logger.log(level, f'[{ERROR}error{RESET}] ({fn.__name__}) {args_info} {r.status_code} {r.text}')
                         return r
 
                 typenames = find_key(data, '__typename')
-                logger.log(level, f'{typenames = }')
+                # logger.log(level, f'{typenames = }')
                 errors = ','.join([t for t in typenames if re.search('fail|error', t, flags=re.I)])
 
                 if errors:
                     message = f'[{ERROR}error{RESET}] {r.status_code} ({BOLD}{fn.__name__}{RESET}) {args_info} {WARN}{errors}{RESET}'
                 else:
                     message = f'[{SUCCESS}success{RESET}] {r.status_code} ({BOLD}{fn.__name__}{RESET}) {args_info}'
```

### Comparing `twitter-api-client-0.6.4/twitter/config/log.py` & `twitter-api-client-0.6.5/twitter/config/log.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.4/twitter/config/operations.py` & `twitter-api-client-0.6.5/twitter/config/operations.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.4/twitter/config/settings.py` & `twitter-api-client-0.6.5/twitter/config/settings.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.4/twitter/constants.py` & `twitter-api-client-0.6.5/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.4/twitter/login.py` & `twitter-api-client-0.6.5/twitter/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def update_token(session: Session, key: str, url: str, payload: dict) -> Session:
     caller_name = sys._getframe(1).f_code.co_name
     try:
         headers = {
             "authorization": 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
             "content-type": "application/json",
-            "user-agent": 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36',
+            "user-agent": 'Mozilla/5.0 (Linux; Android 11; Nokia G20) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.88 Mobile Safari/537.36',
             "x-guest-token": session.cookies.get('guest_token'),
             "x-csrf-token": session.cookies.get("ct0"),
             "x-twitter-auth-type": "OAuth2Session" if session.cookies.get("auth_token") else '',
             "x-twitter-active-user": "yes",
             "x-twitter-client-language": 'en',
         }
         r = session.post(url, headers=headers, json=payload)
```

### Comparing `twitter-api-client-0.6.4/twitter/scraper.py` & `twitter-api-client-0.6.5/twitter/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,16 @@
 
     async def paginate(self, session: ClientSession, data: dict, operation: tuple, limit: int):
         def get_cursor(data):
             # inefficient, but need to deal with arbitrary schema
             entries = find_key(data, 'entries')
             if entries:
                 for entry in entries.pop():
-                    if entry.get('entryId', '').startswith('cursor-bottom'):
+                    entry_id = entry.get('entryId', '')
+                    if ('cursor-bottom' in entry_id) or ('cursor-showmorethreads' in entry_id):
                         content = entry['content']
                         if itemContent := content.get('itemContent'):
                             return itemContent['value']  # v2 cursor
                         return content['value']  # v1 cursor
 
         all_data = []
         try:
```

### Comparing `twitter-api-client-0.6.4/twitter/search.py` & `twitter-api-client-0.6.5/twitter/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,32 +125,20 @@
             return {y.group(): z.group()
                     for x in fp.read().splitlines()
                     if (y := re.search('^[\w-]+(?=:\s)', x),
                         z := re.search(f'(?<={y.group()}:\s).*', x))}
     # default
     headers = {
         'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
-        'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36'
+        'user-agent': 'Mozilla/5.0 (Linux; Android 11; Nokia G20) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.88 Mobile Safari/537.36'
     }
     r = requests.post('https://api.twitter.com/1.1/guest/activate.json', headers=headers)
     headers['x-guest-token'] = r.json()['guest_token']
     return headers
 
 
 def make_output_dirs(path: str) -> Path:
     p = Path(f'~/{path}').expanduser()
     (p / 'raw').mkdir(parents=True, exist_ok=True)
     (p / 'processed').mkdir(parents=True, exist_ok=True)
     (p / 'final').mkdir(parents=True, exist_ok=True)
     return p
-
-
-# @atexit.register
-# def combine_results(in_path: Path = IN_PATH, out_path: Path = OUT_PATH):
-#     try:
-#         out_path.write_text(orjson.dumps({
-#             k: v
-#             for p in in_path.iterdir() if p.suffix == '.json'
-#             for k, v in orjson.loads(p.read_text())['globalObjects']['tweets'].items()
-#         }, option=orjson.OPT_INDENT_2).decode(), encoding='utf-8')
-#     except Exception as e:
-#         logger.debug(f'FAILED to combine search results, {e}')
```

### Comparing `twitter-api-client-0.6.4/twitter/utils.py` & `twitter-api-client-0.6.5/twitter/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     @param session: special requests.Session object, modified during login process. contains attribute `tokens`
     @return: dict representing headers
     """
     return {
         'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
         'cookie': '; '.join(f'{k}={v}' for k, v in session.cookies.items()),
         'referer': 'https://twitter.com/',
-        'user-agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36',
+        'user-agent': 'Mozilla/5.0 (Linux; Android 11; Nokia G20) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.88 Mobile Safari/537.36',
         'x-csrf-token': session.cookies.get('ct0'),
         "x-guest-token": session.cookies.get('guest_token'),
         "x-twitter-auth-type": "OAuth2Session" if session.cookies.get("auth_token") else '',
         "x-twitter-active-user": "yes",
         "x-twitter-client-language": 'en',
     }
```

### Comparing `twitter-api-client-0.6.4/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.6.5/twitter_api_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.6.4
+Version: 0.6.5
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
@@ -164,15 +164,15 @@
  ```python
  from twitter.scraper import Scraper
 
  email, username, password = ..., ..., ...
  scraper = Scraper(email, username, password)  # session
 
  ####### User Data ########
- users = scraper.user_by_screen_name(['bob123', 'jim456', 'stanley789'])
+ users = scraper.user_by_screen_name(['foo', 'bar', 'baz'])
  tweets = scraper.tweets([123, 234, 345])
  likes = scraper.likes([123, 234, 345])
  tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
  media = scraper.media([123, 234, 345])
  following = scraper.following([123, 234, 345])
  followers = scraper.followers([123, 234, 345])
 
@@ -181,14 +181,33 @@
  tweets_details = scraper.tweets_details([456, 567, 678])
  retweeters = scraper.retweeters([456, 567, 678])
  favoriters = scraper.favoriters([456, 567, 678])
 
  scraper.download_media([456, 567, 678])
  ```
 
+ #### Get user/tweet data (no auth)
+
+ ```python
+ from twitter.noauth.scraper import Scraper
+
+ scraper = Scraper()
+
+ users = scraper.user(['foo', 'bar', 'baz'])
+ users = scraper.user_by_id([123, 234, 345])
+ users = scraper.users_by_ids([123, 234, 345])  # special batch query
+
+ tweets = scraper.tweet_by_id([987, 876, 765])  # condensed
+ tweets = scraper.tweet_details([987, 876, 765])
+
+ user_tweets = scraper.tweets([123, 234, 345])
+ user_tweets_replies = scraper.tweets_and_replies([123, 234, 345])
+ user_media = scraper.media([123, 234, 345])
+ ```
+
  #### Search
 
  ```python   
  from twitter.search import search
 
  search(
      '(#dogs OR #cats) min_retweets:500',
```

