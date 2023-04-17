# Comparing `tmp/nb_log-8.2.tar.gz` & `tmp/nb_log-8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nb_log-8.2.tar", last modified: Wed Apr 12 09:54:01 2023, max compression
+gzip compressed data, was "dist\nb_log-8.3.tar", last modified: Mon Apr 17 03:21:52 2023, max compression
```

## Comparing `nb_log-8.2.tar` & `nb_log-8.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 09:54:01.000000 nb_log-8.2/
--rw-rw-rw-   0        0        0    27863 2023-04-12 09:54:01.000000 nb_log-8.2/PKG-INFO
--rw-rw-rw-   0        0        0    26926 2022-12-05 09:46:23.000000 nb_log-8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 09:54:01.000000 nb_log-8.2/nb_log/
--rw-rw-rw-   0        0        0     2329 2022-09-17 07:28:19.000000 nb_log-8.2/nb_log/__init__.py
--rw-rw-rw-   0        0        0    50515 2022-12-23 03:23:06.000000 nb_log-8.2/nb_log/handlers.py
--rw-rw-rw-   0        0        0    49868 2022-09-17 07:28:19.000000 nb_log-8.2/nb_log/handlers0000.py
--rw-rw-rw-   0        0        0    30380 2023-04-12 09:53:33.000000 nb_log-8.2/nb_log/log_manager.py
--rw-rw-rw-   0        0        0     7183 2022-09-17 06:12:29.000000 nb_log-8.2/nb_log/monkey_print.py
--rw-rw-rw-   0        0        0     8847 2023-04-03 09:15:14.000000 nb_log-8.2/nb_log/nb_log_config_default.py
--rw-rw-rw-   0        0        0     7530 2022-09-17 06:13:18.000000 nb_log-8.2/nb_log/set_nb_log_config.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:54:01.000000 nb_log-8.2/nb_log.egg-info/
--rw-rw-rw-   0        0        0    27863 2023-04-12 09:54:00.000000 nb_log-8.2/nb_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-04-12 09:54:00.000000 nb_log-8.2/nb_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 09:54:00.000000 nb_log-8.2/nb_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-04-12 09:54:00.000000 nb_log-8.2/nb_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-12 09:54:00.000000 nb_log-8.2/nb_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 09:54:01.000000 nb_log-8.2/setup.cfg
--rw-rw-rw-   0        0        0     2325 2023-04-12 09:53:51.000000 nb_log-8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:21:52.000000 nb_log-8.3/
+-rw-rw-rw-   0        0        0    27863 2023-04-17 03:21:52.000000 nb_log-8.3/PKG-INFO
+-rw-rw-rw-   0        0        0    26926 2022-12-05 09:46:23.000000 nb_log-8.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 03:21:52.000000 nb_log-8.3/nb_log/
+-rw-rw-rw-   0        0        0     2329 2022-09-17 07:28:19.000000 nb_log-8.3/nb_log/__init__.py
+-rw-rw-rw-   0        0        0    50623 2023-04-17 02:59:39.000000 nb_log-8.3/nb_log/handlers.py
+-rw-rw-rw-   0        0        0    49868 2022-09-17 07:28:19.000000 nb_log-8.3/nb_log/handlers0000.py
+-rw-rw-rw-   0        0        0      246 2023-04-17 02:59:39.000000 nb_log-8.3/nb_log/helper.py
+-rw-rw-rw-   0        0        0    30405 2023-04-17 02:59:07.000000 nb_log-8.3/nb_log/log_manager.py
+-rw-rw-rw-   0        0        0     7350 2023-04-17 02:59:07.000000 nb_log-8.3/nb_log/monkey_print.py
+-rw-rw-rw-   0        0        0     9334 2023-04-17 03:10:36.000000 nb_log-8.3/nb_log/nb_log_config_default.py
+-rw-rw-rw-   0        0        0     7710 2023-04-13 09:47:00.000000 nb_log-8.3/nb_log/set_nb_log_config.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:21:52.000000 nb_log-8.3/nb_log.egg-info/
+-rw-rw-rw-   0        0        0    27863 2023-04-17 03:21:52.000000 nb_log-8.3/nb_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-04-17 03:21:52.000000 nb_log-8.3/nb_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 03:21:52.000000 nb_log-8.3/nb_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-04-17 03:21:52.000000 nb_log-8.3/nb_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 03:21:52.000000 nb_log-8.3/nb_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 03:21:52.000000 nb_log-8.3/setup.cfg
+-rw-rw-rw-   0        0        0     2325 2023-04-17 03:21:43.000000 nb_log-8.3/setup.py
```

### Comparing `nb_log-8.2/PKG-INFO` & `nb_log-8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_log
-Version: 8.2
+Version: 8.3
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-8.2/README.md` & `nb_log-8.3/README.md`

 * *Files identical despite different names*

### Comparing `nb_log-8.2/nb_log/__init__.py` & `nb_log-8.3/nb_log/__init__.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.2/nb_log/handlers.py` & `nb_log-8.3/nb_log/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 # noinspection PyUnresolvedReferences
 from logging.handlers import WatchedFileHandler
 # noinspection PyPackageRequirements
 from nb_filelock import FileLock
 from pythonjsonlogger.jsonlogger import JsonFormatter
 from nb_log import nb_log_config_default
 from nb_log import nb_print
