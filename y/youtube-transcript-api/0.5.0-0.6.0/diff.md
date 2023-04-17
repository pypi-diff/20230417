# Comparing `tmp/youtube_transcript_api-0.5.0.tar.gz` & `tmp/youtube_transcript_api-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube_transcript_api-0.5.0.tar", last modified: Wed Oct 26 10:04:51 2022, max compression
+gzip compressed data, was "youtube_transcript_api-0.6.0.tar", last modified: Mon Apr 17 13:45:01 2023, max compression
```

## Comparing `youtube_transcript_api-0.5.0.tar` & `youtube_transcript_api-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jdepoix    (501) staff       (20)        0 2022-10-26 10:04:51.367343 youtube_transcript_api-0.5.0/
--rw-r--r--   0 jdepoix    (501) staff       (20)     1069 2018-07-03 09:22:52.000000 youtube_transcript_api-0.5.0/LICENSE
--rw-r--r--   0 jdepoix    (501) staff       (20)    16926 2022-10-26 10:04:51.367130 youtube_transcript_api-0.5.0/PKG-INFO
--rw-r--r--   0 jdepoix    (501) staff       (20)    13664 2022-10-26 10:02:49.000000 youtube_transcript_api-0.5.0/README.md
--rw-r--r--   0 jdepoix    (501) staff       (20)       38 2022-10-26 10:04:51.367406 youtube_transcript_api-0.5.0/setup.cfg
--rw-r--r--   0 jdepoix    (501) staff       (20)     1905 2022-10-26 10:04:34.000000 youtube_transcript_api-0.5.0/setup.py
-drwxr-xr-x   0 jdepoix    (501) staff       (20)        0 2022-10-26 10:04:51.364685 youtube_transcript_api-0.5.0/youtube_transcript_api/
--rw-r--r--   0 jdepoix    (501) staff       (20)      427 2021-11-08 10:03:39.000000 youtube_transcript_api-0.5.0/youtube_transcript_api/__init__.py
--rw-r--r--   0 jdepoix    (501) staff       (20)      200 2019-03-14 17:46:41.000000 youtube_transcript_api-0.5.0/youtube_transcript_api/__main__.py
--rw-r--r--   0 jdepoix    (501) staff       (20)     6832 2022-10-26 09:58:08.000000 youtube_transcript_api-0.5.0/youtube_transcript_api/_api.py
--rw-r--r--   0 jdepoix    (501) staff       (20)     5129 2021-03-22 18:14:06.000000 youtube_transcript_api-0.5.0/youtube_transcript_api/_cli.py
--rw-r--r--   0 jdepoix    (501) staff       (20)     4021 2021-11-08 10:03:39.000000 youtube_transcript_api-0.5.0/youtube_transcript_api/_errors.py
--rw-r--r--   0 jdepoix    (501) staff       (20)      585 2019-03-14 17:46:41.000000 youtube_transcript_api-0.5.0/youtube_transcript_api/_html_unescaping.py
--rw-r--r--   0 jdepoix    (501) staff       (20)       57 2019-12-16 15:31:27.000000 youtube_transcript_api-0.5.0/youtube_transcript_api/_settings.py
--rw-r--r--   0 jdepoix    (501) staff       (20)    13127 2022-03-30 15:27:38.000000 youtube_transcript_api-0.5.0/youtube_transcript_api/_transcripts.py
--rw-r--r--   0 jdepoix    (501) staff       (20)     6886 2022-10-26 09:58:08.000000 youtube_transcript_api-0.5.0/youtube_transcript_api/formatters.py
-drwxr-xr-x   0 jdepoix    (501) staff       (20)        0 2022-10-26 10:04:51.366569 youtube_transcript_api-0.5.0/youtube_transcript_api/test/
--rw-r--r--   0 jdepoix    (501) staff       (20)        1 2019-03-14 17:46:41.000000 youtube_transcript_api-0.5.0/youtube_transcript_api/test/__init__.py
-drwxr-xr-x   0 jdepoix    (501) staff       (20)        0 2022-10-26 10:04:51.366695 youtube_transcript_api-0.5.0/youtube_transcript_api/test/assets/
--rw-r--r--   0 jdepoix    (501) staff       (20)        1 2019-03-14 17:46:41.000000 youtube_transcript_api-0.5.0/youtube_transcript_api/test/assets/__init__.py
--rw-r--r--   0 jdepoix    (501) staff       (20)    12719 2022-10-26 09:58:08.000000 youtube_transcript_api-0.5.0/youtube_transcript_api/test/test_api.py
--rw-r--r--   0 jdepoix    (501) staff       (20)    12084 2021-03-22 18:14:06.000000 youtube_transcript_api-0.5.0/youtube_transcript_api/test/test_cli.py
--rw-r--r--   0 jdepoix    (501) staff       (20)     4898 2022-10-26 09:58:08.000000 youtube_transcript_api-0.5.0/youtube_transcript_api/test/test_formatters.py
-drwxr-xr-x   0 jdepoix    (501) staff       (20)        0 2022-10-26 10:04:51.365830 youtube_transcript_api-0.5.0/youtube_transcript_api.egg-info/
--rw-r--r--   0 jdepoix    (501) staff       (20)    16926 2022-10-26 10:04:51.000000 youtube_transcript_api-0.5.0/youtube_transcript_api.egg-info/PKG-INFO
--rw-r--r--   0 jdepoix    (501) staff       (20)      839 2022-10-26 10:04:51.000000 youtube_transcript_api-0.5.0/youtube_transcript_api.egg-info/SOURCES.txt
--rw-r--r--   0 jdepoix    (501) staff       (20)        1 2022-10-26 10:04:51.000000 youtube_transcript_api-0.5.0/youtube_transcript_api.egg-info/dependency_links.txt
--rw-r--r--   0 jdepoix    (501) staff       (20)       81 2022-10-26 10:04:51.000000 youtube_transcript_api-0.5.0/youtube_transcript_api.egg-info/entry_points.txt
--rw-r--r--   0 jdepoix    (501) staff       (20)        9 2022-10-26 10:04:51.000000 youtube_transcript_api-0.5.0/youtube_transcript_api.egg-info/requires.txt
--rw-r--r--   0 jdepoix    (501) staff       (20)       23 2022-10-26 10:04:51.000000 youtube_transcript_api-0.5.0/youtube_transcript_api.egg-info/top_level.txt
+drwxr-xr-x   0 jdepoix    (501) staff       (20)        0 2023-04-17 13:45:01.718451 youtube_transcript_api-0.6.0/
+-rw-r--r--   0 jdepoix    (501) staff       (20)     1069 2018-07-03 09:22:52.000000 youtube_transcript_api-0.6.0/LICENSE
+-rw-r--r--   0 jdepoix    (501) staff       (20)    17290 2023-04-17 13:45:01.718283 youtube_transcript_api-0.6.0/PKG-INFO
+-rw-r--r--   0 jdepoix    (501) staff       (20)    13965 2023-04-17 13:15:55.000000 youtube_transcript_api-0.6.0/README.md
+-rw-r--r--   0 jdepoix    (501) staff       (20)       38 2023-04-17 13:45:01.718503 youtube_transcript_api-0.6.0/setup.cfg
+-rw-r--r--   0 jdepoix    (501) staff       (20)     1905 2023-04-17 13:44:22.000000 youtube_transcript_api-0.6.0/setup.py
+drwxr-xr-x   0 jdepoix    (501) staff       (20)        0 2023-04-17 13:45:01.716621 youtube_transcript_api-0.6.0/youtube_transcript_api/
+-rw-r--r--   0 jdepoix    (501) staff       (20)      447 2023-04-17 13:44:09.000000 youtube_transcript_api-0.6.0/youtube_transcript_api/__init__.py
+-rw-r--r--   0 jdepoix    (501) staff       (20)      200 2019-03-14 17:46:41.000000 youtube_transcript_api-0.6.0/youtube_transcript_api/__main__.py
+-rw-r--r--   0 jdepoix    (501) staff       (20)     7206 2023-04-17 13:15:55.000000 youtube_transcript_api-0.6.0/youtube_transcript_api/_api.py
+-rw-r--r--   0 jdepoix    (501) staff       (20)     5129 2021-03-22 18:14:06.000000 youtube_transcript_api-0.6.0/youtube_transcript_api/_cli.py
+-rw-r--r--   0 jdepoix    (501) staff       (20)     4374 2023-04-17 13:44:09.000000 youtube_transcript_api-0.6.0/youtube_transcript_api/_errors.py
+-rw-r--r--   0 jdepoix    (501) staff       (20)      585 2019-03-14 17:46:41.000000 youtube_transcript_api-0.6.0/youtube_transcript_api/_html_unescaping.py
+-rw-r--r--   0 jdepoix    (501) staff       (20)       57 2019-12-16 15:31:27.000000 youtube_transcript_api-0.6.0/youtube_transcript_api/_settings.py
+-rw-r--r--   0 jdepoix    (501) staff       (20)    14211 2023-04-17 13:44:09.000000 youtube_transcript_api-0.6.0/youtube_transcript_api/_transcripts.py
+-rw-r--r--   0 jdepoix    (501) staff       (20)     6886 2022-10-26 09:58:08.000000 youtube_transcript_api-0.6.0/youtube_transcript_api/formatters.py
+drwxr-xr-x   0 jdepoix    (501) staff       (20)        0 2023-04-17 13:45:01.717930 youtube_transcript_api-0.6.0/youtube_transcript_api/test/
+-rw-r--r--   0 jdepoix    (501) staff       (20)        1 2019-03-14 17:46:41.000000 youtube_transcript_api-0.6.0/youtube_transcript_api/test/__init__.py
+drwxr-xr-x   0 jdepoix    (501) staff       (20)        0 2023-04-17 13:45:01.718053 youtube_transcript_api-0.6.0/youtube_transcript_api/test/assets/
+-rw-r--r--   0 jdepoix    (501) staff       (20)        1 2019-03-14 17:46:41.000000 youtube_transcript_api-0.6.0/youtube_transcript_api/test/assets/__init__.py
+-rw-r--r--   0 jdepoix    (501) staff       (20)    13691 2023-04-17 13:44:09.000000 youtube_transcript_api-0.6.0/youtube_transcript_api/test/test_api.py
+-rw-r--r--   0 jdepoix    (501) staff       (20)    12091 2023-04-17 13:15:55.000000 youtube_transcript_api-0.6.0/youtube_transcript_api/test/test_cli.py
+-rw-r--r--   0 jdepoix    (501) staff       (20)     4898 2022-10-26 09:58:08.000000 youtube_transcript_api-0.6.0/youtube_transcript_api/test/test_formatters.py
+drwxr-xr-x   0 jdepoix    (501) staff       (20)        0 2023-04-17 13:45:01.717474 youtube_transcript_api-0.6.0/youtube_transcript_api.egg-info/
+-rw-r--r--   0 jdepoix    (501) staff       (20)    17290 2023-04-17 13:45:01.000000 youtube_transcript_api-0.6.0/youtube_transcript_api.egg-info/PKG-INFO
+-rw-r--r--   0 jdepoix    (501) staff       (20)      839 2023-04-17 13:45:01.000000 youtube_transcript_api-0.6.0/youtube_transcript_api.egg-info/SOURCES.txt
+-rw-r--r--   0 jdepoix    (501) staff       (20)        1 2023-04-17 13:45:01.000000 youtube_transcript_api-0.6.0/youtube_transcript_api.egg-info/dependency_links.txt
+-rw-r--r--   0 jdepoix    (501) staff       (20)       81 2023-04-17 13:45:01.000000 youtube_transcript_api-0.6.0/youtube_transcript_api.egg-info/entry_points.txt
+-rw-r--r--   0 jdepoix    (501) staff       (20)        9 2023-04-17 13:45:01.000000 youtube_transcript_api-0.6.0/youtube_transcript_api.egg-info/requires.txt
+-rw-r--r--   0 jdepoix    (501) staff       (20)       23 2023-04-17 13:45:01.000000 youtube_transcript_api-0.6.0/youtube_transcript_api.egg-info/top_level.txt
```

### Comparing `youtube_transcript_api-0.5.0/LICENSE` & `youtube_transcript_api-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `youtube_transcript_api-0.5.0/PKG-INFO` & `youtube_transcript_api-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube_transcript_api
-Version: 0.5.0
+Version: 0.6.0
 Summary: This is an python API which allows you to get the transcripts/subtitles for a given YouTube video. It also works for automatically generated subtitles, supports translating subtitles and it does not require a headless browser, like other selenium based solutions do!
 Home-page: https://github.com/jdepoix/youtube-transcript-api
 Author: Jonas Depoix
 Author-email: jonas.depoix@web.de
 License: UNKNOWN
 Description: 
         # YouTube Transcript/Subtitle API (including automatically generated subtitles and subtitle translations)  
@@ -14,15 +14,15 @@
         This is a python API which allows you to get the transcript/subtitles for a given YouTube video. It also works for automatically generated subtitles, supports translating subtitles and it does not require a headless browser, like other selenium based solutions do!
         
         ## Install
         
         It is recommended to [install this module by using pip](https://pypi.org/project/youtube-transcript-api/):
         
         ```
