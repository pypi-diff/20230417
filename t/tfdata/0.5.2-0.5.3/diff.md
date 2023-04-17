# Comparing `tmp/tfdata-0.5.2.tar.gz` & `tmp/tfdata-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfdata-0.5.2.tar", last modified: Tue Apr  4 01:06:57 2023, max compression
+gzip compressed data, was "tfdata-0.5.3.tar", last modified: Mon Apr 17 08:48:32 2023, max compression
```

## Comparing `tfdata-0.5.2.tar` & `tfdata-0.5.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 01:06:57.784324 tfdata-0.5.2/
--rw-rw-rw-   0        0        0       41 2022-01-08 07:41:24.000000 tfdata-0.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0      418 2023-04-04 01:06:57.783325 tfdata-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      140 2023-04-04 01:06:33.000000 tfdata-0.5.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-04 01:06:57.784324 tfdata-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0      633 2023-04-04 01:06:42.000000 tfdata-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 01:06:57.031405 tfdata-0.5.2/tfdata/
--rw-rw-rw-   0        0        0      131 2023-04-03 22:37:31.000000 tfdata-0.5.2/tfdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 01:06:57.595773 tfdata-0.5.2/tfdata/menu_text/
--rw-rw-rw-   0        0        0    28494 2023-04-03 21:24:06.000000 tfdata-0.5.2/tfdata/menu_text/att_list.py
--rw-rw-rw-   0        0        0    14761 2023-04-02 21:36:39.000000 tfdata-0.5.2/tfdata/menu_text/menu_text0.py
--rw-rw-rw-   0        0        0     2081 2022-06-13 22:00:20.000000 tfdata-0.5.2/tfdata/menu_text/update_note.py
--rw-rw-rw-   0        0        0     6762 2023-04-03 19:38:23.000000 tfdata-0.5.2/tfdata/test_stra.py
--rw-rw-rw-   0        0        0    54353 2023-04-04 01:06:09.000000 tfdata-0.5.2/tfdata/tfclient.py
-drwxrwxrwx   0        0        0        0 2023-04-04 01:06:57.782333 tfdata-0.5.2/tfdata/utils/
--rw-rw-rw-   0        0        0       92 2022-01-07 07:10:02.000000 tfdata-0.5.2/tfdata/utils/TF_utils.py
--rw-rw-rw-   0        0        0      169 2021-11-19 16:43:28.000000 tfdata-0.5.2/tfdata/utils/__init__.py
--rw-rw-rw-   0        0        0     2283 2023-04-02 10:02:09.000000 tfdata-0.5.2/tfdata/utils/comm_utils.py
--rw-rw-rw-   0        0        0     1342 2021-07-08 21:36:53.000000 tfdata-0.5.2/tfdata/utils/network_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-04 01:06:57.061400 tfdata-0.5.2/tfdata.egg-info/
--rw-rw-rw-   0        0        0      418 2023-04-04 01:06:55.000000 tfdata-0.5.2/tfdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-04-04 01:06:55.000000 tfdata-0.5.2/tfdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 01:06:55.000000 tfdata-0.5.2/tfdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-04 01:06:55.000000 tfdata-0.5.2/tfdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 08:48:32.197695 tfdata-0.5.3/
+-rw-rw-rw-   0        0        0       41 2022-01-08 07:41:24.000000 tfdata-0.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      418 2023-04-17 08:48:32.195690 tfdata-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      140 2023-04-17 08:29:13.000000 tfdata-0.5.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 08:48:32.197695 tfdata-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      721 2023-04-17 08:48:21.000000 tfdata-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:48:31.765730 tfdata-0.5.3/tfdata/
+-rw-rw-rw-   0        0        0      131 2023-04-03 22:37:31.000000 tfdata-0.5.3/tfdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:48:31.991389 tfdata-0.5.3/tfdata/menu_text/
+-rw-rw-rw-   0        0        0    28494 2023-04-03 21:24:06.000000 tfdata-0.5.3/tfdata/menu_text/att_list.py
+-rw-rw-rw-   0        0        0    14951 2023-04-17 08:41:29.000000 tfdata-0.5.3/tfdata/menu_text/menu_text0.py
+-rw-rw-rw-   0        0        0     2433 2023-04-17 08:31:18.000000 tfdata-0.5.3/tfdata/menu_text/update_note.py
+-rw-rw-rw-   0        0        0     7419 2023-04-15 13:26:27.000000 tfdata-0.5.3/tfdata/test_stra.py
+-rw-rw-rw-   0        0        0    54711 2023-04-17 08:41:29.000000 tfdata-0.5.3/tfdata/tfclient.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:48:32.193105 tfdata-0.5.3/tfdata/utils/
+-rw-rw-rw-   0        0        0       92 2022-01-07 07:10:02.000000 tfdata-0.5.3/tfdata/utils/TF_utils.py
+-rw-rw-rw-   0        0        0      169 2021-11-19 16:43:28.000000 tfdata-0.5.3/tfdata/utils/__init__.py
+-rw-rw-rw-   0        0        0     2435 2023-04-17 05:24:19.000000 tfdata-0.5.3/tfdata/utils/comm_utils.py
+-rw-rw-rw-   0        0        0     1342 2021-07-08 21:36:53.000000 tfdata-0.5.3/tfdata/utils/network_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:48:31.800314 tfdata-0.5.3/tfdata.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-04-17 08:48:29.000000 tfdata-0.5.3/tfdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2023-04-17 08:48:30.000000 tfdata-0.5.3/tfdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 08:48:29.000000 tfdata-0.5.3/tfdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-17 08:48:30.000000 tfdata-0.5.3/tfdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 08:48:30.000000 tfdata-0.5.3/tfdata.egg-info/top_level.txt
```

### Comparing `tfdata-0.5.2/setup.py` & `tfdata-0.5.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tfdata",
-    version="0.5.2",
+    version="0.5.3",
     author="DrEdw",
     author_email="ed@topfintech.org",
     description="NA",
     long_description="NA",
     long_description_content_type="text/markdown",
     url="https://github.com/edwincca/tfdata/blob/master/README.md",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    install_requires=[
+          'tdautils','numpy','pandas'
+                     ],
     include_package_data=True
 )
