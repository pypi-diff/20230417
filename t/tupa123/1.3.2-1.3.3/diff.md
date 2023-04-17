# Comparing `tmp/tupa123-1.3.2.tar.gz` & `tmp/tupa123-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.3.2.tar", last modified: Mon Apr 17 12:28:43 2023, max compression
+gzip compressed data, was "tupa123-1.3.3.tar", last modified: Mon Apr 17 14:28:02 2023, max compression
```

## Comparing `tupa123-1.3.2.tar` & `tupa123-1.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 12:28:43.954535 tupa123-1.3.2/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0     7584 2023-04-17 12:28:43.953543 tupa123-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     7221 2023-04-17 12:27:34.000000 tupa123-1.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 12:28:43.954535 tupa123-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      650 2023-04-17 12:13:09.000000 tupa123-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:28:43.941787 tupa123-1.3.2/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.2/tupa123/__init__.py
--rw-rw-rw-   0        0        0    60186 2023-04-17 11:17:01.000000 tupa123-1.3.2/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:28:43.951551 tupa123-1.3.2/tupa123.egg-info/
--rw-rw-rw-   0        0        0     7584 2023-04-17 12:28:43.000000 tupa123-1.3.2/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-17 12:28:43.000000 tupa123-1.3.2/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:28:43.000000 tupa123-1.3.2/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-17 12:28:43.000000 tupa123-1.3.2/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 12:28:43.000000 tupa123-1.3.2/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 14:28:02.907846 tupa123-1.3.3/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     7810 2023-04-17 14:28:02.906850 tupa123-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7334 2023-04-17 14:18:59.000000 tupa123-1.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 14:28:02.907846 tupa123-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-17 14:09:16.000000 tupa123-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:28:02.894943 tupa123-1.3.3/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.3/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    59976 2023-04-17 13:58:16.000000 tupa123-1.3.3/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:28:02.904859 tupa123-1.3.3/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     7810 2023-04-17 14:28:02.000000 tupa123-1.3.3/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-17 14:28:02.000000 tupa123-1.3.3/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 14:28:02.000000 tupa123-1.3.3/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-17 14:28:02.000000 tupa123-1.3.3/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 14:28:02.000000 tupa123-1.3.3/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.3.2/LICENSE.txt` & `tupa123-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.3.2/PKG-INFO` & `tupa123-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.3.2
+Version: 1.3.3
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
-Keywords: artificial-intelligence neural-networks four-layers regression classification tupa123
+Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 Fully connected four-layer neural network <br>
 Solves a huge number of cases, classification and regression <br>
 The following sequence explains how to use with the help of two example files. <br>
 The first file contains the learning process, where the neural network finds its weights <br>
@@ -64,28 +64,29 @@
 #The data can come from any source, but the ExcelMatrix function allows a practical interaction with Excel <br>
 #ExcelMatrix = collect data from excel, the spreadsheet needs to be in the same folder as the python file <br>
 #'ALETAS.xlsm' = example name of the excel file / 'Sheet1' = example name of the tab where the data are <br>
 #Lineini=2, Columini=1 = example initial row and column of data <br>
 #linesquantity = number of lines of learning data <br>
 #X = regression input data / y = data to be predicted <br>
 <br>
-<b>model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='')</b> <br>
+<b>model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1)</b> <br>
 #creates the Neural Network model <br>
 <br>
 #norma = type of data normalization: (default=2)<br>
 #=-1, standardization <br>
 #=0, do anything <br>
 #=1, between 0 and 1 <br>
 #=2, between -1 and 1 <br>
 #=3, log(x+coef) <br>
 #=4, log(x+coef)  between 0 and 1 <br>
 #=5, log(x+coef)  between -1 and 1 <br>
 #=6, log(x+coef)  and standardization <br>
 #coef = used to avoid zero in log normalizations, example 0.0012345 (default=0)<br>
 #normout = if 1 normalizes the output (default=1), 0 dont <br>
+#shift = (default=1), >=1, stretches the normalization rule. Normalized data falls outside the bounds.
 <br>
 #nn1c=5, nn2c=7, nn3c=5, nn4c=2 = number of neurons from the first to the fourth layer (default=1,5,5,1) <br>
 #rate = learning rate (default=0.01) <br>
 #epochs = number of epochs (default=1000)<br>
 #fa2c=5, fa3c=5, fa4c=0 = second to fourth layer activation functions (default=5,5,0) <br>
 #for regression the fourth layer is recommended as linear = 0 <br>
 #cost=0, cost function, (default=0). 0 = MSE, mean squared error for regression and classification / 1 = BCE, binary cross entropy for classification <br>
