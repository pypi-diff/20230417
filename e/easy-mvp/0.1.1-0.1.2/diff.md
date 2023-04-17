# Comparing `tmp/easy_mvp-0.1.1.tar.gz` & `tmp/easy_mvp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_mvp-0.1.1.tar", last modified: Fri Dec 16 18:08:31 2022, max compression
+gzip compressed data, was "easy_mvp-0.1.2.tar", last modified: Mon Apr 17 19:25:21 2023, max compression
```

## Comparing `easy_mvp-0.1.1.tar` & `easy_mvp-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 roly      (1000) roly      (1000)        0 2022-12-16 18:08:31.106510 easy_mvp-0.1.1/
--rw-rw-r--   0 roly      (1000) roly      (1000)     1080 2022-12-16 15:34:30.000000 easy_mvp-0.1.1/LICENSE
--rw-rw-r--   0 roly      (1000) roly      (1000)     9378 2022-12-16 18:08:31.106510 easy_mvp-0.1.1/PKG-INFO
--rw-rw-r--   0 roly      (1000) roly      (1000)     8954 2022-12-16 15:34:30.000000 easy_mvp-0.1.1/README.md
--rw-rw-r--   0 roly      (1000) roly      (1000)       85 2022-12-16 15:34:30.000000 easy_mvp-0.1.1/pyproject.toml
--rw-rw-r--   0 roly      (1000) roly      (1000)      610 2022-12-16 18:08:31.106510 easy_mvp-0.1.1/setup.cfg
-drwxrwxr-x   0 roly      (1000) roly      (1000)        0 2022-12-16 18:08:31.102510 easy_mvp-0.1.1/src/
-drwxrwxr-x   0 roly      (1000) roly      (1000)        0 2022-12-16 18:08:31.106510 easy_mvp-0.1.1/src/easy_mvp/
--rw-rw-r--   0 roly      (1000) roly      (1000)        0 2022-12-16 15:34:30.000000 easy_mvp-0.1.1/src/easy_mvp/__init__.py
--rw-rw-r--   0 roly      (1000) roly      (1000)     2601 2022-12-16 15:34:30.000000 easy_mvp-0.1.1/src/easy_mvp/abstract_presenter.py
--rw-rw-r--   0 roly      (1000) roly      (1000)     1421 2022-12-16 15:34:30.000000 easy_mvp-0.1.1/src/easy_mvp/application_manager.py
--rw-rw-r--   0 roly      (1000) roly      (1000)      980 2022-12-16 15:34:30.000000 easy_mvp-0.1.1/src/easy_mvp/exception.py
--rw-rw-r--   0 roly      (1000) roly      (1000)     1046 2022-12-16 15:34:30.000000 easy_mvp-0.1.1/src/easy_mvp/intent.py
--rw-rw-r--   0 roly      (1000) roly      (1000)     7939 2022-12-16 17:56:33.000000 easy_mvp-0.1.1/src/easy_mvp/window.py
-drwxrwxr-x   0 roly      (1000) roly      (1000)        0 2022-12-16 18:08:31.106510 easy_mvp-0.1.1/src/easy_mvp.egg-info/
--rw-rw-r--   0 roly      (1000) roly      (1000)     9378 2022-12-16 18:08:31.000000 easy_mvp-0.1.1/src/easy_mvp.egg-info/PKG-INFO
--rw-rw-r--   0 roly      (1000) roly      (1000)      389 2022-12-16 18:08:31.000000 easy_mvp-0.1.1/src/easy_mvp.egg-info/SOURCES.txt
--rw-rw-r--   0 roly      (1000) roly      (1000)        1 2022-12-16 18:08:31.000000 easy_mvp-0.1.1/src/easy_mvp.egg-info/dependency_links.txt
--rw-rw-r--   0 roly      (1000) roly      (1000)       14 2022-12-16 18:08:31.000000 easy_mvp-0.1.1/src/easy_mvp.egg-info/requires.txt
--rw-rw-r--   0 roly      (1000) roly      (1000)        9 2022-12-16 18:08:31.000000 easy_mvp-0.1.1/src/easy_mvp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:25:21.921742 easy_mvp-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-17 19:25:21.921742 easy_mvp-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-17 19:25:21.925742 easy_mvp-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:25:21.921742 easy_mvp-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:25:21.921742 easy_mvp-0.1.2/src/easy_mvp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/src/easy_mvp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/src/easy_mvp/abstract_presenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/src/easy_mvp/application_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/src/easy_mvp/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/src/easy_mvp/intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-04-17 19:25:11.000000 easy_mvp-0.1.2/src/easy_mvp/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:25:21.921742 easy_mvp-0.1.2/src/easy_mvp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-17 19:25:21.000000 easy_mvp-0.1.2/src/easy_mvp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-17 19:25:21.000000 easy_mvp-0.1.2/src/easy_mvp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:25:21.000000 easy_mvp-0.1.2/src/easy_mvp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 19:25:21.000000 easy_mvp-0.1.2/src/easy_mvp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 19:25:21.000000 easy_mvp-0.1.2/src/easy_mvp.egg-info/top_level.txt
```

### Comparing `easy_mvp-0.1.1/LICENSE` & `easy_mvp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_mvp-0.1.1/PKG-INFO` & `easy_mvp-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_mvp
-Version: 0.1.1
+Version: 0.1.2
 Summary: Construct MVP PyQt5 application easily
 Home-page: https://github.com/R0land013/easy-mvp
 Author: Rolando Rio Garaboa
 Author-email: rolandorio06@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `easy_mvp-0.1.1/README.md` & `easy_mvp-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `easy_mvp-0.1.1/setup.cfg` & `easy_mvp-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easy_mvp
