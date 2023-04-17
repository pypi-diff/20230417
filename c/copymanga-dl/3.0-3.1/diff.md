# Comparing `tmp/copymanga_dl-3.0.tar.gz` & `tmp/copymanga_dl-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copymanga_dl-3.0.tar", max compression
+gzip compressed data, was "copymanga_dl-3.1.tar", max compression
```

## Comparing `copymanga_dl-3.0.tar` & `copymanga_dl-3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1328 2023-03-31 15:21:27.501723 copymanga_dl-3.0/Image_stitching.py
--rw-r--r--   0        0        0    35149 2023-03-31 15:21:27.501957 copymanga_dl-3.0/LICENSE
--rw-r--r--   0        0        0    12649 2023-03-31 15:21:27.502206 copymanga_dl-3.0/README.md
--rw-r--r--   0        0        0    28426 2023-03-31 15:21:27.502637 copymanga_dl-3.0/main.py
--rw-r--r--   0        0        0      977 2023-03-31 15:21:27.502713 copymanga_dl-3.0/pyproject.toml
--rw-r--r--   0        0        0    13669 1970-01-01 00:00:00.000000 copymanga_dl-3.0/PKG-INFO
+-rw-r--r--   0        0        0     1328 2023-04-14 02:44:01.000000 copymanga_dl-3.1/Image_stitching.py
+-rw-r--r--   0        0        0    35149 2023-04-14 02:44:01.000000 copymanga_dl-3.1/LICENSE
+-rw-r--r--   0        0        0    12983 2023-04-14 02:44:01.000000 copymanga_dl-3.1/README.md
+-rw-r--r--   0        0        0    30446 2023-04-14 02:44:01.000000 copymanga_dl-3.1/main.py
+-rw-r--r--   0        0        0      958 2023-04-14 02:44:01.000000 copymanga_dl-3.1/pyproject.toml
+-rw-r--r--   0        0        0    13971 1970-01-01 00:00:00.000000 copymanga_dl-3.1/PKG-INFO
```

### Comparing `copymanga_dl-3.0/Image_stitching.py` & `copymanga_dl-3.1/Image_stitching.py`

 * *Files identical despite different names*

### Comparing `copymanga_dl-3.0/LICENSE` & `copymanga_dl-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `copymanga_dl-3.0/README.md` & `copymanga_dl-3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 **请注意，在提交ISSUE前，请确保@misaka10843，以防止长时间未查看！**
 
+**因为尽可能缓解copymanga服务器压力，此程序限制了每分钟只能访问15次API，还请理解！**
+
 # copymanga-downloader
 
 ![Head diagram](https://s2.loli.net/2022/03/30/b4eM9gArp5q2VKu.png)
 
 ## 前言💭
 
 推荐在模拟器/WSA/安卓手机中安装[tachiyomi](https://github.com/tachiyomiorg/tachiyomi)，与[Copymanga插件](https://github.com/stevenyomi/copymanga)，并使用tachiyomi下载！
@@ -27,18 +29,14 @@
 
 or
 
 `git clone https://github.com/misaka10843/copymanga-downloader.git && cd copymanga-downloader && python setup.py install`
 
 `git clone https://github.com/misaka10843/copymanga-downloader.git && cd copymanga-downloader && pip install -r requirements.txt && python main.py`
 