-        pip install youtube_transcript_api
+        pip install youtube-transcript-api
         ```
         
         If you want to use it from source, you'll have to install the dependencies manually:
         
         ```
         pip install -r requirements.txt
         ```
@@ -52,16 +52,17 @@
                 'text': 'how are you',
                 'start': 14.08,
                 'duration': 7.58
             },
             # ...
         ]
         ```
+        ### Translate transcript
         
-        You can also add the `languages` param if you want to make sure the transcripts are retrieved in your desired language (it defaults to english).
+        You can add the `languages` param if you want to make sure the transcripts are retrieved in your desired language (it defaults to english).
         
         ```python
         YouTubeTranscriptApi.get_transcripts(video_ids, languages=['de', 'en'])
         ```
         
         It's a list of language codes in a descending priority. In this example it will first try to fetch the german transcript (`'de'`) and then fetch the english transcript (`'en'`) if it fails to do so. If you want to find out which languages are available first, [have a look at `list_transcripts()`](#list-available-transcripts)
         
@@ -69,14 +70,22 @@
         
         ```python
         YouTubeTranscriptApi.get_transcripts(video_ids, languages=['de', 'en'])
         ```
         
         `languages` also is optional here.
         
+        ### Preserve formatting
+        
+        You can also add `preserve_formatting=True` if you'd like to keep HTML formatting elements such as `<i>` (italics) and `<b>` (bold).
+        
+        ```python
+        YouTubeTranscriptApi.get_transcripts(video_ids, languages=['de', 'en'], preserve_formatting=True)
+        ```
+        
         ### List available transcripts
         
         If you want to list all transcripts which are available for a given video you can call:
         
         ```python
         transcript_list = YouTubeTranscriptApi.list_transcripts(video_id)
         ```