-version = 0.1.1
+version = 0.1.2
 author = Rolando Rio Garaboa
 author_email = rolandorio06@gmail.com
 description = Construct MVP PyQt5 application easily
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/R0land013/easy-mvp
 classifiers =
```

### Comparing `easy_mvp-0.1.1/src/easy_mvp/abstract_presenter.py` & `easy_mvp-0.1.2/src/easy_mvp/abstract_presenter.py`

 * *Files identical despite different names*

### Comparing `easy_mvp-0.1.1/src/easy_mvp/application_manager.py` & `easy_mvp-0.1.2/src/easy_mvp/application_manager.py`

 * *Files identical despite different names*

### Comparing `easy_mvp-0.1.1/src/easy_mvp/exception.py` & `easy_mvp-0.1.2/src/easy_mvp/exception.py`

 * *Files identical despite different names*

### Comparing `easy_mvp-0.1.1/src/easy_mvp/intent.py` & `easy_mvp-0.1.2/src/easy_mvp/intent.py`

 * *Files identical despite different names*

### Comparing `easy_mvp-0.1.1/src/easy_mvp/window.py` & `easy_mvp-0.1.2/src/easy_mvp/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,23 @@
 
 
 class StackWindow(QStackedWidget):
 
     def __init__(self, window_handler):
         super().__init__()
         self.__window_handler = window_handler
+        self.__already_notified_on_closing: bool = False
 
     def closeEvent(self, event: QCloseEvent):
-        super().closeEvent(event)
+        if self.__already_notified_on_closing:
+            super().closeEvent(event)
+        else:
+            self.__already_notified_on_closing = True
+            self.__window_handler.close_handler_and_send_all_notifications()
+
 
 
 class WindowHandler:
 
     def __init__(self, application_manager, parent_window=None):
         self.__presenter_stack = []
         self.__parent_window = None
@@ -191,7 +197,27 @@
         self.__child_windows.append(child_window)
 
     def remove_child_window(self, child_window):
         self.__child_windows.remove(child_window)
 
     def set_window_title(self, window_title: str):
         self.__stacked_widget.setWindowTitle(window_title)
+
+    def close_handler_and_send_all_notifications(self):
+        """
+        Notify all presenters of the child windows with on_window_closing,
+        later close the child windows.
+        Then do the same on the presenter of this window and close this window.
+        """
+        for child_window_handler in self.__child_windows:
+            child_window_handler.close_window()
+
+        self.__child_windows = []
+
+        self.notify_all_presenters_on_window_closing()
+        self.close_window()
+
+
+    def notify_all_presenters_on_window_closing(self):
+        base_stack_index = (len(self.__presenter_stack) + 1) * -1
+        for presenter_index in range(-1, base_stack_index, -1):
+            self.__presenter_stack[presenter_index].on_window_closing()
```

### Comparing `easy_mvp-0.1.1/src/easy_mvp.egg-info/PKG-INFO` & `easy_mvp-0.1.2/src/easy_mvp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-mvp
-Version: 0.1.1
+Version: 0.1.2
 Summary: Construct MVP PyQt5 application easily
 Home-page: https://github.com/R0land013/easy-mvp
 Author: Rolando Rio Garaboa
 Author-email: rolandorio06@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