-## README 语言🌐
-
-**简体中文**|[English](https://github.com/misaka10843/copymanga-downloader/blob/master/README-EN.md)
-
 ## 声明 📢
 
 我们制作此工具是纯粹因为PC端无法下载漫画，我们并不希望个人用户一直依靠此工具并且长时间/多文件下载来增加服务器负担
 
 在使用此工具时理应是小范围/短时间下载，而不是大范围/长时间下载，如果因此出现了问题我们是不会受理的
 
 **请尽量使用官方网站！**
@@ -51,14 +49,19 @@
 
 discord `misaka10843#2282`（早上，中午以及下午5-6点）
 
 QQ `3594254539`（不常工作时间上线）
 
 因为copymanga为简体/繁体中文的漫画网站，所以此程序预计不会添加其他语言，还请谅解
 
+为了尽可能的防止对服务器增加过大负担，我们将API请求限制为15次每分钟，还请谅解！（因为将API请求的时间与次数保存在设置中，您就算重新打开程序都会被限制的！）
+
+![image](https://user-images.githubusercontent.com/69132853/229278511-3b2fe97b-5e01-4df0-9a23-d276de440472.png)
+
+
 ## 技术栈 ⚒️
 
 ![python](https://img.shields.io/badge/Python-3.0+-326c9c?style=for-the-badge&logo=Python&logoColor=326c9c)
 
 ## Thanks 🎁
 
 * [KILLER2017](https://github.com/KILLER2017)(优化下载阅读体验)
```

### Comparing `copymanga_dl-3.0/main.py` & `copymanga_dl-3.1/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import argparse
+import csv
 import datetime
 import json
 import os
+import sys
 import threading
 import time
 
 import retrying as retrying
 from rich import print as print
 from rich.console import Console
 from rich.prompt import Prompt, Confirm, IntPrompt
@@ -120,18 +122,19 @@
 # 正常模式
 
 def welcome():
     choice_manga_path_word = None
     want_to = int(Prompt.ask("您是想搜索还是查看您的收藏？[italic yellow](0:导出收藏,1:搜索,2:收藏,3:添加半自动更新)[/]",
                              choices=["0", "1", "2", "3"], default="1"))
     if want_to == 0:
-        print()
+        collect_expect()
+        return
     if want_to == 3:
         updates()
-        exit()
+        return
     if want_to == 1:
         choice_manga_path_word = search()
     if want_to == 2:
         choice_manga_path_word = search_on_collect()
     manga_group_path_word = manga_group(choice_manga_path_word)
     manga_chapter_json = manga_chapter(choice_manga_path_word, manga_group_path_word)
     chapter_allocation(manga_chapter_json)
@@ -275,15 +278,15 @@
             return
 
 
 def update_download():
     load_settings()
     if not load_updates():
         print("[bold red]update.json并没有内容，请使用正常模式添加！[/]")
-        exit()
+        sys.exit()
     for comic in UPDATE_LIST:
         print(f"[yellow]正在准备下载{comic['manga_name']}[/]")
         manga_chapter_json = update_get_chapter(comic['manga_path_word'],
                                                 comic['manga_group_path_word'],
                                                 comic['now_chapter'])
         if manga_chapter_json != 0:
             chapter_allocation(manga_chapter_json)
@@ -307,15 +310,15 @@
     }
     # Todo 支持500+话的漫画(感觉并不太需要)
     if not manga_chapter_json['results']['list']:
         print(f"[bold blue]此漫画并未有新的章节，我们将跳过此漫画[/]")
         return 0
     if manga_chapter_json['results']['total'] > 500:
         print("[bold red]我们暂时不支持下载到500话以上，还请您去Github中创建Issue！[/]")
-        exit()
+        sys.exit()
     return return_json
 
 
 # 搜索相关
 
 def search():
     search_content = Prompt.ask("您需要搜索什么漫画呢")
@@ -383,15 +386,15 @@
         api_restriction()
         # 解析JSON数据
         data = response.json()
         if data['code'] == 401:
             settings_dir = os.path.join(os.path.expanduser("~"), ".copymanga-downloader/settings.json")
             print(f"[bold red]请求出现问题！疑似Token问题！[{data['message']}][/]")
             print(f"[bold red]请删除{settings_dir}来重新设置！(或者也可以自行修改配置文件)[/]")
-            exit()
+            sys.exit()
         console.rule(f"[bold blue]当前为第{current_page_count}页")
         # 输出每个comic的名称和对应的序号
         for i, comic in enumerate(data["results"]["list"]):
             print("[{}] {}".format(i + 1, comic['comic']["name"]))
 
         # 让用户输入数字来选择comic
         selection = Prompt.ask("请选择一个漫画[italic yellow]（输入Q退出,U为上一页,D为下一页）[/]")
@@ -421,14 +424,52 @@
                 else:
                     current_page_count += 1
             else:
                 # 处理输入错误的情况
                 print("[italic red]无效的选择！[/]")
 
 
+def collect_expect():
+    url = f"https://api.{SETTINGS['api_url']}/api/v3/member/collect/comics"
+    params = {
+        "limit": 12,
+        "offset": 0
+    }
+    data = []
+    want_to = int(Prompt.ask(f"请问是输出json格式还是csv格式？"
+                             f"[italic yellow](0:json,1:csv)[/]",
+                             choices=["0", "1"], default="1"))
+    while True:
+        API_HEADER['authorization'] = SETTINGS['authorization']
+        res = requests.get(url, params=params, headers=API_HEADER)
+        res_json = json.loads(res.text)
+        if res_json["code"] != 200:
+            print(f"[bold red]无法获取到相关信息，请检查相关设置。Error:{res_json['message']}")
+            return
+        for item in res_json['results']['list']:
+            comic = item['comic']
+            data.append([comic['name'], comic['path_word'], comic['datetime_updated'], comic['last_chapter_name']])
+
+        if len(data) >= res_json['results']['total']:
+            break
+        else:
+            params['offset'] += 12
+    if want_to == 0:
+        # 输出到test.json
+        with open('collect.json', 'w') as f:
+            json.dump(data, f, indent=4, ensure_ascii=False)
+        print("[green]已将您的收藏输出到运行目录下的collect.json中[/]")
+    else:
+        with open('collect.csv', 'w', newline='', encoding='utf-8') as f:
+            writer = csv.writer(f)
+            writer.writerow(['Name', 'Path Word', 'Update Time', 'Last Chapter'])
+            writer.writerows(data)
+        print("[green]已将您的收藏输出到运行目录下的collect.csv中[/]")
+
+
 # 漫画详细相关
 
 def manga_group(manga_path_word):
     response = requests.get(f"https://api.{SETTINGS['api_url']}/api/v3/comic2/{manga_path_word}",
                             headers=API_HEADER, proxies=PROXIES)
     # 记录API访问量
     api_restriction()
@@ -462,15 +503,15 @@
         "json": manga_chapter_json,
         "start": None,
         "end": None
     }
     # Todo 支持500+话的漫画(感觉并不太需要)
     if manga_chapter_json['results']['total'] > 500:
         print("[bold red]我们暂时不支持下载到500话以上，还请您去Github中创建Issue！[/]")
-        exit()
+        sys.exit()
     # 询问应该如何下载
     # 如果是命令行参数就直接返回对应
     if ARGS:
         return_json["start"] = int(ARGS.MangaStart) - 1
         return_json["end"] = int(ARGS.MangaEnd)
         return return_json
     want_to = int(Prompt.ask(f"获取到{manga_chapter_json['results']['total']}话内容，请问如何下载?"
@@ -519,15 +560,16 @@
         download_path = SETTINGS['download_path']
         chapter_name = manga_chapter_info_json['results']['chapter']['name']
         # 检查漫画文件夹是否存在
         if not os.path.exists(f"{download_path}/{manga_name}/"):
             os.mkdir(f"{download_path}/{manga_name}/")
         # 创建多线程
         threads = []
-        with console.status(f"[bold yellow]正在下载:[{manga_name}]{chapter_name}[/]"):
+        with console.status(f"[bold yellow]正在下载:[{manga_name}]{chapter_name}(索引ID:"
+                            f"{int(manga_chapter_info_json['results']['chapter']['index']) + 1})[/]"):
             for i in range(num_images):
                 url = img_url_contents[i]['url']
                 # 检查章节文件夹是否存在
                 if not os.path.exists(f"{download_path}/{manga_name}/{chapter_name}/"):
                     os.mkdir(f"{download_path}/{manga_name}/{chapter_name}/")
                 # 组成下载路径
                 filename = f"{download_path}/{manga_name}/{chapter_name}/{str(img_words[i] + 1).zfill(3)}.jpg"
@@ -541,29 +583,29 @@
                         time.sleep(0.5)
                         t.start()
                     for t in threads:
                         time.sleep(0.5)
                         t.join()
                     threads.clear()
         # 实施添加下载进度
-        if ARGS.subscribe == "1":
+        if ARGS and ARGS.subscribe == "1":
             save_new_update(manga_chapter_info_json['results']['chapter']['comic_path_word'],
                             manga_chapter_info_json['results']['chapter']['index'] + 1)
 
-        print(f"[bold green][:white_check_mark: ][{manga_name}]{chapter_name}下载完成！[/]")
+        print(f"[bold green][:white_check_mark:][{manga_name}]{chapter_name}下载完成！[/]")
 
 
 # API限制相关
 
 def api_restriction():
     global API_COUNTER
     API_COUNTER += 1
     # 防止退出后立马再次运行
     current_time = OG_SETTINGS['api_time']
-    time_diff = current_time - time.time()
+    time_diff = time.time() - current_time
     # 判断是否超过60秒
     if time_diff < 60 and API_COUNTER <= 1:
         API_COUNTER = API_COUNTER + OG_SETTINGS['API_COUNTER']
     if API_COUNTER >= 15:
         API_COUNTER = 0
         print("[bold yellow]您已经触发到了API请求阈值，我们将等60秒后再进行[/]")
         time.sleep(60)
@@ -588,47 +630,54 @@
         print(f"[blue]您已经下载了{filename}，跳过下载[/]")
         return
     try:
         response = requests.get(url, headers=API_HEADER, proxies=PROXIES)
         with open(filename, "wb") as f:
             f.write(response.content)
     except:
-        print(f"[bold red]无法下载{filename}，似乎是CopyManga暂时屏蔽了您的IP，请稍后重试或检查网络连接[/]")
+        print(
+            f"[bold red]无法下载{filename}，似乎是CopyManga暂时屏蔽了您的IP，请稍后手动下载对应章节(章节话数为每话下载输出的索引ID)[/]")
 
 
 # 设置相关
 
 def get_org_url():
     print("[italic yellow]正在获取CopyManga网站Url...[/]")
     url = "https://cdn.jsdelivr.net/gh/misaka10843/copymanga-downloader@master/url.json"
     try:
-        response = requests.get(url)
+        response = requests.get(url,proxies=PROXIES)
         response.raise_for_status()
         return response.json()
     except:
         print("[bold yellow]无法链接至jsdelivr，准备直接访问Github[/]")
         # 更换URL
         url = "https://raw.githubusercontent.com/misaka10843/copymanga-downloader/master/url.json"
         try:
-            response = requests.get(url)
+            response = requests.get(url,proxies=PROXIES)
             response.raise_for_status()
             return response.json()
         except:
             print("[bold red]无法链接至GitHub，请检查网络连接[/]", )
-            exit()
+            sys.exit()
 
 
 def set_settings():
+    global PROXIES
     # 获取用户输入
     download_path = Prompt.ask("请输入保存路径")
     authorization = Prompt.ask("请输入账号Token")
     use_oversea_cdn_input = Confirm.ask("是否使用海外CDN？", default=False)
     use_webp_input = Confirm.ask("是否使用Webp？[italic yellow](可以节省服务器资源,下载速度也会加快)[/]",
                                  default=True)
     proxy = Prompt.ask("请输入代理地址[italic yellow](没有的话可以直接回车跳过)[/]")
+    if proxy:
+        PROXIES = {
+            "http": proxy,
+            "https": proxy
+        }
     api_urls = get_org_url()
     for i, url in enumerate(api_urls):
         print(f"{i + 1}->{url}")
     choice = IntPrompt.ask("请输入要使用的API前面的数字")
 
     # input转bool
     use_oversea_cdn = "0"
@@ -698,19 +747,19 @@
         set_settings()
     parse_args()
     if ARGS:
         if ARGS.subscribe == "1":
             print(
                 "[bold purple]请注意！此模式下可能会导致部分img下载失败，如果遇见报错还请您自行删除更新列表然后重新添加后运行，此程序会重新下载并跳过已下载内容[/]")
             update_download()
-            exit()
+            sys.exit()
         if ARGS.MangaPath and ARGS.MangaEnd and ARGS.MangaStart:
             command_mode()
             # 防止运行完成后又触发正常模式
-            exit()
+            sys.exit()
         else:
             print("[bold red]命令行参数中缺少必要字段,将切换到普通模式[/]")
             ARGS = None
     welcome()
 
 
 if __name__ == '__main__':
```

### Comparing `copymanga_dl-3.0/pyproject.toml` & `copymanga_dl-3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copymanga-dl"
-version = "3.0"
+version = "3.1"
 description = "Copymanga Downloader"
 license = "GPL-3.0-or-later"
 authors = ["misaka10843 <misaka10843@outlook.jp>"]
 readme = "README.md"
 homepage = "https://misaka.sakurakoi.top/"
 repository = "https://github.com/misaka10843/copymanga-downloader"
 documentation = ""
@@ -23,15 +23,14 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 requests = ">=2.28.2"
 retrying = ">=1.3.4"
 rich = ">=13.3.2"
-pillow = ">=9.4.0"
 
 [tool.poetry.scripts]
 copymanga-dl = 'main:main'
 image-merge = 'Image_stitching:main'
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `copymanga_dl-3.0/PKG-INFO` & `copymanga_dl-3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copymanga-dl
-Version: 3.0
+Version: 3.1
 Summary: Copymanga Downloader
 Home-page: https://misaka.sakurakoi.top/
 License: GPL-3.0-or-later
 Keywords: copymanga,downloader
 Author: misaka10843
 Author-email: misaka10843@outlook.jp
 Requires-Python: >=3.10,<4
@@ -14,23 +14,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Utilities
-Requires-Dist: pillow (>=9.4.0)
 Requires-Dist: requests (>=2.28.2)
 Requires-Dist: retrying (>=1.3.4)
 Requires-Dist: rich (>=13.3.2)
 Project-URL: Repository, https://github.com/misaka10843/copymanga-downloader
 Description-Content-Type: text/markdown
 
 **请注意，在提交ISSUE前，请确保@misaka10843，以防止长时间未查看！**
 
+**因为尽可能缓解copymanga服务器压力，此程序限制了每分钟只能访问15次API，还请理解！**
+
 # copymanga-downloader
 
 ![Head diagram](https://s2.loli.net/2022/03/30/b4eM9gArp5q2VKu.png)
 
 ## 前言💭
 
 推荐在模拟器/WSA/安卓手机中安装[tachiyomi](https://github.com/tachiyomiorg/tachiyomi)，与[Copymanga插件](https://github.com/stevenyomi/copymanga)，并使用tachiyomi下载！
@@ -54,18 +55,14 @@
 
 or
 
 `git clone https://github.com/misaka10843/copymanga-downloader.git && cd copymanga-downloader && python setup.py install`
 
 `git clone https://github.com/misaka10843/copymanga-downloader.git && cd copymanga-downloader && pip install -r requirements.txt && python main.py`
 
-## README 语言🌐
-
-**简体中文**|[English](https://github.com/misaka10843/copymanga-downloader/blob/master/README-EN.md)
-
 ## 声明 📢
 
 我们制作此工具是纯粹因为PC端无法下载漫画，我们并不希望个人用户一直依靠此工具并且长时间/多文件下载来增加服务器负担
 
 在使用此工具时理应是小范围/短时间下载，而不是大范围/长时间下载，如果因此出现了问题我们是不会受理的
 
 **请尽量使用官方网站！**
@@ -78,14 +75,19 @@
 
 discord `misaka10843#2282`（早上，中午以及下午5-6点）
 
 QQ `3594254539`（不常工作时间上线）
 
 因为copymanga为简体/繁体中文的漫画网站，所以此程序预计不会添加其他语言，还请谅解
 
+为了尽可能的防止对服务器增加过大负担，我们将API请求限制为15次每分钟，还请谅解！（因为将API请求的时间与次数保存在设置中，您就算重新打开程序都会被限制的！）
+
+![image](https://user-images.githubusercontent.com/69132853/229278511-3b2fe97b-5e01-4df0-9a23-d276de440472.png)
+
+
 ## 技术栈 ⚒️
 
 ![python](https://img.shields.io/badge/Python-3.0+-326c9c?style=for-the-badge&logo=Python&logoColor=326c9c)
 
 ## Thanks 🎁
 
 * [KILLER2017](https://github.com/KILLER2017)(优化下载阅读体验)
```

