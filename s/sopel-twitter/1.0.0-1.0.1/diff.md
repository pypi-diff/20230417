# Comparing `tmp/sopel-twitter-1.0.0.tar.gz` & `tmp/sopel-twitter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel-twitter-1.0.0.tar", last modified: Fri Apr 14 21:44:04 2023, max compression
+gzip compressed data, was "sopel-twitter-1.0.1.tar", last modified: Sun Apr 16 22:04:31 2023, max compression
```

## Comparing `sopel-twitter-1.0.0.tar` & `sopel-twitter-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-14 21:44:04.486434 sopel-twitter-1.0.0/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2022-03-02 18:17:04.000000 sopel-twitter-1.0.0/COPYING
--rw-r--r--   0 dgw       (1000) dgw       (1000)      161 2022-03-02 18:17:04.000000 sopel-twitter-1.0.0/MANIFEST.in
--rw-r--r--   0 dgw       (1000) dgw       (1000)     2349 2023-04-14 21:42:23.000000 sopel-twitter-1.0.0/NEWS
--rw-r--r--   0 dgw       (1000) dgw       (1000)     5494 2023-04-14 21:44:04.486434 sopel-twitter-1.0.0/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1298 2023-04-14 21:29:33.000000 sopel-twitter-1.0.0/README.md
--rw-r--r--   0 dgw       (1000) dgw       (1000)        0 2022-03-02 18:17:04.000000 sopel-twitter-1.0.0/dev-requirements.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)      699 2023-04-14 21:44:04.493443 sopel-twitter-1.0.0/setup.cfg
--rwxr-xr-x   0 dgw       (1000) dgw       (1000)      889 2023-04-14 21:20:24.000000 sopel-twitter-1.0.0/setup.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-14 21:44:04.460435 sopel-twitter-1.0.0/sopel_twitter/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     8644 2023-04-14 21:29:33.000000 sopel-twitter-1.0.0/sopel_twitter/__init__.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-14 21:44:04.483440 sopel-twitter-1.0.0/sopel_twitter.egg-info/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     5494 2023-04-14 21:44:04.000000 sopel-twitter-1.0.0/sopel_twitter.egg-info/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)      400 2023-04-14 21:44:04.000000 sopel-twitter-1.0.0/sopel_twitter.egg-info/SOURCES.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-04-14 21:44:04.000000 sopel-twitter-1.0.0/sopel_twitter.egg-info/dependency_links.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       41 2023-04-14 21:44:04.000000 sopel-twitter-1.0.0/sopel_twitter.egg-info/entry_points.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-02-03 12:15:47.000000 sopel-twitter-1.0.0/sopel_twitter.egg-info/not-zip-safe
--rw-r--r--   0 dgw       (1000) dgw       (1000)       36 2023-04-14 21:44:04.000000 sopel-twitter-1.0.0/sopel_twitter.egg-info/requires.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       20 2023-04-14 21:44:04.000000 sopel-twitter-1.0.0/sopel_twitter.egg-info/top_level.txt
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-14 21:44:04.485436 sopel-twitter-1.0.0/tests/
--rw-r--r--   0 dgw       (1000) dgw       (1000)       15 2022-03-02 18:17:04.000000 sopel-twitter-1.0.0/tests/__init__.py
--rw-r--r--   0 dgw       (1000) dgw       (1000)      296 2022-03-02 18:17:04.000000 sopel-twitter-1.0.0/tests/test_twitter.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-16 22:04:31.338235 sopel-twitter-1.0.1/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2022-03-02 18:17:04.000000 sopel-twitter-1.0.1/COPYING
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      161 2023-04-15 06:53:37.000000 sopel-twitter-1.0.1/MANIFEST.in
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     2492 2023-04-16 22:03:50.000000 sopel-twitter-1.0.1/NEWS
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     5693 2023-04-16 22:04:31.339315 sopel-twitter-1.0.1/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     1298 2023-04-15 06:53:37.000000 sopel-twitter-1.0.1/README.md
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        0 2023-04-15 06:53:37.000000 sopel-twitter-1.0.1/dev-requirements.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      699 2023-04-16 22:04:31.346241 sopel-twitter-1.0.1/setup.cfg
+-rwxr-xr-x   0 dgw       (1000) dgw       (1000)      889 2023-04-15 06:53:37.000000 sopel-twitter-1.0.1/setup.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-16 22:04:31.209991 sopel-twitter-1.0.1/sopel_twitter/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     8588 2023-04-16 22:00:49.000000 sopel-twitter-1.0.1/sopel_twitter/__init__.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-16 22:04:31.317003 sopel-twitter-1.0.1/sopel_twitter.egg-info/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     5693 2023-04-16 22:04:30.000000 sopel-twitter-1.0.1/sopel_twitter.egg-info/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      400 2023-04-16 22:04:30.000000 sopel-twitter-1.0.1/sopel_twitter.egg-info/SOURCES.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-04-16 22:04:30.000000 sopel-twitter-1.0.1/sopel_twitter.egg-info/dependency_links.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       41 2023-04-16 22:04:30.000000 sopel-twitter-1.0.1/sopel_twitter.egg-info/entry_points.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-04-15 21:13:31.000000 sopel-twitter-1.0.1/sopel_twitter.egg-info/not-zip-safe
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       36 2023-04-16 22:04:30.000000 sopel-twitter-1.0.1/sopel_twitter.egg-info/requires.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       20 2023-04-16 22:04:30.000000 sopel-twitter-1.0.1/sopel_twitter.egg-info/top_level.txt
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-16 22:04:31.337082 sopel-twitter-1.0.1/tests/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       15 2023-04-15 06:53:37.000000 sopel-twitter-1.0.1/tests/__init__.py
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      296 2023-04-15 06:53:37.000000 sopel-twitter-1.0.1/tests/test_twitter.py
```

### Comparing `sopel-twitter-1.0.0/COPYING` & `sopel-twitter-1.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `sopel-twitter-1.0.0/NEWS` & `sopel-twitter-1.0.1/NEWS`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Changes between 1.0.0 and 1.0.1
+===============================
+
+Fixed:
+* Don't cache Tweety object; it stops working after some hours (#43)
+
+
 Changes between 0.4.1 and 1.0.0
 ===============================
 
 **Important: Package name is now `sopel-twitter`**
 
 Added:
 * Option to specify additional domains that can be treated as Twitter links (#34, #37)
```

### Comparing `sopel-twitter-1.0.0/PKG-INFO` & `sopel-twitter-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-twitter
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Twitter plugin for Sopel
 Home-page: https://github.com/sopel-irc/sopel-twitter
 Author: dgw
 Author-email: dgw@technobabbl.es
 License: Eiffel Forum License, version 2
 Description: # sopel-twitter
         
@@ -53,14 +53,21 @@
         < Wiz> .twitinfo NASA
         < Sopel> [Twitter] NASA (@NASA) ✔️ | Pale Blue Dot | http://www.nasa.gov/
                  | 204 friends, 46,602,251 followers | 65,377 tweets, 13,040 ♥s
                  | Joined: 2007-12-19 - 20:20:32UTC | There's space for everybody. ✨
         ```
         
         
+        Changes between 1.0.0 and 1.0.1
+        ===============================
+        
+        Fixed:
+        * Don't cache Tweety object; it stops working after some hours (#43)
+        
+        
         Changes between 0.4.1 and 1.0.0
         ===============================
         
         **Important: Package name is now `sopel-twitter`**
         
         Added:
         * Option to specify additional domains that can be treated as Twitter links (#34, #37)
```

### Comparing `sopel-twitter-1.0.0/README.md` & `sopel-twitter-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sopel-twitter-1.0.0/setup.cfg` & `sopel-twitter-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sopel-twitter
-version = 1.0.0
+version = 1.0.1
 description = A Twitter plugin for Sopel
 author = dgw
 author_email = dgw@technobabbl.es
 url = https://github.com/sopel-irc/sopel-twitter
 license = Eiffel Forum License, version 2
 classifiers = 
 	Intended Audience :: Developers
```

### Comparing `sopel-twitter-1.0.0/setup.py` & `sopel-twitter-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `sopel-twitter-1.0.0/sopel_twitter/__init__.py` & `sopel-twitter-1.0.1/sopel_twitter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     config.twitter.configure_setting(
         'show_quoted_tweets', 'When a tweet quotes another status, '
         'show the quoted tweet on a second IRC line?')
 
 
 def setup(bot):
     bot.config.define_section('twitter', TwitterSection)
-    bot.memory['tweety_app'] = Twitter()
 
 
 def get_preferred_media_item_link(item):
     """
     Guess the most useful link for a given piece of embedded media.
 
     :param item: a single Media object from Tweety
@@ -176,15 +175,15 @@
         return plugin.NOLIMIT
 
     output_user(bot, trigger, trigger.group(3))
 
 
 def output_status(bot, trigger, id_):
     try:
-        tweet = bot.memory['tweety_app'].tweet_detail(id_)
+        tweet = Twitter().tweet_detail(id_)
     except tweety_errors.InvalidTweetIdentifier:
         bot.say("Couldn't fetch that tweet. Most likely, it's either private or deleted.")
         return
     except (
         tweety_errors.GuestTokenNotFound,
         tweety_errors.ProxyParseError,
         tweety_errors.UnknownError,
```

### Comparing `sopel-twitter-1.0.0/sopel_twitter.egg-info/PKG-INFO` & `sopel-twitter-1.0.1/sopel_twitter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-twitter
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Twitter plugin for Sopel
 Home-page: https://github.com/sopel-irc/sopel-twitter
 Author: dgw
 Author-email: dgw@technobabbl.es
 License: Eiffel Forum License, version 2
 Description: # sopel-twitter
         
@@ -53,14 +53,21 @@
         < Wiz> .twitinfo NASA
         < Sopel> [Twitter] NASA (@NASA) ✔️ | Pale Blue Dot | http://www.nasa.gov/
                  | 204 friends, 46,602,251 followers | 65,377 tweets, 13,040 ♥s
                  | Joined: 2007-12-19 - 20:20:32UTC | There's space for everybody. ✨
         ```
         
         
+        Changes between 1.0.0 and 1.0.1
+        ===============================
+        
+        Fixed:
+        * Don't cache Tweety object; it stops working after some hours (#43)
+        
+        
         Changes between 0.4.1 and 1.0.0
         ===============================
         
         **Important: Package name is now `sopel-twitter`**
         
         Added:
         * Option to specify additional domains that can be treated as Twitter links (#34, #37)
```

