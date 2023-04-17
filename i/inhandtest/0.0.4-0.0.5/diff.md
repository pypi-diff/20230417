# Comparing `tmp/inhandtest-0.0.4.tar.gz` & `tmp/inhandtest-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.4.tar", last modified: Tue Feb  7 11:03:44 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.5.tar", last modified: Thu Feb  9 05:48:27 2023, max compression
```

## Comparing `inhandtest-0.0.4.tar` & `inhandtest-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 11:03:44.000000 inhandtest-0.0.4/
--rw-rw-rw-   0        0        0      293 2023-02-07 11:03:44.000000 inhandtest-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    12524 2023-02-07 10:56:19.000000 inhandtest-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-02-07 11:03:44.000000 inhandtest-0.0.4/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.4/inhandtest/__init__.py
--rw-rw-rw-   0        0        0    26394 2023-02-07 09:49:39.000000 inhandtest-0.0.4/inhandtest/telnet.py
--rw-rw-rw-   0        0        0     2549 2023-02-07 09:10:03.000000 inhandtest-0.0.4/inhandtest/tools.py
--rw-rw-rw-   0        0        0      715 2023-02-07 11:03:18.000000 inhandtest-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-09 05:48:27.000000 inhandtest-0.0.5/
+-rw-rw-rw-   0        0        0      293 2023-02-09 05:48:27.000000 inhandtest-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    12259 2023-02-08 03:38:19.000000 inhandtest-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-02-09 05:48:27.000000 inhandtest-0.0.5/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.5/inhandtest/__init__.py
+-rw-rw-rw-   0        0        0    28861 2023-02-09 05:42:30.000000 inhandtest-0.0.5/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0     2549 2023-02-07 09:10:03.000000 inhandtest-0.0.5/inhandtest/tools.py
+-rw-rw-rw-   0        0        0      715 2023-02-09 05:48:03.000000 inhandtest-0.0.5/setup.py
```

### Comparing `inhandtest-0.0.4/README.md` & `inhandtest-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     - 返回（return）
 
     返回被装饰函数返回的值
 
     - 实例
 
 ```python
-           from inhandtest.tools import loop_inspector
+    from inhandtest.tools import loop_inspector
 
-           @loop_inspector(flag='status', timeout=90, interval=5, assertion=True)
-           def assert_status():
-               return True
+    @loop_inspector(flag='status', timeout=90, interval=5, assertion=True)
+    def assert_status():
+        return True
                
    ```
 - dict_merge(dict_a: dict, dict_b: dict)
 
 字典合并，如果都为空
 
     - 参数解析
@@ -45,20 +45,20 @@
     - 返回（return）
         
     返回合并后的字典，
     
     - 实例
 
 ```python
-           from inhandtest.tools import dict_merge
-           
-           if __name__ == '__main__':
-               print(dict_merge({'key': 'value'}, {'key1': 'value1'}))
-               
-           {'key': 'value', 'key1': 'value1'}
+   from inhandtest.tools import dict_merge
+   
+   if __name__ == '__main__':
+       print(dict_merge({'key': 'value'}, {'key1': 'value1'}))
+       
+   {'key': 'value', 'key1': 'value1'}
         
   ```
 - dict_flatten(in_dict, separator=":", dict_out=None, parent_key=None)
 
 字典平铺，让多层级字典直接平铺，方便做字典的断言
 
     - 参数解析
@@ -69,110 +69,110 @@
     - 返回（return）
         
     返回平铺后的字典，
     
     - 实例
 
 ```python
-           from inhandtest.tools import dict_flatten
-           
-           if __name__ == '__main__':
-               print(dict_flatten({'key': {'key1': 'value1'}, 'key2': [0, 1]}))
-               
-           {'key:key1': 'value1', 'key2': [0, 1]}
+   from inhandtest.tools import dict_flatten
+   
+   if __name__ == '__main__':
+       print(dict_flatten({'key': {'key1': 'value1'}, 'key2': [0, 1]}))
+       
+   {'key:key1': 'value1', 'key2': [0, 1]}
            
    ```
 			
 # Telnet 使用
 - __init__(self, model: str, host: str, super_user: str, super_password: str, user='adm', password='123456', port=23, **kwargs)
 
 初始化函数 设备Telnet操作封装，让测试同事更易用, 
 
     - 参数解析
