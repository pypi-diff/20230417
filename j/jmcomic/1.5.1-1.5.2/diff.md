# Comparing `tmp/jmcomic-1.5.1.tar.gz` & `tmp/jmcomic-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-hn88r5vv/jmcomic-1.5.1.tar", last modified: Fri Apr  7 10:21:21 2023, max compression
+gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-xgyf_ajn/jmcomic-1.5.2.tar", last modified: Mon Apr 17 12:24:02 2023, max compression
```

## Comparing `jmcomic-1.5.1.tar` & `jmcomic-1.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:21:21.000000 jmcomic-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-07 10:21:12.000000 jmcomic-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-07 10:21:21.000000 jmcomic-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-07 10:21:12.000000 jmcomic-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 10:21:21.000000 jmcomic-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-07 10:21:12.000000 jmcomic-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:21:21.000000 jmcomic-1.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:21:21.000000 jmcomic-1.5.1/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-07 10:21:12.000000 jmcomic-1.5.1/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-07 10:21:12.000000 jmcomic-1.5.1/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-04-07 10:21:12.000000 jmcomic-1.5.1/src/jmcomic/jm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-07 10:21:12.000000 jmcomic-1.5.1/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-04-07 10:21:12.000000 jmcomic-1.5.1/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-04-07 10:21:12.000000 jmcomic-1.5.1/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-04-07 10:21:12.000000 jmcomic-1.5.1/src/jmcomic/jm_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-04-07 10:21:12.000000 jmcomic-1.5.1/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:21:21.000000 jmcomic-1.5.1/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-07 10:21:21.000000 jmcomic-1.5.1/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-07 10:21:21.000000 jmcomic-1.5.1/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 10:21:21.000000 jmcomic-1.5.1/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-07 10:21:21.000000 jmcomic-1.5.1/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 10:21:21.000000 jmcomic-1.5.1/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:24:02.000000 jmcomic-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 12:23:53.000000 jmcomic-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-17 12:24:02.000000 jmcomic-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-17 12:23:53.000000 jmcomic-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 12:24:02.000000 jmcomic-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-17 12:23:53.000000 jmcomic-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/jm_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/jm_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-1.5.1/LICENSE` & `jmcomic-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-1.5.1/PKG-INFO` & `jmcomic-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-1.5.1/README.md` & `jmcomic-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-1.5.1/setup.py` & `jmcomic-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.5.1/src/jmcomic/api.py` & `jmcomic-1.5.2/src/jmcomic/api.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.5.1/src/jmcomic/jm_client.py` & `jmcomic-1.5.2/src/jmcomic/jm_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,44 +138,48 @@
                                  f"响应状态码为{resp.status_code}，"
                                  f"URL=[{resp.url}]，"
                                  +
                                  (f"响应文本=[{resp.text}]" if len(resp.text) < 50 else
                                   f'响应文本过长(len={len(resp.text)})，不打印')
                                  )
 
-        if is_api is True and resp.text.strip() == JmModuleConfig.JM_SERVER_ERROR_HTML:
-            raise AssertionError("【JM异常】Could not connect to mysql! Please check your database settings!")
+        if is_api is True:
+            JmModuleConfig.check_html(resp.text.strip(), url)
 
         return resp
 
     # -- 类方法 --
 
     @classmethod
     def is_empty_image(cls, resp):
         return resp.status_code != 200 or len(resp.content) == 0
 
     @classmethod
     def img_is_not_need_to_decode(cls, data_original: str, _resp):
         return data_original.endswith('.gif')
 
     # noinspection PyAttributeOutsideInit
-    def enable_cache(self):
+    def enable_cache(self, debug=False):
         def wrap_func_cache(func_name, cache_dict_name):
             if hasattr(self, cache_dict_name):
                 return
 
             cache_dict = {}
             setattr(self, cache_dict_name, cache_dict)
 
             # 重载本对象的方法
             func = getattr(self, func_name)
+
+            cache_hit_msg = f'【缓存命中】{cache_dict_name} ' + '→ [{}]' if debug is True else None
+            cache_miss_msg = f'【缓存缺失】{cache_dict_name} ' + '← [{}]' if debug is True else None
+
             wrap_func = enable_cache(
                 cache_dict=cache_dict,
-                cache_hit_msg=f'命中 {cache_dict_name} ' + '→ [{}]]',
-                cache_miss_msg=f'缺失 {cache_dict_name} ' + '← [{}]',
+                cache_hit_msg=cache_hit_msg,
+                cache_miss_msg=cache_miss_msg,
             )(func)
 
             setattr(self, func_name, wrap_func)
 
         wrap_func_cache('get_photo_detail', 'album_cache_dict')
         wrap_func_cache('get_album_detail', 'photo_cache_dict')
```

### Comparing `jmcomic-1.5.1/src/jmcomic/jm_config.py` & `jmcomic-1.5.2/src/jmcomic/jm_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 class JmModuleConfig:
     # 网站相关
     PROT = "https://"
     _DOMAIN = None
     JM_REDIRECT_URL = f'{PROT}jm365.xyz/3YeBdF'  # 永久網域，怕走失的小伙伴收藏起来
     JM_PUB_URL = f'{PROT}jmcomic1.bet'
     JM_CDN_IMAGE_URL_TEMPLATE = PROT + 'cdn-msp.{domain}/media/photos/{photo_id}/{index:05}{suffix}'  # index 从1开始