@@ -293,15 +302,15 @@
         
         ```python  
         from youtube_transcript_api import YouTubeTranscriptApi  
         
         YouTubeTranscriptApi.get_transcript(video_id, proxies={"https": "https://user:pass@domain:port"})
         ```  
         
-        As the `proxies` dict is passed on to the `requests.get(...)` call, it follows the [format used by the requests library](http://docs.python-requests.org/en/master/user/advanced/#proxies).  
+        As the `proxies` dict is passed on to the `requests.get(...)` call, it follows the [format used by the requests library](https://requests.readthedocs.io/en/latest/user/advanced/#proxies).  
         
         Using the CLI:  
         
         ```  
         youtube_transcript_api <first_video_id> <second_video_id> --https-proxy https://user:pass@domain:port
         ```
```

### Comparing `youtube_transcript_api-0.5.0/README.md` & `youtube_transcript_api-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 This is a python API which allows you to get the transcript/subtitles for a given YouTube video. It also works for automatically generated subtitles, supports translating subtitles and it does not require a headless browser, like other selenium based solutions do!
 
 ## Install
 
 It is recommended to [install this module by using pip](https://pypi.org/project/youtube-transcript-api/):
 
 ```
-pip install youtube_transcript_api
+pip install youtube-transcript-api
 ```
 
 If you want to use it from source, you'll have to install the dependencies manually:
 
 ```
 pip install -r requirements.txt
 ```
@@ -44,16 +44,17 @@
         'text': 'how are you',
         'start': 14.08,
         'duration': 7.58
     },
     # ...
 ]
 ```
+### Translate transcript
 
-You can also add the `languages` param if you want to make sure the transcripts are retrieved in your desired language (it defaults to english).
+You can add the `languages` param if you want to make sure the transcripts are retrieved in your desired language (it defaults to english).
 
 ```python
 YouTubeTranscriptApi.get_transcripts(video_ids, languages=['de', 'en'])
 ```
 
 It's a list of language codes in a descending priority. In this example it will first try to fetch the german transcript (`'de'`) and then fetch the english transcript (`'en'`) if it fails to do so. If you want to find out which languages are available first, [have a look at `list_transcripts()`](#list-available-transcripts)
 
@@ -61,14 +62,22 @@
 
 ```python
 YouTubeTranscriptApi.get_transcripts(video_ids, languages=['de', 'en'])
 ```
 
 `languages` also is optional here.
 
+### Preserve formatting
+
+You can also add `preserve_formatting=True` if you'd like to keep HTML formatting elements such as `<i>` (italics) and `<b>` (bold).
+
+```python
+YouTubeTranscriptApi.get_transcripts(video_ids, languages=['de', 'en'], preserve_formatting=True)
+```
+
 ### List available transcripts
 
 If you want to list all transcripts which are available for a given video you can call:
 
 ```python
 transcript_list = YouTubeTranscriptApi.list_transcripts(video_id)
 ```
@@ -285,15 +294,15 @@
 
 ```python  
 from youtube_transcript_api import YouTubeTranscriptApi  
 
 YouTubeTranscriptApi.get_transcript(video_id, proxies={"https": "https://user:pass@domain:port"})
 ```  
 
-As the `proxies` dict is passed on to the `requests.get(...)` call, it follows the [format used by the requests library](http://docs.python-requests.org/en/master/user/advanced/#proxies).  
+As the `proxies` dict is passed on to the `requests.get(...)` call, it follows the [format used by the requests library](https://requests.readthedocs.io/en/latest/user/advanced/#proxies).  
 
 Using the CLI:  
 
 ```  
 youtube_transcript_api <first_video_id> <second_video_id> --https-proxy https://user:pass@domain:port
 ```
```

### Comparing `youtube_transcript_api-0.5.0/setup.py` & `youtube_transcript_api-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         top_level_dir='{dirname}/youtube_transcript_api'.format(dirname=os.path.dirname(__file__))
     )
     return test_suite
 
 
 setuptools.setup(
     name="youtube_transcript_api",
-    version="0.5.0",
+    version="0.6.0",
     author="Jonas Depoix",
     author_email="jonas.depoix@web.de",
     description="This is an python API which allows you to get the transcripts/subtitles for a given YouTube video. It also works for automatically generated subtitles, supports translating subtitles and it does not require a headless browser, like other selenium based solutions do!",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     keywords="youtube-api subtitles youtube transcripts transcript subtitle youtube-subtitles youtube-transcripts cli",
     url="https://github.com/jdepoix/youtube-transcript-api",
```

### Comparing `youtube_transcript_api-0.5.0/youtube_transcript_api/_api.py` & `youtube_transcript_api-0.6.0/youtube_transcript_api/_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,15 +67,16 @@
         with requests.Session() as http_client:
             if cookies:
                 http_client.cookies = cls._load_cookies(cookies, video_id)
             http_client.proxies = proxies if proxies else {}
             return TranscriptListFetcher(http_client).fetch(video_id)
 
     @classmethod
-    def get_transcripts(cls, video_ids, languages=('en',), continue_after_error=False, proxies=None, cookies=None):
+    def get_transcripts(cls, video_ids, languages=('en',), continue_after_error=False, proxies=None,
+                        cookies=None, preserve_formatting=False):
         """
         Retrieves the transcripts for a list of videos.
 
         :param video_ids: a list of youtube video ids
         :type video_ids: list[str]
         :param languages: A list of language codes in a descending priority. For example, if this is set to ['de', 'en']
         it will first try to fetch the german transcript (de) and then fetch the english transcript (en) if it fails to
@@ -84,36 +85,38 @@
         :param continue_after_error: if this is set the execution won't be stopped, if an error occurs while retrieving
         one of the video transcripts
         :type continue_after_error: bool
         :param proxies: a dictionary mapping of http and https proxies to be used for the network requests
         :type proxies: {'http': str, 'https': str} - http://docs.python-requests.org/en/master/user/advanced/#proxies
         :param cookies: a string of the path to a text file containing youtube authorization cookies
         :type cookies: str
+        :param preserve_formatting: whether to keep select HTML text formatting
+        :type preserve_formatting: bool
         :return: a tuple containing a dictionary mapping video ids onto their corresponding transcripts, and a list of
         video ids, which could not be retrieved
         :rtype ({str: [{'text': str, 'start': float, 'end': float}]}, [str]}):
         """
         assert isinstance(video_ids, list), "`video_ids` must be a list of strings"
 
         data = {}
         unretrievable_videos = []
 
         for video_id in video_ids:
             try:
-                data[video_id] = cls.get_transcript(video_id, languages, proxies, cookies)
+                data[video_id] = cls.get_transcript(video_id, languages, proxies, cookies, preserve_formatting)
             except Exception as exception:
                 if not continue_after_error:
                     raise exception
 
                 unretrievable_videos.append(video_id)
 
         return data, unretrievable_videos
 
     @classmethod
-    def get_transcript(cls, video_id, languages=('en',), proxies=None, cookies=None):
+    def get_transcript(cls, video_id, languages=('en',), proxies=None, cookies=None, preserve_formatting=False):
         """
         Retrieves the transcript for a single video. This is just a shortcut for calling::
 
             YouTubeTranscriptApi.list_transcripts(video_id, proxies).find_transcript(languages).fetch()
 
         :param video_id: the youtube video id
         :type video_id: str
@@ -121,20 +124,22 @@
         it will first try to fetch the german transcript (de) and then fetch the english transcript (en) if it fails to
         do so.
         :type languages: list[str]
         :param proxies: a dictionary mapping of http and https proxies to be used for the network requests
         :type proxies: {'http': str, 'https': str} - http://docs.python-requests.org/en/master/user/advanced/#proxies
         :param cookies: a string of the path to a text file containing youtube authorization cookies
         :type cookies: str
+        :param preserve_formatting: whether to keep select HTML text formatting
+        :type preserve_formatting: bool
         :return: a list of dictionaries containing the 'text', 'start' and 'duration' keys
         :rtype [{'text': str, 'start': float, 'end': float}]:
         """
         assert isinstance(video_id, str), "`video_id` must be a string"
-        return cls.list_transcripts(video_id, proxies, cookies).find_transcript(languages).fetch()
-    
+        return cls.list_transcripts(video_id, proxies, cookies).find_transcript(languages).fetch(preserve_formatting=preserve_formatting)
+
     @classmethod
     def _load_cookies(cls, cookies, video_id):
         try:
             cookie_jar = cookiejar.MozillaCookieJar()
             cookie_jar.load(cookies)
             if not cookie_jar:
                 raise CookiesInvalid(video_id)
```

### Comparing `youtube_transcript_api-0.5.0/youtube_transcript_api/_cli.py` & `youtube_transcript_api-0.6.0/youtube_transcript_api/_cli.py`

 * *Files identical despite different names*

### Comparing `youtube_transcript_api-0.5.0/youtube_transcript_api/_errors.py` & `youtube_transcript_api-0.6.0/youtube_transcript_api/_errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,14 +49,22 @@
         )
 
 
 class VideoUnavailable(CouldNotRetrieveTranscript):
     CAUSE_MESSAGE = 'The video is no longer available'
 
 