-        + model :  设备型号，‘VG710'， 大小写无关
+        + model : 设备型号，VG710'|'IR302'|'ER805'|'ER605'，大小写无关
         + host : 设备lan ip， 192.168.2.1
         + super_user : 超级管理员的用户名称
         + super_password :  超级管理员的密码
         + user : 用户名
         + password : 用户密码
         + port : 端口
         + kwargs : interface_replace, 字典类型，只替换输入命令 {'wan': 'wan0', 'wifi_sta': 'wan2', 'cellular1': 'wwan0'}，在telnet里面接口名称转换，使得输入命令时接口名称统一。
 
     - 实例
 
 ```python
-           from inhandtest.telnet import Telnet
+   from inhandtest.telnet import Telnet
 
-           if __name__ == '__main__':
-                import sys
+   if __name__ == '__main__':
+        import sys
 
-                logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
-                                    stream=sys.stdout)
-                my_device = Telnet('VG710', '10.5.47.197', '*****', '******', interface_replace={'wifi': 'ath0'})
-                my_device.super_mode()
+        logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
+                            stream=sys.stdout)
+        my_device = Telnet('VG710', '10.5.47.197', '*****', '******', interface_replace={'wifi': 'ath0'})
+        my_device.super_mode()
                 
    ```
 - super_mode(self)
 
 进入超级模式 /www
 
     - 参数解析
     - 返回（return）
     
     None
     
     - 实例
 
 ```python
-           my_device.super_mode()
+   my_device.super_mode()
            
    ```
 - config_mode(self)
 
 进入配置模式 (config)#
 
     - 参数解析
     - 返回（return）
     
     None
     
     - 实例
 
 ```python
-           my_device.config_mode()
+   my_device.config_mode()
            
    ```
 - user_mode(self)
 
 进入用户模式 f'{hostname}#'
 
     - 参数解析
     - 返回（return）
     
     None
     
     - 实例
 
 ```python
-           my_device.user_mode()
+   my_device.user_mode()
            
    ```
 - normal_mode(self)
 
 进入普通模式 f'{hostname}>'
 
     - 参数解析
     - 返回（return）
     
     None
     
     - 实例
 
 ```python
-           my_device.normal_mode()
+   my_device.normal_mode()
            
    ```
 - update_hostname(self, hostname: str)
 
 更新主机名，在使用telnet时，因为读取命令要read_until, 所以一旦界面更改主机名后需要手动调用该方法更新主机名
 
     - 参数解析
@@ -180,15 +180,15 @@
     - 返回（return）
         
     None
     
     - 实例
 
 ```python
-           my_device.update_hostname('new_host_name')
+   my_device.update_hostname('new_host_name')
            
    ```
         
 - send_cli(self, command: list or str, read_until=None, type_=None, **kwargs) -> str:
 
 发送命令，支持多条，返回最后一条命令输入后的结果
 
@@ -211,15 +211,15 @@
     - 返回（return）
         
     读取超时时返回Exception， 如果命令执行正确，返回最后一条命令输入后的结果
     
     - 实例
 
 ```python
-           my_device.send_cli('ifconfig ath0')
+   my_device.send_cli('ifconfig ath0')
            
    ```
 	
 - assert_cli(self, cli=None, expect=None, timeout=120, interval=5, type_='super', key_replace=None, key_replace_type='last_read', interface_replace_type='cli'):
 
 在某个模式下支持输入一条或多条命令, 且支持对执行时最后一条命令返回的结果做断言, 该方法对ping tcpdump命令 无效
 
@@ -247,15 +247,15 @@
         
     None|Exception
     
     - 实例
 
 
 ```python
-           my_device.assert_cli('ifconfig ath0', expect='HWaddr 00:18:05:A0:00:03')
+   my_device.assert_cli('ifconfig ath0', expect='HWaddr 00:18:05:A0:00:03')
            
    ```
  
 - ping(self, address='www.baidu.com', packets_number=4, params='', key_replace=None, lost_packets=False):
 
 设备里面ping地址
 
