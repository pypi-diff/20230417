# Comparing `tmp/lamda-3.95.tar.gz` & `tmp/lamda-3.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lamda-3.95.tar", last modified: Wed Feb  1 12:08:53 2023, max compression
+gzip compressed data, was "dist/lamda-3.98.tar", last modified: Sun Feb  5 16:32:07 2023, max compression
```

## Comparing `lamda-3.95.tar` & `lamda-3.98.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2023-02-01 12:08:53.168324 lamda-3.95/
--rw-r--r--   0 whoami    (4096) whoami    (4096)      524 2023-02-01 12:08:53.168324 lamda-3.95/PKG-INFO
--rw-r--r--   0 whoami    (4096) whoami    (4096)    65078 2000-01-01 00:00:00.000000 lamda-3.95/README.md
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2023-02-01 12:08:53.156323 lamda-3.95/lamda/
--rw-r--r--   0 whoami    (4096) whoami    (4096)      207 2000-01-01 00:00:00.000000 lamda-3.95/lamda/__init__.py
--rw-r--r--   0 whoami    (4096) whoami    (4096)      896 2000-01-01 00:00:00.000000 lamda-3.95/lamda/bcast.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)    63887 2000-01-01 00:00:00.000000 lamda-3.95/lamda/client.py
--rw-r--r--   0 whoami    (4096) whoami    (4096)     2211 2000-01-01 00:00:00.000000 lamda-3.95/lamda/const.py
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1420 2000-01-01 00:00:00.000000 lamda-3.95/lamda/exceptions.py
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2023-02-01 12:08:53.152322 lamda-3.95/lamda/google/
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2023-02-01 12:08:53.160323 lamda-3.95/lamda/google/protobuf/
--rw-r--r--   0 whoami    (4096) whoami    (4096)     5916 2000-01-01 00:00:00.000000 lamda-3.95/lamda/google/protobuf/any.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     7734 2000-01-01 00:00:00.000000 lamda-3.95/lamda/google/protobuf/api.proto
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2023-02-01 12:08:53.164323 lamda-3.95/lamda/google/protobuf/compiler/
--rw-r--r--   0 whoami    (4096) whoami    (4096)     8754 2000-01-01 00:00:00.000000 lamda-3.95/lamda/google/protobuf/compiler/plugin.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)    37969 2000-01-01 00:00:00.000000 lamda-3.95/lamda/google/protobuf/descriptor.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     4895 2000-01-01 00:00:00.000000 lamda-3.95/lamda/google/protobuf/duration.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     2429 2000-01-01 00:00:00.000000 lamda-3.95/lamda/google/protobuf/empty.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     8185 2000-01-01 00:00:00.000000 lamda-3.95/lamda/google/protobuf/field_mask.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     2341 2000-01-01 00:00:00.000000 lamda-3.95/lamda/google/protobuf/source_context.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     3778 2000-01-01 00:00:00.000000 lamda-3.95/lamda/google/protobuf/struct.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     6459 2000-01-01 00:00:00.000000 lamda-3.95/lamda/google/protobuf/timestamp.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     6126 2000-01-01 00:00:00.000000 lamda-3.95/lamda/google/protobuf/type.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     4042 2000-01-01 00:00:00.000000 lamda-3.95/lamda/google/protobuf/wrappers.proto
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2023-02-01 12:08:53.168324 lamda-3.95/lamda/rpc/
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1854 2000-01-01 00:00:00.000000 lamda-3.95/lamda/rpc/application.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      432 2000-01-01 00:00:00.000000 lamda-3.95/lamda/rpc/debug.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      712 2000-01-01 00:00:00.000000 lamda-3.95/lamda/rpc/file.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      377 2000-01-01 00:00:00.000000 lamda-3.95/lamda/rpc/policy.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     2460 2000-01-01 00:00:00.000000 lamda-3.95/lamda/rpc/proxy.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)    11194 2000-01-01 00:00:00.000000 lamda-3.95/lamda/rpc/services.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      468 2000-01-01 00:00:00.000000 lamda-3.95/lamda/rpc/settings.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      544 2000-01-01 00:00:00.000000 lamda-3.95/lamda/rpc/shell.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1884 2000-01-01 00:00:00.000000 lamda-3.95/lamda/rpc/status.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      420 2000-01-01 00:00:00.000000 lamda-3.95/lamda/rpc/types.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)    18718 2000-01-01 00:00:00.000000 lamda-3.95/lamda/rpc/uiautomator.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1064 2000-01-01 00:00:00.000000 lamda-3.95/lamda/rpc/util.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1777 2000-01-01 00:00:00.000000 lamda-3.95/lamda/rpc/wifi.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1009 2000-01-01 00:00:00.000000 lamda-3.95/lamda/types.py
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2023-02-01 12:08:53.156323 lamda-3.95/lamda.egg-info/
--rw-r--r--   0 whoami    (4096) whoami    (4096)      524 2023-02-01 12:08:53.000000 lamda-3.95/lamda.egg-info/PKG-INFO
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1038 2023-02-01 12:08:53.000000 lamda-3.95/lamda.egg-info/SOURCES.txt
--rw-r--r--   0 whoami    (4096) whoami    (4096)        1 2023-02-01 12:08:53.000000 lamda-3.95/lamda.egg-info/dependency_links.txt
--rw-r--r--   0 whoami    (4096) whoami    (4096)        1 2023-02-01 12:08:53.000000 lamda-3.95/lamda.egg-info/not-zip-safe
--rw-r--r--   0 whoami    (4096) whoami    (4096)      211 2023-02-01 12:08:53.000000 lamda-3.95/lamda.egg-info/requires.txt
--rw-r--r--   0 whoami    (4096) whoami    (4096)        6 2023-02-01 12:08:53.000000 lamda-3.95/lamda.egg-info/top_level.txt
--rw-r--r--   0 whoami    (4096) whoami    (4096)       38 2023-02-01 12:08:53.168324 lamda-3.95/setup.cfg
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1531 2000-01-01 00:00:00.000000 lamda-3.95/setup.py
+drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2023-02-05 16:32:07.451433 lamda-3.98/
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      524 2023-02-05 16:32:07.451433 lamda-3.98/PKG-INFO
+-rw-r--r--   0 whoami    (4096) whoami    (4096)    64429 2000-01-01 00:00:00.000000 lamda-3.98/README.md
+drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2023-02-05 16:32:07.439432 lamda-3.98/lamda/
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      207 2000-01-01 00:00:00.000000 lamda-3.98/lamda/__init__.py
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      896 2000-01-01 00:00:00.000000 lamda-3.98/lamda/bcast.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)    63887 2000-01-01 00:00:00.000000 lamda-3.98/lamda/client.py
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     2211 2000-01-01 00:00:00.000000 lamda-3.98/lamda/const.py
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     1420 2000-01-01 00:00:00.000000 lamda-3.98/lamda/exceptions.py
+drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2023-02-05 16:32:07.431431 lamda-3.98/lamda/google/
+drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2023-02-05 16:32:07.447433 lamda-3.98/lamda/google/protobuf/
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     5916 2000-01-01 00:00:00.000000 lamda-3.98/lamda/google/protobuf/any.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     7734 2000-01-01 00:00:00.000000 lamda-3.98/lamda/google/protobuf/api.proto
+drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2023-02-05 16:32:07.447433 lamda-3.98/lamda/google/protobuf/compiler/
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     8754 2000-01-01 00:00:00.000000 lamda-3.98/lamda/google/protobuf/compiler/plugin.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)    37969 2000-01-01 00:00:00.000000 lamda-3.98/lamda/google/protobuf/descriptor.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     4895 2000-01-01 00:00:00.000000 lamda-3.98/lamda/google/protobuf/duration.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     2429 2000-01-01 00:00:00.000000 lamda-3.98/lamda/google/protobuf/empty.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     8185 2000-01-01 00:00:00.000000 lamda-3.98/lamda/google/protobuf/field_mask.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     2341 2000-01-01 00:00:00.000000 lamda-3.98/lamda/google/protobuf/source_context.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     3778 2000-01-01 00:00:00.000000 lamda-3.98/lamda/google/protobuf/struct.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     6459 2000-01-01 00:00:00.000000 lamda-3.98/lamda/google/protobuf/timestamp.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     6126 2000-01-01 00:00:00.000000 lamda-3.98/lamda/google/protobuf/type.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     4042 2000-01-01 00:00:00.000000 lamda-3.98/lamda/google/protobuf/wrappers.proto
+drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2023-02-05 16:32:07.451433 lamda-3.98/lamda/rpc/
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     1854 2000-01-01 00:00:00.000000 lamda-3.98/lamda/rpc/application.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      432 2000-01-01 00:00:00.000000 lamda-3.98/lamda/rpc/debug.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      712 2000-01-01 00:00:00.000000 lamda-3.98/lamda/rpc/file.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      377 2000-01-01 00:00:00.000000 lamda-3.98/lamda/rpc/policy.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     2460 2000-01-01 00:00:00.000000 lamda-3.98/lamda/rpc/proxy.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)    11194 2000-01-01 00:00:00.000000 lamda-3.98/lamda/rpc/services.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      468 2000-01-01 00:00:00.000000 lamda-3.98/lamda/rpc/settings.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      544 2000-01-01 00:00:00.000000 lamda-3.98/lamda/rpc/shell.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     1884 2000-01-01 00:00:00.000000 lamda-3.98/lamda/rpc/status.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      420 2000-01-01 00:00:00.000000 lamda-3.98/lamda/rpc/types.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)    18718 2000-01-01 00:00:00.000000 lamda-3.98/lamda/rpc/uiautomator.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     1064 2000-01-01 00:00:00.000000 lamda-3.98/lamda/rpc/util.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     1777 2000-01-01 00:00:00.000000 lamda-3.98/lamda/rpc/wifi.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     1009 2000-01-01 00:00:00.000000 lamda-3.98/lamda/types.py
+drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2023-02-05 16:32:07.439432 lamda-3.98/lamda.egg-info/
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      524 2023-02-05 16:32:07.000000 lamda-3.98/lamda.egg-info/PKG-INFO
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     1038 2023-02-05 16:32:07.000000 lamda-3.98/lamda.egg-info/SOURCES.txt
+-rw-r--r--   0 whoami    (4096) whoami    (4096)        1 2023-02-05 16:32:07.000000 lamda-3.98/lamda.egg-info/dependency_links.txt
+-rw-r--r--   0 whoami    (4096) whoami    (4096)        1 2023-02-05 16:32:07.000000 lamda-3.98/lamda.egg-info/not-zip-safe
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      211 2023-02-05 16:32:07.000000 lamda-3.98/lamda.egg-info/requires.txt
+-rw-r--r--   0 whoami    (4096) whoami    (4096)        6 2023-02-05 16:32:07.000000 lamda-3.98/lamda.egg-info/top_level.txt
+-rw-r--r--   0 whoami    (4096) whoami    (4096)       38 2023-02-05 16:32:07.451433 lamda-3.98/setup.cfg
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     1531 2000-01-01 00:00:00.000000 lamda-3.98/setup.py
```

### Comparing `lamda-3.95/PKG-INFO` & `lamda-3.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamda
-Version: 3.95
+Version: 3.98
 Summary: Android reverse engineering & automation framework
 Home-page: https://github.com/rev1si0n/lamda
 Author: rev1si0n
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lamda-3.95/README.md` & `lamda-3.98/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -688,44 +688,37 @@
 
 ```bash
 # jnitrace 示例连接方法 (-R 192.168.0.2:65000)
 jnitrace -R 192.168.0.2:65000 -l libc.so com.some.package
 ```
 
 ```bash
-# frida-dexdump 示例连接方法 (-H 192.168.0.2:65000)
-frida-dexdump -H 192.168.0.2:65000 -p PID
+# hooker 示例连接方法 (-H 192.168.0.2:65000)
+# 修改 .hooker_driver 内容为 -H 192.168.0.2:65000 即可
 ```
 
 ```bash
-# hooker 示例连接方法 (-H 192.168.0.2:65000)
-# 修改 .hooker_driver 文件的内容为 -H 192.168.0.2:65000 即可
+# frida-dexdump 示例连接方法 (-H 192.168.0.2:65000)
+frida-dexdump -H 192.168.0.2:65000 -p PID
 ```
 
 其他未提及的第三方工具请自行查看其使用方法。
 
 ## 使用自带的 crontab (定时任务)
 
 内置了用于执行定时任务的 cron 服务，这样你可以在设备上定期执行一些脚本，所有规则都将以 root 身份执行。
 
