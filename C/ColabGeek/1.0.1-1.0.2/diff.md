# Comparing `tmp/ColabGeek-1.0.1.tar.gz` & `tmp/ColabGeek-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ColabGeek-1.0.1.tar", last modified: Mon Apr 10 10:18:45 2023, max compression
+gzip compressed data, was "ColabGeek-1.0.2.tar", last modified: Mon Apr 17 11:27:43 2023, max compression
```

## Comparing `ColabGeek-1.0.1.tar` & `ColabGeek-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:18:45.395829 ColabGeek-1.0.1/
--rw-rw-r--   0 root         (0) root         (0)     1067 2023-04-10 10:11:42.000000 ColabGeek-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5169 2023-04-10 10:18:45.395829 ColabGeek-1.0.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4432 2023-04-10 10:11:42.000000 ColabGeek-1.0.1/README.md
--rw-rw-r--   0 root         (0) root         (0)      939 2023-04-10 10:11:42.000000 ColabGeek-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 10:18:45.395829 ColabGeek-1.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:18:45.392829 ColabGeek-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:18:45.393828 ColabGeek-1.0.1/src/ColabGeek/
--rw-rw-r--   0 root         (0) root         (0)     6335 2023-04-10 10:11:42.000000 ColabGeek-1.0.1/src/ColabGeek/ColabGeek.py
--rw-rw-r--   0 root         (0) root         (0)       24 2023-04-10 10:11:42.000000 ColabGeek-1.0.1/src/ColabGeek/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:18:45.394829 ColabGeek-1.0.1/src/ColabGeek/shell_scripts/
--rw-rw-r--   0 root         (0) root         (0)      382 2023-04-10 10:11:42.000000 ColabGeek-1.0.1/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
--rw-rw-r--   0 root         (0) root         (0)     1192 2023-04-10 10:11:42.000000 ColabGeek-1.0.1/src/ColabGeek/shell_scripts/Run_code_server.exp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:18:45.394829 ColabGeek-1.0.1/src/ColabGeek.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5169 2023-04-10 10:18:45.000000 ColabGeek-1.0.1/src/ColabGeek.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-04-10 10:18:45.000000 ColabGeek-1.0.1/src/ColabGeek.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 10:18:45.000000 ColabGeek-1.0.1/src/ColabGeek.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-10 10:18:45.000000 ColabGeek-1.0.1/src/ColabGeek.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:27:43.284695 ColabGeek-1.0.2/
+-rw-rw-r--   0 root         (0) root         (0)     1067 2023-04-17 10:15:07.000000 ColabGeek-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-04-17 11:27:43.284695 ColabGeek-1.0.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4417 2023-04-17 11:20:28.000000 ColabGeek-1.0.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)      939 2023-04-17 11:20:28.000000 ColabGeek-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 11:27:43.284695 ColabGeek-1.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:27:43.282695 ColabGeek-1.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:27:43.283695 ColabGeek-1.0.2/src/ColabGeek/
+-rw-rw-r--   0 root         (0) root         (0)     6650 2023-04-17 11:20:28.000000 ColabGeek-1.0.2/src/ColabGeek/ColabGeek.py
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-04-17 10:15:07.000000 ColabGeek-1.0.2/src/ColabGeek/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:27:43.284695 ColabGeek-1.0.2/src/ColabGeek/shell_scripts/
+-rw-rw-r--   0 root         (0) root         (0)      382 2023-04-17 10:15:07.000000 ColabGeek-1.0.2/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
+-rw-rw-r--   0 root         (0) root         (0)     1192 2023-04-17 10:15:07.000000 ColabGeek-1.0.2/src/ColabGeek/shell_scripts/Run_code_server.exp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:27:43.283695 ColabGeek-1.0.2/src/ColabGeek.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-04-17 11:27:43.000000 ColabGeek-1.0.2/src/ColabGeek.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-04-17 11:27:43.000000 ColabGeek-1.0.2/src/ColabGeek.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 11:27:43.000000 ColabGeek-1.0.2/src/ColabGeek.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-17 11:27:43.000000 ColabGeek-1.0.2/src/ColabGeek.egg-info/top_level.txt
```

### Comparing `ColabGeek-1.0.1/LICENSE` & `ColabGeek-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.0.1/PKG-INFO` & `ColabGeek-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColabGeek
-Version: 1.0.1
+Version: 1.0.2
 Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
 Author-email: Yiming Sun <yiming.sun12138@gmail.com>
 Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
 Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -25,25 +25,23 @@
 ## Get started
 
 First load the ColabGeek module and update all the packages and dependencies in the system.
 
 ```python
 import ColabGeek
 
-GolabGeek.update_environment()
+ColabGeek.update_environment()
 ```
 
 Initiate the Colab session by add linux users and mount Google Drive.
 
 ```python
 main = ColabGeek.ColabSession(user='Knight',password='midnight',mount_GD=True)
 ```
 
