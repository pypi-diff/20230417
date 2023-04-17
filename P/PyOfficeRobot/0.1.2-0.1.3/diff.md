# Comparing `tmp/PyOfficeRobot-0.1.2.tar.gz` & `tmp/PyOfficeRobot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyOfficeRobot-0.1.2.tar", last modified: Sun Mar 19 12:08:28 2023, max compression
+gzip compressed data, was "PyOfficeRobot-0.1.3.tar", last modified: Mon Apr 17 13:43:48 2023, max compression
```

## Comparing `PyOfficeRobot-0.1.2.tar` & `PyOfficeRobot-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-03-19 12:08:28.202337 PyOfficeRobot-0.1.2/
--rw-rw-rw-   0        0        0     1093 2022-09-09 17:29:26.000000 PyOfficeRobot-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     7729 2023-03-19 12:08:28.202337 PyOfficeRobot-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-19 12:08:28.118454 PyOfficeRobot-0.1.2/PyOfficeRobot/
--rw-rw-rw-   0        0        0      122 2023-02-13 13:46:39.000000 PyOfficeRobot-0.1.2/PyOfficeRobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 12:08:28.169089 PyOfficeRobot-0.1.2/PyOfficeRobot/api/
--rw-rw-rw-   0        0        0        0 2022-09-09 17:57:22.000000 PyOfficeRobot-0.1.2/PyOfficeRobot/api/__init__.py
--rw-rw-rw-   0        0        0     3834 2023-03-19 10:39:04.000000 PyOfficeRobot-0.1.2/PyOfficeRobot/api/chat.py
--rw-rw-rw-   0        0        0     6885 2023-02-24 16:03:39.000000 PyOfficeRobot-0.1.2/PyOfficeRobot/api/file.py
-drwxrwxrwx   0        0        0        0 2023-03-19 12:08:28.177586 PyOfficeRobot-0.1.2/PyOfficeRobot/core/
--rw-rw-rw-   0        0        0    11727 2022-09-26 13:46:19.000000 PyOfficeRobot-0.1.2/PyOfficeRobot/core/WeChatType.py
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.2/PyOfficeRobot/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 12:08:28.183120 PyOfficeRobot-0.1.2/PyOfficeRobot/lib/
--rw-rw-rw-   0        0        0      117 2023-03-19 07:06:10.000000 PyOfficeRobot-0.1.2/PyOfficeRobot/lib/CONST.py
--rw-rw-rw-   0        0        0        0 2022-09-12 08:16:33.000000 PyOfficeRobot-0.1.2/PyOfficeRobot/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 12:08:28.186121 PyOfficeRobot-0.1.2/PyOfficeRobot/lib/dec/
--rw-rw-rw-   0        0        0        0 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.2/PyOfficeRobot/lib/dec/__init__.py
--rw-rw-rw-   0        0        0      385 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.2/PyOfficeRobot/lib/dec/act_dec.py
-drwxrwxrwx   0        0        0        0 2023-03-19 12:08:28.194644 PyOfficeRobot-0.1.2/PyOfficeRobot/lib/decorator_utils/
--rw-rw-rw-   0        0        0        0 2023-01-31 14:24:33.000000 PyOfficeRobot-0.1.2/PyOfficeRobot/lib/decorator_utils/__init__.py
--rw-rw-rw-   0        0        0     2323 2023-03-19 12:08:23.000000 PyOfficeRobot-0.1.2/PyOfficeRobot/lib/decorator_utils/instruction_url.py
-drwxrwxrwx   0        0        0        0 2023-03-19 12:08:28.162100 PyOfficeRobot-0.1.2/PyOfficeRobot.egg-info/
--rw-rw-rw-   0        0        0     7729 2023-03-19 12:08:27.000000 PyOfficeRobot-0.1.2/PyOfficeRobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      702 2023-03-19 12:08:27.000000 PyOfficeRobot-0.1.2/PyOfficeRobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-19 12:08:27.000000 PyOfficeRobot-0.1.2/PyOfficeRobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-19 12:08:27.000000 PyOfficeRobot-0.1.2/PyOfficeRobot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-03-19 12:08:27.000000 PyOfficeRobot-0.1.2/PyOfficeRobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-03-19 12:08:27.000000 PyOfficeRobot-0.1.2/PyOfficeRobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7154 2023-03-19 07:33:09.000000 PyOfficeRobot-0.1.2/README.md
--rw-rw-rw-   0        0        0      780 2023-03-19 12:08:28.205336 PyOfficeRobot-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 PyOfficeRobot-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-19 12:08:28.200163 PyOfficeRobot-0.1.2/tests/
--rw-rw-rw-   0        0        0      193 2023-02-13 13:41:39.000000 PyOfficeRobot-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2022-11-10 09:37:41.000000 PyOfficeRobot-0.1.2/tests/chat.py
--rw-rw-rw-   0        0        0      695 2023-03-19 08:15:19.000000 PyOfficeRobot-0.1.2/tests/test_file.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.079286 PyOfficeRobot-0.1.3/
+-rw-rw-rw-   0        0        0     1093 2022-09-09 17:29:26.000000 PyOfficeRobot-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     7869 2023-04-17 13:43:48.080301 PyOfficeRobot-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.002703 PyOfficeRobot-0.1.3/PyOfficeRobot/
+-rw-rw-rw-   0        0        0      120 2023-04-16 15:36:09.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.049697 PyOfficeRobot-0.1.3/PyOfficeRobot/api/
+-rw-rw-rw-   0        0        0        0 2022-09-09 17:57:22.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/api/__init__.py
+-rw-rw-rw-   0        0        0     3834 2023-03-19 10:39:04.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/api/chat.py
+-rw-rw-rw-   0        0        0     6984 2023-04-17 13:43:21.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/api/file.py
+-rw-rw-rw-   0        0        0     1625 2023-04-16 15:41:21.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/api/test.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.057208 PyOfficeRobot-0.1.3/PyOfficeRobot/core/
+-rw-rw-rw-   0        0        0    13388 2023-04-17 13:43:22.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/core/WeChatType.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.061229 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/
+-rw-rw-rw-   0        0        0      117 2023-03-19 07:06:10.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/CONST.py
+-rw-rw-rw-   0        0        0        0 2022-09-12 08:16:33.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.067229 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/dec/
+-rw-rw-rw-   0        0        0        0 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/dec/__init__.py
+-rw-rw-rw-   0        0        0      385 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/dec/act_dec.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.071747 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/decorator_utils/
+-rw-rw-rw-   0        0        0        0 2023-01-31 14:24:33.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/decorator_utils/__init__.py
+-rw-rw-rw-   0        0        0     2323 2023-03-19 12:08:23.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/decorator_utils/instruction_url.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.040158 PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/
+-rw-rw-rw-   0        0        0     7869 2023-04-17 13:43:47.000000 PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      728 2023-04-17 13:43:47.000000 PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 13:43:47.000000 PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 13:36:22.000000 PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-04-17 13:43:47.000000 PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-17 13:43:47.000000 PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7289 2023-04-02 05:09:27.000000 PyOfficeRobot-0.1.3/README.md
+-rw-rw-rw-   0        0        0      785 2023-04-17 13:43:48.088315 PyOfficeRobot-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 PyOfficeRobot-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.077746 PyOfficeRobot-0.1.3/tests/
+-rw-rw-rw-   0        0        0      193 2023-02-13 13:41:39.000000 PyOfficeRobot-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0       13 2023-04-17 13:43:22.000000 PyOfficeRobot-0.1.3/tests/chat.py
+-rw-rw-rw-   0        0        0     1229 2023-04-17 13:43:31.000000 PyOfficeRobot-0.1.3/tests/test_file.py
```

### Comparing `PyOfficeRobot-0.1.2/LICENSE` & `PyOfficeRobot-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.2/PKG-INFO` & `PyOfficeRobot-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: PyOfficeRobot
-Version: 0.1.2
+Version: 0.1.3
 Summary: pip install PyOfficeRobot