-> 此功能需要你会编写 crontab 规则以及基础的 linux 命令行编辑文件的能力。
-> **注意**：受限于安卓休眠机制，息屏后定时任务可能并不会以你期望的时间运行，你可能需要将设备设置为常亮。
-
-注意这与你在 linux 使用 crontab 并不相同，在 linux 正常使用 `crontab -e` 命令
-来编辑任务，但是框架并未提供此命令，你需要直接编辑文件来写入规则（道理是相同的，都是编辑文件而已）
-
-现在，请打开 web 控制台或者连接设备的 ssh/adb shell，执行命令 `cd` 来切换到家目录。
-此时家目录中有个名为 crontab 的文件夹。执行命令 `busybox vi crontab/jobs`，你将进入编辑文件，在英文输入模式下按下字母 `i`，随后写下相关规则，并按下 `ESC`，`SHIFT` + `:`，输入 `wq` 并按下回车来保存。你可以在这个 jobs 文件中写入多行，同样，你也可以在这个文件夹下创建其他名字的规则文件。
+> 此功能需要你会编写 crontab 规则。
 
-如果你还是不懂怎么编辑，请在电脑编辑完成后使用adb转移到此目录。
+现在，请打开 web 控制台或者连接设备的 ssh/adb shell，执行命令 `crontab -e`，你将进入编辑模式，在英文输入模式下按下字母 `i`，随后写下相关规则，并依次按下 `ESC`，`SHIFT` + `:`，输入 `wq` 并按下回车来保存即可。受限于安卓休眠机制，息屏后定时任务可能并不会以你期望的时间运行，你可能需要将设备设置为常亮。
 
 > 一些规则示例
 
 ```
-@reboot      echo 每次框架启动/重载(reload)时执行
+@reboot      echo 框架启动/重载(reload)时执行
 0 */1 * * *  echo 每一小时执行
 * * * * *    echo 每一分钟执行
 0 8 * * *    echo 每天八点执行
 ```
 
 ## 通过 frida 暴露内部 Java/Jni 接口（类sekiro）