```

### Comparing `tupa123-1.3.2/README.md` & `tupa123-1.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,28 +53,29 @@
 #The data can come from any source, but the ExcelMatrix function allows a practical interaction with Excel <br>
 #ExcelMatrix = collect data from excel, the spreadsheet needs to be in the same folder as the python file <br>
 #'ALETAS.xlsm' = example name of the excel file / 'Sheet1' = example name of the tab where the data are <br>
 #Lineini=2, Columini=1 = example initial row and column of data <br>
 #linesquantity = number of lines of learning data <br>
 #X = regression input data / y = data to be predicted <br>
 <br>
-<b>model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='')</b> <br>
+<b>model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1)</b> <br>
 #creates the Neural Network model <br>
 <br>
 #norma = type of data normalization: (default=2)<br>
 #=-1, standardization <br>
 #=0, do anything <br>
 #=1, between 0 and 1 <br>
 #=2, between -1 and 1 <br>
 #=3, log(x+coef) <br>
 #=4, log(x+coef)  between 0 and 1 <br>
 #=5, log(x+coef)  between -1 and 1 <br>
 #=6, log(x+coef)  and standardization <br>
 #coef = used to avoid zero in log normalizations, example 0.0012345 (default=0)<br>
 #normout = if 1 normalizes the output (default=1), 0 dont <br>
+#shift = (default=1), >=1, stretches the normalization rule. Normalized data falls outside the bounds.
 <br>
 #nn1c=5, nn2c=7, nn3c=5, nn4c=2 = number of neurons from the first to the fourth layer (default=1,5,5,1) <br>
 #rate = learning rate (default=0.01) <br>
 #epochs = number of epochs (default=1000)<br>
 #fa2c=5, fa3c=5, fa4c=0 = second to fourth layer activation functions (default=5,5,0) <br>
 #for regression the fourth layer is recommended as linear = 0 <br>
 #cost=0, cost function, (default=0). 0 = MSE, mean squared error for regression and classification / 1 = BCE, binary cross entropy for classification <br>
```

### Comparing `tupa123-1.3.2/setup.py` & `tupa123-1.3.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.3.2',
+    version='1.3.3',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy','matplotlib','pandas'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    keywords='artificial-intelligence neural-networks four-layers regression classification tupa123'
+    keywords='artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source'
 )
```

### Comparing `tupa123-1.3.2/tupa123/tupa123.py` & `tupa123-1.3.3/tupa123/tupa123.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,14 @@
             
     for j in range(0,numevar):    
         eixoY1= Targeted[:,j]
         eixoY2= Calculated[:,j]
         
         eixoY3 = eixoY2 - eixoY1
 
-
         # preparação para a média móvel
         rolling_mean = pd.Series(eixoY3).rolling(window_size).mean()
 
         plt.figure(figsize=(12, 5))
         plt.title('Comparison chart calculated variable vs targeted')
         plt.xlabel('Sequence of events')
         plt.ylabel('Error, Calculated - Targeted ' + str(j+1))
@@ -185,19 +184,14 @@
         plt.plot(eixoX, eixoY1 + erro_medio - 2*sigma, marker = '', c='black', alpha=0.5, linestyle='dashed', label='Expected minimum, -2S')
         plt.plot(eixoX, eixoY1 + erro_medio + 2*sigma, marker = '', c='black', alpha=0.5, linestyle='dashed', label='Expected maximum, +2S')
         plt.fill_between(np.arange(len(eixoY1)), eixoY1 + erro_medio - 2*sigma, eixoY1 + erro_medio + 2*sigma, color='gray', alpha=0.1)
                 
         #plt.plot(eixoX, eixoY2, linestyle='none', c='black', marker = '.', label='Calculated', alpha=0.33)
         plt.legend(loc = "upper right")
 
-        # Preenchendo a área entre as curvas
-        #plt.fill_between(np.arange(len(eixoY1)), eixoY1 + erro_medio - sigma, eixoY1 + erro_medio + sigma, color='gray', alpha=0.3)
-        #plt.fill_between(np.arange(len(eixoY1)), eixoY1 + erro_medio - 2*sigma, eixoY1 + erro_medio + 2*sigma, color='gray', alpha=0.2)
-        #plt.fill_between(np.arange(len(eixoY1)), eixoY1 + erro_medio - 3*sigma, eixoY1 + erro_medio + 3*sigma, color='gray', alpha=0.1)
-
         # Adicionando o valor do desvio padrão ao canto superior esquerdo do gráfico
         plt.text(0.025, 0.95, "sigma = {:.2f}".format(sigma) + ", average = {:.2f}".format(erro_medio), transform=plt.gca().transAxes, fontsize=12, verticalalignment='top')
         
         plt.show()
 
 
         
@@ -384,15 +378,15 @@
 
 
 
 #Neural network 4 layers--------------------------------------------------------------------------------------------------------------------
 class nnet4:
 
     #global variables-------------------------------------------------------------------------