+class InvalidVideoId(CouldNotRetrieveTranscript):
+    CAUSE_MESSAGE = (
+        'You provided an invalid video id. Make sure you are using the video id and NOT the url!\n\n'
+        'Do NOT run: `YouTubeTranscriptApi.get_transcript("https://www.youtube.com/watch?v=1234")`\n'
+        'Instead run: `YouTubeTranscriptApi.get_transcript("1234")`'
+    )
+
+
 class TooManyRequests(CouldNotRetrieveTranscript):
     CAUSE_MESSAGE = (
         'YouTube is receiving too many requests from this IP and now requires solving a captcha to continue. '
         'One of the following things can be done to work around this:\n\
         - Manually solve the captcha in a browser and export the cookie. '
         'Read here how to use that cookie with '
         'youtube-transcript-api: https://github.com/jdepoix/youtube-transcript-api#cookies\n\
```

### Comparing `youtube_transcript_api-0.5.0/youtube_transcript_api/_html_unescaping.py` & `youtube_transcript_api-0.6.0/youtube_transcript_api/_html_unescaping.py`

 * *Files identical despite different names*

### Comparing `youtube_transcript_api-0.5.0/youtube_transcript_api/_transcripts.py` & `youtube_transcript_api-0.6.0/youtube_transcript_api/_transcripts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 
 # This can only be tested by using different python versions, therefore it is not covered by coverage.py
-if sys.version_info.major == 2: # pragma: no cover
+if sys.version_info.major == 2:  # pragma: no cover
     reload(sys)
     sys.setdefaultencoding('utf-8')
 
 import json
 
 from xml.etree import ElementTree
 
@@ -20,14 +20,15 @@
     YouTubeRequestFailed,
     NoTranscriptFound,
     TranscriptsDisabled,
     NotTranslatable,
     TranslationLanguageNotAvailable,
     NoTranscriptAvailable,
     FailedToCreateConsentCookie,
+    InvalidVideoId,
 )
 from ._settings import WATCH_URL
 
 
 def _raise_http_errors(response, video_id):
     try:
         response.raise_for_status()