@@ -269,15 +269,15 @@
     - 返回（return）
         
     None|Exception
     
     - 实例
 
 ```python
-           my_device.ping()
+   my_device.ping()
            
    ```
         
 - tcpdump(self, expect: str or list or dict, key_replace=None, timeout=30, interval=5, **kwargs):
 
 设备里面抓包
 
@@ -294,15 +294,15 @@
     - 返回（return）
         
     None|Exception
     
     - 实例
 
 ```python
-           my_device.tcpdump()
+   my_device.tcpdump()
            
    ```
         
 - re_match(self, command: str or list, regular: str or list, type_='super', key_replace=None, key_replace_type='last_read') -> str or list:
 
 根据表达式获取最后一次执行命令的匹配值
 
@@ -322,15 +322,15 @@
     - 返回（return）
         
     Exception|str or list ，根据正则表达式的个数返回值
     
     - 实例
 
 ```python
-           my_device.re_match('ifconfig ath0', r'HWaddr(.*)inet6')
+   my_device.re_match('ifconfig ath0', r'HWaddr(.*)inet6')
            
    ```
 - kill_process(self, name: str)
 
 使用kill杀死对应进程
 
     - 参数解析
@@ -338,15 +338,15 @@
     - 返回（return）
         
     None
     
     - 实例
 
 ```python
-           my_device.kill_process('DeviceManager')
+   my_device.kill_process('DeviceManager')
            
    ```
 
 - reboot(self)
 
 重启设备
 
@@ -354,25 +354,25 @@
     - 返回（return）
         
     None
     
     - 实例
 
 ```python
-           my_device.reboot()
+   my_device.reboot()
            
    ```
 - close(self)
 
 关闭连接
 
     - 参数解析
     - 返回（return）
         
     None
     
     - 实例
 
 ```python
-           my_device.close()
+   my_device.close()
            
    ```
```

### Comparing `inhandtest-0.0.4/inhandtest/telnet.py` & `inhandtest-0.0.5/inhandtest/telnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,49 +6,49 @@
 telnet
 
 """
 import logging
 import re
 import telnetlib
 import time
-from tools import loop_inspector
+from inhandtest.tools import loop_inspector
 
 
 class Telnet:
     __doc__ = '使用telnet连接设备，封装下面命令'
 
     def __init__(self, model: str, host: str, super_user: str, super_password: str, user='adm', password='123456',
                  port=23, **kwargs):
         """使用telnet连接设备
 
-        :param model: 设备型号，‘VG710'
+        :param model: 设备型号，VG710'|'IR302'|'ER805'|'ER605'
         :param host: 设备lan ip， 192.168.2.1
         :param super_user: 超级管理员的用户名称
         :param super_password:  超级管理员的密码
         :param user: 用户名
         :param password: 用户密码
         :param port: 端口
         :param kwargs: interface_replace, 字典类型，只替换输入命令 {'wan': 'wan0', 'wifi_sta': 'wan2', 'cellular1': 'wwan0'}
                        在telnet里面接口名称转换，使得输入命令时接口名称统一。
 
         """
-        self.model = model
+        self.model = model.upper()
         self.host = host
         self.super_user = super_user
         self.super_password = super_password
         self.user = user
         self.password = password
         self.port = port
         self.host_name = ''
         self.super_tag = '/www #'
         self.config_tag = '(config)#'
         self.user_tag = '#'
         self.normal_tag = '>'
         self.interface_replace: dict = kwargs.get('interface_replace')
-        if self.model.upper() not in ['VG710']:
+        if self.model not in ['VG710', 'IR302', 'ER805', 'ER605']:
             raise Exception(f'Not support this device model {self.model}')
         self.tn: telnetlib.Telnet
         self.__login()
 
     def update_hostname(self, hostname: str):
         """更新hostname 后对应的telnet也需要更新
 
@@ -61,15 +61,15 @@
 
     def __login(self):
         """
 
 
         :return:
         """
-        login_spe = {"VG710": '#'}
+        login_spe = {"VG710": '#', 'IR302': '>', 'ER805': '#', 'ER605': '#'}
         try:
             # 连接telnet服务器
             logging.info("Start telnet 【%s:%s】" % (self.host, self.port))
             self.tn = telnetlib.Telnet(self.host, self.port, timeout=10)
         except:
             raise ConnectionError(f'Device【{self.host}:{self.port} connect failed】')
         logging.info("Telnet 【%s:%s】 connected" % (self.host, self.port))