```

### Comparing `tfdata-0.5.2/tfdata/menu_text/att_list.py` & `tfdata-0.5.3/tfdata/menu_text/att_list.py`

 * *Files identical despite different names*

### Comparing `tfdata-0.5.2/tfdata/menu_text/menu_text0.py` & `tfdata-0.5.3/tfdata/menu_text/menu_text0.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 islogin = 'islogin\n简介 函数返回登录状态,True表示已成功登录数据服务器False表示未成功登录'
 get_btdata_text ="get_btdata\n简介:函数用于下载补充回测时间轴内context数据\n参数：trade_func:数据频率-daily/tick/min,必填;code:标的代码集合,选填,默认包含所有在self.context[freq]下的标的代码; start_date,回测时间轴起始日,格式yyyy-mm-dd,必填;end_date,回测时间轴结束日,格式yyyy-mm-dd,必填;overwrite,是否覆盖context目录下已存在的数据点,选填,默认=False,即已存在的数据点不会被覆盖,将节省API网络资源和下载时间"
 run_bt_text = "run_bt\n简介:函数根据用户交易函数对context数据进行实盘回测运算,运算结果直接添加至context\n参数：trade_func:用户编写的交易函数,详见self.get_menu('trade_func'), 必填;freq:数据频率-daily/tick/min,必填; start_time,回测时间轴起始日,,必填;end_date,回测时间轴结束日,格式yyyy-mm-dd,必填;code_base: 回测程序包含的标的代码集合,选填,默认包含所有在self.context[freq]下的标的代码; trade_cost_rate: 模拟实盘交易费率,选填,默认每笔交易金额的万分之一,最低消费1分;thread_pool: 运算线程数目, 当标的合集包含多个标的证券时, 可使用多线程尝试提高运行速度, 默认使用单线程, 返回: None,报错文本"
 cal_portf_text ="cal_portf\n简介: 函数计算回测策略综合收益并生成报表, 使用前必须确保针对所有的标的回测计算已经完成并写入self.context\n参数：freq: 分析对象的数据频率-daily/tick/min,必填; init_fund: 模拟实盘投资的起始资本额,默认100万,选填; margin_cost: 当模拟实盘账户现金不足是, 融资利率, 不设融资上限, 用户需自行监控爆仓的情况; ss_cost: 融券利率, 不设融券障碍, 用户需按实际情况设定障碍; ON_rate: 账户中现金的隔夜回报年化利率,返回: 如有错误返回错误报告文本否则返回每日组合收益表单, 综合收益统计表单, 两个表单以tuple格式返回, 其中收益统计表单各项指标说明如下: total_trading_points交易点总数,active_rate信号输出率,即有信号的交易日占比, ave_t_cash平均持有现金数额(每个交易节点),ave_t_asset平均持有交易标的价值数额, init_pvalue起始资产额度, end_pvalue回测期末资产额度, max_pvalue回测期组合资产额最大值, min_pvalue回测期组合资产额最小值, total_trade_cost总交易费用, total_int_paid融资利率费用, overall_return期末综合回报率(非年化), ave_t_return平均每个交易节点收益率(非年化), std_t_return 交易节点收益协方差, MDD最大回撤, sharpe_ratio夏普比率"
 trade_func_text = "trade_func\n简介: 用户根据回测框架编写的交易函数, 回测程序在每一个交易点(如,日线,分钟线,tick跳价), 将发生在该节点时间戳前的context数据作为信息集供与交易函数, 该设计模拟投资者在实盘中的交易决策.\n 对交易函数框架要求如下: 1.必须包含context参数并置于首位,用户可添加其他自定义参数; 2.必须以文本格式返回符合规范的交易信号; 3.下单交易信号以 dirction@price表示,其中dirction代表买卖方向,用'B'表示买入,'S'表示卖出,price即信号买入/卖出价,例: B@3.31, 表示以3.31元买入, 注意买卖信号同样代表交易结果, 用户需考虑撮合机制并在交易函数中协调实现; 4. 交易函数返回'0'表示无交易,并下单清空持有仓位, 'HB'/'HS' 分别表示继续持有多头或空头仓位至下一个交易点\n 工作原理: 用户自定交易函数一般套用于回测函数trade_func位置. 回测函数模拟实盘时间流, 将每个交易点对应的context信息集, 即模拟环境下投资者能得到的市场数据, 作为参数向trade_func推送并得到相应的交易信号, 回测程序将根据该交易信号计算收益."
 event_study_text = 'event_study\n简介: 事件研究框架函数, 程序根据用户提供的事件定义函数, 对context数据进行筛选,对符合条件的交易点进行标签以及数据筛查.\n参数：target:指定的context数据(例:daily,tick), event_func:用户编写的事件函数(详见self.menu("event_func"),event_name: 事件标签名, start_time,回测时间轴起点,选填,默认为None,表示使用context数据最早时间点, end_time,回测时间轴终点,选填,默认为None,表示使用context数据的最后时间点;code_base: 回测程序包含的标的代码集合'
 event_func_text = "event_func\n简介:用户指定的事件函数须符合以下基本要求: 1.以t日可用context数据作为基础参数, 2. 返回一组元组数据, 其中首位为二维代码 1/0用于表示是否赋予event标签,次位返回 None 或与该event相关的用于后期统计的数据"