@@ -40,21 +41,23 @@
     def __init__(self, http_client):
         self._http_client = http_client
 
     def fetch(self, video_id):
         return TranscriptList.build(
             self._http_client,
             video_id,
-            self._extract_captions_json(self._fetch_video_html(video_id), video_id)
+            self._extract_captions_json(self._fetch_video_html(video_id), video_id),
         )
 
     def _extract_captions_json(self, html, video_id):
         splitted_html = html.split('"captions":')
 
         if len(splitted_html) <= 1:
+            if video_id.startswith('http://') or video_id.startswith('https://'):
+                raise InvalidVideoId(video_id)
             if 'class="g-recaptcha"' in html:
                 raise TooManyRequests(video_id)
             if '"playabilityStatus":' not in html:
                 raise VideoUnavailable(video_id)
 
             raise TranscriptsDisabled(video_id)
 
@@ -90,14 +93,15 @@
 
 
 class TranscriptList(object):
     """
     This object represents a list of transcripts. It can be iterated over to list all transcripts which are available
     for a given YouTube video. Also it provides functionality to search for a transcript in a given language.
     """
+
     def __init__(self, video_id, manually_created_transcripts, generated_transcripts, translation_languages):
         """
         The constructor is only for internal use. Use the static build method instead.
 
         :param video_id: the id of the video this TranscriptList is for
         :type video_id: str
         :param manually_created_transcripts: dict mapping language codes to the manually created transcripts
@@ -145,15 +149,15 @@
             transcript_dict[caption['languageCode']] = Transcript(
                 http_client,
                 video_id,
                 caption['baseUrl'],
                 caption['name']['simpleText'],
                 caption['languageCode'],
                 caption.get('kind', '') == 'asr',
-                translation_languages if caption.get('isTranslatable', False) else []
+                translation_languages if caption.get('isTranslatable', False) else [],
             )
 
         return TranscriptList(
             video_id,
             manually_created_transcripts,
             generated_transcripts,
             translation_languages,
@@ -176,39 +180,39 @@
         :rtype Transcript:
         :raises: NoTranscriptFound
         """
         return self._find_transcript(language_codes, [self._manually_created_transcripts, self._generated_transcripts])
 
     def find_generated_transcript(self, language_codes):
         """
-        Finds a automatically generated transcript for a given language code.
+        Finds an automatically generated transcript for a given language code.
 
         :param language_codes: A list of language codes in a descending priority. For example, if this is set to
         ['de', 'en'] it will first try to fetch the german transcript (de) and then fetch the english transcript (en) if
         it fails to do so.
         :type languages: list[str]
         :return: the found Transcript
         :rtype Transcript:
         :raises: NoTranscriptFound
         """