+from nb_log.helper import need_filter_print
 
 very_nb_print = nb_print
 os_name = os.name
 
 
 class MongoHandler(logging.Handler):
     """
@@ -579,14 +580,16 @@
         The record is then written to the stream with a trailing newline.  If
         exception information is present, it is formatted using
         traceback.print_exception and appended to the stream.  If the stream
         has an 'encoding' attribute, it is used to determine how to do the
         output to the stream.
         """
         # noinspection PyBroadException
+        if need_filter_print(record.msg):
+            return
         try:
             # very_nb_print(record)
             # record.message = record.getMessage()
             # effective_information_msg = record.getMessage()  # 不能用msg字段，例如有的包的日志格式化还有其他字段
             # record_copy = copy.copy(record)  # copy是因为，不要因为要屏幕彩色日志而影响例如文件日志 叮叮日志等其他handler的格式。
             # record_copy.for_segmentation_color = '彩色分段标志属性而已'
             # del record_copy.msg
```

### Comparing `nb_log-8.2/nb_log/handlers0000.py` & `nb_log-8.3/nb_log/handlers0000.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.2/nb_log/log_manager.py` & `nb_log-8.3/nb_log/log_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 使极限多进程安全切片的文件日志写入性能在win下提高100倍，linux下提高10倍。
 
 """
 import logging
 import multiprocessing
 import typing
 from functools import lru_cache
-from logging import FileHandler, _checkLevel
+from logging import FileHandler, _checkLevel  # noqa
 from nb_log import nb_log_config_default  # noqa
 from nb_log.handlers import *
+import deprecated
 
 
 # noinspection DuplicatedCode
 def revision_call_handlers(self, record):  # 对logging标准模块打猴子补丁。主要是使父命名空间的handler不重复记录当前命名空间日志已有种类的handler。
     """
     重要。这可以使同名logger或父logger随意添加同种类型的handler，确保不会重复打印。
     例如对"a"命名空间加上streamhandler，对"a.b"命名空间也加上streamhandler，则"a.b"命名空间的日志会被打印两次
@@ -123,19 +124,18 @@
     """
     Set the logging level of this logger.  level must be an int or a str.
     """
     level2 = LogManager.preset_name__level_map.get(self.name, level)
     if level2 != level:
         very_nb_print(f'日志命名空间 {self.name} 已经锁定了为了 {level2} 级别 ,后续不可以更改为 {level} 级别')
     self.level = _checkLevel(level2)
-    if sys.version_info.minor >=7:  # python3.6 没有 _clear_cache 方法
+    if sys.version_info.minor >= 7:  # python3.6 没有 _clear_cache 方法
         self.manager._clear_cache()
 
 
-
 logging.Logger.callHandlers = revision_call_handlers  # 打猴子补丁。
 logging.Logger.addHandler = revision_add_handler  # 打猴子补丁。
 logging.Logger.setLevel = revision_setLevel  # 打猴子补丁。
 
 
 # noinspection PyShadowingBuiltins
 # print = very_nb_print