-Home-page: http://python-office.com/office/robot.html
+Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/README.md
 Project-URL: Source Code, https://github.com/CoderWanFeng/PyOfficeRobot
 Platform: any
@@ -60,15 +60,15 @@
 
 在经过技术检索和开发以后，支持所有微信使用的：**PyOfficeRobot**来啦~
 
 ## 1、安装PyOfficeRobot
 
 1行命令，安装PyOfficeRobot这个库
 ```
-pip install -i https://pypi.tuna.tsinghua.edu.cn/simple PyOfficeRobot -U
+pip install -i https://mirrors.aliyun.com/pypi/simple/ PyOfficeRobot -U
 ```
 
 ## 2、视频教程
 
 - ⭐全套源码：[Github](https://github.com/CoderWanFeng/PyOfficeRobot)
 
 
@@ -79,14 +79,15 @@
 | 003-自动发文件 | [点我直达](https://www.bilibili.com/video/BV1te4y1y7Ro)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/003-file.py)     |
 | 004-根据关键词，自动回复 | [点我直达](https://www.bilibili.com/video/BV1fV4y1M7ju)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/004-%E6%A0%B9%E6%8D%AE%E5%85%B3%E9%94%AE%E8%AF%8D%E5%9B%9E%E5%A4%8D.py)     |
 | ⌚005-定时自动发消息 | [点我直达](https://www.bilibili.com/video/BV1m8411b7LZ/)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/06-%E5%AE%9A%E6%97%B6.py)     |
 | 006-自己加功能 | [点我直达](https://www.bilibili.com/video/BV14R4y127h6)     |     |
 | ⭐007-独立使用 | [点我直达](https://www.bilibili.com/video/BV1SY411y7Uh)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot)     |
 | 08-收集群信息 | [点我直达](https://www.bilibili.com/video/BV1eD4y1g7yZ)     |[点我直达](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw)     |
 | 09-发消息如何换行？ | [点我直达](https://www.bilibili.com/video/BV1Xg4y1s79z/)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/08-new_line.py)     |
+| 10-微信 + ChatGPT | [点我直达](http://xhslink.com/zXZAeo)     |[点我直达](https://blog.51cto.com/u_15493782/6131326)     |
 
 > 持续更新中，交流群：[点我加入](http://www.python4office.cn/wechat-group/)
 #### 微信机器人-其它实现方式
 
 
 | 功能说明       | 视频 |代码 |
 | -------------- | -------- |-------- |
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.2 Summary: pip install
-PyOfficeRobot Home-page: http://python-office.com/office/robot.html Author:
-CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL: Bug
-Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
+Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.3 Summary: pip install
+PyOfficeRobot Home-page: https://www.python-office.com/office/robot.html
+Author: CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL:
+Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
 Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/
 README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 PyOfficeRobot Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
                                  tencent.jpg]
                             ð é¡¹ç®å®ç½ ð
@@ -18,15 +18,15 @@
 [ä¸ä¸ª15åéçè§é¢ï¼æä½ ç¨Pythonåå»ºèªå·±çå¾®ä¿¡èå¤©æºå¨äººï¼]
 (http://t.cn/A66p30bI)
 ä½æ¯ä¹åè¿ä¸ªæºå¨äººï¼éè¦åºäºç½é¡µçæè½ç¨ï¼ç¶èå¾å¤æåçå¾®ä¿¡ï¼æ¯ä¸è½ç»å½ç½é¡µçå¾®ä¿¡çã
 >
 ææ²¡æä¸ç§å¾®ä¿¡æºå¨äººï¼ä»»ä½äººçå¾®ä¿¡é½å¯ä»¥ç¨ï¼ä¸éè¦ç½é¡µå¾®ä¿¡åè½å¢ï¼
 å¨ç»è¿ææ¯æ£ç´¢åå¼åä»¥åï¼æ¯æææå¾®ä¿¡ä½¿ç¨çï¼**PyOfficeRobot**æ¥å¦~
 ## 1ãå®è£PyOfficeRobot 1è¡å½ä»¤ï¼å®è£PyOfficeRobotè¿ä¸ªåº ``` pip
-install -i https://pypi.tuna.tsinghua.edu.cn/simple PyOfficeRobot -U ``` ##
+install -i https://mirrors.aliyun.com/pypi/simple/ PyOfficeRobot -U ``` ##
 2ãè§é¢æç¨ - â­å¨å¥æºç ï¼[Github](https://github.com/CoderWanFeng/
 PyOfficeRobot) | åè½è¯´æ | è§é¢ |ä»£ç  | | -------------- | -------- |-
 ------- | | ð¥001-é¡¹ç®åå¸ | [ç¹æç´è¾¾](https://www.bilibili.com/
 video/BV1Xa411u7yU) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
 6slx8hyv_WuK7v5Nzt3XKQ) | | 002-èªå¨åæ¶æ¯ | [ç¹æç´è¾¾](https://
 www.bilibili.com/video/BV1Jt4y1j7F1) |[ç¹æç´è¾¾](https://github.com/
 CoderWanFeng/PyOfficeRobot/blob/main/demo/001-message.py) | | 003-
@@ -42,25 +42,26 @@
 [ç¹æç´è¾¾](https://www.bilibili.com/video/BV14R4y127h6) | | | â­007-
 ç¬ç«ä½¿ç¨ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1SY411y7Uh) |
 [ç¹æç´è¾¾](https://github.com/CoderWanFeng/PyOfficeRobot) | | 08-
 æ¶éç¾¤ä¿¡æ¯ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1eD4y1g7yZ) |
 [ç¹æç´è¾¾](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw) | | 09-
 åæ¶æ¯å¦ä½æ¢è¡ï¼ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
 BV1Xg4y1s79z/) |[ç¹æç´è¾¾](https://gitee.com/CoderWanFeng/PyOfficeRobot/
-blob/main/demo/08-new_line.py) | > æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼[ç¹æå å¥]
-(http://www.python4office.cn/wechat-group/) #### å¾®ä¿¡æºå¨äºº-
-å¶å®å®ç°æ¹å¼ | åè½è¯´æ | è§é¢ |ä»£ç  | | -------------- | -------
-- |-------- | | æºå¨äºº.exe | [ç¹æç´è¾¾](https://www.bilibili.com/video/
-BV1Q64y1Z7TB/) | | | ChatGPTçæ¬ | [ç¹æç´è¾¾](https://www.bilibili.com/
-video/BV1Dx4y157qy) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
-HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾]
-(https://www.bilibili.com/video/BV11L411L7oi/) |[ç¹æç´è¾¾](https://
-mp.weixin.qq.com/s/ubJ1OhOFVKfFVT8sBNZ0pg) | | ä¼ä¸å¾®ä¿¡æºå¨äºº | |
-[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/mt-ONvz0DdhbMB96eTZDKA) | ##
-3ãåè½Demo
+blob/main/demo/08-new_line.py) | | 10-å¾®ä¿¡ + ChatGPT | [ç¹æç´è¾¾](http://
+xhslink.com/zXZAeo) |[ç¹æç´è¾¾](https://blog.51cto.com/u_15493782/6131326)
+| > æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼[ç¹æå å¥](http://www.python4office.cn/
+wechat-group/) #### å¾®ä¿¡æºå¨äºº-å¶å®å®ç°æ¹å¼ | åè½è¯´æ | è§é¢
+|ä»£ç  | | -------------- | -------- |-------- | | æºå¨äºº.exe |
+[ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Q64y1Z7TB/) | | |
+ChatGPTçæ¬ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Dx4y157qy) |
+[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-
+24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
+BV11L411L7oi/) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
+ubJ1OhOFVKfFVT8sBNZ0pg) | | ä¼ä¸å¾®ä¿¡æºå¨äºº | |[ç¹æç´è¾¾](https://
+mp.weixin.qq.com/s/mt-ONvz0DdhbMB96eTZDKA) | ## 3ãåè½Demo
 ææè¿å¼æºäºè¿ä¸ªåºçå¨é¨æºä»£ç ï¼åè½æ­£å¨å¼åä¸­ï¼æ¬¢è¿å¤§å®¶åä¸å¼å~
 - [æ¼ç¤ºä»£ç ](https://github.com/CoderWanFeng/PyOfficeRobot/tree/main/demo)
 --- ![](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-
 office-qr.jpg) ## â­Star [![Stargazers over time](https://starchart.cc/
 CoderWanFeng/PyOfficeRobot.svg)](https://starchart.cc/CoderWanFeng/
 PyOfficeRobot) ## ðæå±èµæ
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
```

### Comparing `PyOfficeRobot-0.1.2/PyOfficeRobot/api/chat.py` & `PyOfficeRobot-0.1.3/PyOfficeRobot/api/chat.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.2/PyOfficeRobot/api/file.py` & `PyOfficeRobot-0.1.3/PyOfficeRobot/api/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from PyOfficeRobot.core.WeChatType import WeChat
 from PyOfficeRobot.lib.decorator_utils.instruction_url import instruction
 
 wx = WeChat()
 
+
 # @act_info(ACT_TYPE.FILE)
 @instruction
 def send_file(who, file):
     """
     发送任意类型的文件
     :param who:
     :param file: 文件路径
     :return:
     """
     # 向某人发送文件（以`文件传输助手`为例，发送三个不同类型文件）
     wx.ChatWith(who)  # 打开`文件传输助手`聊天窗口
-    wx.SendFiles(file)  # 向`文件传输助手`发送上述三个文件
+    # wx.SendFiles(file)  # 向`文件传输助手`发送上述三个文件
+    wx.test_SendFiles(filepath=file)  # 向`文件传输助手`发送上述三个文件
+
     # 注：为保证发送文件稳定性，首次发送文件可能花费时间较长，后续调用会缩短发送时间
 
+
 import uiautomation as uia
 
 """ isinstance()函数知识点:
 
 type判断函数类型是什么，而isinstance是通过判断对象是否是已知的类型
 但是isinstance比type高级一些（功能上的差异）
 type() ，不考虑继承关系（子类不是父类类型）
@@ -28,14 +32,15 @@
 
 a = 10086
 isinstance (a,int)  # true
 isinstance (a,str) # false
 isinstance (a,(str,int,list))    # 只要满足元组类型中的其中一个即可，答案是满足，所以为false
 """
 
+
 def get_group_list():
     """
     author: Zijian
     :return:
     """
     uia.uiautomation.SetGlobalSearchTimeout(2)
     wechat_win = uia.WindowControl(Depth=1, Name="微信", ClassName="WeChatMainWndForPC")
```

### Comparing `PyOfficeRobot-0.1.2/PyOfficeRobot/core/WeChatType.py` & `PyOfficeRobot-0.1.3/PyOfficeRobot/core/WeChatType.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # -*-coding:utf-8-*-
 # sys.stdout = io.TextIOWrapper(sys.stdout.buffer,encoding='gb18030')
 
 
+import os
+import time
+from ctypes import *
+from pathlib import Path
+
 import uiautomation as uia
-import win32gui, win32con
+import win32clipboard
 import win32clipboard as wc
-import time
-import os
+import win32con
+import win32gui
 
 PUBLISH_ID = '公众号：程序员晚枫'
 
 COPYDICT = {}
 
 
 class WxParam:
@@ -294,7 +299,53 @@
             return 1
         else:
             return 0
 
     def SavePic(self, savepath=None, filename=None):
         WxUtils.SavePic()
         # Pic = uia.WindowControl(ClassName='ImagePreviewWnd', Name='图片查看')
+
+    ################################微信发文件崩溃 https://blog.csdn.net/weixin_45081575/article/details/126810748
+
+    def test_SendFiles(self, filepath, not_exists='ignore'):
+        """向当前聊天窗口发送文件
+        not_exists: 如果未找到指定文件，继续或终止程序
+        filepath: 要复制文件的绝对路径"""
+
+        class DROPFILES(Structure):
+            _fields_ = [
+                ("pFiles", c_uint),
+                ("x", c_long),
+                ("y", c_long),
+                ("fNC", c_int),
+                ("fWide", c_bool),
+            ]
+
+        def setClipboardFiles(paths):
+            files = ("\0".join(paths)).replace("/", "\\")
+            data = files.encode("U16")[2:] + b"\0\0"
+            wc.OpenClipboard()
+            try:
+                wc.EmptyClipboard()
+                wc.SetClipboardData(
+                    wc.CF_HDROP, matedata + data)
+            finally:
+                wc.CloseClipboard()
+
+        def readClipboardFilePaths():
+            wc.OpenClipboard()
+            try:
+                return wc.GetClipboardData(win32clipboard.CF_HDROP)
+            finally:
+                wc.CloseClipboard()
+
+        pDropFiles = DROPFILES()
+        pDropFiles.pFiles = sizeof(DROPFILES)
+        pDropFiles.fWide = True
+        matedata = bytes(pDropFiles)
+        filepath = str(Path(filepath).absolute())
+        filename = [r"%s" % filepath]
+        setClipboardFiles(filename)
+
+        # wc.CloseClipboard()
+        self.SendClipboard()
+        return 1
```

### Comparing `PyOfficeRobot-0.1.2/PyOfficeRobot/lib/decorator_utils/instruction_url.py` & `PyOfficeRobot-0.1.3/PyOfficeRobot/lib/decorator_utils/instruction_url.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.2/PyOfficeRobot.egg-info/PKG-INFO` & `PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: PyOfficeRobot
-Version: 0.1.2
+Version: 0.1.3
 Summary: pip install PyOfficeRobot
-Home-page: http://python-office.com/office/robot.html
+Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/README.md
 Project-URL: Source Code, https://github.com/CoderWanFeng/PyOfficeRobot
 Platform: any
@@ -60,15 +60,15 @@
 
 在经过技术检索和开发以后，支持所有微信使用的：**PyOfficeRobot**来啦~
 
 ## 1、安装PyOfficeRobot
 
 1行命令，安装PyOfficeRobot这个库
 ```
-pip install -i https://pypi.tuna.tsinghua.edu.cn/simple PyOfficeRobot -U
+pip install -i https://mirrors.aliyun.com/pypi/simple/ PyOfficeRobot -U
 ```
 
 ## 2、视频教程
 
 - ⭐全套源码：[Github](https://github.com/CoderWanFeng/PyOfficeRobot)
 
 
@@ -79,14 +79,15 @@
 | 003-自动发文件 | [点我直达](https://www.bilibili.com/video/BV1te4y1y7Ro)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/003-file.py)     |
 | 004-根据关键词，自动回复 | [点我直达](https://www.bilibili.com/video/BV1fV4y1M7ju)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/004-%E6%A0%B9%E6%8D%AE%E5%85%B3%E9%94%AE%E8%AF%8D%E5%9B%9E%E5%A4%8D.py)     |
 | ⌚005-定时自动发消息 | [点我直达](https://www.bilibili.com/video/BV1m8411b7LZ/)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/06-%E5%AE%9A%E6%97%B6.py)     |
 | 006-自己加功能 | [点我直达](https://www.bilibili.com/video/BV14R4y127h6)     |     |
 | ⭐007-独立使用 | [点我直达](https://www.bilibili.com/video/BV1SY411y7Uh)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot)     |
 | 08-收集群信息 | [点我直达](https://www.bilibili.com/video/BV1eD4y1g7yZ)     |[点我直达](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw)     |
 | 09-发消息如何换行？ | [点我直达](https://www.bilibili.com/video/BV1Xg4y1s79z/)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/08-new_line.py)     |
+| 10-微信 + ChatGPT | [点我直达](http://xhslink.com/zXZAeo)     |[点我直达](https://blog.51cto.com/u_15493782/6131326)     |
 
 > 持续更新中，交流群：[点我加入](http://www.python4office.cn/wechat-group/)
 #### 微信机器人-其它实现方式
 
 
 | 功能说明       | 视频 |代码 |
 | -------------- | -------- |-------- |
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.2 Summary: pip install
-PyOfficeRobot Home-page: http://python-office.com/office/robot.html Author:
-CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL: Bug
-Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
+Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.3 Summary: pip install
+PyOfficeRobot Home-page: https://www.python-office.com/office/robot.html
+Author: CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL:
+Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
 Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/
 README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 PyOfficeRobot Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
                                  tencent.jpg]
                             ð é¡¹ç®å®ç½ ð
@@ -18,15 +18,15 @@
 [ä¸ä¸ª15åéçè§é¢ï¼æä½ ç¨Pythonåå»ºèªå·±çå¾®ä¿¡èå¤©æºå¨äººï¼]
 (http://t.cn/A66p30bI)
 ä½æ¯ä¹åè¿ä¸ªæºå¨äººï¼éè¦åºäºç½é¡µçæè½ç¨ï¼ç¶èå¾å¤æåçå¾®ä¿¡ï¼æ¯ä¸è½ç»å½ç½é¡µçå¾®ä¿¡çã
 >
 ææ²¡æä¸ç§å¾®ä¿¡æºå¨äººï¼ä»»ä½äººçå¾®ä¿¡é½å¯ä»¥ç¨ï¼ä¸éè¦ç½é¡µå¾®ä¿¡åè½å¢ï¼
 å¨ç»è¿ææ¯æ£ç´¢åå¼åä»¥åï¼æ¯æææå¾®ä¿¡ä½¿ç¨çï¼**PyOfficeRobot**æ¥å¦~
 ## 1ãå®è£PyOfficeRobot 1è¡å½ä»¤ï¼å®è£PyOfficeRobotè¿ä¸ªåº ``` pip
-install -i https://pypi.tuna.tsinghua.edu.cn/simple PyOfficeRobot -U ``` ##
+install -i https://mirrors.aliyun.com/pypi/simple/ PyOfficeRobot -U ``` ##
 2ãè§é¢æç¨ - â­å¨å¥æºç ï¼[Github](https://github.com/CoderWanFeng/
 PyOfficeRobot) | åè½è¯´æ | è§é¢ |ä»£ç  | | -------------- | -------- |-
 ------- | | ð¥001-é¡¹ç®åå¸ | [ç¹æç´è¾¾](https://www.bilibili.com/
 video/BV1Xa411u7yU) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
 6slx8hyv_WuK7v5Nzt3XKQ) | | 002-èªå¨åæ¶æ¯ | [ç¹æç´è¾¾](https://
 www.bilibili.com/video/BV1Jt4y1j7F1) |[ç¹æç´è¾¾](https://github.com/
 CoderWanFeng/PyOfficeRobot/blob/main/demo/001-message.py) | | 003-
@@ -42,25 +42,26 @@
 [ç¹æç´è¾¾](https://www.bilibili.com/video/BV14R4y127h6) | | | â­007-
 ç¬ç«ä½¿ç¨ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1SY411y7Uh) |
 [ç¹æç´è¾¾](https://github.com/CoderWanFeng/PyOfficeRobot) | | 08-
 æ¶éç¾¤ä¿¡æ¯ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1eD4y1g7yZ) |
 [ç¹æç´è¾¾](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw) | | 09-
 åæ¶æ¯å¦ä½æ¢è¡ï¼ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
 BV1Xg4y1s79z/) |[ç¹æç´è¾¾](https://gitee.com/CoderWanFeng/PyOfficeRobot/
-blob/main/demo/08-new_line.py) | > æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼[ç¹æå å¥]
-(http://www.python4office.cn/wechat-group/) #### å¾®ä¿¡æºå¨äºº-
-å¶å®å®ç°æ¹å¼ | åè½è¯´æ | è§é¢ |ä»£ç  | | -------------- | -------
-- |-------- | | æºå¨äºº.exe | [ç¹æç´è¾¾](https://www.bilibili.com/video/
-BV1Q64y1Z7TB/) | | | ChatGPTçæ¬ | [ç¹æç´è¾¾](https://www.bilibili.com/
-video/BV1Dx4y157qy) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
-HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾]
-(https://www.bilibili.com/video/BV11L411L7oi/) |[ç¹æç´è¾¾](https://
-mp.weixin.qq.com/s/ubJ1OhOFVKfFVT8sBNZ0pg) | | ä¼ä¸å¾®ä¿¡æºå¨äºº | |
-[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/mt-ONvz0DdhbMB96eTZDKA) | ##
-3ãåè½Demo
+blob/main/demo/08-new_line.py) | | 10-å¾®ä¿¡ + ChatGPT | [ç¹æç´è¾¾](http://
+xhslink.com/zXZAeo) |[ç¹æç´è¾¾](https://blog.51cto.com/u_15493782/6131326)
+| > æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼[ç¹æå å¥](http://www.python4office.cn/
+wechat-group/) #### å¾®ä¿¡æºå¨äºº-å¶å®å®ç°æ¹å¼ | åè½è¯´æ | è§é¢
+|ä»£ç  | | -------------- | -------- |-------- | | æºå¨äºº.exe |
+[ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Q64y1Z7TB/) | | |
+ChatGPTçæ¬ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Dx4y157qy) |
+[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-
+24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
+BV11L411L7oi/) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
+ubJ1OhOFVKfFVT8sBNZ0pg) | | ä¼ä¸å¾®ä¿¡æºå¨äºº | |[ç¹æç´è¾¾](https://
+mp.weixin.qq.com/s/mt-ONvz0DdhbMB96eTZDKA) | ## 3ãåè½Demo
 ææè¿å¼æºäºè¿ä¸ªåºçå¨é¨æºä»£ç ï¼åè½æ­£å¨å¼åä¸­ï¼æ¬¢è¿å¤§å®¶åä¸å¼å~
 - [æ¼ç¤ºä»£ç ](https://github.com/CoderWanFeng/PyOfficeRobot/tree/main/demo)
 --- ![](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-
 office-qr.jpg) ## â­Star [![Stargazers over time](https://starchart.cc/
 CoderWanFeng/PyOfficeRobot.svg)](https://starchart.cc/CoderWanFeng/
 PyOfficeRobot) ## ðæå±èµæ
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
```

### Comparing `PyOfficeRobot-0.1.2/PyOfficeRobot.egg-info/SOURCES.txt` & `PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 PyOfficeRobot.egg-info/dependency_links.txt
 PyOfficeRobot.egg-info/not-zip-safe
 PyOfficeRobot.egg-info/requires.txt
 PyOfficeRobot.egg-info/top_level.txt
 PyOfficeRobot/api/__init__.py
 PyOfficeRobot/api/chat.py
 PyOfficeRobot/api/file.py
+PyOfficeRobot/api/test.py
 PyOfficeRobot/core/WeChatType.py
 PyOfficeRobot/core/__init__.py
 PyOfficeRobot/lib/CONST.py
 PyOfficeRobot/lib/__init__.py
 PyOfficeRobot/lib/dec/__init__.py
 PyOfficeRobot/lib/dec/act_dec.py
 PyOfficeRobot/lib/decorator_utils/__init__.py
```

### Comparing `PyOfficeRobot-0.1.2/README.md` & `PyOfficeRobot-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 在经过技术检索和开发以后，支持所有微信使用的：**PyOfficeRobot**来啦~
 
 ## 1、安装PyOfficeRobot
 
 1行命令，安装PyOfficeRobot这个库
 ```
-pip install -i https://pypi.tuna.tsinghua.edu.cn/simple PyOfficeRobot -U
+pip install -i https://mirrors.aliyun.com/pypi/simple/ PyOfficeRobot -U
 ```
 
 ## 2、视频教程
 
 - ⭐全套源码：[Github](https://github.com/CoderWanFeng/PyOfficeRobot)
 
 
@@ -63,14 +63,15 @@
 | 003-自动发文件 | [点我直达](https://www.bilibili.com/video/BV1te4y1y7Ro)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/003-file.py)     |
 | 004-根据关键词，自动回复 | [点我直达](https://www.bilibili.com/video/BV1fV4y1M7ju)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/004-%E6%A0%B9%E6%8D%AE%E5%85%B3%E9%94%AE%E8%AF%8D%E5%9B%9E%E5%A4%8D.py)     |
 | ⌚005-定时自动发消息 | [点我直达](https://www.bilibili.com/video/BV1m8411b7LZ/)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/06-%E5%AE%9A%E6%97%B6.py)     |
 | 006-自己加功能 | [点我直达](https://www.bilibili.com/video/BV14R4y127h6)     |     |
 | ⭐007-独立使用 | [点我直达](https://www.bilibili.com/video/BV1SY411y7Uh)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot)     |
 | 08-收集群信息 | [点我直达](https://www.bilibili.com/video/BV1eD4y1g7yZ)     |[点我直达](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw)     |
 | 09-发消息如何换行？ | [点我直达](https://www.bilibili.com/video/BV1Xg4y1s79z/)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/08-new_line.py)     |
+| 10-微信 + ChatGPT | [点我直达](http://xhslink.com/zXZAeo)     |[点我直达](https://blog.51cto.com/u_15493782/6131326)     |
 
 > 持续更新中，交流群：[点我加入](http://www.python4office.cn/wechat-group/)
 #### 微信机器人-其它实现方式
 
 
 | 功能说明       | 视频 |代码 |
 | -------------- | -------- |-------- |
```

#### html2text {}

```diff
@@ -10,15 +10,15 @@
 [ä¸ä¸ª15åéçè§é¢ï¼æä½ ç¨Pythonåå»ºèªå·±çå¾®ä¿¡èå¤©æºå¨äººï¼]
 (http://t.cn/A66p30bI)
 ä½æ¯ä¹åè¿ä¸ªæºå¨äººï¼éè¦åºäºç½é¡µçæè½ç¨ï¼ç¶èå¾å¤æåçå¾®ä¿¡ï¼æ¯ä¸è½ç»å½ç½é¡µçå¾®ä¿¡çã
 >
 ææ²¡æä¸ç§å¾®ä¿¡æºå¨äººï¼ä»»ä½äººçå¾®ä¿¡é½å¯ä»¥ç¨ï¼ä¸éè¦ç½é¡µå¾®ä¿¡åè½å¢ï¼
 å¨ç»è¿ææ¯æ£ç´¢åå¼åä»¥åï¼æ¯æææå¾®ä¿¡ä½¿ç¨çï¼**PyOfficeRobot**æ¥å¦~
 ## 1ãå®è£PyOfficeRobot 1è¡å½ä»¤ï¼å®è£PyOfficeRobotè¿ä¸ªåº ``` pip
-install -i https://pypi.tuna.tsinghua.edu.cn/simple PyOfficeRobot -U ``` ##
+install -i https://mirrors.aliyun.com/pypi/simple/ PyOfficeRobot -U ``` ##
 2ãè§é¢æç¨ - â­å¨å¥æºç ï¼[Github](https://github.com/CoderWanFeng/
 PyOfficeRobot) | åè½è¯´æ | è§é¢ |ä»£ç  | | -------------- | -------- |-
 ------- | | ð¥001-é¡¹ç®åå¸ | [ç¹æç´è¾¾](https://www.bilibili.com/
 video/BV1Xa411u7yU) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
 6slx8hyv_WuK7v5Nzt3XKQ) | | 002-èªå¨åæ¶æ¯ | [ç¹æç´è¾¾](https://
 www.bilibili.com/video/BV1Jt4y1j7F1) |[ç¹æç´è¾¾](https://github.com/
 CoderWanFeng/PyOfficeRobot/blob/main/demo/001-message.py) | | 003-
@@ -34,25 +34,26 @@
 [ç¹æç´è¾¾](https://www.bilibili.com/video/BV14R4y127h6) | | | â­007-
 ç¬ç«ä½¿ç¨ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1SY411y7Uh) |
 [ç¹æç´è¾¾](https://github.com/CoderWanFeng/PyOfficeRobot) | | 08-
 æ¶éç¾¤ä¿¡æ¯ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1eD4y1g7yZ) |
 [ç¹æç´è¾¾](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw) | | 09-
 åæ¶æ¯å¦ä½æ¢è¡ï¼ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
 BV1Xg4y1s79z/) |[ç¹æç´è¾¾](https://gitee.com/CoderWanFeng/PyOfficeRobot/
-blob/main/demo/08-new_line.py) | > æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼[ç¹æå å¥]
-(http://www.python4office.cn/wechat-group/) #### å¾®ä¿¡æºå¨äºº-
-å¶å®å®ç°æ¹å¼ | åè½è¯´æ | è§é¢ |ä»£ç  | | -------------- | -------
-- |-------- | | æºå¨äºº.exe | [ç¹æç´è¾¾](https://www.bilibili.com/video/
-BV1Q64y1Z7TB/) | | | ChatGPTçæ¬ | [ç¹æç´è¾¾](https://www.bilibili.com/
-video/BV1Dx4y157qy) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
-HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾]
-(https://www.bilibili.com/video/BV11L411L7oi/) |[ç¹æç´è¾¾](https://
-mp.weixin.qq.com/s/ubJ1OhOFVKfFVT8sBNZ0pg) | | ä¼ä¸å¾®ä¿¡æºå¨äºº | |
-[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/mt-ONvz0DdhbMB96eTZDKA) | ##
-3ãåè½Demo
+blob/main/demo/08-new_line.py) | | 10-å¾®ä¿¡ + ChatGPT | [ç¹æç´è¾¾](http://
+xhslink.com/zXZAeo) |[ç¹æç´è¾¾](https://blog.51cto.com/u_15493782/6131326)
+| > æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼[ç¹æå å¥](http://www.python4office.cn/
+wechat-group/) #### å¾®ä¿¡æºå¨äºº-å¶å®å®ç°æ¹å¼ | åè½è¯´æ | è§é¢
+|ä»£ç  | | -------------- | -------- |-------- | | æºå¨äºº.exe |
+[ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Q64y1Z7TB/) | | |
+ChatGPTçæ¬ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Dx4y157qy) |
+[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-
+24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
+BV11L411L7oi/) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
+ubJ1OhOFVKfFVT8sBNZ0pg) | | ä¼ä¸å¾®ä¿¡æºå¨äºº | |[ç¹æç´è¾¾](https://
+mp.weixin.qq.com/s/mt-ONvz0DdhbMB96eTZDKA) | ## 3ãåè½Demo
 ææè¿å¼æºäºè¿ä¸ªåºçå¨é¨æºä»£ç ï¼åè½æ­£å¨å¼åä¸­ï¼æ¬¢è¿å¤§å®¶åä¸å¼å~
 - [æ¼ç¤ºä»£ç ](https://github.com/CoderWanFeng/PyOfficeRobot/tree/main/demo)
 --- ![](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-
 office-qr.jpg) ## â­Star [![Stargazers over time](https://starchart.cc/
 CoderWanFeng/PyOfficeRobot.svg)](https://starchart.cc/CoderWanFeng/
 PyOfficeRobot) ## ðæå±èµæ
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
```

### Comparing `PyOfficeRobot-0.1.2/setup.cfg` & `PyOfficeRobot-0.1.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 794f 6666 6963 6552 6f62 6f74   = PyOfficeRobot
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 312e  ..version = 0.1.
-00000030: 320d 0a64 6573 6372 6970 7469 6f6e 203d  2..description =
+00000030: 330d 0a64 6573 6372 6970 7469 6f6e 203d  3..description =
 00000040: 2070 6970 2069 6e73 7461 6c6c 2050 794f   pip install PyO
 00000050: 6666 6963 6552 6f62 6f74 0d0a 6c6f 6e67  fficeRobot..long
 00000060: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000070: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000080: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000090: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 000000a0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
-000000b0: 726c 203d 2068 7474 703a 2f2f 7079 7468  rl = http://pyth
-000000c0: 6f6e 2d6f 6666 6963 652e 636f 6d2f 6f66  on-office.com/of
-000000d0: 6669 6365 2f72 6f62 6f74 2e68 746d 6c0d  fice/robot.html.
-000000e0: 0a61 7574 686f 7220 3d20 436f 6465 7257  .author = CoderW
-000000f0: 616e 4665 6e67 0d0a 6175 7468 6f72 5f65  anFeng..author_e
-00000100: 6d61 696c 203d 2031 3935 3738 3735 3037  mail = 195787507
-00000110: 3340 7171 2e63 6f6d 0d0a 6c69 6365 6e73  3@qq.com..licens
-00000120: 6520 3d20 4d49 540d 0a6c 6963 656e 7365  e = MIT..license
-00000130: 5f66 696c 6520 3d20 4c49 4345 4e53 450d  _file = LICENSE.
-00000140: 0a70 6c61 7466 6f72 6d73 203d 2061 6e79  .platforms = any
-00000150: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
-00000160: 200d 0a09 4275 6720 5472 6163 6b65 7220   ...Bug Tracker 
-00000170: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000180: 2e63 6f6d 2f43 6f64 6572 5761 6e46 656e  .com/CoderWanFen
-00000190: 672f 5079 4f66 6669 6365 526f 626f 742f  g/PyOfficeRobot/
-000001a0: 6973 7375 6573 0d0a 0944 6f63 756d 656e  issues...Documen
-000001b0: 7461 7469 6f6e 203d 2068 7474 7073 3a2f  tation = https:/
-000001c0: 2f67 6974 6875 622e 636f 6d2f 436f 6465  /github.com/Code
-000001d0: 7257 616e 4665 6e67 2f50 794f 6666 6963  rWanFeng/PyOffic
-000001e0: 6552 6f62 6f74 2f62 6c6f 622f 6d61 696e  eRobot/blob/main
-000001f0: 2f52 4541 444d 452e 6d64 0d0a 0953 6f75  /README.md...Sou
-00000200: 7263 6520 436f 6465 203d 2068 7474 7073  rce Code = https
-00000210: 3a2f 2f67 6974 6875 622e 636f 6d2f 436f  ://github.com/Co
-00000220: 6465 7257 616e 4665 6e67 2f50 794f 6666  derWanFeng/PyOff
-00000230: 6963 6552 6f62 6f74 0d0a 0d0a 5b6f 7074  iceRobot....[opt
-00000240: 696f 6e73 5d0d 0a70 6163 6b61 6765 7320  ions]..packages 
-00000250: 3d20 6669 6e64 3a0d 0a69 6e73 7461 6c6c  = find:..install
-00000260: 5f72 6571 7569 7265 7320 3d20 0d0a 0975  _requires = ...u
-00000270: 6961 7574 6f6d 6174 696f 6e0d 0a09 7363  iautomation...sc
-00000280: 6865 6475 6c65 0d0a 0970 616e 6461 730d  hedule...pandas.
-00000290: 0a09 706f 6169 0d0a 7079 7468 6f6e 5f72  ..poai..python_r
-000002a0: 6571 7569 7265 7320 3d20 3e3d 332e 360d  equires = >=3.6.
-000002b0: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
-000002c0: 5f64 6174 6120 3d20 5472 7565 0d0a 7a69  _data = True..zi
-000002d0: 705f 7361 6665 203d 2046 616c 7365 0d0a  p_safe = False..
-000002e0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000002f0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000300: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+000000b0: 726c 203d 2068 7474 7073 3a2f 2f77 7777  rl = https://www
+000000c0: 2e70 7974 686f 6e2d 6f66 6669 6365 2e63  .python-office.c
+000000d0: 6f6d 2f6f 6666 6963 652f 726f 626f 742e  om/office/robot.
+000000e0: 6874 6d6c 0d0a 6175 7468 6f72 203d 2043  html..author = C
+000000f0: 6f64 6572 5761 6e46 656e 670d 0a61 7574  oderWanFeng..aut
+00000100: 686f 725f 656d 6169 6c20 3d20 3139 3537  hor_email = 1957
+00000110: 3837 3530 3733 4071 712e 636f 6d0d 0a6c  875073@qq.com..l
+00000120: 6963 656e 7365 203d 204d 4954 0d0a 6c69  icense = MIT..li
+00000130: 6365 6e73 655f 6669 6c65 203d 204c 4943  cense_file = LIC
+00000140: 454e 5345 0d0a 706c 6174 666f 726d 7320  ENSE..platforms 
+00000150: 3d20 616e 790d 0a70 726f 6a65 6374 5f75  = any..project_u
+00000160: 726c 7320 3d20 0d0a 0942 7567 2054 7261  rls = ...Bug Tra
+00000170: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
+00000180: 6974 6875 622e 636f 6d2f 436f 6465 7257  ithub.com/CoderW
+00000190: 616e 4665 6e67 2f50 794f 6666 6963 6552  anFeng/PyOfficeR
+000001a0: 6f62 6f74 2f69 7373 7565 730d 0a09 446f  obot/issues...Do
+000001b0: 6375 6d65 6e74 6174 696f 6e20 3d20 6874  cumentation = ht
+000001c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000001d0: 2f43 6f64 6572 5761 6e46 656e 672f 5079  /CoderWanFeng/Py
+000001e0: 4f66 6669 6365 526f 626f 742f 626c 6f62  OfficeRobot/blob
+000001f0: 2f6d 6169 6e2f 5245 4144 4d45 2e6d 640d  /main/README.md.
+00000200: 0a09 536f 7572 6365 2043 6f64 6520 3d20  ..Source Code = 
+00000210: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000220: 6f6d 2f43 6f64 6572 5761 6e46 656e 672f  om/CoderWanFeng/
+00000230: 5079 4f66 6669 6365 526f 626f 740d 0a0d  PyOfficeRobot...
+00000240: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
+00000250: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
+00000260: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
+00000270: 200d 0a09 7569 6175 746f 6d61 7469 6f6e   ...uiautomation
+00000280: 0d0a 0973 6368 6564 756c 650d 0a09 7061  ...schedule...pa
+00000290: 6e64 6173 0d0a 0970 6f61 690d 0a70 7974  ndas...poai..pyt
+000002a0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+000002b0: 3d33 2e36 0d0a 696e 636c 7564 655f 7061  =3.6..include_pa
+000002c0: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
+000002d0: 650d 0a7a 6970 5f73 6166 6520 3d20 4661  e..zip_safe = Fa
+000002e0: 6c73 650d 0a0d 0a5b 6567 675f 696e 666f  lse....[egg_info
+000002f0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000300: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000310: 0a                                       .
```