@@ -139,21 +139,30 @@
         @return:
         """
         self.tn.write(("\003" + "\r").encode("cp936"))
         time.sleep(1)
         read_contents = self.tn.read_very_eager().decode('cp936').strip()
         logging.info(read_contents)
         if self.config_tag in read_contents:
-            self.send_cli(["exit", self.super_user + " " + self.super_password])
+            if self.model in ['VG710', 'ER805', 'ER605']:
+                self.send_cli(["exit", self.super_user + " " + self.super_password])
+            elif self.model == 'IR302':
+                self.send_cli(["exit", "exit", "support enable", self.super_user, self.super_password])
         elif self.super_tag in read_contents or (('/' in read_contents) and (' #' in read_contents)):
             self.send_cli(['cd /www'])
         elif self.user_tag in read_contents:
-            self.send_cli([self.super_user + " " + self.super_password])
+            if self.model in ['VG710', 'ER805', 'ER605']:
+                self.send_cli([self.super_user + " " + self.super_password])
+            elif self.model == 'IR302':
+                self.send_cli(["exit", "support enable", self.super_user, self.super_password])
         elif self.normal_tag in read_contents:
-            self.send_cli(["enable", self.password, self.super_user + ' ' + self.super_password])
+            if self.model in ['VG710', 'ER805', 'ER605']:
+                self.send_cli(["enable", self.password, self.super_user + ' ' + self.super_password])
+            elif self.model == 'IR302':
+                self.send_cli(["support enable", self.super_user, self.super_password])
         else:
             logging.warning(f'not support this mode. telnet return contents: {read_contents}')
             self.close()
             self.__login()
             self.super_mode()
         logging.info(f"Device {self.host} access in super mode")
 
@@ -166,19 +175,24 @@
         self.tn.write(("\003" + "\r").encode("cp936"))
         time.sleep(1)
         read_contents = self.tn.read_very_eager().decode('cp936').strip()
         logging.info(read_contents)
         if self.config_tag in read_contents:
             pass
         elif self.super_tag in read_contents or (('/' in read_contents) and (' #' in read_contents)):
-            self.send_cli(["cli", "con t"])
+            if self.model in ['VG710', 'ER805', 'ER605']:
+                self.send_cli(["cli", "con t"])
+            elif self.model == 'IR302':
+                self.send_cli(["console", "enable", self.password, 'con t'])
         elif self.user_tag in read_contents:
-            self.send_cli(['con t'])
+            if self.model in ['VG710', 'IR302', 'ER805', 'ER605']:
+                self.send_cli(['con t'])
         elif self.normal_tag in read_contents:
-            self.send_cli(["enable", self.password, 'con t'])
+            if self.model in ['VG710', 'IR302', 'ER805', 'ER605']:
+                self.send_cli(["enable", self.password, 'con t'])
         else:
             logging.warning(f'not support this mode, last content:{read_contents}')
             self.close()
             self.__login()
             self.config_mode()
         logging.info(f"Device {self.host} access in config mode")
 
@@ -189,21 +203,26 @@
         :return:
         """
         self.tn.write(("\003" + "\r").encode("cp936"))
         time.sleep(1)
         read_contents = self.tn.read_very_eager().decode('cp936').strip()
         logging.info(read_contents)
         if self.config_tag in read_contents:
-            self.send_cli(['exit'])
+            if self.model in ['VG710', 'IR302', 'ER805', 'ER605']:
+                self.send_cli(['exit'])
         elif self.super_tag in read_contents or (('/' in read_contents) and (' #' in read_contents)):
-            self.send_cli(["cli"])
+            if self.model in ['VG710', 'ER805', 'ER605']:
+                self.send_cli(["cli"])
+            elif self.model in ['IR302']:
+                self.send_cli(["console", "enable", self.password])
         elif self.user_tag in read_contents:
             pass
         elif self.normal_tag in read_contents:
-            self.send_cli(["enable", self.password])
+            if self.model in ['VG710', 'IR302', 'ER805', 'ER605']:
+                self.send_cli(["enable", self.password])
         else:
             logging.warning(f'not support this mode. telnet return contents: {read_contents}')
             self.close()
             self.__login()
             self.user_mode()
         logging.info(f"Device {self.host} access in user mode")
 