-    JM_SERVER_ERROR_HTML = "Could not connect to mysql! Please check your database settings!"
     JM_IMAGE_SUFFIX = ['.jpg', '.webp', '.png', '.gif']
 
+    # 访问JM可能会遇到的异常网页
+    JM_ERROR_RESPONSE_HTML = {
+        "Could not connect to mysql! Please check your database settings!": "禁漫服务器内部报错",
+        "Restricted Access!": "禁漫拒绝你所在ip地区的访问，你可以选择: 换域名/换代理",
+    }
+
     # 图片分隔相关
     SCRAMBLE_0 = 220980
     SCRAMBLE_10 = 268850
     SCRAMBLE_NUM_8 = 421926  # 2023-02-08后改了图片切割算法
 
     # 下载时的一些默认值
     default_author = 'default-author'
@@ -69,20 +74,27 @@
     @classmethod
     def get_jmcomic_url(cls, postman=None):
         """
         访问禁漫的永久网域，从而得到一个可用的禁漫网址，
         """
         if postman is None:
             from common import Postmans
-            postman = Postmans.get_impl_clazz('cffi') \
+            postman = Postmans \
+                .get_impl_clazz('cffi') \
                 .create(headers=cls.headers(cls.JM_REDIRECT_URL))
 
-        domain = postman.with_wrap_resp() \
-            .get(cls.JM_REDIRECT_URL, allow_redirects=False) \
-            .redirect_url
-
-        cls.jm_debug('获取禁漫地址', f'获取成功，最新可用的禁漫地址: {domain}')
+        domain = postman.with_redirect_catching().get(cls.JM_REDIRECT_URL)
+        cls.jm_debug('获取禁漫地址', f'[{cls.JM_REDIRECT_URL}] → [{domain}]')
         return domain
 
+    @classmethod
+    def check_html(cls, html: str, url=None):
+        html = html.strip()
+        error_msg = cls.JM_ERROR_RESPONSE_HTML.get(html, None)
+        if error_msg is None:
+            return
+
+        raise AssertionError(f'{error_msg}' + f': {url}' if url is not None else '')
+
 
 jm_debug = JmModuleConfig.jm_debug
 disable_jm_debug = JmModuleConfig.disable_jm_debug
```

### Comparing `jmcomic-1.5.1/src/jmcomic/jm_entity.py` & `jmcomic-1.5.2/src/jmcomic/jm_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,15 +235,15 @@
 
         photo_detail = JmPhotoDetail(
             photo_id=photo_id,
             scramble_id=self.scramble_id,
             title=photo_title,
             keywords='',
             series_id=self.album_id,
-            sort=index + 1,
+            sort=episode_info[1] if len(self) != 1 else 1,
             author=self.author,
             from_album=self,
             page_arr=None,
             data_original_domain=None
         )
 
         return photo_detail, episode_info
```

### Comparing `jmcomic-1.5.1/src/jmcomic/jm_option.py` & `jmcomic-1.5.2/src/jmcomic/jm_option.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.5.1/src/jmcomic/jm_service.py` & `jmcomic-1.5.2/src/jmcomic/jm_service.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.5.1/src/jmcomic/jm_toolkit.py` & `jmcomic-1.5.2/src/jmcomic/jm_toolkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
                                               '<[\s\S]*?>(\d+-\d+-\d+).*?')
     pattern_html_album_page_count = compile('<span class="pagecount">.*?:(\d+)</span>')
     pattern_html_album_pub_date = compile('>上架日期 : (.*?)</span>')
     pattern_html_album_update_date = compile('>更新日期 : (.*?)</span>')
 
     # album 作者
     pattern_html_album_author_list = [
-        compile('作者： <span itemprop="author" data-type="author">(\s*<a.*?>(.*?)</a>)*\s*</span>'),
-        compile("<a.*?>(.*?)</a>"),
+        compile('作者： *<span itemprop="author" data-type="author">([\s\S]*?)</span>'),
+        compile("<a[\s\S]*?>(.*?)</a>"),
     ]
 
     @classmethod
     def parse_to_jm_domain(cls, text: str):
         if text.startswith("https"):
             return cls.pattern_jm_domain.search(text)[1]
 
@@ -123,15 +123,16 @@
                 continue
 
             # 获取字段名和值
             field_name = pattern_name[pattern_name.index(cls_field_prefix) + len(cls_field_prefix):]
             field_value = match_field(field_name, pattern_value, html)
 
             if field_value is None:
-                raise AssertionError(f"文本没有匹配上字段：字段名为{field_name}，pattern为cls.{pattern_name}")
+                write_text('./resp.txt', html)  # debug
+                raise AssertionError(f"文本没有匹配上字段：字段名为'{field_name}'，pattern: [{pattern_value.pattern}]")
 
             # 保存字段
             field_dict[field_name] = field_value
 
         return clazz(**field_dict)
```

### Comparing `jmcomic-1.5.1/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-1.5.2/src/jmcomic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