-        return self._find_transcript(language_codes, [self._generated_transcripts,])
+        return self._find_transcript(language_codes, [self._generated_transcripts])
 
     def find_manually_created_transcript(self, language_codes):
         """
         Finds a manually created transcript for a given language code.
 
         :param language_codes: A list of language codes in a descending priority. For example, if this is set to
         ['de', 'en'] it will first try to fetch the german transcript (de) and then fetch the english transcript (en) if
         it fails to do so.
         :type languages: list[str]
         :return: the found Transcript
         :rtype Transcript:
         :raises: NoTranscriptFound
         """
-        return self._find_transcript(language_codes, [self._manually_created_transcripts,])
+        return self._find_transcript(language_codes, [self._manually_created_transcripts])
 
     def _find_transcript(self, language_codes, transcript_dicts):
         for language_code in language_codes:
             for transcript_dict in transcript_dicts:
                 if language_code in transcript_dict:
                     return transcript_dict[language_code]
 
@@ -272,23 +276,24 @@
         self.is_generated = is_generated
         self.translation_languages = translation_languages
         self._translation_languages_dict = {
             translation_language['language_code']: translation_language['language']
             for translation_language in translation_languages
         }
 
-    def fetch(self):
+    def fetch(self, preserve_formatting=False):
         """
         Loads the actual transcript data.
-
+        :param preserve_formatting: whether to keep select HTML text formatting
+        :type preserve_formatting: bool
         :return: a list of dictionaries containing the 'text', 'start' and 'duration' keys
         :rtype [{'text': str, 'start': float, 'end': float}]:
         """
         response = self._http_client.get(self._url)
-        return _TranscriptParser().parse(
+        return _TranscriptParser(preserve_formatting=preserve_formatting).parse(
             _raise_http_errors(response, self.video_id).text,
         )
 
     def __str__(self):
         return '{language_code} ("{language}"){translation_description}'.format(
             language=self.language,
             language_code=self.language_code,
@@ -314,19 +319,42 @@
             language_code,
             True,
             [],
         )
 
 
 class _TranscriptParser(object):
-    HTML_TAG_REGEX = re.compile(r'<[^>]*>', re.IGNORECASE)
+    _FORMATTING_TAGS = [
+        'strong',  # important
+        'em',  # emphasized
+        'b',  # bold
+        'i',  # italic
+        'mark',  # marked
+        'small',  # smaller
+        'del',  # deleted
+        'ins',  # inserted
+        'sub',  # subscript
+        'sup',  # superscript
+    ]
+
+    def __init__(self, preserve_formatting=False):
+        self._html_regex = self._get_html_regex(preserve_formatting)
+
+    def _get_html_regex(self, preserve_formatting):
+        if preserve_formatting:
+            formats_regex = '|'.join(self._FORMATTING_TAGS)
+            formats_regex = r'<\/?(?!\/?(' + formats_regex + r')\b).*?\b>'
+            html_regex = re.compile(formats_regex, re.IGNORECASE)
+        else:
+            html_regex = re.compile(r'<[^>]*>', re.IGNORECASE)
+        return html_regex
 
     def parse(self, plain_data):
         return [
             {
-                'text': re.sub(self.HTML_TAG_REGEX, '', unescape(xml_element.text)),
+                'text': re.sub(self._html_regex, '', unescape(xml_element.text)),
                 'start': float(xml_element.attrib['start']),
                 'duration': float(xml_element.attrib.get('dur', '0.0')),
             }
             for xml_element in ElementTree.fromstring(plain_data)
             if xml_element.text is not None
         ]
```

### Comparing `youtube_transcript_api-0.5.0/youtube_transcript_api/formatters.py` & `youtube_transcript_api-0.6.0/youtube_transcript_api/formatters.py`

 * *Files identical despite different names*

### Comparing `youtube_transcript_api-0.5.0/youtube_transcript_api/test/test_api.py` & `youtube_transcript_api-0.6.0/youtube_transcript_api/test/test_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     NoTranscriptAvailable,
     NotTranslatable,
     TranslationLanguageNotAvailable,
     CookiePathInvalid,
     CookiesInvalid,
     FailedToCreateConsentCookie,
     YouTubeRequestFailed,
+    InvalidVideoId,
 )
 
 
 def load_asset(filename):
     filepath = '{dirname}/assets/{filename}'.format(
         dirname=os.path.dirname(__file__), filename=filename)
 
@@ -57,14 +58,26 @@
             [
                 {'text': 'Hey, this is just a test', 'start': 0.0, 'duration': 1.54},
                 {'text': 'this is not the original transcript', 'start': 1.54, 'duration': 4.16},
                 {'text': 'just something shorter, I made up for testing', 'start': 5.7, 'duration': 3.239}
             ]
         )
 