@@ -204,15 +204,15 @@
     logger_list = []
     preset_name__level_map = dict()
 
     def __init__(self, logger_name: typing.Union[str, None] = 'nb_log_default_namespace'):
         """
         :param logger_name: 日志名称，当为None时候创建root命名空间的日志，一般情况下千万不要传None，除非你确定需要这么做和是在做什么.这个命名空间是双刃剑
         """
-        if logger_name in (None, '', ) and multiprocessing.process.current_process().name == 'MainProcess':
+        if logger_name in (None, '',) and multiprocessing.process.current_process().name == 'MainProcess':
             very_nb_print('logger_name 设置为None和空字符串都是一个意义，在操作根日志命名空间，任何其他日志的行为将会发生变化，'
                           '一定要弄清楚原生logging包的日志name的意思。这个命名空间是双刃剑')
         self._logger_name = logger_name
         self.logger = logging.getLogger(logger_name)
 
     def preset_log_level(self, log_level_int=20):
         """
```

### Comparing `nb_log-8.2/nb_log/monkey_print.py` & `nb_log-8.3/nb_log/monkey_print.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 """
 import multiprocessing
 import sys
 import time
 import traceback
 from nb_log import nb_log_config_default
+from nb_log.helper import need_filter_print
 
 print_raw = print
 
 WORD_COLOR = 37
 
 
 def stdout_write(msg: str):
@@ -29,14 +30,18 @@
 # noinspection PyProtectedMember,PyUnusedLocal,PyIncorrectDocstring,DuplicatedCode
 def nb_print(*args, sep=' ', end='\n', file=None, flush=True):
     """
     超流弊的print补丁
     :param x:
     :return:
     """
+
+    if need_filter_print(sep.join(args)):
+        return
+
     args = (str(arg) for arg in args)  # REMIND 防止是数字不能被join
     if file == sys.stderr:
         stderr_write(sep.join(args))  # 如 threading 模块第926行，打印线程错误，希望保持原始的红色错误方式，不希望转成蓝色。
     elif file in [sys.stdout, None]:
         # 获取被调用函数在被调用时所处代码行数
         line = sys._getframe().f_back.f_lineno
         # 获取被调用函数所在模块文件名
@@ -141,14 +146,16 @@
 def is_main_process():
     return multiprocessing.process.current_process().name == 'MainProcess'
 
 
 # noinspection DuplicatedCode
 def only_print_on_main_process(*args, sep=' ', end='\n', file=None, flush=True):
     # 获取被调用函数在被调用时所处代码行数
+    if need_filter_print(sep.join(args)):
+        return
     if is_main_process():
         args = (str(arg) for arg in args)  # REMIND 防止是数字不能被join
         if file == sys.stderr:
             stderr_write(sep.join(args))  # 如 threading 模块第926行，打印线程错误，希望保持原始的红色错误方式，不希望转成蓝色。
         elif file in [sys.stdout, None]:
             # 获取被调用函数在被调用时所处代码行数
             line = sys._getframe().f_back.f_lineno
