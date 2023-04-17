# Comparing `tmp/bestconfig-1.3.5.tar.gz` & `tmp/bestconfig-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bestconfig-1.3.5.tar", last modified: Sun Jul 18 15:25:40 2021, max compression
+gzip compressed data, was "bestconfig-1.3.6.tar", last modified: Mon Apr 17 19:57:06 2023, max compression
```

## Comparing `bestconfig-1.3.5.tar` & `bestconfig-1.3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 fiobond   (1000) fiobond   (1000)        0 2021-07-18 15:25:40.698178 bestconfig-1.3.5/
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)     8151 2021-07-18 15:25:40.698178 bestconfig-1.3.5/PKG-INFO
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)     7870 2021-07-18 15:08:31.000000 bestconfig-1.3.5/README.md
-drwxrwxr-x   0 fiobond   (1000) fiobond   (1000)        0 2021-07-18 15:25:40.694178 bestconfig-1.3.5/bestconfig/
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)       83 2021-07-18 14:36:07.000000 bestconfig-1.3.5/bestconfig/__init__.py
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)     2440 2021-07-18 15:11:07.000000 bestconfig-1.3.5/bestconfig/adapters.py
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)     2820 2021-07-18 15:08:08.000000 bestconfig-1.3.5/bestconfig/config.py
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)     7579 2021-07-18 14:36:07.000000 bestconfig-1.3.5/bestconfig/config_provider.py
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)     3620 2021-07-18 14:36:07.000000 bestconfig-1.3.5/bestconfig/converters.py
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)     5648 2021-07-18 14:36:07.000000 bestconfig-1.3.5/bestconfig/file_parsers.py
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)     1589 2021-07-18 14:36:07.000000 bestconfig-1.3.5/bestconfig/source.py
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)     7196 2021-07-18 14:36:07.000000 bestconfig-1.3.5/bestconfig/source_resolver.py
-drwxrwxr-x   0 fiobond   (1000) fiobond   (1000)        0 2021-07-18 15:25:40.698178 bestconfig-1.3.5/bestconfig.egg-info/
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)     8151 2021-07-18 15:25:40.000000 bestconfig-1.3.5/bestconfig.egg-info/PKG-INFO
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)      387 2021-07-18 15:25:40.000000 bestconfig-1.3.5/bestconfig.egg-info/SOURCES.txt
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)        1 2021-07-18 15:25:40.000000 bestconfig-1.3.5/bestconfig.egg-info/dependency_links.txt
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)       14 2021-07-18 15:25:40.000000 bestconfig-1.3.5/bestconfig.egg-info/requires.txt
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)       11 2021-07-18 15:25:40.000000 bestconfig-1.3.5/bestconfig.egg-info/top_level.txt
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)       38 2021-07-18 15:25:40.698178 bestconfig-1.3.5/setup.cfg
--rw-rw-r--   0 fiobond   (1000) fiobond   (1000)      672 2021-07-18 15:20:13.000000 bestconfig-1.3.5/setup.py
+drwxr-xr-x   0 fiobond    (501) staff       (20)        0 2023-04-17 19:57:06.980580 bestconfig-1.3.6/
+-rw-r--r--   0 fiobond    (501) staff       (20)     8131 2023-04-17 19:57:06.980449 bestconfig-1.3.6/PKG-INFO
+-rw-r--r--   0 fiobond    (501) staff       (20)     7870 2023-04-17 19:41:03.000000 bestconfig-1.3.6/README.md
+drwxr-xr-x   0 fiobond    (501) staff       (20)        0 2023-04-17 19:57:06.979724 bestconfig-1.3.6/bestconfig/
+-rw-r--r--   0 fiobond    (501) staff       (20)       73 2023-04-17 19:41:03.000000 bestconfig-1.3.6/bestconfig/__init__.py
+-rw-r--r--   0 fiobond    (501) staff       (20)     2420 2023-04-17 19:41:03.000000 bestconfig-1.3.6/bestconfig/adapters.py
+-rw-r--r--   0 fiobond    (501) staff       (20)     2790 2023-04-17 19:41:03.000000 bestconfig-1.3.6/bestconfig/config.py
+-rw-r--r--   0 fiobond    (501) staff       (20)     7626 2023-04-17 19:49:42.000000 bestconfig-1.3.6/bestconfig/config_provider.py
+-rw-r--r--   0 fiobond    (501) staff       (20)     3620 2023-04-17 19:41:03.000000 bestconfig-1.3.6/bestconfig/converters.py
+-rw-r--r--   0 fiobond    (501) staff       (20)     5648 2023-04-17 19:41:03.000000 bestconfig-1.3.6/bestconfig/file_parsers.py
+-rw-r--r--   0 fiobond    (501) staff       (20)     1589 2023-04-17 19:41:03.000000 bestconfig-1.3.6/bestconfig/source.py
+-rw-r--r--   0 fiobond    (501) staff       (20)     7160 2023-04-17 19:41:03.000000 bestconfig-1.3.6/bestconfig/source_resolver.py
+drwxr-xr-x   0 fiobond    (501) staff       (20)        0 2023-04-17 19:57:06.980273 bestconfig-1.3.6/bestconfig.egg-info/
+-rw-r--r--   0 fiobond    (501) staff       (20)     8131 2023-04-17 19:57:06.000000 bestconfig-1.3.6/bestconfig.egg-info/PKG-INFO
+-rw-r--r--   0 fiobond    (501) staff       (20)      387 2023-04-17 19:57:06.000000 bestconfig-1.3.6/bestconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 fiobond    (501) staff       (20)        1 2023-04-17 19:57:06.000000 bestconfig-1.3.6/bestconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 fiobond    (501) staff       (20)       14 2023-04-17 19:57:06.000000 bestconfig-1.3.6/bestconfig.egg-info/requires.txt
+-rw-r--r--   0 fiobond    (501) staff       (20)       11 2023-04-17 19:57:06.000000 bestconfig-1.3.6/bestconfig.egg-info/top_level.txt
+-rw-r--r--   0 fiobond    (501) staff       (20)       38 2023-04-17 19:57:06.980615 bestconfig-1.3.6/setup.cfg
+-rw-r--r--   0 fiobond    (501) staff       (20)      672 2023-04-17 19:56:03.000000 bestconfig-1.3.6/setup.py
```

### Comparing `bestconfig-1.3.5/PKG-INFO` & `bestconfig-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: bestconfig
-Version: 1.3.5
+Version: 1.3.6
 Summary: Setup your project config easily
 Home-page: https://github.com/fivol/bestconfig
 Author: Boris Bondarenko
 Author-email: borisoffficial@gmail.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # bestconfig
 ### *Python модуль для работы с файлами конфигурации проекта*
 
 Этот модуль поможет сильно упростить использование конфигурационных
 файлов, вы предпочитаете хранить константы и 