@@ -214,19 +233,28 @@
         :return:
         """
         self.tn.write(("\003" + "\r").encode("cp936"))  # 普通模式下输入ctrl+c会返回  % Command is not supported!
         time.sleep(1)
         read_contents = self.tn.read_very_eager().decode('cp936').strip()
         logging.info(read_contents)
         if self.config_tag in read_contents:
-            self.send_cli(['exit', 'disable'])
+            if self.model in ['VG710', 'ER805', 'ER605']:
+                self.send_cli(['exit', 'disable'])
+            elif self.model in ['IR302']:
+                self.send_cli(['exit', 'exit'])
         elif self.super_tag in read_contents or (('/' in read_contents) and (' #' in read_contents)):
-            self.send_cli(["cli", "disable"])
+            if self.model in ['VG710', 'ER805', 'ER605']:
+                self.send_cli(["cli", "disable"])
+            elif self.model in ['IR302']:
+                self.send_cli(["console"])
         elif self.user_tag in read_contents:
-            self.send_cli(['disable'])
+            if self.model in ['VG710', 'ER805', 'ER605']:
+                self.send_cli(['disable'])
+            elif self.model in ['IR302']:
+                self.send_cli(['exit'])
         elif self.normal_tag in read_contents:
             pass
 
         else:
             logging.warning(
                 f'not support this mode. telnet return contents: {read_contents} normal_tag: {self.normal_tag}')
             self.close()
@@ -482,15 +510,14 @@
         :param key_replace: dict 替换最后一次命令返回内容的值 默认：{'\r\n':'', ' ': ''}
         :param key_replace_type: 'cli'|'last_read'|'cli_last_read'，仅在key_replace 有值时生效，默认last_read
                                  'cli': 仅替换发出去的命令
                                  'last_read': 仅替换最后读取到的内容
                                  'cli_last_read': 既要替换cli 也要替换最后读取到的内容
         :return: str or list ，根据正则表达式的个数返回值
         """
-        key_replace = {'\r\n': '', ' ': ''} if not key_replace else key_replace
         result = self.send_cli(command, type_=type_, key_replace=key_replace, key_replace_type=key_replace_type)
         if isinstance(regular, str):
             re_list = re.findall(regular, result)
             if re_list:
                 for i in re_list:
                     if isinstance(i, str):
                         return re.findall(regular, result)[0]
@@ -511,14 +538,31 @@
                             result_.append(re.findall(regular_, result)[0][0])
                 else:
                     logging.info(f'regular {regular_} match content None')
                     return False
             else:
                 return result_
 
+    # intools 实现获取信息更改信息
+    @__auto_login
+    def in_tools(self, get_info: str or list) -> str or list or None:
+        """在超级模式下可以获取或者设置相关intools的属性
+
+        :param get_info: 常用属性可能会有productnumber,oem_name,等intools里面的属性
+                       列： get_info='productnumber'，需要获取多个属性时采用列表传入
+
+        :return: 返回需要获取的信息
+        """
+        if get_info:
+            if isinstance(get_info, str):
+                regular = f'{get_info}=(.*)\\r\\n'
+            else:
+                regular = [f'{info}=(.*)\\r\\n' for info in get_info]
+            return self.re_match('intools', regular)
+
     @__auto_login
     def kill_process(self, name: str):
         """使用kill杀死对应进程
 
         :param name: 进程相关名称
         :return:
         """
@@ -554,8 +598,8 @@
 
 if __name__ == '__main__':
     import sys
 
     logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
                         stream=sys.stdout)
     my = Telnet('VG710', '10.5.47.197', 'inhand', '64391099@inhand', interface_replace={'wifi': 'ath0'})
-    my.kill_process('DeviceManager')
+    my.in_tools(get_info='productnumber')
```

### Comparing `inhandtest-0.0.4/inhandtest/tools.py` & `inhandtest-0.0.5/inhandtest/tools.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.4/setup.py` & `inhandtest-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 setup
 
 """
 from distutils.core import setup
 
 setup(
     name='inhandtest',
-    version='0.0.4',
+    version='0.0.5',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     py_modules=['inhandtest.tools', 'inhandtest.telnet'],
     long_description='inhand test tools, so easy',
```