+gen_tdlist_text = "gen_tdlist\n简介:按照date_range参数返回A股交易日集合,关于date_range参数见self.get_menu('date_range')"
 
 
 
 menu_basic_cn = {'intro':intro_text,
                  'code':code_text,
                  'att':att_text,
                  'usage':usage_text,
@@ -55,9 +56,10 @@
                  'get_btdata':get_btdata_text,
                  'run_bt':run_bt_text,
                  'cal_portf': cal_portf_text,
                  "trade_func":trade_func_text,
                  "event_study":event_study_text,
                  "event_func":event_func_text,
                  "get_stock_fs":get_stock_fs_text,
-                 "get_hist_share":get_hist_share_text
+                 "get_hist_share":get_hist_share_text,
+                 "gen_tdlist": gen_tdlist_text
                  }
```

### Comparing `tfdata-0.5.2/tfdata/menu_text/update_note.py` & `tfdata-0.5.3/tfdata/menu_text/update_note.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 @author: edlaptop
 """
 update_note = { 
 "top0": "内测会员账户已开放, 欢迎提交申请(http://www.topfintech.org/user_management); 提交bug报告,送永久免费数据使用权限",
 "top1": "API数据接口用户手册PDF文档已开放下载:http://www.topfintech.org/TF_API",
 "top2": "邀请内测用户加wx群讨论问题： wx: dredw_tf (加好友请备注账户名)",
 "top3": '用户验证流程已优化, 现只需要提供访问密匙就可在客户端登录服务器, 旧用户请在微信公众号输入"重置密匙"获取访问密匙',
+"v0.5.3": "开放国债逆回购tick数据, 开放gen_tdlist函数, 用于返回指定A股交易日集合",
+"v0.5.0": "优化hf_min数据获取方法,现可选1-60min freq, 重新整理get_daily接口, 将数据分为daily,valuation,ms三大类,将HSGT设为独立接口,详见最新说明文档",
+"v0.4.0": "加入事件学习,策略回测功能",
 "v0.3.1": "优化用户验证方式,客户端不再需要安装加密库以便兼容用户在其他量化平台使用客户端, 现采用动态访问密匙,而不再需要用户名+密码, 用户信息加密由服务器处理",
 "v0.2.9": "日间分钟线(股票, ETF) 可选择 1,3,5,10,15,30分钟频率数据, 详见 说明文本, self.hf_min",
 "v0.2.8": "日间分钟线(股票, ETF) 数据开放, 详见 说明文本, self.hf_min",
 "v0.2.7": "hot fix self.get_daily 错误",
 "v0.2.6": "ETF期权表单get_1d数据标签，修正get_daily pindex 错误问题",
 "v0.2.5": "添加可转债日线、扩展日线，tick，hf5数据接口，添加上交所股指期权日线、扩展日线，tick、hf5数据接口",
 "v0.2.4": "添加一系列可转债get_1d 数据标签",
```

### Comparing `tfdata-0.5.2/tfdata/test_stra.py` & `tfdata-0.5.3/tfdata/test_stra.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,37 @@
 the signal starts with a char represent the trade direction B = Buy, S=sell, 
 H = holding the previous position ,followed by trading vol and then @ as the hint for limit price, 
 e.g B1000@5.1 means a trading signal for buying 1000 units at a limit price of 5.1,
 'HB'/'HS' means to hold the previous generated buy/sell signal
 signal = '0' means to liquidate all positions. 
 
 """