@@ -211,9 +210,7 @@
 
 ## Запланированные обновления
 - Поддержка загрузки из базы данных
 - Поддержка загрузки с config сервера
 - Перевод документации и комментариев на английский
 
 
-
-
```

### Comparing `bestconfig-1.3.5/README.md` & `bestconfig-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `bestconfig-1.3.5/bestconfig/adapters.py` & `bestconfig-1.3.6/bestconfig/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from pathlib import Path
 import typing as t
 
-from bestconfig.source import Source
-from bestconfig.file_parsers import *
+from .source import Source
+from .file_parsers import *
 
 
 class AbstractAdapter(metaclass=ABCMeta):
 
     @classmethod
     @abstractmethod
     def get_dict(cls, source: Source) -> dict:
```

### Comparing `bestconfig-1.3.5/bestconfig/config.py` & `bestconfig-1.3.6/bestconfig/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing as t
-from bestconfig.config_provider import ConfigProvider
-from bestconfig.source import Source, TargetType
-from bestconfig.source_resolver import SourceResolver, FilesScanner
+from .config_provider import ConfigProvider
+from .source import Source, TargetType
+from .source_resolver import SourceResolver, FilesScanner
 
 supported_extensions = ['json', 'yaml', 'yml', 'ini', 'cfg', 'env']
 applicant_files = ['config', 'conf', 'setting', 'settings', 'configuration']
 
 
 def generate_targets(files: t.List[str], extensions: t.List[str]) -> t.List[str]:
     """Генерирует всевозможные названия файлов
```

### Comparing `bestconfig-1.3.5/bestconfig/config_provider.py` & `bestconfig-1.3.6/bestconfig/config_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from warnings import warn
 import inspect
-from bestconfig.converters import *
-from bestconfig.source_resolver import SourceResolver, FilesScanner
-from bestconfig.source import TargetType
+from .converters import *
+from .source_resolver import SourceResolver, FilesScanner
+from .source import TargetType
 
 """Тип, которым может быть значение конфига"""
 ConfigType = t.Union[str, int, float, bool, dict, list]
 
 """
 Используется по умолчанию, при
 config.get()
