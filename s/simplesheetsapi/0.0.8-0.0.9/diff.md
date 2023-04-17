# Comparing `tmp/simplesheetsapi-0.0.8.tar.gz` & `tmp/simplesheetsapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplesheetsapi-0.0.8.tar", last modified: Wed Dec 14 15:48:41 2022, max compression
+gzip compressed data, was "simplesheetsapi-0.0.9.tar", last modified: Mon Apr 17 16:06:46 2023, max compression
```

## Comparing `simplesheetsapi-0.0.8.tar` & `simplesheetsapi-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-12-14 15:48:41.440637 simplesheetsapi-0.0.8/
--rw-rw-rw-   0        0        0     1086 2022-11-27 20:46:23.000000 simplesheetsapi-0.0.8/LICENCE
--rw-rw-rw-   0        0        0     1945 2022-12-14 15:48:41.439638 simplesheetsapi-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1557 2022-12-14 15:47:03.000000 simplesheetsapi-0.0.8/README.md
--rw-rw-rw-   0        0        0      611 2022-12-14 15:47:03.000000 simplesheetsapi-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-14 15:48:41.440637 simplesheetsapi-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-14 15:48:41.426634 simplesheetsapi-0.0.8/simplesheetsapi/
--rw-rw-rw-   0        0        0     3133 2022-12-14 15:47:03.000000 simplesheetsapi-0.0.8/simplesheetsapi/SheetsApi.py
--rw-rw-rw-   0        0        0        0 2022-11-27 20:05:19.000000 simplesheetsapi-0.0.8/simplesheetsapi/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-14 15:48:41.438638 simplesheetsapi-0.0.8/simplesheetsapi.egg-info/
--rw-rw-rw-   0        0        0     1945 2022-12-14 15:48:41.000000 simplesheetsapi-0.0.8/simplesheetsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2022-12-14 15:48:41.000000 simplesheetsapi-0.0.8/simplesheetsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-14 15:48:41.000000 simplesheetsapi-0.0.8/simplesheetsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-12-14 15:48:41.000000 simplesheetsapi-0.0.8/simplesheetsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 16:06:46.029681 simplesheetsapi-0.0.9/
+-rw-rw-rw-   0        0        0     1086 2022-11-27 20:46:23.000000 simplesheetsapi-0.0.9/LICENCE
+-rw-rw-rw-   0        0        0     1939 2023-04-17 16:06:46.028680 simplesheetsapi-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1551 2023-04-17 15:19:12.000000 simplesheetsapi-0.0.9/README.md
+-rw-rw-rw-   0        0        0      611 2023-04-17 16:05:41.000000 simplesheetsapi-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 16:06:46.029681 simplesheetsapi-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 16:06:46.013671 simplesheetsapi-0.0.9/simplesheetsapi/
+-rw-rw-rw-   0        0        0     3133 2022-12-14 15:47:03.000000 simplesheetsapi-0.0.9/simplesheetsapi/SheetsApi.py
+-rw-rw-rw-   0        0        0        0 2022-11-27 20:05:19.000000 simplesheetsapi-0.0.9/simplesheetsapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:06:46.027680 simplesheetsapi-0.0.9/simplesheetsapi.egg-info/
+-rw-rw-rw-   0        0        0     1939 2023-04-17 16:06:45.000000 simplesheetsapi-0.0.9/simplesheetsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-04-17 16:06:45.000000 simplesheetsapi-0.0.9/simplesheetsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 16:06:45.000000 simplesheetsapi-0.0.9/simplesheetsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-17 16:06:45.000000 simplesheetsapi-0.0.9/simplesheetsapi.egg-info/top_level.txt
```

### Comparing `simplesheetsapi-0.0.8/LICENCE` & `simplesheetsapi-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `simplesheetsapi-0.0.8/PKG-INFO` & `simplesheetsapi-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplesheetsapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Author-email: Sheets Try <sheetsapitry@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -28,15 +28,15 @@
 + Инициализация:
 ```python 
 sheet = SheetsApiTry("id_таблицы", os.getcwd())
 ```
 
 + Получение содержимого ячейки:
 ```python 
-print(sheet.get_cell_value("колонка", "строка", "название_листа")
+print(sheet.get_cell("колонка", "строка", "название_листа")
 ```
 
 + Установка содержимого ячеек:
 ```python 
 sheet.update_cell("ячейка_начала:ячейка_конца", "название_листа", [[значения_строки_1, ...], [значения_строки_2, ...]])
 ```
```

### Comparing `simplesheetsapi-0.0.8/README.md` & `simplesheetsapi-0.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 + Инициализация:
 ```python 
 sheet = SheetsApiTry("id_таблицы", os.getcwd())
 ```
 
 + Получение содержимого ячейки:
 ```python 
-print(sheet.get_cell_value("колонка", "строка", "название_листа")
+print(sheet.get_cell("колонка", "строка", "название_листа")
 ```
 
 + Установка содержимого ячеек:
 ```python 
 sheet.update_cell("ячейка_начала:ячейка_конца", "название_листа", [[значения_строки_1, ...], [значения_строки_2, ...]])
 ```
```

### Comparing `simplesheetsapi-0.0.8/pyproject.toml` & `simplesheetsapi-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "simplesheetsapi"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Sheets Try", email="sheetsapitry@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplesheetsapi-0.0.8/simplesheetsapi/SheetsApi.py` & `simplesheetsapi-0.0.9/simplesheetsapi/SheetsApi.py`

 * *Files identical despite different names*

### Comparing `simplesheetsapi-0.0.8/simplesheetsapi.egg-info/PKG-INFO` & `simplesheetsapi-0.0.9/simplesheetsapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplesheetsapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Author-email: Sheets Try <sheetsapitry@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -28,15 +28,15 @@
 + Инициализация:
 ```python 
 sheet = SheetsApiTry("id_таблицы", os.getcwd())
 ```
 
 + Получение содержимого ячейки:
 ```python 
-print(sheet.get_cell_value("колонка", "строка", "название_листа")
+print(sheet.get_cell("колонка", "строка", "название_листа")
 ```
 
 + Установка содержимого ячеек:
 ```python 
 sheet.update_cell("ячейка_начала:ячейка_конца", "название_листа", [[значения_строки_1, ...], [значения_строки_2, ...]])
 ```
```