-***
-
 As a cloud computing platform based on Jupyter notebooks, Google Colab does not provide a top-notch comfortable environment for R language data analysis and other non-Python programming. Therefore, this project provides a method for quickly installing other web IDE on Google Colab, enabling it to expand its range of capabilities.
 
 ### Run code server
 
 [code server](https://github.com/coder/code-server) is a web IDE provided by Coder that enables developers to write, run and debug code from a web browser. It is built on the open-source Visual Studio Code editor and offers many of the same features, such as code highlighting, auto completion, and debugging.
 
 ```python
@@ -63,16 +61,14 @@
 # ColabGeek.Run_Rstudio_server has the following parameters:
 # - port The port you want to run Rstudio on, set to None to use the default port.
 # - verbose Show the running logs.
 
 main.Run_Rstudio_server()
 ```
 
-***
-
 Google Colab does not allow any internet connections to their servers except the official web interface. So, port forwarding methods are required to proxy the web IDE installed.
 
 ### localtunnel
 
 ```python
 # ColabGeek.Run_localtunnel has the following parameters:
 # - port The port you want to expose to localtunnel, set to None and you will use the default port.
@@ -91,16 +87,14 @@
 # - domain The customized ngrok URL, check the ngrok document.
 
 main.Run_ngrok()
 ```
 
 For now, all the port forwarding methods built in ColabGeek only accept http protocal. I am still tring to add TCP forwarding methods to ColabGeek. If you have any good ideas and advices, leave an issue.
 
-***
-
 ### shadowsocks
 
 Although not allowed by Google and not recommended by myself, building a proxy server using Colab sounds pretty 'Geek'. However, due to the lack of TCP forwarding method, ColabGeek can now only install shadowsocks on Colab but have no method to help to connect it. Just use this method on your own Ubuntu servers, that should work.
 
 ```python
 # ColabGeek.Run_shadowsocks has the following parameters:
 # - port The server port of shadowsocks, set to None and you will use the default port.
```

### Comparing `ColabGeek-1.0.1/README.md` & `ColabGeek-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,23 @@
 ## Get started
 
 First load the ColabGeek module and update all the packages and dependencies in the system.
 
 ```python
 import ColabGeek
 
-GolabGeek.update_environment()
+ColabGeek.update_environment()
 ```
 
 Initiate the Colab session by add linux users and mount Google Drive.
 
 ```python
 main = ColabGeek.ColabSession(user='Knight',password='midnight',mount_GD=True)
 ```
 
-***
-
 As a cloud computing platform based on Jupyter notebooks, Google Colab does not provide a top-notch comfortable environment for R language data analysis and other non-Python programming. Therefore, this project provides a method for quickly installing other web IDE on Google Colab, enabling it to expand its range of capabilities.
 
 ### Run code server
 
 [code server](https://github.com/coder/code-server) is a web IDE provided by Coder that enables developers to write, run and debug code from a web browser. It is built on the open-source Visual Studio Code editor and offers many of the same features, such as code highlighting, auto completion, and debugging.
 
 ```python
@@ -49,16 +47,14 @@
 # ColabGeek.Run_Rstudio_server has the following parameters:
 # - port The port you want to run Rstudio on, set to None to use the default port.
 # - verbose Show the running logs.
 
 main.Run_Rstudio_server()
 ```
 
-***
-
 Google Colab does not allow any internet connections to their servers except the official web interface. So, port forwarding methods are required to proxy the web IDE installed.
 
 ### localtunnel
 
 ```python
 # ColabGeek.Run_localtunnel has the following parameters:
 # - port The port you want to expose to localtunnel, set to None and you will use the default port.
@@ -77,16 +73,14 @@
 # - domain The customized ngrok URL, check the ngrok document.
 
 main.Run_ngrok()
 ```
 
 For now, all the port forwarding methods built in ColabGeek only accept http protocal. I am still tring to add TCP forwarding methods to ColabGeek. If you have any good ideas and advices, leave an issue.
 
-***
-
 ### shadowsocks
 
 Although not allowed by Google and not recommended by myself, building a proxy server using Colab sounds pretty 'Geek'. However, due to the lack of TCP forwarding method, ColabGeek can now only install shadowsocks on Colab but have no method to help to connect it. Just use this method on your own Ubuntu servers, that should work.
 
 ```python
 # ColabGeek.Run_shadowsocks has the following parameters:
 # - port The server port of shadowsocks, set to None and you will use the default port.
```

### Comparing `ColabGeek-1.0.1/pyproject.toml` & `ColabGeek-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 "ColabGeek.shell_scripts" = ["*"]
 
 [project]
 name = "ColabGeek"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     {name = "Yiming Sun",email = "yiming.sun12138@gmail.com"},
 ]
 description = "ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ColabGeek-1.0.1/src/ColabGeek/ColabGeek.py` & `ColabGeek-1.0.2/src/ColabGeek/ColabGeek.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,16 +27,23 @@
         self.tmp_path()
 
     '''
     init methods
     '''
     # add user method
     def add_user(self):
-        os.system("useradd -m -s /bin/bash" + " " + str(self.user))
+        # check user list
+        user_list = os.popen("getent passwd | awk -F: '{print $1}'").readlines()
+        for i in range(0,len(user_list)):
+            user_list[i] = user_list[i].replace("\n","")
+        if (str(self.user) not in user_list):
+            os.system("useradd -m -s /bin/bash" + " " + str(self.user))
+        # change user passwd
         os.system("echo '" + str(self.user) + ":" + str(self.password) + "' | chpasswd")
+        # add sudo permission
         if self.sudo:
             os.system("usermod -G sudo" + " " + str(self.user))
 
     # mount Google Drive method
     def Google_Drive(self):
         if self.mount_GD:
             from google.colab import drive
```

### Comparing `ColabGeek-1.0.1/src/ColabGeek/shell_scripts/Run_code_server.exp` & `ColabGeek-1.0.2/src/ColabGeek/shell_scripts/Run_code_server.exp`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.0.1/src/ColabGeek.egg-info/PKG-INFO` & `ColabGeek-1.0.2/src/ColabGeek.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColabGeek
-Version: 1.0.1
+Version: 1.0.2
 Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
 Author-email: Yiming Sun <yiming.sun12138@gmail.com>
 Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
 Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -25,25 +25,23 @@
 ## Get started
 
 First load the ColabGeek module and update all the packages and dependencies in the system.
 
 ```python
 import ColabGeek
 
-GolabGeek.update_environment()
+ColabGeek.update_environment()
 ```
 
 Initiate the Colab session by add linux users and mount Google Drive.
 
 ```python
 main = ColabGeek.ColabSession(user='Knight',password='midnight',mount_GD=True)
 ```
 
-***
-
 As a cloud computing platform based on Jupyter notebooks, Google Colab does not provide a top-notch comfortable environment for R language data analysis and other non-Python programming. Therefore, this project provides a method for quickly installing other web IDE on Google Colab, enabling it to expand its range of capabilities.
 
 ### Run code server
 
 [code server](https://github.com/coder/code-server) is a web IDE provided by Coder that enables developers to write, run and debug code from a web browser. It is built on the open-source Visual Studio Code editor and offers many of the same features, such as code highlighting, auto completion, and debugging.
 
 ```python
@@ -63,16 +61,14 @@
 # ColabGeek.Run_Rstudio_server has the following parameters:
 # - port The port you want to run Rstudio on, set to None to use the default port.
 # - verbose Show the running logs.
 
 main.Run_Rstudio_server()
 ```
 
-***
-
 Google Colab does not allow any internet connections to their servers except the official web interface. So, port forwarding methods are required to proxy the web IDE installed.
 
 ### localtunnel
 
 ```python
 # ColabGeek.Run_localtunnel has the following parameters:
 # - port The port you want to expose to localtunnel, set to None and you will use the default port.
@@ -91,16 +87,14 @@
 # - domain The customized ngrok URL, check the ngrok document.
 
 main.Run_ngrok()
 ```
 
 For now, all the port forwarding methods built in ColabGeek only accept http protocal. I am still tring to add TCP forwarding methods to ColabGeek. If you have any good ideas and advices, leave an issue.
 
-***
-
 ### shadowsocks
 
 Although not allowed by Google and not recommended by myself, building a proxy server using Colab sounds pretty 'Geek'. However, due to the lack of TCP forwarding method, ColabGeek can now only install shadowsocks on Colab but have no method to help to connect it. Just use this method on your own Ubuntu servers, that should work.
 
 ```python
 # ColabGeek.Run_shadowsocks has the following parameters:
 # - port The server port of shadowsocks, set to None and you will use the default port.
```