```

### Comparing `lamda-3.95/lamda/bcast.proto` & `lamda-3.98/lamda/bcast.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/client.py` & `lamda-3.98/lamda/client.py`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/const.py` & `lamda-3.98/lamda/const.py`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/exceptions.py` & `lamda-3.98/lamda/exceptions.py`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/google/protobuf/any.proto` & `lamda-3.98/lamda/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/google/protobuf/api.proto` & `lamda-3.98/lamda/google/protobuf/api.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/google/protobuf/compiler/plugin.proto` & `lamda-3.98/lamda/google/protobuf/compiler/plugin.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/google/protobuf/descriptor.proto` & `lamda-3.98/lamda/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/google/protobuf/duration.proto` & `lamda-3.98/lamda/google/protobuf/duration.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/google/protobuf/empty.proto` & `lamda-3.98/lamda/google/protobuf/empty.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/google/protobuf/field_mask.proto` & `lamda-3.98/lamda/google/protobuf/field_mask.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/google/protobuf/source_context.proto` & `lamda-3.98/lamda/google/protobuf/source_context.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/google/protobuf/struct.proto` & `lamda-3.98/lamda/google/protobuf/struct.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/google/protobuf/timestamp.proto` & `lamda-3.98/lamda/google/protobuf/timestamp.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/google/protobuf/type.proto` & `lamda-3.98/lamda/google/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/google/protobuf/wrappers.proto` & `lamda-3.98/lamda/google/protobuf/wrappers.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/rpc/application.proto` & `lamda-3.98/lamda/rpc/application.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/rpc/file.proto` & `lamda-3.98/lamda/rpc/file.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/rpc/proxy.proto` & `lamda-3.98/lamda/rpc/proxy.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/rpc/services.proto` & `lamda-3.98/lamda/rpc/services.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/rpc/shell.proto` & `lamda-3.98/lamda/rpc/shell.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/rpc/status.proto` & `lamda-3.98/lamda/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/rpc/uiautomator.proto` & `lamda-3.98/lamda/rpc/uiautomator.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/rpc/util.proto` & `lamda-3.98/lamda/rpc/util.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/rpc/wifi.proto` & `lamda-3.98/lamda/rpc/wifi.proto`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda/types.py` & `lamda-3.98/lamda/types.py`

 * *Files identical despite different names*

### Comparing `lamda-3.95/lamda.egg-info/PKG-INFO` & `lamda-3.98/lamda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamda
-Version: 3.95
+Version: 3.98
 Summary: Android reverse engineering & automation framework
 Home-page: https://github.com/rev1si0n/lamda
 Author: rev1si0n
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lamda-3.95/lamda.egg-info/SOURCES.txt` & `lamda-3.98/lamda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lamda-3.95/setup.py` & `lamda-3.98/setup.py`

 * *Files identical despite different names*