```

### Comparing `nb_log-8.2/nb_log/nb_log_config_default.py` & `nb_log-8.3/nb_log/nb_log_config_default.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,16 +90,19 @@
 3为不自动切割的单个文件的日志(不切割文件就不会出现所谓进程安不安全的问题) 
 4为 WatchedFileHandler，这个是需要在linux下才能使用，需要借助lograte外力进行日志文件的切割，多进程安全。
 5 为第三方的concurrent_log_handler.ConcurrentRotatingFileHandler按日志文件大小切割的文件日志，
    这个是采用了文件锁，多进程安全切割，文件锁在linux上使用fcntl性能还行，win上使用win32con性能非常惨。按大小切割建议不要选第5个个filehandler而是选择第1个。
 """
 
 LOG_LEVEL_FILTER = logging.DEBUG  # 默认日志级别，低于此级别的日志不记录了。例如设置为INFO，那么logger.debug的不会记录，只会记录logger.info以上级别的。
-                                  # 强烈不建议调高这里的级别为INFO，日志是有命名空间的，单独提高打印啰嗦的日志命名空间的日志级别就可以了，不要全局提高日志级别。
-                                  # https://nb-log-doc.readthedocs.io/zh_CN/latest/articles/c9.html#id2  文档9.5里面讲了几百次 python logging的命名空间的作用了，有些人到现在还不知道日志的name作用。
+# 强烈不建议调高这里的级别为INFO，日志是有命名空间的，单独提高打印啰嗦的日志命名空间的日志级别就可以了，不要全局提高日志级别。
+# https://nb-log-doc.readthedocs.io/zh_CN/latest/articles/c9.html#id2  文档9.5里面讲了几百次 python logging的命名空间的作用了，有些人到现在还不知道日志的name作用。
+
+# 屏蔽的字符串显示，用 if in {打印信息} 来判断实现的,如果打印的消息中包括 FILTER_WORDS_PRINT 数组中的任何一个字符串，那么消息就不执行打印。这个配置对 print 和 logger的控制台输出都生效。这个可以过滤某些啰嗦的print信息，也可以过滤同级别日志中的某些烦人的日志。
+FILTER_WORDS_PRINT = []  # 例如， 你希望消息中包括阿弥陀佛 或者 包括善哉善哉 就不打印，那么可以把  FILTER_WORDS_PRINT = ['阿弥陀佛','善哉善哉']
 
 RUN_ENV = 'test'
 
 FORMATTER_DICT = {
     1: logging.Formatter(
         '日志时间【%(asctime)s】 - 日志名称【%(name)s】 - 文件【%(filename)s】 - 第【%(lineno)d】行 - 日志等级【%(levelname)s】 - 日志信息【%(message)s】',
         "%Y-%m-%d %H:%M:%S"),
@@ -127,7 +130,9 @@
     10: logging.Formatter(
         '[p%(process)d_t%(thread)d] %(asctime)s - %(name)s - "%(filename)s:%(lineno)d" - %(levelname)s - %(message)s', "%Y-%m-%d %H:%M:%S"),  # 对7改进，带进程和线程显示的日志模板。
     11: logging.Formatter(
         f'({computer_ip},{computer_name})-[p%(process)d_t%(thread)d] %(asctime)s - %(name)s - "%(filename)s:%(lineno)d" - %(levelname)s - %(message)s', "%Y-%m-%d %H:%M:%S"),  # 对7改进，带进程和线程显示的日志模板以及ip和主机名。
 }
 
 FORMATTER_KIND = 5  # 如果get_logger不指定日志模板，则默认选择第几个模板
+
+
```

### Comparing `nb_log-8.2/nb_log/set_nb_log_config.py` & `nb_log-8.3/nb_log/set_nb_log_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,10 +101,10 @@
                                知道PYTHONPATH的人无论项目有多少层级的文件夹，无论是多深层级文件夹导入外层文件夹，代码里面永久都不需要出现手动硬编码操纵sys.path.append
                                
                                懂PYTHONPATH 的重要性和妙用见： https://github.com/ydf0509/pythonpathdemo
                                ''')
     # with (Path(sys.path[1]) / Path('nb_log_config.py')).open(mode='w', encoding='utf8') as f:
     #     f.write(config_file_content)
     copyfile(Path(__file__).parent / Path('nb_log_config_default.py'), Path(sys.path[1]) / Path('nb_log_config.py'))
-
+    nb_print(f'''在  {Path(sys.path[1])} 目录下自动生成了一个文件， 请刷新文件夹查看或修改 \n "{Path(sys.path[1]) / Path('nb_log_config.py')}:1" 文件''')
 
 use_config_form_nb_log_config_module()
```

### Comparing `nb_log-8.2/nb_log.egg-info/PKG-INFO` & `nb_log-8.3/nb_log.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-log
-Version: 8.2
+Version: 8.3
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-8.2/setup.py` & `nb_log-8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ]
 
 if os.name == 'nt':
     install_requires.append('pywin32')
 
 setup(
     name='nb_log',  #
-    version="8.2",
+    version="8.3",
     description=(
         'very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on '
     ),
     keywords=["logging", "logger", "multiprocess file handler", "color handler"],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
@@ -61,14 +61,14 @@
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
 
 python setup.py sdist & twine upload dist/nb_log-6.0.tar.gz
-python setup.py sdist & python -m  twine upload dist/nb_log-8.2.tar.gz
+python setup.py sdist & python -m  twine upload dist/nb_log-8.3.tar.gz
 
 twine upload dist/*
 
 
 python -m pip install nb_log --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```

