# Comparing `tmp/Alpha_Rabbit-1.3.7.tar.gz` & `tmp/Alpha_Rabbit-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Alpha_Rabbit-1.3.7.tar", last modified: Mon Apr 17 06:11:23 2023, max compression
+gzip compressed data, was "Alpha_Rabbit-1.3.8.tar", last modified: Mon Apr 17 06:21:20 2023, max compression
```

## Comparing `Alpha_Rabbit-1.3.7.tar` & `Alpha_Rabbit-1.3.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 06:11:23.640563 Alpha_Rabbit-1.3.7/
-drwxrwxrwx   0        0        0        0 2023-04-17 06:11:23.635571 Alpha_Rabbit-1.3.7/Alpha_Rabbit/
--rw-rw-rw-   0        0        0    25924 2023-04-17 06:09:48.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit/Alpha_Rabbit.py
--rw-rw-rw-   0        0        0    13938 2023-03-24 06:59:51.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit/Factor_Calculator.py
--rw-rw-rw-   0        0        0    22640 2023-03-24 01:41:23.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit/Factor_Def_and_Get_Method.py
--rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit/trade_strategy.py
-drwxrwxrwx   0        0        0        0 2023-04-17 06:11:23.640563 Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/
--rw-rw-rw-   0        0        0      787 2023-04-17 06:11:23.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-04-17 06:11:23.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 06:11:23.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-17 06:11:23.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-17 06:11:23.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.7/LICENSE.txt
--rw-rw-rw-   0        0        0      787 2023-04-17 06:11:23.640563 Alpha_Rabbit-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.7/README.md
--rw-rw-rw-   0        0        0       85 2023-04-17 06:11:23.641556 Alpha_Rabbit-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1229 2023-04-17 06:11:15.000000 Alpha_Rabbit-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 06:21:20.761835 Alpha_Rabbit-1.3.8/
+drwxrwxrwx   0        0        0        0 2023-04-17 06:21:20.754912 Alpha_Rabbit-1.3.8/Alpha_Rabbit/
+-rw-rw-rw-   0        0        0    25944 2023-04-17 06:21:05.000000 Alpha_Rabbit-1.3.8/Alpha_Rabbit/Alpha_Rabbit.py
+-rw-rw-rw-   0        0        0    13938 2023-03-24 06:59:51.000000 Alpha_Rabbit-1.3.8/Alpha_Rabbit/Factor_Calculator.py
+-rw-rw-rw-   0        0        0    22640 2023-03-24 01:41:23.000000 Alpha_Rabbit-1.3.8/Alpha_Rabbit/Factor_Def_and_Get_Method.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.8/Alpha_Rabbit/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.8/Alpha_Rabbit/trade_strategy.py
+drwxrwxrwx   0        0        0        0 2023-04-17 06:21:20.760650 Alpha_Rabbit-1.3.8/Alpha_Rabbit.egg-info/
+-rw-rw-rw-   0        0        0      787 2023-04-17 06:21:20.000000 Alpha_Rabbit-1.3.8/Alpha_Rabbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-04-17 06:21:20.000000 Alpha_Rabbit-1.3.8/Alpha_Rabbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 06:21:20.000000 Alpha_Rabbit-1.3.8/Alpha_Rabbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-17 06:21:20.000000 Alpha_Rabbit-1.3.8/Alpha_Rabbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-17 06:21:20.000000 Alpha_Rabbit-1.3.8/Alpha_Rabbit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.8/Alpha_Rabbit.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      787 2023-04-17 06:21:20.761835 Alpha_Rabbit-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.8/README.md
+-rw-rw-rw-   0        0        0       85 2023-04-17 06:21:20.762839 Alpha_Rabbit-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2023-04-17 06:21:10.000000 Alpha_Rabbit-1.3.8/setup.py
```

### Comparing `Alpha_Rabbit-1.3.7/Alpha_Rabbit/Alpha_Rabbit.py` & `Alpha_Rabbit-1.3.8/Alpha_Rabbit/Alpha_Rabbit.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         pcaModel.fit(data)
         pcaFactors = pcaModel.transform(data)
         pcaFactors = pd.DataFrame(pcaFactors)
         pcaFactors.index = originalFactor.index
         pcaFactors.columns = ['pca_'+str(i) for i in range(domain_factor_nums)]
         return pcaModel.explained_variance_,pcaModel.explained_variance_ratio_,pcaFactors
 