+    def test_get_transcript_formatted(self):
+        transcript = YouTubeTranscriptApi.get_transcript('GJLlxj_dtq8', preserve_formatting=True)
+
+        self.assertEqual(
+            transcript,
+            [
+                {'text': 'Hey, this is just a test', 'start': 0.0, 'duration': 1.54},
+                {'text': 'this is <i>not</i> the original transcript', 'start': 1.54, 'duration': 4.16},
+                {'text': 'just something shorter, I made up for testing', 'start': 5.7, 'duration': 3.239}
+            ]
+        )
+
     def test_list_transcripts(self):
         transcript_list = YouTubeTranscriptApi.list_transcripts('GJLlxj_dtq8')
 
         language_codes = {transcript.language_code for transcript in transcript_list}
 
         self.assertEqual(language_codes, {'zh', 'de', 'en', 'hi', 'ja', 'ko', 'es', 'cs', 'en'})
 
@@ -81,14 +94,24 @@
         with self.assertRaises(NoTranscriptFound):
             transcript_list.find_generated_transcript(['cs'])
 
         transcript = transcript_list.find_generated_transcript(['en'])
 
         self.assertTrue(transcript.is_generated)
 
+    def test_list_transcripts__url_as_video_id(self):
+        httpretty.register_uri(
+            httpretty.GET,
+            'https://www.youtube.com/watch',
+            body=load_asset('youtube_transcripts_disabled.html.static')
+        )
+
+        with self.assertRaises(InvalidVideoId):
+            YouTubeTranscriptApi.list_transcripts('https://www.youtube.com/watch?v=GJLlxj_dtq8')
+
     def test_translate_transcript(self):
         transcript = YouTubeTranscriptApi.list_transcripts('GJLlxj_dtq8').find_transcript(['en'])
 
         translated_transcript = transcript.translate('af')
 
         self.assertEqual(translated_transcript.language_code, 'af')
         self.assertIn('&tlang=af', translated_transcript._url)
@@ -250,61 +273,61 @@
             transcript,
             [
                 {'text': 'Hey, this is just a test', 'start': 0.0, 'duration': 1.54},
                 {'text': 'this is not the original transcript', 'start': 1.54, 'duration': 4.16},
                 {'text': 'just something shorter, I made up for testing', 'start': 5.7, 'duration': 3.239}
             ]
         )
-    
+
     def test_get_transcript__assertionerror_if_input_not_string(self):
         with self.assertRaises(AssertionError):
             YouTubeTranscriptApi.get_transcript(['video_id_1', 'video_id_2'])
-    
+
     def test_get_transcripts__assertionerror_if_input_not_list(self):
         with self.assertRaises(AssertionError):
             YouTubeTranscriptApi.get_transcripts('video_id_1')
 
     @patch('youtube_transcript_api.YouTubeTranscriptApi.get_transcript')
     def test_get_transcripts(self, mock_get_transcript):
         video_id_1 = 'video_id_1'
         video_id_2 = 'video_id_2'
         languages = ['de', 'en']
 
         YouTubeTranscriptApi.get_transcripts([video_id_1, video_id_2], languages=languages)
 
-        mock_get_transcript.assert_any_call(video_id_1, languages, None, None)
-        mock_get_transcript.assert_any_call(video_id_2, languages, None, None)
+        mock_get_transcript.assert_any_call(video_id_1, languages, None, None, False)
+        mock_get_transcript.assert_any_call(video_id_2, languages, None, None, False)
         self.assertEqual(mock_get_transcript.call_count, 2)
 
     @patch('youtube_transcript_api.YouTubeTranscriptApi.get_transcript', side_effect=Exception('Error'))
     def test_get_transcripts__stop_on_error(self, mock_get_transcript):
         with self.assertRaises(Exception):
             YouTubeTranscriptApi.get_transcripts(['video_id_1', 'video_id_2'])
 
     @patch('youtube_transcript_api.YouTubeTranscriptApi.get_transcript', side_effect=Exception('Error'))
     def test_get_transcripts__continue_on_error(self, mock_get_transcript):
         video_id_1 = 'video_id_1'
         video_id_2 = 'video_id_2'
 
         YouTubeTranscriptApi.get_transcripts(['video_id_1', 'video_id_2'], continue_after_error=True)
 
-        mock_get_transcript.assert_any_call(video_id_1, ('en',), None, None)
-        mock_get_transcript.assert_any_call(video_id_2, ('en',), None, None)
+        mock_get_transcript.assert_any_call(video_id_1, ('en',), None, None, False)
+        mock_get_transcript.assert_any_call(video_id_2, ('en',), None, None, False)
     
     @patch('youtube_transcript_api.YouTubeTranscriptApi.get_transcript')
     def test_get_transcripts__with_cookies(self, mock_get_transcript):
         cookies = '/example_cookies.txt'
         YouTubeTranscriptApi.get_transcripts(['GJLlxj_dtq8'], cookies=cookies)
-        mock_get_transcript.assert_any_call('GJLlxj_dtq8', ('en',), None, cookies)
+        mock_get_transcript.assert_any_call('GJLlxj_dtq8', ('en',), None, cookies, False)
 
     @patch('youtube_transcript_api.YouTubeTranscriptApi.get_transcript')
     def test_get_transcripts__with_proxies(self, mock_get_transcript):
         proxies = {'http': '', 'https:': ''}
         YouTubeTranscriptApi.get_transcripts(['GJLlxj_dtq8'], proxies=proxies)
