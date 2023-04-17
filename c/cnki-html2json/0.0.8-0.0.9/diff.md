# Comparing `tmp/cnki_html2json-0.0.8.tar.gz` & `tmp/cnki_html2json-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnki_html2json-0.0.8.tar", last modified: Sun Apr 16 17:02:06 2023, max compression
+gzip compressed data, was "cnki_html2json-0.0.9.tar", last modified: Mon Apr 17 04:20:21 2023, max compression
```

## Comparing `cnki_html2json-0.0.8.tar` & `cnki_html2json-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:02:06.493581 cnki_html2json-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-04-16 17:02:06.493581 cnki_html2json-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:02:06.489581 cnki_html2json-0.0.8/cnki_html2json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/cnki_html2json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/cnki_html2json/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/cnki_html2json/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/cnki_html2json/html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/cnki_html2json/parse_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/cnki_html2json/recognize_slider_coordinate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:02:06.489581 cnki_html2json-0.0.8/cnki_html2json.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-04-16 17:02:06.000000 cnki_html2json-0.0.8/cnki_html2json.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-16 17:02:06.000000 cnki_html2json-0.0.8/cnki_html2json.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:02:06.000000 cnki_html2json-0.0.8/cnki_html2json.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-16 17:02:06.000000 cnki_html2json-0.0.8/cnki_html2json.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 17:02:06.000000 cnki_html2json-0.0.8/cnki_html2json.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-16 17:02:06.000000 cnki_html2json-0.0.8/cnki_html2json.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 17:02:06.493581 cnki_html2json-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:02:06.489581 cnki_html2json-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/test/test_html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/test/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:20:21.541720 cnki_html2json-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-04-17 04:20:21.541720 cnki_html2json-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:20:21.537720 cnki_html2json-0.0.9/cnki_html2json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/cnki_html2json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/cnki_html2json/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/cnki_html2json/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/cnki_html2json/html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/cnki_html2json/parse_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/cnki_html2json/recognize_slider_coordinate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:20:21.541720 cnki_html2json-0.0.9/cnki_html2json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-04-17 04:20:21.000000 cnki_html2json-0.0.9/cnki_html2json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-17 04:20:21.000000 cnki_html2json-0.0.9/cnki_html2json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 04:20:21.000000 cnki_html2json-0.0.9/cnki_html2json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 04:20:21.000000 cnki_html2json-0.0.9/cnki_html2json.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 04:20:21.000000 cnki_html2json-0.0.9/cnki_html2json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 04:20:21.000000 cnki_html2json-0.0.9/cnki_html2json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 04:20:21.541720 cnki_html2json-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:20:21.541720 cnki_html2json-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/test/test_html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-17 04:20:10.000000 cnki_html2json-0.0.9/test/test_metadata.py
```

### Comparing `cnki_html2json-0.0.8/PKG-INFO` & `cnki_html2json-0.0.9/cnki_html2json.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cnki_html2json
-Version: 0.0.8
+Name: cnki-html2json
+Version: 0.0.9
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Programming Language :: Python :: 3
@@ -44,28 +44,28 @@
 - 确保你所在的网络环境能正常使用知网
 - 仅能提取 <b>期刊论文</b> 的文本，其他文献类型未做测试
 - 无法提取文献中的图片、公式等，因此提取的内容可能不完整
 - 本工具已经尽力覆盖大多数情况，但不能保证每一篇文献都能正常提取
 
 ## 快速开始
 