-    def batch_factors_test(allfactors,Price,quantiles,days,barranorm):
+    def batch_factors_test(self,allfactors,Price,quantiles,days,barranorm):
         from alphalens import utils
         returndict = {}
         corrdict = {}
         for fc in list(allfactors):
             print(fc)
             test_fc = allfactors[[fc]].copy().rename_axis(['date','symbol'])
             res_df = sst.one_factor_grouper(test_fc,fc,quantiles)# 序数标准化
@@ -432,15 +432,15 @@
         a2.tick_params(axis='x', labelrotation= 30)
         a2.xaxis.set_major_locator(ticker.MultipleLocator(tickspace))
         
 
         fig.legend(frameon = False,labels = [bname+'(left)',fname+'(right)'],loc = 'upper center')
         plt.show()
 
-    def factor_plt(qreturn,fc,quantiles,savedir):
+    def factor_plt(self,qreturn,fc,quantiles,savedir):
         from alphalens import utils
         utils.print_table(pd.concat([qreturn.mean(),qreturn.sum()],axis = 1).rename(columns= {0:'avg',1:'sum'}).T)
         totalSeed = qreturn.index
         xticks = list(range(0, len(totalSeed), 60))
         xlabels = [str(totalSeed[x]) for x in xticks]
         import matplotlib.pyplot as plt
         plt.figure(dpi=300, figsize=(24, 13))
@@ -457,15 +457,15 @@
         plt.xticks(rotation=30)
         plt.xticks(ticks=xticks, labels=xlabels)
         plt.savefig(savedir+fc+'.jpg')
         plt.show()
         plt.close()
 
     # 热力图展示
-    def ShowHeatMap(DataFrame,savedir):
+    def ShowHeatMap(self,DataFrame,savedir):
         import matplotlib.pyplot as plt
         import seaborn as sns
         f, ax = plt.subplots(figsize=(35, 15))
         ax.set_title('Wine GRA')
         # 设置展示一半，如果不需要注释掉mask即可
         mask = np.zeros_like(DataFrame)
         mask[np.triu_indices_from(mask)] = True  # np.triu_indices 上三角矩阵
@@ -475,15 +475,15 @@
                         cmap="YlGnBu",
                         annot=True,
                         mask=mask,
                         )
         plt.savefig(savedir)
         plt.show()
 
-    def combine_imgs_pdf(folder_path, pdf_file_path,idstname):
+    def combine_imgs_pdf(self,folder_path, pdf_file_path,idstname):
         import os
         from PIL import Image
         """
         合成文件夹下的所有图片为pdf
         Args:
             folder_path (str): 源文件夹
             pdf_file_path (str): 输出路径
```

### Comparing `Alpha_Rabbit-1.3.7/Alpha_Rabbit/Factor_Calculator.py` & `Alpha_Rabbit-1.3.8/Alpha_Rabbit/Factor_Calculator.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.3.7/Alpha_Rabbit/Factor_Def_and_Get_Method.py` & `Alpha_Rabbit-1.3.8/Alpha_Rabbit/Factor_Def_and_Get_Method.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.3.7/Alpha_Rabbit/trade_strategy.py` & `Alpha_Rabbit-1.3.8/Alpha_Rabbit/trade_strategy.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/PKG-INFO` & `Alpha_Rabbit-1.3.8/Alpha_Rabbit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Alpha-Rabbit
-Version: 1.3.7
+Version: 1.3.8
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.3.7/LICENSE.txt` & `Alpha_Rabbit-1.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.3.7/PKG-INFO` & `Alpha_Rabbit-1.3.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Alpha_Rabbit
-Version: 1.3.7
+Version: 1.3.8
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.3.7/setup.py` & `Alpha_Rabbit-1.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Alpha_Rabbit",
-    version="1.3.7",
+    version="1.3.8",
     author="lijiongting",
     author_email="448986334@qq.com",
     description="Alpha_Rabbit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="",
```