-    def __init__ (self, norma=2, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=5, nn4c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet=''):
+    def __init__ (self, norma=2, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=5, nn4c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1):
         
         self.nn1c=nn1c
         self.nn2c=nn2c
         self.nn3c=nn3c
         self.nn4c=nn4c
         self.rate=rate
         self.epochs=epochs
@@ -401,14 +395,15 @@
         self.fa4c=fa4c
         self.norma=norma
         self.coef=coef
         self.normout=normout
         self.cost=cost
         self.regu=regu
         self.namenet=namenet
+        self.shift=shift
 
 
 
 
 
     #data normalization by calculating maximums and minimums-----------------------------------------------
     def Normalize(self, data, maxiname, mininame, medianame, desvioname):          
@@ -424,14 +419,18 @@
 
         if (self.norma>=3): 
             data = np.log(data + self.coef)
         normalized = data*1
         
         vetormax = np.max(data,0) 
         vetormin = np.min(data,0)
+        if self.shift>1:
+            vetormax=np.where(vetormax < 0, vetormax*(1/self.shift), vetormax*self.shift)
+            vetormin=np.where(vetormin < 0, vetormin*self.shift, vetormin*(1/self.shift))
+
         vetormed = (vetormax+vetormin)/2
         media = np.mean(data,0)
         desvio = np.std(data,0)        
                                     
         if (self.norma==1) or (self.norma==4):  
             normalized = (data - vetormin) / (vetormax - vetormin)
             
@@ -441,23 +440,22 @@
         if (self.norma==6) or (self.norma==-1):
             normalized = (data - media)/desvio
 
         np.savetxt(maxiname, vetormax)
         np.savetxt(mininame, vetormin)
         np.savetxt(medianame, media)
         np.savetxt(desvioname, desvio)
+        
         return normalized
 
 
 
 
 
 
-
-
     #normalizing the data by entering maximums and minimums-----------------------------------------------
     def Normalize2(self, data, maxiname, mininame, medianame, desvioname):         
 
         vetormax = np.loadtxt(maxiname) 
         vetormin = np.loadtxt(mininame) 
         vetormed = (vetormax+vetormin)/2
         media = np.loadtxt(medianame)
```

### Comparing `tupa123-1.3.2/tupa123.egg-info/PKG-INFO` & `tupa123-1.3.3/tupa123.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.3.2
+Version: 1.3.3
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
-Keywords: artificial-intelligence neural-networks four-layers regression classification tupa123
+Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 Fully connected four-layer neural network <br>
 Solves a huge number of cases, classification and regression <br>
 The following sequence explains how to use with the help of two example files. <br>
 The first file contains the learning process, where the neural network finds its weights <br>
@@ -64,28 +64,29 @@
 #The data can come from any source, but the ExcelMatrix function allows a practical interaction with Excel <br>
 #ExcelMatrix = collect data from excel, the spreadsheet needs to be in the same folder as the python file <br>
 #'ALETAS.xlsm' = example name of the excel file / 'Sheet1' = example name of the tab where the data are <br>
 #Lineini=2, Columini=1 = example initial row and column of data <br>
 #linesquantity = number of lines of learning data <br>
 #X = regression input data / y = data to be predicted <br>
 <br>
-<b>model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='')</b> <br>
+<b>model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1)</b> <br>
 #creates the Neural Network model <br>
 <br>
 #norma = type of data normalization: (default=2)<br>
 #=-1, standardization <br>
 #=0, do anything <br>
 #=1, between 0 and 1 <br>
 #=2, between -1 and 1 <br>
 #=3, log(x+coef) <br>
 #=4, log(x+coef)  between 0 and 1 <br>
 #=5, log(x+coef)  between -1 and 1 <br>
 #=6, log(x+coef)  and standardization <br>
 #coef = used to avoid zero in log normalizations, example 0.0012345 (default=0)<br>
 #normout = if 1 normalizes the output (default=1), 0 dont <br>
+#shift = (default=1), >=1, stretches the normalization rule. Normalized data falls outside the bounds.
 <br>
 #nn1c=5, nn2c=7, nn3c=5, nn4c=2 = number of neurons from the first to the fourth layer (default=1,5,5,1) <br>
 #rate = learning rate (default=0.01) <br>
 #epochs = number of epochs (default=1000)<br>
 #fa2c=5, fa3c=5, fa4c=0 = second to fourth layer activation functions (default=5,5,0) <br>
 #for regression the fourth layer is recommended as linear = 0 <br>
 #cost=0, cost function, (default=0). 0 = MSE, mean squared error for regression and classification / 1 = BCE, binary cross entropy for classification <br>
```