-本工具使用 Python 开发，请确保你的电脑上已经安装了 `Python3.8` 或以上版本。
+本工具使用 Python 开发，请确保你的电脑上已经安装了 `Python3.8` 或以上版本。如果使用爬虫，需要提前配置好对应浏览器的驱动，例如chrome的驱动为 [chromedriver](https://chromedriver.chromium.org/downloads)
 
 ```console
 $ python3 -m pip install cnki_html2json
 ```
 
 ## 使用方法
 
 1、调用 `html2json` 函数
 
 ```python
 from cnki_html2json import html2json
 with open('paper.html', 'r', encoding='utf-8') as f:
-	html = f.read()
+    html = f.read()
 print(html2json.extract(html, mode='structure'))
 ```
 `html2json` 参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
 | `paper_html` | 一篇期刊论文的html字符串 |
@@ -77,42 +77,42 @@
 
 2、使用命令行工具，启动一个selenium爬虫，然后在弹出的浏览器窗口(默认为Chrome)中进行检索
 ```console
 $ 无需设置任何参数，直接运行
 $ cnki-crawler
 ```
 ```console
-$ 设置论文提取的起始索引和终止索引，模式设置为structure
-$ cnki-crawler -s 1 -e 100 -m structure
+$ 设置论文提取的起始索引和终止索引，模式设置为structure，不记录日志
+$ cnki-crawler -s 1 -e 100 -m structure -l false
 $ 或者是
-$ cnki-crawler --start_paper_index 1 --end_paper_index 100 -mode structure
+$ cnki-crawler --start_paper_index 1 --end_paper_index 100 -mode structure --log false
 ```
 ```console
 $ 查看可选参数
 $ cnki-crawler --help
 ```
 
 参数说明：
 | 简写参数 | 参数 | 说明 |
 | --- | --- | --- |
-| s | `start_paper_index` | 论文提取的起始索引，默认为1 |
-| e | `end_paper_index` | 论文提取的终止索引，默认为None，爬取到最后 |
-| m | `mode` | 模式，可选值为 `structure`, `plain`, `raw`，默认为 `structure` |
-| b | `browser` | 浏览器类型，Chrome(默认),可选 Edge, Firefox, 不支持Safari|
-| save | `save_path` | 下载文件的保存路径，默认为当前目录的data文件夹 |
-| wait | `wait_time` | 为检索预留的等待时间，默认120秒 |
+| s | `start_paper_index` | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
+| e | `end_paper_index` | 论文提取的终止索引，默认为 `None`，爬取到最后 |
+| m | `mode` | 模式，可选值为 `structure`， `plain`， `raw`，默认为 `structure` |
+| b | `browser` | 浏览器类型，Chrome(默认),可选Edge， Firefox， 不支持Safari |
+| l | `log` | 是否记录日志，默认为 `true`，日志将保存在 `save_path` 下的 `log` 文件夹中 |
+| save | `save_path` | 下载文件的保存路径，默认为当前目录的 `data` 文件夹 |
+| wait | `wait_time` | 为检索预留的等待时间，默认 `120` 秒 |
 
-注：爬虫将自动保存日志到 `save_path` 的log文件夹中，如果不想保存日志，请传入参数 `--debug`
-> 提取结果可以参考examples文件夹中给出的样例。如果未指定保存路径，将下载结果默认保存在当前目录下的data文件夹下  
+> 提取结果可以参考examples文件夹中给出的样例。如果未指定保存路径，将下载结果默认保存在当前目录下的data文件夹下;  
 > 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (可以自动过滑块验证)
 
 ```python
-# 也可以在代码中调用爬虫
-from cnki_html2json.crawl import start_crawl:
-	start_crawl() # 默认参数
+# 也可以在代码中调用爬虫，可选参数参考上方的参数说明
+from cnki_html2json.crawl import start_crawl
+start_crawl(start_paper_index=1,end_paper_index=100,mode='structure',log='false')
 ```
 
 ## json文件字段说明
 
 | 一级字段 | 二级字段 |三级字段| 说明 |
 | --- | --- | --- | --- |
 | metadata | title |  |论文标题|
@@ -130,12 +130,12 @@
 |  | ...| ... ||
 | 参考文献 |  |  |参考文献|
 
 ## 工具推荐
 
 | 工具  | 描述 |
 | --- | --- |
-| [vermin](https://github.com/netromdk/vermin) | 从语法层面检测一个项目最低支持的 `python` 版本 |
+| [vermin](https://github.com/netromdk/vermin) | 从语法层面检测一个项目最低支持的 `Python` 版本 |
 
 ## 责任声明
 
 - 使用者使用本工具造成的一切后果，由使用者自行承担
```

### Comparing `cnki_html2json-0.0.8/README.md` & `cnki_html2json-0.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -22,28 +22,28 @@
 - 确保你所在的网络环境能正常使用知网
 - 仅能提取 <b>期刊论文</b> 的文本，其他文献类型未做测试
 - 无法提取文献中的图片、公式等，因此提取的内容可能不完整
 - 本工具已经尽力覆盖大多数情况，但不能保证每一篇文献都能正常提取
 
 ## 快速开始
 
-本工具使用 Python 开发，请确保你的电脑上已经安装了 `Python3.8` 或以上版本。
+本工具使用 Python 开发，请确保你的电脑上已经安装了 `Python3.8` 或以上版本。如果使用爬虫，需要提前配置好对应浏览器的驱动，例如chrome的驱动为 [chromedriver](https://chromedriver.chromium.org/downloads)
 
 ```console
 $ python3 -m pip install cnki_html2json
 ```
 
 ## 使用方法
 
 1、调用 `html2json` 函数
 
 ```python
 from cnki_html2json import html2json
 with open('paper.html', 'r', encoding='utf-8') as f:
-	html = f.read()
+    html = f.read()
 print(html2json.extract(html, mode='structure'))
 ```
 `html2json` 参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
 | `paper_html` | 一篇期刊论文的html字符串 |
@@ -55,42 +55,42 @@
 
 2、使用命令行工具，启动一个selenium爬虫，然后在弹出的浏览器窗口(默认为Chrome)中进行检索
 ```console
 $ 无需设置任何参数，直接运行
 $ cnki-crawler
 ```
 ```console
-$ 设置论文提取的起始索引和终止索引，模式设置为structure
-$ cnki-crawler -s 1 -e 100 -m structure
+$ 设置论文提取的起始索引和终止索引，模式设置为structure，不记录日志
+$ cnki-crawler -s 1 -e 100 -m structure -l false
 $ 或者是
-$ cnki-crawler --start_paper_index 1 --end_paper_index 100 -mode structure
+$ cnki-crawler --start_paper_index 1 --end_paper_index 100 -mode structure --log false
 ```
 ```console
 $ 查看可选参数
 $ cnki-crawler --help
 ```
 
 参数说明：
 | 简写参数 | 参数 | 说明 |
 | --- | --- | --- |
-| s | `start_paper_index` | 论文提取的起始索引，默认为1 |
-| e | `end_paper_index` | 论文提取的终止索引，默认为None，爬取到最后 |
-| m | `mode` | 模式，可选值为 `structure`, `plain`, `raw`，默认为 `structure` |
-| b | `browser` | 浏览器类型，Chrome(默认),可选 Edge, Firefox, 不支持Safari|
-| save | `save_path` | 下载文件的保存路径，默认为当前目录的data文件夹 |
-| wait | `wait_time` | 为检索预留的等待时间，默认120秒 |
+| s | `start_paper_index` | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
+| e | `end_paper_index` | 论文提取的终止索引，默认为 `None`，爬取到最后 |
+| m | `mode` | 模式，可选值为 `structure`， `plain`， `raw`，默认为 `structure` |
+| b | `browser` | 浏览器类型，Chrome(默认),可选Edge， Firefox， 不支持Safari |
+| l | `log` | 是否记录日志，默认为 `true`，日志将保存在 `save_path` 下的 `log` 文件夹中 |
+| save | `save_path` | 下载文件的保存路径，默认为当前目录的 `data` 文件夹 |
+| wait | `wait_time` | 为检索预留的等待时间，默认 `120` 秒 |
 
-注：爬虫将自动保存日志到 `save_path` 的log文件夹中，如果不想保存日志，请传入参数 `--debug`
-> 提取结果可以参考examples文件夹中给出的样例。如果未指定保存路径，将下载结果默认保存在当前目录下的data文件夹下  
+> 提取结果可以参考examples文件夹中给出的样例。如果未指定保存路径，将下载结果默认保存在当前目录下的data文件夹下;  
 > 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (可以自动过滑块验证)
 
 ```python
-# 也可以在代码中调用爬虫
-from cnki_html2json.crawl import start_crawl:
-	start_crawl() # 默认参数
+# 也可以在代码中调用爬虫，可选参数参考上方的参数说明
+from cnki_html2json.crawl import start_crawl
+start_crawl(start_paper_index=1,end_paper_index=100,mode='structure',log='false')
 ```
 
 ## json文件字段说明
 
 | 一级字段 | 二级字段 |三级字段| 说明 |
 | --- | --- | --- | --- |
 | metadata | title |  |论文标题|
@@ -108,12 +108,12 @@
 |  | ...| ... ||
 | 参考文献 |  |  |参考文献|
 
 ## 工具推荐
 
 | 工具  | 描述 |
 | --- | --- |
-| [vermin](https://github.com/netromdk/vermin) | 从语法层面检测一个项目最低支持的 `python` 版本 |
+| [vermin](https://github.com/netromdk/vermin) | 从语法层面检测一个项目最低支持的 `Python` 版本 |
 
 ## 责任声明
 
-- 使用者使用本工具造成的一切后果，由使用者自行承担
+- 使用者使用本工具造成的一切后果，由使用者自行承担
```

### Comparing `cnki_html2json-0.0.8/cnki_html2json/cli.py` & `cnki_html2json-0.0.9/cnki_html2json/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 
 def main():
     parser = argparse.ArgumentParser(description='CNKI crawler. Convert the html format of papers to json format.')
     parser.add_argument('-s','--start_paper_index',type=int,default=1,help='开始下载索引, 默认为1')
     parser.add_argument('-e','--end_paper_index',type=int,default=None,help='结束下载索引, 默认为None, 即下载到最后')
     parser.add_argument('-m','--mode',type=str,default='structure',help='模式: structure|plain|raw, 默认为structure')
     parser.add_argument('-b','--browser_type',type=str,default='Chrome',help='浏览器类型: Chrome(default)|Firefox|Edge')
+    parser.add_argument('-l','--log',type=str,default='true',help='是否保存日志, true(default)|false')
     parser.add_argument('-save','--save_path',type=str,default='data',help='文件保存路径, 默认为当前目录的data文件夹')
     parser.add_argument('-wait','--wait_time',type=int,default=120,help='为检索预留的等待时间, 默认为120秒')
-    parser.add_argument('--debug',action='store_false')
+    # parser.add_argument('--debug',action='store_false')
     args = parser.parse_args()
     start_crawl(start_paper_index = args.start_paper_index,
                 end_paper_index = args.end_paper_index,
                 mode = args.mode,
                 save_path = args.save_path,
-                log = args.debug,
+                log = args.log,
                 wait_time = args.wait_time,
                 browser_type = args.browser_type,
                 )
     
 if __name__ == '__main__':
     main()
```

### Comparing `cnki_html2json-0.0.8/cnki_html2json/crawl.py` & `cnki_html2json-0.0.9/cnki_html2json/crawl.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,27 +105,27 @@
         else:
             driver.execute_script('window.scrollTo(0,0)')
             driver.find_element(By.XPATH,f'//a[@id="page{visible_page_index[-1]}"]').click()
             time.sleep(3)
             current_page = visible_page_index[-1]
 
         
-def start_crawl(start_paper_index=1,end_paper_index=None,mode='structure',save_path='data',log=True,wait_time=120,browser_type='Chrome'):
+def start_crawl(start_paper_index=1,end_paper_index=None,mode='structure',browser_type='Chrome',log='true',save_path='data',wait_time=120):
     """爬取cnki网站的论文
     start_paper_index: 开始爬取的论文索引，默认为1
     end_paper_index: 结束爬取的论文索引，默认为None，即爬取到最后
     mode: 模式，structure|plain|raw，默认为structure
     save_path: 下载文件的保存路径，默认为当前目录的data文件夹
     log: 是否保存日志，默认为True
     wait_time: 为检索预留的等待时间，单位为秒
     browser_type: Chrome(默认)|Firefox|Edge|Safari
     """
-    if log:
+    if log=='true':
         if not os.path.exists(f'{save_path}/log'):
-            os.mkdir(f'{save_path}/log')
+            os.makedirs(f'{save_path}/log')
             logger.info(f'已在{save_path}文件夹下创建log文件夹')
 
         current_time = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
         logger.add(f"{save_path}/log/{current_time}.log",format="{time} {level} {message}",level="INFO",mode='w')
         logger.info('本次任务记录日志')
     else:
         logger.info('本次任务不记录日志')
@@ -177,15 +177,15 @@
     total_records_num = int(''.join(driver.find_element(By.XPATH,'//*[@id="countPageDiv"]/span[1]/em').text.split(',')))
     if end_paper_index:
         avaiable_records_num = min([total_records_num,end_paper_index,6000])
     else:
         avaiable_records_num = min([total_records_num,6000])
     
     need_download_num = avaiable_records_num-start_paper_index+1
-    logger.info(f'总文献数量 {total_records_num} \t可下载文献数 {avaiable_records_num}' )
+    logger.info(f'总文献数量 {total_records_num}; 可下载文献数 {avaiable_records_num}' )
     
     start_page = start_paper_index//papers_per_page+1
     
     # 总页数
     # total_page_num = int(driver.find_element(By.XPATH,'//*[@id="countPageDiv"]/span[2]').text.split('/')[1])
     # print(f'总页数{total_page_num}')
     
@@ -196,15 +196,15 @@
         current_page = start_page
     logger.info(f'将从第 {start_paper_index} 篇文献开始下载')
     logger.info(f'模式设置为 {mode}')
     minutes = math.ceil(need_download_num/3)
     if minutes < 60:
         logger.info(f'预计耗时 {minutes}分钟')
     else:
-        logger.info(f'预计耗时 {minutes//60}小时 {minutes%60}分钟')
+        logger.info(f'预计耗时 {minutes//60}小时 {minutes%60} 分钟')
     
     # 下载文献数据
     current_paper_index = start_paper_index
 
     while current_paper_index < avaiable_records_num+1:
         current_url_list = obtain_page_papers_url(driver)[current_paper_index%papers_per_page-1:]  
         for url in current_url_list:
```

### Comparing `cnki_html2json-0.0.8/cnki_html2json/html2json.py` & `cnki_html2json-0.0.9/cnki_html2json/html2json.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.0.8/cnki_html2json/parse_metadata.py` & `cnki_html2json-0.0.9/cnki_html2json/parse_metadata.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.0.8/cnki_html2json/recognize_slider_coordinate.py` & `cnki_html2json-0.0.9/cnki_html2json/recognize_slider_coordinate.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.0.8/cnki_html2json.egg-info/PKG-INFO` & `cnki_html2json-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cnki-html2json
-Version: 0.0.8
+Name: cnki_html2json
+Version: 0.0.9
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Programming Language :: Python :: 3
@@ -44,28 +44,28 @@
 - 确保你所在的网络环境能正常使用知网
 - 仅能提取 <b>期刊论文</b> 的文本，其他文献类型未做测试
 - 无法提取文献中的图片、公式等，因此提取的内容可能不完整
 - 本工具已经尽力覆盖大多数情况，但不能保证每一篇文献都能正常提取
 
 ## 快速开始
 
-本工具使用 Python 开发，请确保你的电脑上已经安装了 `Python3.8` 或以上版本。
+本工具使用 Python 开发，请确保你的电脑上已经安装了 `Python3.8` 或以上版本。如果使用爬虫，需要提前配置好对应浏览器的驱动，例如chrome的驱动为 [chromedriver](https://chromedriver.chromium.org/downloads)
 
 ```console
 $ python3 -m pip install cnki_html2json
 ```
 
 ## 使用方法
 
 1、调用 `html2json` 函数
 
 ```python
 from cnki_html2json import html2json
 with open('paper.html', 'r', encoding='utf-8') as f:
-	html = f.read()
+    html = f.read()
 print(html2json.extract(html, mode='structure'))
 ```
 `html2json` 参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
 | `paper_html` | 一篇期刊论文的html字符串 |
@@ -77,42 +77,42 @@
 
 2、使用命令行工具，启动一个selenium爬虫，然后在弹出的浏览器窗口(默认为Chrome)中进行检索
 ```console
 $ 无需设置任何参数，直接运行
 $ cnki-crawler
 ```
 ```console
-$ 设置论文提取的起始索引和终止索引，模式设置为structure
-$ cnki-crawler -s 1 -e 100 -m structure
+$ 设置论文提取的起始索引和终止索引，模式设置为structure，不记录日志
+$ cnki-crawler -s 1 -e 100 -m structure -l false
 $ 或者是
-$ cnki-crawler --start_paper_index 1 --end_paper_index 100 -mode structure
+$ cnki-crawler --start_paper_index 1 --end_paper_index 100 -mode structure --log false
 ```
 ```console
 $ 查看可选参数
 $ cnki-crawler --help
 ```
 
 参数说明：
 | 简写参数 | 参数 | 说明 |
 | --- | --- | --- |
-| s | `start_paper_index` | 论文提取的起始索引，默认为1 |
-| e | `end_paper_index` | 论文提取的终止索引，默认为None，爬取到最后 |
-| m | `mode` | 模式，可选值为 `structure`, `plain`, `raw`，默认为 `structure` |
-| b | `browser` | 浏览器类型，Chrome(默认),可选 Edge, Firefox, 不支持Safari|
-| save | `save_path` | 下载文件的保存路径，默认为当前目录的data文件夹 |
-| wait | `wait_time` | 为检索预留的等待时间，默认120秒 |
+| s | `start_paper_index` | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
+| e | `end_paper_index` | 论文提取的终止索引，默认为 `None`，爬取到最后 |
+| m | `mode` | 模式，可选值为 `structure`， `plain`， `raw`，默认为 `structure` |
+| b | `browser` | 浏览器类型，Chrome(默认),可选Edge， Firefox， 不支持Safari |
+| l | `log` | 是否记录日志，默认为 `true`，日志将保存在 `save_path` 下的 `log` 文件夹中 |
+| save | `save_path` | 下载文件的保存路径，默认为当前目录的 `data` 文件夹 |
+| wait | `wait_time` | 为检索预留的等待时间，默认 `120` 秒 |
 
-注：爬虫将自动保存日志到 `save_path` 的log文件夹中，如果不想保存日志，请传入参数 `--debug`
-> 提取结果可以参考examples文件夹中给出的样例。如果未指定保存路径，将下载结果默认保存在当前目录下的data文件夹下  
+> 提取结果可以参考examples文件夹中给出的样例。如果未指定保存路径，将下载结果默认保存在当前目录下的data文件夹下;  
 > 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (可以自动过滑块验证)
 
 ```python
-# 也可以在代码中调用爬虫
-from cnki_html2json.crawl import start_crawl:
-	start_crawl() # 默认参数
+# 也可以在代码中调用爬虫，可选参数参考上方的参数说明
+from cnki_html2json.crawl import start_crawl
+start_crawl(start_paper_index=1,end_paper_index=100,mode='structure',log='false')
 ```
 
 ## json文件字段说明
 
 | 一级字段 | 二级字段 |三级字段| 说明 |
 | --- | --- | --- | --- |
 | metadata | title |  |论文标题|
@@ -130,12 +130,12 @@
 |  | ...| ... ||
 | 参考文献 |  |  |参考文献|
 
 ## 工具推荐
 
 | 工具  | 描述 |
 | --- | --- |
-| [vermin](https://github.com/netromdk/vermin) | 从语法层面检测一个项目最低支持的 `python` 版本 |
+| [vermin](https://github.com/netromdk/vermin) | 从语法层面检测一个项目最低支持的 `Python` 版本 |
 
 ## 责任声明
 
 - 使用者使用本工具造成的一切后果，由使用者自行承担
```

### Comparing `cnki_html2json-0.0.8/setup.py` & `cnki_html2json-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup,find_packages
 
 setup(
     name="cnki_html2json",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.0.8",
+    version="0.0.9",
     description="A package to convert cnki html to json",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["cnki","text-structure","crawler"],
     license="MIT",
     url="https://github.com/doublessay/cnki-html2json",
     packages=find_packages(),
```

### Comparing `cnki_html2json-0.0.8/test/test_html2json.py` & `cnki_html2json-0.0.9/test/test_html2json.py`

 * *Files identical despite different names*