+def gap_event_daily(context,t=0.005):
+
+    # context为必选参数, t为用户设计的可选参数, 这里t为决定事件市场成立的临界值,设置越接近0, 事件被标签机会越大
+
+    if 'close' not in context.columns or 'open' not in context.columns:
+
+        return 'open/close columns not found'
+
+    else:
+
+        if context.shape[0] <2 :
+
+            return 0,None
+        else:
+
+            if context["open"].iat[-1]/context["close"].iat[-2] - 1 >t:
+
+                return 1,context[['open','close']].iloc[[-1]]
+
+#标签事件并返回需收集的事件数据
+            else:
+                return 0,None
+
 
 def daily_3mom (context,p='close',q=10000):
     #p is the trade price
     #q is the trade quant
     """
     buy/sell when the last three trade days have positive/negative returns
     assume buy/sell at the last window day at market close when the investor realizes the signal at the leat minute and act on it
```

### Comparing `tfdata-0.5.2/tfdata/tfclient.py` & `tfdata-0.5.3/tfdata/tfclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 TFdata client package manages the communicaton between TFdata servers and user-side client application.
 User acct and user_pw are required for communicating with the data server. Check www.topfintech.org for details
 """
 
 __author__ = "DrEdw  (ed@topfintech.org)"
 __copyright__ = "Copyright (c) 2020-2021 ed@topfintech.org by the MIT license"
 __license__ = "MIT"
-__verson__ = '0.5.2'
+__verson__ = '0.5.3'
 
 from tfdata.menu_text.menu_text0 import menu_basic_cn
 from tfdata.menu_text.att_list import *
 from tfdata.utils.network_utils import tryrq  
 from tfdata.utils.comm_utils import timenow,pro_ts,get_codetype
 import pandas as pd
 import numpy as np
@@ -45,15 +45,15 @@
                            'get_HSGT_name':get_HSGT_name,'get_econ_name':get_econ_name,'get_daily_name':get_daily_name,\
                                'get_stock_fs_name':get_stock_fs_name,\
                                    'get_hist_share_att':get_hist_share_att}
         self.report_usage=False #if True, program will print out data usage after successful request
         self.__current_usage=0 #store usage only in current instance
         self.__offline_dir = None
         self.context = {'tick':{},'daily':{},'min':{},"econ":{},"val":{},"fs":{},"HSGT":{},"mszy":{}}
-        
+        self._ta = tradedate_A() 
         if not self.slient:
             print (menu_basic_cn['intro'])
         if auto_login:
             lo = self.login()
             if isinstance(lo,str):
                 print (lo)            
     
@@ -394,14 +394,22 @@
         if rt is None:
             return f'暂无关于{keyword}的用户手册说明'
         else:
             if printout:
                 print (rt)
             else:
                 return rt
+   
+    def gen_dtlist(self,start_date=None,end_date=None,sample_size=None):
+        """
+        return A-share market trade day list 
+        use tdautils access 
+        """
+        self._ta.update_dtindex()
+        return list(pro_ts(self._ta.gen_dtindex(start_date=start_date,end_date=end_date,sample_size=sample_size)))
     
     def _get_hf(self,code,hf_type,date,timeout=200):
         """
         provide intraday data
 
         Parameters
         ----------
```

### Comparing `tfdata-0.5.2/tfdata/utils/comm_utils.py` & `tfdata-0.5.3/tfdata/utils/comm_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,16 @@
         return 'NA' 
     elif '.CNi' in code:
         return 'index_CN'
     elif '.CNo' in code:
         return 'ETFO_CN'
     elif ('.SHb' in code or '.SZb' in code) and code[0] == '1':
         return 'CB_CN'
+    elif ('1318' in code and code[:4] == '1318' and '.SZ' in code) or ('204' in code and code[:3] =='204' and '.SH' in code):
+        return 'nhg_CN'
     else:
         if ('.SH' in code or '.SZ' in code or '.BJ' in code):
             if code[0] in ['1','5']:
                 return 'ETF_CN'
             else:
                 if code[0] in ['0','6','3','8','4']:
                     return 'stock_A'
```

### Comparing `tfdata-0.5.2/tfdata/utils/network_utils.py` & `tfdata-0.5.3/tfdata/utils/network_utils.py`

 * *Files identical despite different names*