-        mock_get_transcript.assert_any_call('GJLlxj_dtq8', ('en',), proxies, None)
+        mock_get_transcript.assert_any_call('GJLlxj_dtq8', ('en',), proxies, None, False)
 
     def test_load_cookies(self):
         dirname, filename = os.path.split(os.path.abspath(__file__))
         cookies = dirname + '/example_cookies.txt'
         session_cookies = YouTubeTranscriptApi._load_cookies(cookies, 'GJLlxj_dtq8')
         self.assertEqual({'TEST_FIELD': 'TEST_VALUE'},  requests.utils.dict_from_cookiejar(session_cookies))
```

### Comparing `youtube_transcript_api-0.5.0/youtube_transcript_api/test/test_cli.py` & `youtube_transcript_api-0.6.0/youtube_transcript_api/test/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class TestYouTubeTranscriptCli(TestCase):
     def setUp(self):
         self.transcript_mock = MagicMock()
         self.transcript_mock.fetch = MagicMock(return_value=[
             {'text': 'Hey, this is just a test', 'start': 0.0, 'duration': 1.54},
-            {'text': 'this is not the original transcript', 'start': 1.54, 'duration': 4.16},
+            {'text': 'this is <i>not</i> the original transcript', 'start': 1.54, 'duration': 4.16},
             {'text': 'just something shorter, I made up for testing', 'start': 5.7, 'duration': 3.239}
         ])
         self.transcript_mock.translate = MagicMock(return_value=self.transcript_mock)
 
         self.transcript_list_mock = MagicMock()
         self.transcript_list_mock.find_generated_transcript = MagicMock(return_value=self.transcript_mock)
         self.transcript_list_mock.find_manually_created_transcript = MagicMock(return_value=self.transcript_mock)
```

### Comparing `youtube_transcript_api-0.5.0/youtube_transcript_api/test/test_formatters.py` & `youtube_transcript_api-0.6.0/youtube_transcript_api/test/test_formatters.py`

 * *Files identical despite different names*

### Comparing `youtube_transcript_api-0.5.0/youtube_transcript_api.egg-info/PKG-INFO` & `youtube_transcript_api-0.6.0/youtube_transcript_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube-transcript-api
-Version: 0.5.0
+Version: 0.6.0
 Summary: This is an python API which allows you to get the transcripts/subtitles for a given YouTube video. It also works for automatically generated subtitles, supports translating subtitles and it does not require a headless browser, like other selenium based solutions do!
 Home-page: https://github.com/jdepoix/youtube-transcript-api
 Author: Jonas Depoix
 Author-email: jonas.depoix@web.de
 License: UNKNOWN
 Description: 
         # YouTube Transcript/Subtitle API (including automatically generated subtitles and subtitle translations)  
@@ -14,15 +14,15 @@
         This is a python API which allows you to get the transcript/subtitles for a given YouTube video. It also works for automatically generated subtitles, supports translating subtitles and it does not require a headless browser, like other selenium based solutions do!
         
         ## Install
         
         It is recommended to [install this module by using pip](https://pypi.org/project/youtube-transcript-api/):
         
         ```
-        pip install youtube_transcript_api
+        pip install youtube-transcript-api
         ```
         
         If you want to use it from source, you'll have to install the dependencies manually:
         
         ```
         pip install -r requirements.txt
         ```
@@ -52,16 +52,17 @@
                 'text': 'how are you',
                 'start': 14.08,
                 'duration': 7.58
             },
             # ...
         ]
         ```
+        ### Translate transcript
         
-        You can also add the `languages` param if you want to make sure the transcripts are retrieved in your desired language (it defaults to english).
+        You can add the `languages` param if you want to make sure the transcripts are retrieved in your desired language (it defaults to english).
         
         ```python
         YouTubeTranscriptApi.get_transcripts(video_ids, languages=['de', 'en'])
         ```
         
         It's a list of language codes in a descending priority. In this example it will first try to fetch the german transcript (`'de'`) and then fetch the english transcript (`'en'`) if it fails to do so. If you want to find out which languages are available first, [have a look at `list_transcripts()`](#list-available-transcripts)
         
@@ -69,14 +70,22 @@
         
         ```python
         YouTubeTranscriptApi.get_transcripts(video_ids, languages=['de', 'en'])
         ```
         
         `languages` also is optional here.
         
+        ### Preserve formatting
+        
+        You can also add `preserve_formatting=True` if you'd like to keep HTML formatting elements such as `<i>` (italics) and `<b>` (bold).
+        
+        ```python
+        YouTubeTranscriptApi.get_transcripts(video_ids, languages=['de', 'en'], preserve_formatting=True)
+        ```
+        
         ### List available transcripts
         
         If you want to list all transcripts which are available for a given video you can call:
         
         ```python
         transcript_list = YouTubeTranscriptApi.list_transcripts(video_id)
         ```
@@ -293,15 +302,15 @@
         
         ```python  
         from youtube_transcript_api import YouTubeTranscriptApi  
         
         YouTubeTranscriptApi.get_transcript(video_id, proxies={"https": "https://user:pass@domain:port"})
         ```  
         
-        As the `proxies` dict is passed on to the `requests.get(...)` call, it follows the [format used by the requests library](http://docs.python-requests.org/en/master/user/advanced/#proxies).  
+        As the `proxies` dict is passed on to the `requests.get(...)` call, it follows the [format used by the requests library](https://requests.readthedocs.io/en/latest/user/advanced/#proxies).  
         
         Using the CLI:  
         
         ```  
         youtube_transcript_api <first_video_id> <second_video_id> --https-proxy https://user:pass@domain:port
         ```
```

### Comparing `youtube_transcript_api-0.5.0/youtube_transcript_api.egg-info/SOURCES.txt` & `youtube_transcript_api-0.6.0/youtube_transcript_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