@@ -60,15 +60,15 @@
 
             # Преобразуем объект в соответствии с переданным в параметрах cast
             if cast:
                 return cast.cast(value)
             return value
         except KeyError:
             if raise_absent:
-                raise KeyError
+                raise
 
         return default_value
 
     def get_raw(self, item: str):
         """Возвращает значение по ключу, не изменяя его
         Такое, какое было считано из файла"""
         return self.get(item, cast=None)
@@ -172,15 +172,15 @@
             return super().__getitem__(item)
 
         # Попытка пройти по частям ключей, разделенным точками
         keys = item.split('.')
         value = self.to_dict()
         for key in keys:
             if not hasattr(value, '__getitem__'):
-                raise KeyError
+                raise KeyError(f'Key "{key}" not found on path "{item}"')
 
             if key not in value:
-                raise KeyError
+                raise KeyError(f'Key "{key}" not found on path "{item}"')
 
             value = value[key]
 
         return value
```

### Comparing `bestconfig-1.3.5/bestconfig/converters.py` & `bestconfig-1.3.6/bestconfig/converters.py`

 * *Files identical despite different names*

### Comparing `bestconfig-1.3.5/bestconfig/file_parsers.py` & `bestconfig-1.3.6/bestconfig/file_parsers.py`

 * *Files identical despite different names*

### Comparing `bestconfig-1.3.5/bestconfig/source.py` & `bestconfig-1.3.6/bestconfig/source.py`

 * *Files identical despite different names*

### Comparing `bestconfig-1.3.5/bestconfig/source_resolver.py` & `bestconfig-1.3.6/bestconfig/source_resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import traceback
 import typing as t
-import warnings
 from pathlib import Path
 
-from bestconfig.adapters import EnvAdapter, FileAdapter, DictAdapter
+from .adapters import EnvAdapter, FileAdapter, DictAdapter
 
-from bestconfig.source import Source, TargetType, SourceType
+from .source import Source, TargetType, SourceType
 
 
 class SourceResolver:
     """
     Получает сырые данные:
     1. Названия файлов
     2. python словари
```

### Comparing `bestconfig-1.3.5/bestconfig.egg-info/PKG-INFO` & `bestconfig-1.3.6/bestconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: bestconfig
-Version: 1.3.5
+Version: 1.3.6
 Summary: Setup your project config easily
 Home-page: https://github.com/fivol/bestconfig
 Author: Boris Bondarenko
 Author-email: borisoffficial@gmail.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # bestconfig
 ### *Python модуль для работы с файлами конфигурации проекта*
 
 Этот модуль поможет сильно упростить использование конфигурационных
 файлов, вы предпочитаете хранить константы и 
@@ -211,9 +210,7 @@
 
 ## Запланированные обновления
 - Поддержка загрузки из базы данных
 - Поддержка загрузки с config сервера
 - Перевод документации и комментариев на английский
 
 
-
-
```

### Comparing `bestconfig-1.3.5/setup.py` & `bestconfig-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name='bestconfig',
     packages=find_packages(include=['bestconfig']),
-    version='1.3.5',
+    version='1.3.6',
     description="""Setup your project config easily""",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/fivol/bestconfig",
     author='Boris Bondarenko',
     author_email="borisoffficial@gmail.com",
     license='MIT',
```

