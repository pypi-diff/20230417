# Comparing `tmp/optimtool-2.4.1.tar.gz` & `tmp/optimtool-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimtool-2.4.1.tar", last modified: Thu Nov 10 06:11:43 2022, max compression
+gzip compressed data, was "optimtool-2.4.2.tar", last modified: Mon Apr 17 14:54:10 2023, max compression
```

## Comparing `optimtool-2.4.1.tar` & `optimtool-2.4.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2022-11-10 06:11:43.989116 optimtool-2.4.1/
--rw-rw-rw-   0        0        0     1089 2022-10-30 15:21:41.000000 optimtool-2.4.1/LICENSE
--rw-rw-rw-   0        0        0    17282 2022-11-10 06:11:43.986709 optimtool-2.4.1/PKG-INFO
--rw-rw-rw-   0        0        0    16026 2022-11-10 05:37:31.000000 optimtool-2.4.1/README.md
-drwxrwxrwx   0        0        0        0 2022-11-10 06:11:43.913680 optimtool-2.4.1/optimtool/
--rw-rw-rw-   0        0        0     1382 2022-11-08 14:22:53.000000 optimtool-2.4.1/optimtool/__init__.py
--rw-rw-rw-   0        0        0     3018 2022-11-10 05:38:19.000000 optimtool-2.4.1/optimtool/_convert.py
--rw-rw-rw-   0        0        0    10976 2022-11-10 05:40:04.000000 optimtool-2.4.1/optimtool/_drive.py
--rw-rw-rw-   0        0        0     1766 2022-11-08 07:32:12.000000 optimtool-2.4.1/optimtool/_kernel.py
--rw-rw-rw-   0        0        0     9127 2022-11-10 05:42:29.000000 optimtool-2.4.1/optimtool/_search.py
--rw-rw-rw-   0        0        0     1808 2022-11-10 06:00:33.000000 optimtool-2.4.1/optimtool/_typing.py
--rw-rw-rw-   0        0        0     2583 2022-11-10 05:43:01.000000 optimtool-2.4.1/optimtool/_utils.py
--rw-rw-rw-   0        0        0     1132 2022-11-08 13:40:41.000000 optimtool-2.4.1/optimtool/_version.py
-drwxrwxrwx   0        0        0        0 2022-11-10 06:11:43.939641 optimtool-2.4.1/optimtool/constrain/
--rw-rw-rw-   0        0        0     1177 2022-11-08 10:25:08.000000 optimtool-2.4.1/optimtool/constrain/__init__.py
--rw-rw-rw-   0        0        0     5464 2022-11-10 05:12:36.000000 optimtool-2.4.1/optimtool/constrain/equal.py
--rw-rw-rw-   0        0        0     9649 2022-11-10 05:12:49.000000 optimtool-2.4.1/optimtool/constrain/mixequal.py
--rw-rw-rw-   0        0        0     8420 2022-11-10 05:17:26.000000 optimtool-2.4.1/optimtool/constrain/unequal.py
-drwxrwxrwx   0        0        0        0 2022-11-10 06:11:43.948560 optimtool-2.4.1/optimtool/example/
--rw-rw-rw-   0        0        0     8313 2022-11-10 05:19:01.000000 optimtool-2.4.1/optimtool/example/Lasso.py
--rw-rw-rw-   0        0        0    10603 2022-11-10 05:19:48.000000 optimtool-2.4.1/optimtool/example/WanYuan.py
--rw-rw-rw-   0        0        0     1153 2022-11-08 10:19:28.000000 optimtool-2.4.1/optimtool/example/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-10 06:11:43.960841 optimtool-2.4.1/optimtool/hybrid/
--rw-rw-rw-   0        0        0     1151 2022-11-08 10:20:03.000000 optimtool-2.4.1/optimtool/hybrid/__init__.py
--rw-rw-rw-   0        0        0     1104 2022-11-07 14:27:41.000000 optimtool-2.4.1/optimtool/hybrid/approximate_point_gradient.py
-drwxrwxrwx   0        0        0        0 2022-11-10 06:11:43.983552 optimtool-2.4.1/optimtool/unconstrain/
--rw-rw-rw-   0        0        0     1257 2022-11-08 10:26:00.000000 optimtool-2.4.1/optimtool/unconstrain/__init__.py
--rw-rw-rw-   0        0        0     6412 2022-11-10 05:23:41.000000 optimtool-2.4.1/optimtool/unconstrain/gradient_descent.py
--rw-rw-rw-   0        0        0     6247 2022-11-10 05:26:35.000000 optimtool-2.4.1/optimtool/unconstrain/newton.py
--rw-rw-rw-   0        0        0     7800 2022-11-10 05:24:50.000000 optimtool-2.4.1/optimtool/unconstrain/newton_quasi.py
--rw-rw-rw-   0        0        0     5951 2022-11-10 05:27:25.000000 optimtool-2.4.1/optimtool/unconstrain/nonlinear_least_square.py
--rw-rw-rw-   0        0        0     4005 2022-11-10 05:28:00.000000 optimtool-2.4.1/optimtool/unconstrain/trust_region.py
-drwxrwxrwx   0        0        0        0 2022-11-10 06:11:43.929611 optimtool-2.4.1/optimtool.egg-info/
--rw-rw-rw-   0        0        0    17282 2022-11-10 06:11:43.000000 optimtool-2.4.1/optimtool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      909 2022-11-10 06:11:43.000000 optimtool-2.4.1/optimtool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-10 06:11:43.000000 optimtool-2.4.1/optimtool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-11-10 06:11:43.000000 optimtool-2.4.1/optimtool.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       43 2022-11-10 06:11:43.000000 optimtool-2.4.1/optimtool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-11-10 06:11:43.000000 optimtool-2.4.1/optimtool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-10 06:11:43.990489 optimtool-2.4.1/setup.cfg
--rw-rw-rw-   0        0        0     2964 2022-11-10 06:11:07.000000 optimtool-2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:54:10.919752 optimtool-2.4.2/
+-rw-rw-rw-   0        0        0     1089 2023-04-17 13:50:21.000000 optimtool-2.4.2/LICENSE
+-rw-rw-rw-   0        0        0    17700 2023-04-17 14:54:10.903757 optimtool-2.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0    16392 2023-04-17 14:53:03.000000 optimtool-2.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 14:54:10.723751 optimtool-2.4.2/optimtool/
+-rw-rw-rw-   0        0        0     1404 2023-04-17 13:59:09.000000 optimtool-2.4.2/optimtool/__init__.py
+-rw-rw-rw-   0        0        0     2802 2023-04-17 14:01:20.000000 optimtool-2.4.2/optimtool/_convert.py
+-rw-rw-rw-   0        0        0    10976 2023-04-17 13:50:21.000000 optimtool-2.4.2/optimtool/_drive.py
+-rw-rw-rw-   0        0        0     1804 2023-04-17 14:14:24.000000 optimtool-2.4.2/optimtool/_kernel.py
+-rw-rw-rw-   0        0        0     8878 2023-04-17 14:42:57.000000 optimtool-2.4.2/optimtool/_search.py
+-rw-rw-rw-   0        0        0     1832 2023-04-17 13:55:26.000000 optimtool-2.4.2/optimtool/_typing.py
+-rw-rw-rw-   0        0        0     2535 2023-04-17 13:54:24.000000 optimtool-2.4.2/optimtool/_utils.py
+-rw-rw-rw-   0        0        0     1132 2023-04-17 13:52:58.000000 optimtool-2.4.2/optimtool/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:54:10.820754 optimtool-2.4.2/optimtool/constrain/
+-rw-rw-rw-   0        0        0     1177 2023-04-17 13:50:21.000000 optimtool-2.4.2/optimtool/constrain/__init__.py
+-rw-rw-rw-   0        0        0     5357 2023-04-17 14:14:47.000000 optimtool-2.4.2/optimtool/constrain/equal.py
+-rw-rw-rw-   0        0        0     9429 2023-04-17 14:15:14.000000 optimtool-2.4.2/optimtool/constrain/mixequal.py
+-rw-rw-rw-   0        0        0     8216 2023-04-17 14:18:23.000000 optimtool-2.4.2/optimtool/constrain/unequal.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:54:10.831758 optimtool-2.4.2/optimtool/example/
+-rw-rw-rw-   0        0        0     8263 2023-04-17 14:18:57.000000 optimtool-2.4.2/optimtool/example/Lasso.py
+-rw-rw-rw-   0        0        0    10603 2023-04-17 13:50:21.000000 optimtool-2.4.2/optimtool/example/WanYuan.py
+-rw-rw-rw-   0        0        0     1153 2023-04-17 13:50:21.000000 optimtool-2.4.2/optimtool/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:54:10.853753 optimtool-2.4.2/optimtool/hybrid/
+-rw-rw-rw-   0        0        0     1185 2023-04-17 14:12:40.000000 optimtool-2.4.2/optimtool/hybrid/__init__.py
+-rw-rw-rw-   0        0        0     1104 2023-04-17 13:50:21.000000 optimtool-2.4.2/optimtool/hybrid/approximate_point_gradient.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:54:10.887751 optimtool-2.4.2/optimtool/unconstrain/
+-rw-rw-rw-   0        0        0     1257 2023-04-17 13:50:21.000000 optimtool-2.4.2/optimtool/unconstrain/__init__.py
+-rw-rw-rw-   0        0        0     6456 2023-04-17 14:09:25.000000 optimtool-2.4.2/optimtool/unconstrain/gradient_descent.py
+-rw-rw-rw-   0        0        0     6034 2023-04-17 14:11:11.000000 optimtool-2.4.2/optimtool/unconstrain/newton.py
+-rw-rw-rw-   0        0        0     7656 2023-04-17 14:10:40.000000 optimtool-2.4.2/optimtool/unconstrain/newton_quasi.py
+-rw-rw-rw-   0        0        0     5858 2023-04-17 14:28:17.000000 optimtool-2.4.2/optimtool/unconstrain/nonlinear_least_square.py
+-rw-rw-rw-   0        0        0     3821 2023-04-17 14:12:08.000000 optimtool-2.4.2/optimtool/unconstrain/trust_region.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:54:10.806333 optimtool-2.4.2/optimtool.egg-info/
+-rw-rw-rw-   0        0        0    17700 2023-04-17 14:54:10.000000 optimtool-2.4.2/optimtool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      909 2023-04-17 14:54:10.000000 optimtool-2.4.2/optimtool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 14:54:10.000000 optimtool-2.4.2/optimtool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 14:54:10.000000 optimtool-2.4.2/optimtool.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       43 2023-04-17 14:54:10.000000 optimtool-2.4.2/optimtool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-17 14:54:10.000000 optimtool-2.4.2/optimtool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 14:54:10.920752 optimtool-2.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     3048 2023-04-17 14:53:49.000000 optimtool-2.4.2/setup.py
```

### Comparing `optimtool-2.4.1/LICENSE` & `optimtool-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.1/PKG-INFO` & `optimtool-2.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimtool
-Version: 2.4.1
+Version: 2.4.2
 Summary: The fundamental package for scientific research in optimization.
 Home-page: https://github.com/linjing-lab/optimtool
 Download-URL: https://github.com/linjing-lab/optimtool/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: MIT
 Project-URL: Source, https://github.com/linjing-lab/optimtool/tree/master/optimtool/
@@ -13,14 +13,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
@@ -38,29 +39,45 @@
     </a>
     <a href='https://pepy.tech/project/optimtool'>
         <img src="https://pepy.tech/badge/optimtool" alt="Total Downloads" height="20"/>
     </a>
     <a href='https://pepy.tech/project/optimtool'>
         <img src="https://pepy.tech/badge/optimtool/month" alt="Monthly Downloads" height="20"/> 
     </a>
-    <a href='https://code.visualstudio.com/'>
+    <a href='https://pepy.tech/project/optimtool'>
         <img src="https://pepy.tech/badge/optimtool/week" alt="Weekly Downloads" height="20"/> 
     </a>
 </p>
 
 If you want to participate in the development, please follow the [baseline](./baseline.md).
 
 如果你想参与开发，请遵循[baseline](./baseline.md)。
 
 简体中文 | [English](./README_en.md)
 
 ## 项目介绍
 
 &emsp;&emsp;optimtool采用了北京大学出版的《最优化：建模、算法与理论》这本书中的部分理论方法框架，运用了 [`Numpy`](https://github.com/numpy/numpy) 包高效处理数组间运算等的特性，巧妙地应用了 [`Sympy`](https://github.com/sympy/sympy) 内部支持的 .jacobian 等方法，并结合 Python 内置函数 dict 与 zip 实现了 Sympy 矩阵到 Numpy 矩阵的转换，最终设计了一个用于最优化科学研究领域的Python工具包。 研究人员可以通过简单的 [`pip`](https://github.com/pypa/pip) 指令进行下载与使用。
 
+如果你在研究中使用 **optimtool**，欢迎引用它在你的参考资料中（按照下面的格式）。
+
+```text
+林景. optimtool: The fundamental package for scientific research in optimization. 2021. https://pypi.org/project/optimtool/.
+```
+
+下载最新版：
+```text
+git clone https://github.com/linjing-lab/optimtool.git
+cd optimtool
+pip install -e . --verbose
+```
+下载稳定版：
+```text
+pip install optimtool --upgrade
+```
 ## 项目结构
 
 ```textile
 |- optimtool
     |-- constrain
         |-- __init__.py
         |-- equal.py
@@ -87,15 +104,15 @@
     |-- _search.py
     |-- _typing.py
     |-- _utils.py
     |-- _version.py
 ```
 &emsp;&emsp;因为在求解不同的目标函数的全局或局部收敛点时，不同的求取收敛点的方法会有不同的收敛效率以及不同的适用范围，而且在研究过程中不同领域的研究方法被不断地提出、修改、完善、扩充，所以这些方法成了现在人们口中的`最优化方法`。 此项目中的所有内部支持的算法，都是在范数、导数、凸集、凸函数、共轭函数、次梯度和最优化理论等基础方法论的基础上进行设计与完善的。
 
-&emsp;&emsp;optimtool内置了诸如Barzilar Borwein非单调梯度下降法、修正牛顿法、有限内存BFGS方法、截断共轭梯度法-信赖域方法、高斯-牛顿法等无约束优化领域收敛效率与性质较好的算法，以及用于解决约束优化问题的二次罚函数法、增广拉格朗日法等算法。
+&emsp;&emsp;optimtool内置了诸如Barzilar Borwein非单调梯度下降法、修正牛顿法、有限内存BFGS方法、截断共轭梯度法-信赖域方法、高斯-牛顿法等无约束优化领域收敛效率与性质好的算法，以及用于解决约束优化问题的二次罚函数法、增广拉格朗日法等算法。
 
 ## 开始使用
 
 ### 无约束优化算法（unconstrain）
 
 ```python
 import optimtool.unconstrain as ou
@@ -110,58 +127,58 @@
 
 | 方法头                                                                                                                                 | 解释                                   |
 | ----------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
 | solve(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10, k: int=0) -> OutputType                                                             | 通过解方程的方式来求解精确步长                      |
 | steepest(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType                                           | 使用线搜索方法求解非精确步长（默认使用wolfe线搜索）         |
 | barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta: float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType | 使用Grippo与ZhangHanger提出的非单调线搜索方法更新步长 |
 
-#### 牛顿法（newton)
+#### 牛顿法（newton）
 
 ```python
 ou.newton.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
 | 方法头                                                                                             | 解释                                |
 | ----------------------------------------------------------------------------------------------- | --------------------------------- |
 | classic(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10, k: int=0) -> OutputType                        | 通过直接对目标函数二阶导矩阵（海瑟矩阵）进行求逆来获取下一步的步长 |
-| modified(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: int=20, epsilon: float=1e-10, k: int=0) -> OutputType | 修正当前海瑟矩阵保证其正定性（目前只接入了一种修正方法）      |
+| modified(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType | 修正当前海瑟矩阵保证其正定性（目前只接入了一种修正方法）      |
 | CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-6, k: int=0) -> OutputType              | 采用牛顿-共轭梯度法求解梯度（非精确牛顿法的一种）         |
 
 #### 拟牛顿法（newton_quasi）
 
 ```python
 ou.newton_quasi.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
 | 方法头                                                                                          | 解释              |
 | -------------------------------------------------------------------------------------------- | --------------- |
-| bfgs(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: float=20, epsilon: float=1e-10, k: int=0) -> OutputType  | BFGS方法更新海瑟矩阵    |
-| dfp(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: float=20, epsilon: float=1e-4, k: int=0) -> OutputType    | DFP方法更新海瑟矩阵     |
+| bfgs(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType  | BFGS方法更新海瑟矩阵    |
+| dfp(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-4, k: int=0) -> OutputType    | DFP方法更新海瑟矩阵     |
 | L_BFGS(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: float=6, epsilon: float=1e-10, k: int=0) -> OutputType | 双循环方法更新BFGS海瑟矩阵 |
 
 #### 非线性最小二乘法（nonlinear_least_square）
 
 ```python
 ou.nonlinear_least_square.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                  | 解释                         |
 | ---------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------- |
 | gauss_newton(funcr: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType                                                        | 高斯-牛顿提出的方法框架，包括OR分解等操作     |
-| levenberg_marquardt(funcr: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, m: float=100, lamk: float=1, eta: float=0.2, p1: float=0.4, p2: float=0.9, gamma1: float=0.7, gamma2: float=1.3, epsilon: float=1e-10, k: int=0) -> OutputType | Levenberg Marquardt提出的方法框架 |
+| levenberg_marquardt(funcr: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, lamk: float=1, eta: float=0.2, p1: float=0.4, p2: float=0.9, gamma1: float=0.7, gamma2: float=1.3, epsilon: float=1e-10, k: int=0) -> OutputType | Levenberg Marquardt提出的方法框架 |
 
 #### 信赖域方法（trust_region）
 
 ```python
 ou.trust_region.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                               | 解释                  |
 | ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------- |
-| steihaug_CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, m: float=100, r0: float=1, rmax: float=2, eta: float=0.2, p1: float=0.4, p2: float=0.6, gamma1: float=0.5, gamma2: float=1.5, epsilon: float=1e-6, k: int=0) -> OutputType | 截断共轭梯度法在此方法中被用于搜索步长 |
+| steihaug_CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, r0: float=1, rmax: float=2, eta: float=0.2, p1: float=0.4, p2: float=0.6, gamma1: float=0.5, gamma2: float=1.5, epsilon: float=1e-6, k: int=0) -> OutputType | 截断共轭梯度法在此方法中被用于搜索步长 |
 
 ### 约束优化算法（constrain）
 
 ```python
 import optimtool.constrain as oc
 oc.[方法名].[函数名]([目标函数], [参数表], [等式约束表], [不等式约数表], [初始迭代点])
 ```
@@ -170,40 +187,40 @@
 
 ```python
 oc.equal.[函数名]([目标函数], [参数表], [等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                   | 解释        |
 | ----------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
-| penalty_quadratice(funcs: FuncArray, args: FuncArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=10, p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType                     | 增加二次罚项    |
-| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadratice(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType                     | 增加二次罚项    |
+| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 #### 不等式约束（unequal）
 
 ```python
 oc.unequal.[函数名]([目标函数], [参数表], [不等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                                      | 解释        |
 | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------- |
-| penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=10, p: float=0.4, epsilon: float=1e-10, k: int=0) -> OutputType                                     | 增加二次罚项    |
-| penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k: int=0) -> OutputType                              | 增加分式函数罚项  |
-| lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.4, epsilon: float=1e-10, k: int=0) -> OutputType                                     | 增加二次罚项    |
+| penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k: int=0) -> OutputType                              | 增加分式函数罚项  |
+| lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 #### 混合等式约束（mixequal）
 
 ```python
 oc.mixequal.[函数名]([目标函数], [参数表], [等式约束表], [不等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                                                                  | 解释        |
 | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
-| penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=10, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                             | 增加二次罚项    |
-| penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=1, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                                     | L1精确罚函数法  |
-| lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                             | 增加二次罚项    |
+| penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=1, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                                     | L1精确罚函数法  |
+| lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 ### 方法的应用（example）
 
 ```python
 import optimtool.example as oe
 ```
```

#### html2text {}

```diff
@@ -1,52 +1,58 @@
-Metadata-Version: 2.1 Name: optimtool Version: 2.4.1 Summary: The fundamental
+Metadata-Version: 2.1 Name: optimtool Version: 2.4.2 Summary: The fundamental
 package for scientific research in optimization. Home-page: https://github.com/
 linjing-lab/optimtool Download-URL: https://github.com/linjing-lab/optimtool/
 tags Author: ææ¯ Author-email: linjing010729@163.com License: MIT Project-
 URL: Source, https://github.com/linjing-lab/optimtool/tree/master/optimtool/
 Project-URL: Tracker, https://github.com/linjing-lab/optimtool/issues
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License Classifier: Topic ::
-Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
-Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Description-Content-Type: text/markdown License-
-File: LICENSE
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: MIT License Classifier: Topic :: Scientific/Engineering Classifier:
+Topic :: Scientific/Engineering :: Mathematics Classifier: Topic :: Software
+Development Classifier: Topic :: Software Development :: Libraries Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Description-
+Content-Type: text/markdown License-File: LICENSE
                             ****** optimtool ******
       The fundamental package for scientific research in optimization.[?]
     [OSCS_Status] [Total_Downloads] [Monthly_Downloads] [Weekly_Downloads]
 If you want to participate in the development, please follow the [baseline](./
 baseline.md). å¦æä½ æ³åä¸å¼åï¼è¯·éµå¾ª[baseline](./baseline.md)ã
 ç®ä½ä¸­æ | [English](./README_en.md) ## é¡¹ç®ä»ç»
 &emsp;&emsp;optimtooléç¨äºåäº¬å¤§å­¦åºççãæä¼åï¼å»ºæ¨¡ãç®æ³ä¸çè®ºãè¿æ¬ä¹¦ä¸­çé¨åçè®ºæ¹æ³æ¡æ¶ï¼è¿ç¨äº
 [`Numpy`](https://github.com/numpy/numpy)
 åé«æå¤çæ°ç»é´è¿ç®ç­çç¹æ§ï¼å·§å¦å°åºç¨äº [`Sympy`]
 (https://github.com/sympy/sympy) åé¨æ¯æç .jacobian
 ç­æ¹æ³ï¼å¹¶ç»å Python åç½®å½æ° dict ä¸ zip å®ç°äº Sympy
 ç©éµå° Numpy
 ç©éµçè½¬æ¢ï¼æç»è®¾è®¡äºä¸ä¸ªç¨äºæä¼åç§å­¦ç ç©¶é¢åçPythonå·¥å·åã
 ç ç©¶äººåå¯ä»¥éè¿ç®åç [`pip`](https://github.com/pypa/pip)
-æä»¤è¿è¡ä¸è½½ä¸ä½¿ç¨ã ## é¡¹ç®ç»æ ```textile |- optimtool |-
-- constrain |-- __init__.py |-- equal.py |-- mixequal.py |-- unequal.py |-
-- example |-- __init__.py |-- Lasso.py |-- WanYuan.py |-- hybrid |-
-- __init__.py |-- approximate_point_gradient.py |-- unconstrain |-- __init__.py
-|-- gradient_descent.py |-- newton.py |-- newton_quasi.py |-
+æä»¤è¿è¡ä¸è½½ä¸ä½¿ç¨ã å¦æä½ å¨ç ç©¶ä¸­ä½¿ç¨
+**optimtool**ï¼æ¬¢è¿å¼ç¨å®å¨ä½ çåèèµæä¸­ï¼æç§ä¸é¢çæ ¼å¼ï¼ã
+```text ææ¯. optimtool: The fundamental package for scientific research in
+optimization. 2021. https://pypi.org/project/optimtool/. ``` ä¸è½½ææ°çï¼
+```text git clone https://github.com/linjing-lab/optimtool.git cd optimtool pip
+install -e . --verbose ``` ä¸è½½ç¨³å®çï¼ ```text pip install optimtool --
+upgrade ``` ## é¡¹ç®ç»æ ```textile |- optimtool |-- constrain |-
+- __init__.py |-- equal.py |-- mixequal.py |-- unequal.py |-- example |-
+- __init__.py |-- Lasso.py |-- WanYuan.py |-- hybrid |-- __init__.py |-
+- approximate_point_gradient.py |-- unconstrain |-- __init__.py |-
+- gradient_descent.py |-- newton.py |-- newton_quasi.py |-
 - nonlinear_least_square.py |-- trust_region.py |-- __init__.py |-- _convert.py
 |-- _drive.py |-- _kernel.py |-- _search.py |-- _typing.py |-- _utils.py |-
 - _version.py ```
 &emsp;&emsp;å ä¸ºå¨æ±è§£ä¸åçç®æ å½æ°çå¨å±æå±é¨æ¶æç¹æ¶ï¼ä¸åçæ±åæ¶æç¹çæ¹æ³ä¼æä¸åçæ¶ææçä»¥åä¸åçéç¨èå´ï¼èä¸å¨ç ç©¶è¿ç¨ä¸­ä¸åé¢åçç ç©¶æ¹æ³è¢«ä¸æ­å°æåºãä¿®æ¹ãå®åãæ©åï¼æä»¥è¿äºæ¹æ³æäºç°å¨äººä»¬å£ä¸­ç`æä¼åæ¹æ³`ã
 æ­¤é¡¹ç®ä¸­çææåé¨æ¯æçç®æ³ï¼é½æ¯å¨èæ°ãå¯¼æ°ãå¸éãå¸å½æ°ãå±è½­å½æ°ãæ¬¡æ¢¯åº¦åæä¼åçè®ºç­åºç¡æ¹æ³è®ºçåºç¡ä¸è¿è¡è®¾è®¡ä¸å®åçã
 &emsp;&emsp;optimtoolåç½®äºè¯¸å¦Barzilar
 Borweinéåè°æ¢¯åº¦ä¸éæ³ãä¿®æ­£çé¡¿æ³ãæéåå­BFGSæ¹æ³ãæªæ­å±è½­æ¢¯åº¦æ³-
 ä¿¡èµåæ¹æ³ãé«æ¯-
-çé¡¿æ³ç­æ çº¦æä¼åé¢åæ¶ææçä¸æ§è´¨è¾å¥½çç®æ³ï¼ä»¥åç¨äºè§£å³çº¦æä¼åé®é¢çäºæ¬¡ç½å½æ°æ³ãå¢å¹¿ææ ¼ææ¥æ³ç­ç®æ³ã
+çé¡¿æ³ç­æ çº¦æä¼åé¢åæ¶ææçä¸æ§è´¨å¥½çç®æ³ï¼ä»¥åç¨äºè§£å³çº¦æä¼åé®é¢çäºæ¬¡ç½å½æ°æ³ãå¢å¹¿ææ ¼ææ¥æ³ç­ç®æ³ã
 ## å¼å§ä½¿ç¨ ### æ çº¦æä¼åç®æ³ï¼unconstrainï¼ ```python import
 optimtool.unconstrain as ou ou.[æ¹æ³å].[å½æ°å]([ç®æ å½æ°],
 [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` #### æ¢¯åº¦ä¸éæ³ï¼gradient_descentï¼
 ```python ou.gradient_descent.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 --------------------- | ------------------------------------ | | solve(funcs:
@@ -56,112 +62,110 @@
 args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method:
 str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType |
 ä½¿ç¨çº¿æç´¢æ¹æ³æ±è§£éç²¾ç¡®æ­¥é¿ï¼é»è®¤ä½¿ç¨wolfeçº¿æç´¢ï¼ | |
 barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw:
 bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta:
 float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType |
 ä½¿ç¨Grippoä¸ZhangHangeræåºçéåè°çº¿æç´¢æ¹æ³æ´æ°æ­¥é¿ | ####
-çé¡¿æ³ï¼newton) ```python ou.newton.[å½æ°å]([ç®æ å½æ°],
+çé¡¿æ³ï¼newtonï¼ ```python ou.newton.[å½æ°å]([ç®æ å½æ°],
 [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | ------------------
 ----------------------------------------------------------------------------- |
 --------------------------------- | | classic(funcs: FuncArray, args: ArgArray,
 x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10,
 k: int=0) -> OutputType |
 éè¿ç´æ¥å¯¹ç®æ å½æ°äºé¶å¯¼ç©éµï¼æµ·çç©éµï¼è¿è¡æ±éæ¥è·åä¸ä¸æ­¥çæ­¥é¿
 | | modified(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw:
-bool=True, output_f: bool=False, method: str="wolfe", m: int=20, epsilon:
-float=1e-10, k: int=0) -> OutputType |
+bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k:
+int=0) -> OutputType |
 ä¿®æ­£å½åæµ·çç©éµä¿è¯å¶æ­£å®æ§ï¼ç®ååªæ¥å¥äºä¸ç§ä¿®æ­£æ¹æ³ï¼
 | | CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True,
 output_f: bool=False, method: str="wolfe", epsilon: float=1e-6, k: int=0) -
 > OutputType | éç¨çé¡¿-
 å±è½­æ¢¯åº¦æ³æ±è§£æ¢¯åº¦ï¼éç²¾ç¡®çé¡¿æ³çä¸ç§ï¼ | ####
 æçé¡¿æ³ï¼newton_quasiï¼ ```python ou.newton_quasi.[å½æ°å](
 [ç®æ å½æ°], [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | --
 -------------------------------------------------------------------------------
 ----------- | --------------- | | bfgs(funcs: FuncArray, args: ArgArray, x_0:
-PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m:
-float=20, epsilon: float=1e-10, k: int=0) -> OutputType |
-BFGSæ¹æ³æ´æ°æµ·çç©éµ | | dfp(funcs: FuncArray, args: ArgArray, x_0:
-PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m:
-float=20, epsilon: float=1e-4, k: int=0) -> OutputType |
-DFPæ¹æ³æ´æ°æµ·çç©éµ | | L_BFGS(funcs: FuncArray, args: ArgArray, x_0:
-PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m:
-float=6, epsilon: float=1e-10, k: int=0) -> OutputType |
+PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe",
+epsilon: float=1e-10, k: int=0) -> OutputType | BFGSæ¹æ³æ´æ°æµ·çç©éµ |
+| dfp(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True,
+output_f: bool=False, method: str="wolfe", epsilon: float=1e-4, k: int=0) -
+> OutputType | DFPæ¹æ³æ´æ°æµ·çç©éµ | | L_BFGS(funcs: FuncArray, args:
+ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method:
+str="wolfe", m: float=6, epsilon: float=1e-10, k: int=0) -> OutputType |
 åå¾ªç¯æ¹æ³æ´æ°BFGSæµ·çç©éµ | ####
 éçº¿æ§æå°äºä¹æ³ï¼nonlinear_least_squareï¼ ```python
 ou.nonlinear_least_square.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------- | -------------------------- | |
 gauss_newton(funcr: FuncArray, args: ArgArray, x_0: PointArray, draw:
 bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k:
 int=0) -> OutputType | é«æ¯-
 çé¡¿æåºçæ¹æ³æ¡æ¶ï¼åæ¬ORåè§£ç­æä½ | | levenberg_marquardt
 (funcr: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, m: float=100, lamk: float=1, eta: float=0.2, p1: float=0.4, p2:
-float=0.9, gamma1: float=0.7, gamma2: float=1.3, epsilon: float=1e-10, k:
-int=0) -> OutputType | Levenberg Marquardtæåºçæ¹æ³æ¡æ¶ | ####
+bool=False, lamk: float=1, eta: float=0.2, p1: float=0.4, p2: float=0.9,
+gamma1: float=0.7, gamma2: float=1.3, epsilon: float=1e-10, k: int=0) -
+> OutputType | Levenberg Marquardtæåºçæ¹æ³æ¡æ¶ | ####
 ä¿¡èµåæ¹æ³ï¼trust_regionï¼ ```python ou.trust_region.[å½æ°å](
 [ç®æ å½æ°], [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | --
 -------------------------------------------------------------------------------
 ---------------------------------------------------------------- | ------------
 ------- | | steihaug_CG(funcs: FuncArray, args: ArgArray, x_0: PointArray,
-draw: bool=True, output_f: bool=False, m: float=100, r0: float=1, rmax:
-float=2, eta: float=0.2, p1: float=0.4, p2: float=0.6, gamma1: float=0.5,
-gamma2: float=1.5, epsilon: float=1e-6, k: int=0) -> OutputType |
+draw: bool=True, output_f: bool=False, r0: float=1, rmax: float=2, eta:
+float=0.2, p1: float=0.4, p2: float=0.6, gamma1: float=0.5, gamma2: float=1.5,
+epsilon: float=1e-6, k: int=0) -> OutputType |
 æªæ­å±è½­æ¢¯åº¦æ³å¨æ­¤æ¹æ³ä¸­è¢«ç¨äºæç´¢æ­¥é¿ | ###
 çº¦æä¼åç®æ³ï¼constrainï¼ ```python import optimtool.constrain as oc
 oc.[æ¹æ³å].[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨],
 [ä¸ç­å¼çº¦æ°è¡¨], [åå§è¿­ä»£ç¹]) ``` #### ç­å¼çº¦æï¼equalï¼
 ```python oc.equal.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------- | --------- | | penalty_quadratice
-(funcs: FuncArray, args: FuncArray, cons: FuncArray, x_0: PointArray, draw:
-bool=True, output_f: bool=False, method: str="gradient_descent", sigma:
-float=10, p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType |
-å¢å äºæ¬¡ç½é¡¹ | | lagrange_augmentede(funcs: FuncArray, args: ArgArray,
-cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False,
-method: str="gradient_descent", lamk: float=6, sigma: float=10, p: float=2,
-etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType |
-å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | #### ä¸ç­å¼çº¦æï¼unequalï¼ ```python
-oc.unequal.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ä¸ç­å¼çº¦æè¡¨],
-[åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
+(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw:
+bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10,
+p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType | å¢å äºæ¬¡ç½é¡¹ |
+| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0:
+PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region",
+lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon:
+float=1e-6, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | ####
+ä¸ç­å¼çº¦æï¼unequalï¼ ```python oc.unequal.[å½æ°å]([ç®æ å½æ°],
+[åæ°è¡¨], [ä¸ç­å¼çº¦æè¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é
+| | ---------------------------------------------------------------------------
 -------------------------------------------------------------------------------
----------------------------------------------------------- | --------- | |
-penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0:
-PointArray, draw: bool=True, output_f: bool=False, method:
-str="gradient_descent", sigma: float=10, p: float=0.4, epsilon: float=1e-10, k:
-int=0) -> OutputType | å¢å äºæ¬¡ç½é¡¹ | | penalty_interior_fraction(funcs:
-FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True,
-output_f: bool=False, method: str="gradient_descent", sigma: float=12, p:
-float=0.6, epsilon: float=1e-6, k: int=0) -> OutputType |
-å¢å åå¼å½æ°ç½é¡¹ | | lagrange_augmentedu(funcs: FuncArray, args:
+-------------- | --------- | | penalty_quadraticu(funcs: FuncArray, args:
 ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="gradient_descent", muk: float=10, sigma: float=8,
-alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon:
-float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | ####
-æ··åç­å¼çº¦æï¼mixequalï¼ ```python oc.mixequal.[å½æ°å](
+bool=False, method: str="trust_region", sigma: float=10, p: float=0.4, epsilon:
+float=1e-10, k: int=0) -> OutputType | å¢å äºæ¬¡ç½é¡¹ | |
+penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray,
+x_0: PointArray, draw: bool=True, output_f: bool=False, method:
+str="trust_region", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k:
+int=0) -> OutputType | å¢å åå¼å½æ°ç½é¡¹ | | lagrange_augmentedu(funcs:
+FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True,
+output_f: bool=False, method: str="trust_region", muk: float=10, sigma:
+float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1,
+epsilon: float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ |
+#### æ··åç­å¼çº¦æï¼mixequalï¼ ```python oc.mixequal.[å½æ°å](
 [ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨], [ä¸ç­å¼çº¦æè¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 ------- | --------- | | penalty_quadraticm(funcs: FuncArray, args: ArgArray,
 cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw:
-bool=True, output_f: bool=False, method: str="gradient_descent", sigma:
-float=10, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType |
+bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10,
+p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType |
 å¢å äºæ¬¡ç½é¡¹ | | penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal:
 FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="gradient_descent", sigma: float=1, p: float=0.6,
-epsilon: float=1e-10, k: int=0) -> OutputType | L1ç²¾ç¡®ç½å½æ°æ³ | |
+bool=False, method: str="trust_region", sigma: float=1, p: float=0.6, epsilon:
+float=1e-10, k: int=0) -> OutputType | L1ç²¾ç¡®ç½å½æ°æ³ | |
 lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray,
 cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="gradient_descent", lamk: float=6, muk: float=10,
-sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3,
+bool=False, method: str="trust_region", lamk: float=6, muk: float=10, sigma:
+float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3,
 epsilon: float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ |
 ### æ¹æ³çåºç¨ï¼exampleï¼ ```python import optimtool.example as oe ```
 #### Lassoé®é¢ï¼Lassoï¼ ```python oe.Lasso.[å½æ°å]([ç©éµA],
 [ç©éµb], [å å­mu], [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é
 | | ---------------------------------------------------------------------------
 ---------------------------- | ---------------- | | gradient(A: NDArray, b:
 NDArray, mu: float, args: ArgArray, x_0: PointArray, draw: bool=True, output_f:
```

### Comparing `optimtool-2.4.1/README.md` & `optimtool-2.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,29 +10,45 @@
     </a>
     <a href='https://pepy.tech/project/optimtool'>
         <img src="https://pepy.tech/badge/optimtool" alt="Total Downloads" height="20"/>
     </a>
     <a href='https://pepy.tech/project/optimtool'>
         <img src="https://pepy.tech/badge/optimtool/month" alt="Monthly Downloads" height="20"/> 
     </a>
-    <a href='https://code.visualstudio.com/'>
+    <a href='https://pepy.tech/project/optimtool'>
         <img src="https://pepy.tech/badge/optimtool/week" alt="Weekly Downloads" height="20"/> 
     </a>
 </p>
 
 If you want to participate in the development, please follow the [baseline](./baseline.md).
 
 如果你想参与开发，请遵循[baseline](./baseline.md)。
 
 简体中文 | [English](./README_en.md)
 
 ## 项目介绍
 
 &emsp;&emsp;optimtool采用了北京大学出版的《最优化：建模、算法与理论》这本书中的部分理论方法框架，运用了 [`Numpy`](https://github.com/numpy/numpy) 包高效处理数组间运算等的特性，巧妙地应用了 [`Sympy`](https://github.com/sympy/sympy) 内部支持的 .jacobian 等方法，并结合 Python 内置函数 dict 与 zip 实现了 Sympy 矩阵到 Numpy 矩阵的转换，最终设计了一个用于最优化科学研究领域的Python工具包。 研究人员可以通过简单的 [`pip`](https://github.com/pypa/pip) 指令进行下载与使用。
 
+如果你在研究中使用 **optimtool**，欢迎引用它在你的参考资料中（按照下面的格式）。
+
+```text
+林景. optimtool: The fundamental package for scientific research in optimization. 2021. https://pypi.org/project/optimtool/.
+```
+
+下载最新版：
+```text
+git clone https://github.com/linjing-lab/optimtool.git
+cd optimtool
+pip install -e . --verbose
+```
+下载稳定版：
+```text
+pip install optimtool --upgrade
+```
 ## 项目结构
 
 ```textile
 |- optimtool
     |-- constrain
         |-- __init__.py
         |-- equal.py
@@ -59,15 +75,15 @@
     |-- _search.py
     |-- _typing.py
     |-- _utils.py
     |-- _version.py
 ```
 &emsp;&emsp;因为在求解不同的目标函数的全局或局部收敛点时，不同的求取收敛点的方法会有不同的收敛效率以及不同的适用范围，而且在研究过程中不同领域的研究方法被不断地提出、修改、完善、扩充，所以这些方法成了现在人们口中的`最优化方法`。 此项目中的所有内部支持的算法，都是在范数、导数、凸集、凸函数、共轭函数、次梯度和最优化理论等基础方法论的基础上进行设计与完善的。
 
-&emsp;&emsp;optimtool内置了诸如Barzilar Borwein非单调梯度下降法、修正牛顿法、有限内存BFGS方法、截断共轭梯度法-信赖域方法、高斯-牛顿法等无约束优化领域收敛效率与性质较好的算法，以及用于解决约束优化问题的二次罚函数法、增广拉格朗日法等算法。
+&emsp;&emsp;optimtool内置了诸如Barzilar Borwein非单调梯度下降法、修正牛顿法、有限内存BFGS方法、截断共轭梯度法-信赖域方法、高斯-牛顿法等无约束优化领域收敛效率与性质好的算法，以及用于解决约束优化问题的二次罚函数法、增广拉格朗日法等算法。
 
 ## 开始使用
 
 ### 无约束优化算法（unconstrain）
 
 ```python
 import optimtool.unconstrain as ou
@@ -82,58 +98,58 @@
 
 | 方法头                                                                                                                                 | 解释                                   |
 | ----------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
 | solve(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10, k: int=0) -> OutputType                                                             | 通过解方程的方式来求解精确步长                      |
 | steepest(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType                                           | 使用线搜索方法求解非精确步长（默认使用wolfe线搜索）         |
 | barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta: float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType | 使用Grippo与ZhangHanger提出的非单调线搜索方法更新步长 |
 
-#### 牛顿法（newton)
+#### 牛顿法（newton）
 
 ```python
 ou.newton.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
 | 方法头                                                                                             | 解释                                |
 | ----------------------------------------------------------------------------------------------- | --------------------------------- |
 | classic(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10, k: int=0) -> OutputType                        | 通过直接对目标函数二阶导矩阵（海瑟矩阵）进行求逆来获取下一步的步长 |
-| modified(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: int=20, epsilon: float=1e-10, k: int=0) -> OutputType | 修正当前海瑟矩阵保证其正定性（目前只接入了一种修正方法）      |
+| modified(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType | 修正当前海瑟矩阵保证其正定性（目前只接入了一种修正方法）      |
 | CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-6, k: int=0) -> OutputType              | 采用牛顿-共轭梯度法求解梯度（非精确牛顿法的一种）         |
 
 #### 拟牛顿法（newton_quasi）
 
 ```python
 ou.newton_quasi.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
 | 方法头                                                                                          | 解释              |
 | -------------------------------------------------------------------------------------------- | --------------- |
-| bfgs(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: float=20, epsilon: float=1e-10, k: int=0) -> OutputType  | BFGS方法更新海瑟矩阵    |
-| dfp(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: float=20, epsilon: float=1e-4, k: int=0) -> OutputType    | DFP方法更新海瑟矩阵     |
+| bfgs(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType  | BFGS方法更新海瑟矩阵    |
+| dfp(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-4, k: int=0) -> OutputType    | DFP方法更新海瑟矩阵     |
 | L_BFGS(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: float=6, epsilon: float=1e-10, k: int=0) -> OutputType | 双循环方法更新BFGS海瑟矩阵 |
 
 #### 非线性最小二乘法（nonlinear_least_square）
 
 ```python
 ou.nonlinear_least_square.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                  | 解释                         |
 | ---------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------- |
 | gauss_newton(funcr: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType                                                        | 高斯-牛顿提出的方法框架，包括OR分解等操作     |
-| levenberg_marquardt(funcr: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, m: float=100, lamk: float=1, eta: float=0.2, p1: float=0.4, p2: float=0.9, gamma1: float=0.7, gamma2: float=1.3, epsilon: float=1e-10, k: int=0) -> OutputType | Levenberg Marquardt提出的方法框架 |
+| levenberg_marquardt(funcr: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, lamk: float=1, eta: float=0.2, p1: float=0.4, p2: float=0.9, gamma1: float=0.7, gamma2: float=1.3, epsilon: float=1e-10, k: int=0) -> OutputType | Levenberg Marquardt提出的方法框架 |
 
 #### 信赖域方法（trust_region）
 
 ```python
 ou.trust_region.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                               | 解释                  |
 | ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------- |
-| steihaug_CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, m: float=100, r0: float=1, rmax: float=2, eta: float=0.2, p1: float=0.4, p2: float=0.6, gamma1: float=0.5, gamma2: float=1.5, epsilon: float=1e-6, k: int=0) -> OutputType | 截断共轭梯度法在此方法中被用于搜索步长 |
+| steihaug_CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, r0: float=1, rmax: float=2, eta: float=0.2, p1: float=0.4, p2: float=0.6, gamma1: float=0.5, gamma2: float=1.5, epsilon: float=1e-6, k: int=0) -> OutputType | 截断共轭梯度法在此方法中被用于搜索步长 |
 
 ### 约束优化算法（constrain）
 
 ```python
 import optimtool.constrain as oc
 oc.[方法名].[函数名]([目标函数], [参数表], [等式约束表], [不等式约数表], [初始迭代点])
 ```
@@ -142,40 +158,40 @@
 
 ```python
 oc.equal.[函数名]([目标函数], [参数表], [等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                   | 解释        |
 | ----------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
-| penalty_quadratice(funcs: FuncArray, args: FuncArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=10, p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType                     | 增加二次罚项    |
-| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadratice(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType                     | 增加二次罚项    |
+| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 #### 不等式约束（unequal）
 
 ```python
 oc.unequal.[函数名]([目标函数], [参数表], [不等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                                      | 解释        |
 | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------- |
-| penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=10, p: float=0.4, epsilon: float=1e-10, k: int=0) -> OutputType                                     | 增加二次罚项    |
-| penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k: int=0) -> OutputType                              | 增加分式函数罚项  |
-| lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.4, epsilon: float=1e-10, k: int=0) -> OutputType                                     | 增加二次罚项    |
+| penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k: int=0) -> OutputType                              | 增加分式函数罚项  |
+| lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 #### 混合等式约束（mixequal）
 
 ```python
 oc.mixequal.[函数名]([目标函数], [参数表], [等式约束表], [不等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                                                                  | 解释        |
 | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
-| penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=10, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                             | 增加二次罚项    |
-| penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=1, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                                     | L1精确罚函数法  |
-| lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                             | 增加二次罚项    |
+| penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=1, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                                     | L1精确罚函数法  |
+| lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 ### 方法的应用（example）
 
 ```python
 import optimtool.example as oe
 ```
```

#### html2text {}

```diff
@@ -8,28 +8,34 @@
 [`Numpy`](https://github.com/numpy/numpy)
 åé«æå¤çæ°ç»é´è¿ç®ç­çç¹æ§ï¼å·§å¦å°åºç¨äº [`Sympy`]
 (https://github.com/sympy/sympy) åé¨æ¯æç .jacobian
 ç­æ¹æ³ï¼å¹¶ç»å Python åç½®å½æ° dict ä¸ zip å®ç°äº Sympy
 ç©éµå° Numpy
 ç©éµçè½¬æ¢ï¼æç»è®¾è®¡äºä¸ä¸ªç¨äºæä¼åç§å­¦ç ç©¶é¢åçPythonå·¥å·åã
 ç ç©¶äººåå¯ä»¥éè¿ç®åç [`pip`](https://github.com/pypa/pip)
-æä»¤è¿è¡ä¸è½½ä¸ä½¿ç¨ã ## é¡¹ç®ç»æ ```textile |- optimtool |-
-- constrain |-- __init__.py |-- equal.py |-- mixequal.py |-- unequal.py |-
-- example |-- __init__.py |-- Lasso.py |-- WanYuan.py |-- hybrid |-
-- __init__.py |-- approximate_point_gradient.py |-- unconstrain |-- __init__.py
-|-- gradient_descent.py |-- newton.py |-- newton_quasi.py |-
+æä»¤è¿è¡ä¸è½½ä¸ä½¿ç¨ã å¦æä½ å¨ç ç©¶ä¸­ä½¿ç¨
+**optimtool**ï¼æ¬¢è¿å¼ç¨å®å¨ä½ çåèèµæä¸­ï¼æç§ä¸é¢çæ ¼å¼ï¼ã
+```text ææ¯. optimtool: The fundamental package for scientific research in
+optimization. 2021. https://pypi.org/project/optimtool/. ``` ä¸è½½ææ°çï¼
+```text git clone https://github.com/linjing-lab/optimtool.git cd optimtool pip
+install -e . --verbose ``` ä¸è½½ç¨³å®çï¼ ```text pip install optimtool --
+upgrade ``` ## é¡¹ç®ç»æ ```textile |- optimtool |-- constrain |-
+- __init__.py |-- equal.py |-- mixequal.py |-- unequal.py |-- example |-
+- __init__.py |-- Lasso.py |-- WanYuan.py |-- hybrid |-- __init__.py |-
+- approximate_point_gradient.py |-- unconstrain |-- __init__.py |-
+- gradient_descent.py |-- newton.py |-- newton_quasi.py |-
 - nonlinear_least_square.py |-- trust_region.py |-- __init__.py |-- _convert.py
 |-- _drive.py |-- _kernel.py |-- _search.py |-- _typing.py |-- _utils.py |-
 - _version.py ```
 &emsp;&emsp;å ä¸ºå¨æ±è§£ä¸åçç®æ å½æ°çå¨å±æå±é¨æ¶æç¹æ¶ï¼ä¸åçæ±åæ¶æç¹çæ¹æ³ä¼æä¸åçæ¶ææçä»¥åä¸åçéç¨èå´ï¼èä¸å¨ç ç©¶è¿ç¨ä¸­ä¸åé¢åçç ç©¶æ¹æ³è¢«ä¸æ­å°æåºãä¿®æ¹ãå®åãæ©åï¼æä»¥è¿äºæ¹æ³æäºç°å¨äººä»¬å£ä¸­ç`æä¼åæ¹æ³`ã
 æ­¤é¡¹ç®ä¸­çææåé¨æ¯æçç®æ³ï¼é½æ¯å¨èæ°ãå¯¼æ°ãå¸éãå¸å½æ°ãå±è½­å½æ°ãæ¬¡æ¢¯åº¦åæä¼åçè®ºç­åºç¡æ¹æ³è®ºçåºç¡ä¸è¿è¡è®¾è®¡ä¸å®åçã
 &emsp;&emsp;optimtoolåç½®äºè¯¸å¦Barzilar
 Borweinéåè°æ¢¯åº¦ä¸éæ³ãä¿®æ­£çé¡¿æ³ãæéåå­BFGSæ¹æ³ãæªæ­å±è½­æ¢¯åº¦æ³-
 ä¿¡èµåæ¹æ³ãé«æ¯-
-çé¡¿æ³ç­æ çº¦æä¼åé¢åæ¶ææçä¸æ§è´¨è¾å¥½çç®æ³ï¼ä»¥åç¨äºè§£å³çº¦æä¼åé®é¢çäºæ¬¡ç½å½æ°æ³ãå¢å¹¿ææ ¼ææ¥æ³ç­ç®æ³ã
+çé¡¿æ³ç­æ çº¦æä¼åé¢åæ¶ææçä¸æ§è´¨å¥½çç®æ³ï¼ä»¥åç¨äºè§£å³çº¦æä¼åé®é¢çäºæ¬¡ç½å½æ°æ³ãå¢å¹¿ææ ¼ææ¥æ³ç­ç®æ³ã
 ## å¼å§ä½¿ç¨ ### æ çº¦æä¼åç®æ³ï¼unconstrainï¼ ```python import
 optimtool.unconstrain as ou ou.[æ¹æ³å].[å½æ°å]([ç®æ å½æ°],
 [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` #### æ¢¯åº¦ä¸éæ³ï¼gradient_descentï¼
 ```python ou.gradient_descent.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 --------------------- | ------------------------------------ | | solve(funcs:
@@ -39,112 +45,110 @@
 args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method:
 str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType |
 ä½¿ç¨çº¿æç´¢æ¹æ³æ±è§£éç²¾ç¡®æ­¥é¿ï¼é»è®¤ä½¿ç¨wolfeçº¿æç´¢ï¼ | |
 barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw:
 bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta:
 float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType |
 ä½¿ç¨Grippoä¸ZhangHangeræåºçéåè°çº¿æç´¢æ¹æ³æ´æ°æ­¥é¿ | ####
-çé¡¿æ³ï¼newton) ```python ou.newton.[å½æ°å]([ç®æ å½æ°],
+çé¡¿æ³ï¼newtonï¼ ```python ou.newton.[å½æ°å]([ç®æ å½æ°],
 [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | ------------------
 ----------------------------------------------------------------------------- |
 --------------------------------- | | classic(funcs: FuncArray, args: ArgArray,
 x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10,
 k: int=0) -> OutputType |
 éè¿ç´æ¥å¯¹ç®æ å½æ°äºé¶å¯¼ç©éµï¼æµ·çç©éµï¼è¿è¡æ±éæ¥è·åä¸ä¸æ­¥çæ­¥é¿
 | | modified(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw:
-bool=True, output_f: bool=False, method: str="wolfe", m: int=20, epsilon:
-float=1e-10, k: int=0) -> OutputType |
+bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k:
+int=0) -> OutputType |
 ä¿®æ­£å½åæµ·çç©éµä¿è¯å¶æ­£å®æ§ï¼ç®ååªæ¥å¥äºä¸ç§ä¿®æ­£æ¹æ³ï¼
 | | CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True,
 output_f: bool=False, method: str="wolfe", epsilon: float=1e-6, k: int=0) -
 > OutputType | éç¨çé¡¿-
 å±è½­æ¢¯åº¦æ³æ±è§£æ¢¯åº¦ï¼éç²¾ç¡®çé¡¿æ³çä¸ç§ï¼ | ####
 æçé¡¿æ³ï¼newton_quasiï¼ ```python ou.newton_quasi.[å½æ°å](
 [ç®æ å½æ°], [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | --
 -------------------------------------------------------------------------------
 ----------- | --------------- | | bfgs(funcs: FuncArray, args: ArgArray, x_0:
-PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m:
-float=20, epsilon: float=1e-10, k: int=0) -> OutputType |
-BFGSæ¹æ³æ´æ°æµ·çç©éµ | | dfp(funcs: FuncArray, args: ArgArray, x_0:
-PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m:
-float=20, epsilon: float=1e-4, k: int=0) -> OutputType |
-DFPæ¹æ³æ´æ°æµ·çç©éµ | | L_BFGS(funcs: FuncArray, args: ArgArray, x_0:
-PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m:
-float=6, epsilon: float=1e-10, k: int=0) -> OutputType |
+PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe",
+epsilon: float=1e-10, k: int=0) -> OutputType | BFGSæ¹æ³æ´æ°æµ·çç©éµ |
+| dfp(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True,
+output_f: bool=False, method: str="wolfe", epsilon: float=1e-4, k: int=0) -
+> OutputType | DFPæ¹æ³æ´æ°æµ·çç©éµ | | L_BFGS(funcs: FuncArray, args:
+ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method:
+str="wolfe", m: float=6, epsilon: float=1e-10, k: int=0) -> OutputType |
 åå¾ªç¯æ¹æ³æ´æ°BFGSæµ·çç©éµ | ####
 éçº¿æ§æå°äºä¹æ³ï¼nonlinear_least_squareï¼ ```python
 ou.nonlinear_least_square.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------- | -------------------------- | |
 gauss_newton(funcr: FuncArray, args: ArgArray, x_0: PointArray, draw:
 bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k:
 int=0) -> OutputType | é«æ¯-
 çé¡¿æåºçæ¹æ³æ¡æ¶ï¼åæ¬ORåè§£ç­æä½ | | levenberg_marquardt
 (funcr: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, m: float=100, lamk: float=1, eta: float=0.2, p1: float=0.4, p2:
-float=0.9, gamma1: float=0.7, gamma2: float=1.3, epsilon: float=1e-10, k:
-int=0) -> OutputType | Levenberg Marquardtæåºçæ¹æ³æ¡æ¶ | ####
+bool=False, lamk: float=1, eta: float=0.2, p1: float=0.4, p2: float=0.9,
+gamma1: float=0.7, gamma2: float=1.3, epsilon: float=1e-10, k: int=0) -
+> OutputType | Levenberg Marquardtæåºçæ¹æ³æ¡æ¶ | ####
 ä¿¡èµåæ¹æ³ï¼trust_regionï¼ ```python ou.trust_region.[å½æ°å](
 [ç®æ å½æ°], [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | --
 -------------------------------------------------------------------------------
 ---------------------------------------------------------------- | ------------
 ------- | | steihaug_CG(funcs: FuncArray, args: ArgArray, x_0: PointArray,
-draw: bool=True, output_f: bool=False, m: float=100, r0: float=1, rmax:
-float=2, eta: float=0.2, p1: float=0.4, p2: float=0.6, gamma1: float=0.5,
-gamma2: float=1.5, epsilon: float=1e-6, k: int=0) -> OutputType |
+draw: bool=True, output_f: bool=False, r0: float=1, rmax: float=2, eta:
+float=0.2, p1: float=0.4, p2: float=0.6, gamma1: float=0.5, gamma2: float=1.5,
+epsilon: float=1e-6, k: int=0) -> OutputType |
 æªæ­å±è½­æ¢¯åº¦æ³å¨æ­¤æ¹æ³ä¸­è¢«ç¨äºæç´¢æ­¥é¿ | ###
 çº¦æä¼åç®æ³ï¼constrainï¼ ```python import optimtool.constrain as oc
 oc.[æ¹æ³å].[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨],
 [ä¸ç­å¼çº¦æ°è¡¨], [åå§è¿­ä»£ç¹]) ``` #### ç­å¼çº¦æï¼equalï¼
 ```python oc.equal.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------- | --------- | | penalty_quadratice
-(funcs: FuncArray, args: FuncArray, cons: FuncArray, x_0: PointArray, draw:
-bool=True, output_f: bool=False, method: str="gradient_descent", sigma:
-float=10, p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType |
-å¢å äºæ¬¡ç½é¡¹ | | lagrange_augmentede(funcs: FuncArray, args: ArgArray,
-cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False,
-method: str="gradient_descent", lamk: float=6, sigma: float=10, p: float=2,
-etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType |
-å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | #### ä¸ç­å¼çº¦æï¼unequalï¼ ```python
-oc.unequal.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ä¸ç­å¼çº¦æè¡¨],
-[åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
+(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw:
+bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10,
+p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType | å¢å äºæ¬¡ç½é¡¹ |
+| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0:
+PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region",
+lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon:
+float=1e-6, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | ####
+ä¸ç­å¼çº¦æï¼unequalï¼ ```python oc.unequal.[å½æ°å]([ç®æ å½æ°],
+[åæ°è¡¨], [ä¸ç­å¼çº¦æè¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é
+| | ---------------------------------------------------------------------------
 -------------------------------------------------------------------------------
----------------------------------------------------------- | --------- | |
-penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0:
-PointArray, draw: bool=True, output_f: bool=False, method:
-str="gradient_descent", sigma: float=10, p: float=0.4, epsilon: float=1e-10, k:
-int=0) -> OutputType | å¢å äºæ¬¡ç½é¡¹ | | penalty_interior_fraction(funcs:
-FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True,
-output_f: bool=False, method: str="gradient_descent", sigma: float=12, p:
-float=0.6, epsilon: float=1e-6, k: int=0) -> OutputType |
-å¢å åå¼å½æ°ç½é¡¹ | | lagrange_augmentedu(funcs: FuncArray, args:
+-------------- | --------- | | penalty_quadraticu(funcs: FuncArray, args:
 ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="gradient_descent", muk: float=10, sigma: float=8,
-alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon:
-float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | ####
-æ··åç­å¼çº¦æï¼mixequalï¼ ```python oc.mixequal.[å½æ°å](
+bool=False, method: str="trust_region", sigma: float=10, p: float=0.4, epsilon:
+float=1e-10, k: int=0) -> OutputType | å¢å äºæ¬¡ç½é¡¹ | |
+penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray,
+x_0: PointArray, draw: bool=True, output_f: bool=False, method:
+str="trust_region", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k:
+int=0) -> OutputType | å¢å åå¼å½æ°ç½é¡¹ | | lagrange_augmentedu(funcs:
+FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True,
+output_f: bool=False, method: str="trust_region", muk: float=10, sigma:
+float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1,
+epsilon: float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ |
+#### æ··åç­å¼çº¦æï¼mixequalï¼ ```python oc.mixequal.[å½æ°å](
 [ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨], [ä¸ç­å¼çº¦æè¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 ------- | --------- | | penalty_quadraticm(funcs: FuncArray, args: ArgArray,
 cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw:
-bool=True, output_f: bool=False, method: str="gradient_descent", sigma:
-float=10, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType |
+bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10,
+p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType |
 å¢å äºæ¬¡ç½é¡¹ | | penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal:
 FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="gradient_descent", sigma: float=1, p: float=0.6,
-epsilon: float=1e-10, k: int=0) -> OutputType | L1ç²¾ç¡®ç½å½æ°æ³ | |
+bool=False, method: str="trust_region", sigma: float=1, p: float=0.6, epsilon:
+float=1e-10, k: int=0) -> OutputType | L1ç²¾ç¡®ç½å½æ°æ³ | |
 lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray,
 cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="gradient_descent", lamk: float=6, muk: float=10,
-sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3,
+bool=False, method: str="trust_region", lamk: float=6, muk: float=10, sigma:
+float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3,
 epsilon: float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ |
 ### æ¹æ³çåºç¨ï¼exampleï¼ ```python import optimtool.example as oe ```
 #### Lassoé®é¢ï¼Lassoï¼ ```python oe.Lasso.[å½æ°å]([ç©éµA],
 [ç©éµb], [å å­mu], [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é
 | | ---------------------------------------------------------------------------
 ---------------------------- | ---------------- | | gradient(A: NDArray, b:
 NDArray, mu: float, args: ArgArray, x_0: PointArray, draw: bool=True, output_f:
```

### Comparing `optimtool-2.4.1/optimtool/__init__.py` & `optimtool-2.4.2/optimtool/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,13 +19,13 @@
 # SOFTWARE.
 
 import sys
 
 from . import constrain
 from . import unconstrain
 from . import example
-from . import hybrid
+from . import hybrid # not implemented yet
 
 from ._version import __version__
 
 if sys.version_info < (3, 7, 0):
-    raise OSError(f'optimtool-2.4.1 requires Python >=3.7, but yours is {sys.version}')
+    raise OSError(f'optimtool-2.4.2 requires Python >=3.7, but yours is {sys.version}')
```

### Comparing `optimtool-2.4.1/optimtool/_convert.py` & `optimtool-2.4.2/optimtool/_convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,15 @@
     Returns
     -------
     funcs : SympyMutableDenseMatrix
         目标函数
 
     '''
     # convert funcs
-    if isinstance(funcs, (list, tuple)):
-        funcs = sp.Matrix(funcs)
-    else:
-        funcs = sp.Matrix([funcs])
-    return funcs
+    return sp.Matrix(funcs) if isinstance(funcs, (list, tuple)) else sp.Matrix([funcs])
 
 def a2m(args: ArgArray) -> SympyMutableDenseMatrix:
     '''
     Parameters
     ----------
     args : ArgArray
         参数
@@ -52,19 +48,15 @@
     Returns
     -------
     args : SympyMutableDenseMatrix
         参数
 
     '''
     # convert args
-    if isinstance(args, (list, tuple)):
-        args = sp.Matrix(args)
-    else:
-        args = sp.Matrix([args])
-    return args
+    return sp.Matrix(args) if isinstance(args, (list, tuple)) else sp.Matrix([args])
 
 def p2t(x_0: PointArray) -> PointArray:
     '''
     Parameters
     ----------
     x_0 : PointArray
         参数
@@ -72,43 +64,36 @@
     Returns
     -------
     x_0 : PointArray
         参数
 
     '''
     # convert x_0
-    if not isinstance(x_0, (list, tuple)):
-        x_0 = (x_0)
-    return x_0
+    return (x_0,) if not isinstance(x_0, (list, tuple)) else x_0
 
-def h2h(hessian: NDArray, m: float, pk: int=1) -> NDArray:
+def h2h(hessian: NDArray, pk: int=1) -> NDArray:
     '''
     Parameters
     ----------
     hessian : numpy.array
         未修正的海瑟矩阵值
         
-    m : float
-        条件数阈值
-        
     pk : int
         常数
         
 
     Returns
     -------
     numpy.array
         修正后的海瑟矩阵
         
     '''
-    l = hessian.shape[0]
+    l = hessian.shape[0] # hessian.shape = (l, l)
     while 1:
-        values, _ = np.linalg.eig(hessian)
-        flag = (all(values) > 0) & (np.linalg.cond(hessian) <= m)
-        if flag:
+        rank = np.linalg.matrix_rank(hessian)
+        if rank == l:
             break
         else:
             hessian = hessian + pk * np.identity(l)
-            pk = pk + 1
+            pk += 1
     return hessian
-
 __all__ = [f2m, a2m, p2t, h2h]
```

### Comparing `optimtool-2.4.1/optimtool/_drive.py` & `optimtool-2.4.2/optimtool/_drive.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.1/optimtool/_kernel.py` & `optimtool-2.4.2/optimtool/_kernel.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from .unconstrain.gradient_descent import barzilar_borwein
-from .unconstrain.newton import CG
+from .unconstrain.newton import modified
 from .unconstrain.newton_quasi import L_BFGS
 from .unconstrain.trust_region import steihaug_CG
-
+# will be updated in the future
 def kernel(method: str) -> str:
     '''
     method : str
         无约束优化方法内核
 
 
     Returns
     -------
     str
         内核方法名
         
     '''
-    if method == "gradient_descent":
-        return 'barzilar_borwein'
+    if method == "trust_region":
+        return 'steihaug_CG'
     elif method == "newton":
-        return 'CG'
+        return 'modified'
     elif method == "newton_quasi":
         return 'L_BFGS'
-    elif method == "trust_region":
-        return 'steihaug_CG'
-    return 'barzilar_borwein'
+    elif method == "gradient_descent":
+        return 'barzilar_borwein'
+    return 'steihaug_CG'
```

### Comparing `optimtool-2.4.1/optimtool/_search.py` & `optimtool-2.4.2/optimtool/_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import numpy as np
 from ._typing import List, NDArray, SympyMutableDenseMatrix, DataType, IterPointType
 
-# Armijo线搜索准则
 def armijo(funcs: SympyMutableDenseMatrix, args: SympyMutableDenseMatrix, x_0: IterPointType, d: NDArray, gamma: float=0.5, c: float=0.1) -> float:
     '''
     Parameters
     ----------
     funcs : SympyMutableDenseMatrix
         当前目标方程
         
@@ -51,29 +50,28 @@
         最优步长
         
     '''
     assert gamma > 0
     assert gamma < 1
     assert c > 0
     assert c < 1
-    alpha = 1.0
+    alpha = 1
     res = funcs.jacobian(args)
     reps = dict(zip(args, x_0))
     f0 = np.array(funcs.subs(reps)).astype(DataType)
     res0 = np.array(res.subs(reps)).astype(DataType)
     while 1:
         x = x_0 + (alpha*d)[0]
         f1 = np.array(funcs.subs(dict(zip(args, x)))).astype(DataType)
         if f1 <= f0 + c*alpha*res0.dot(d.T):
             break
         else:
             alpha = gamma * alpha
     return alpha
 
-# Goldstein线搜索准则
 def goldstein(funcs: SympyMutableDenseMatrix, args: SympyMutableDenseMatrix, x_0: IterPointType, d: NDArray, c: float=0.1, alphas: float=0, alphae: float=10, t: float=1.2, eps: float=1e-3) -> float:
     '''
     Parameters
     ----------
     funcs : SympyMutableDenseMatrix
         当前目标方程
         
@@ -129,15 +127,14 @@
         else:
             alphae = alpha
             alpha = 0.5 * (alphas + alphae)
         if np.abs(alphas-alphae) < eps:
             break
     return alpha
 
-# Wolfe线搜索准则
 def wolfe(funcs: SympyMutableDenseMatrix, args: SympyMutableDenseMatrix, x_0: IterPointType, d: NDArray, c1: float=0.3, c2: float=0.5, alphas: float=0, alphae: float=2, eps: float=1e-3) -> float:
     '''
     Parameters
     ----------
     funcs : SympyMutableDenseMatrix
         当前目标方程
         
@@ -196,15 +193,14 @@
         else:
             alphae = alpha
             alpha = 0.5 * (alphas + alphae)
         if np.abs(alphas-alphae) < eps:
             break
     return alpha
 
-# 非单调线搜索准则之Grippo（一般与Barzilar Borwein梯度下降法配合使用）
 def Grippo(funcs: SympyMutableDenseMatrix, args: SympyMutableDenseMatrix, x_0: IterPointType, d: NDArray, k: int, point: List[IterPointType], c1: float, beta: float, alpha: float, M: int=20) -> float:
     '''
     Parameters
     ----------
     funcs : SympyMutableDenseMatrix
         当前目标方程
         
@@ -259,15 +255,14 @@
             fk = max(fk, np.array(funcs.subs(dict(zip(args, point[k-j])))).astype(DataType))
         if f1 <= fk + c1 * alpha * res0.dot(d.T):
             break
         else:
             alpha = beta * alpha
     return alpha
 
-# 非单调线搜索准则之ZhangHanger（一般与程序配套使用）
 def ZhangHanger(funcs: SympyMutableDenseMatrix, args: SympyMutableDenseMatrix, x_0: IterPointType, d: NDArray, k: int, point: List[IterPointType], c1: float, beta: float, alpha: float, eta: float=0.6) -> float:
     '''
     Parameters
     ----------
     funcs : SympyMutableDenseMatrix
         当前目标方程
         
@@ -307,15 +302,15 @@
     '''
     assert eta > 0
     assert eta < 1
     assert c1 > 0
     assert c1 < 1
     assert beta > 0
     assert beta < 1
-    from ._utils import C_k
+    from ._drive import C_k
     reps = dict(zip(args, x_0))
     res = funcs.jacobian(args)
     res0 = np.array(res.subs(reps)).astype(DataType)
     while 1:
         x = x_0 + (alpha*d)[0]
         f1 = np.array(funcs.subs(dict(zip(args, x)))).astype(DataType)
         Ck = C_k(funcs, args, point, eta, k)
```

### Comparing `optimtool-2.4.1/optimtool/_typing.py` & `optimtool-2.4.2/optimtool/_typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 
 FuncArray = Union[SympyMutableDenseMatrix, FuncType, List[FuncType], Tuple[FuncType]]
 ArgArray = Union[SympyMutableDenseMatrix, ArgType, List[ArgType], Tuple[ArgType]]
 PointArray = Union[PointType, List[PointType], Tuple[PointType]]
 
 IterPointType = Union[NDArray, List[PointType], Tuple[PointType]]
 
-OutputType = Tuple[IterPointType, int, Optional[List[DataType]]]
+OutputType = Union[Tuple[IterPointType, int], Tuple[IterPointType, int, List[DataType]]]
```

### Comparing `optimtool-2.4.1/optimtool/_utils.py` & `optimtool-2.4.2/optimtool/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,19 +59,14 @@
         
     draw : bool
         绘图参数
         
     method : str
         最优化方法
         
-
-    Returns
-    -------
-    None
-        
     '''
     import matplotlib.pyplot as plt
     if draw is True:
         plt.plot([i for i in range(len(f))], f, marker='o', c="firebrick", ls='--')
         plt.xlabel("$k$")
         plt.ylabel("$f(x_k)$")
         plt.title(method)
```

### Comparing `optimtool-2.4.1/optimtool/_version.py` & `optimtool-2.4.2/optimtool/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = '2.4.1'
+__version__ = '2.4.2'
```

### Comparing `optimtool-2.4.1/optimtool/constrain/__init__.py` & `optimtool-2.4.2/optimtool/constrain/__init__.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.1/optimtool/constrain/equal.py` & `optimtool-2.4.2/optimtool/constrain/equal.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 import numpy as np
 import sympy as sp
 from .._utils import get_value, plot_iteration
 from .._convert import f2m, a2m, p2t
 
 from .._typing import FuncArray, ArgArray, PointArray, OutputType, DataType
 
-# 二次罚函数法（等式约束）
-def penalty_quadratice(funcs: FuncArray, args: FuncArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=10.0, p: float=2.0, epsilon: float=1e-4, k: int=0) -> OutputType:
+def penalty_quadratice(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10.0, p: float=2.0, epsilon: float=1e-4, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -68,37 +67,34 @@
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     assert sigma > 0
     assert p > 1
-    from .._kernel import kernel, barzilar_borwein, CG, L_BFGS, steihaug_CG
+    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
     funcs, args, x_0, cons = f2m(funcs), a2m(args), p2t(x_0), f2m(cons)
-    search = eval(kernel(method))
-    point = []
+    search, point, f = eval(kernel(method)), [], []
     sig = sp.symbols("sig")
     pen = funcs + (sig / 2) * cons.T * cons
-    f = []
     while 1:
         point.append(np.array(x_0))
         f.append(get_value(funcs, args, x_0))
         pe = pen.subs(sig, sigma)
         x_0, _ = search(pe, args, tuple(x_0), draw=False)
         k = k + 1
         if np.linalg.norm(x_0 - point[k - 1]) < epsilon:
             point.append(np.array(x_0))
             f.append(get_value(funcs, args, x_0))
             break
         sigma = p * sigma
     plot_iteration(f, draw, "penalty_quadratic_equal")     
     return (x_0, k, f) if output_f is True else (x_0, k)
 
-# 增广拉格朗日函数乘子法（等式约束）
-def lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType:
+def lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -142,18 +138,17 @@
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     assert sigma > 0
     assert p > 1
-    from .._kernel import kernel, barzilar_borwein, CG, L_BFGS, steihaug_CG
-    search = eval(kernel(method))
+    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
+    search, f = eval(kernel(method)), []
     funcs, args, x_0, cons = f2m(funcs), a2m(args), p2t(x_0), f2m(cons)
-    f = []
     lamk = np.array([lamk for i in range(cons.shape[0])]).reshape(cons.shape[0], 1)
     while 1:
         L = sp.Matrix([funcs + (sigma / 2) * cons.T * cons + cons.T * lamk])
         f.append(get_value(funcs, args, x_0))
         x_0, _ = search(L, args, tuple(x_0), draw=False, epsilon=etak)
         k = k + 1
         reps = dict(zip(args, x_0))
```

### Comparing `optimtool-2.4.1/optimtool/constrain/mixequal.py` & `optimtool-2.4.2/optimtool/constrain/mixequal.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 import numpy as np
 import sympy as sp
 from .._utils import get_value, plot_iteration
 from .._convert import f2m, a2m, p2t
 
 from .._typing import FuncArray, ArgArray, PointArray, OutputType, DataType
 
-# 二次罚函数法（混合约束）
-def penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=10, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType:
+def penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -71,19 +70,17 @@
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     assert sigma > 0
     assert p > 0
-    from .._kernel import kernel, barzilar_borwein, CG, L_BFGS, steihaug_CG
+    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
     funcs, args, cons_equal, cons_unequal, x_0 = f2m(funcs), a2m(args), f2m(cons_equal), f2m(cons_unequal), p2t(x_0)
-    search = eval(kernel(method))
-    f = []
-    point = []
+    search, point, f = eval(kernel(method)), [], []
     while 1:
         point.append(np.array(x_0))
         f.append(get_value(funcs, args, x_0))
         reps = dict(zip(args, x_0))
         consv = np.array(cons_unequal.subs(reps)).astype(DataType)
         consv = np.where(consv <= 0, consv, 1)
         consv = np.where(consv > 0, consv, 0)
@@ -94,16 +91,15 @@
             point.append(np.array(x_0))
             f.append(get_value(funcs, args, x_0))
             break
         sigma = p * sigma
     plot_iteration(f, draw, "penalty_quadratic_mixequal")
     return (x_0, k, f) if output_f is True else (x_0, k)
 
-# 精确罚函数法-l1罚函数法 （混合约束）
-def penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=1, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType:
+def penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=1, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -144,19 +140,17 @@
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     assert sigma > 0
     assert p > 0
-    from .._kernel import kernel, barzilar_borwein, CG, L_BFGS, steihaug_CG
+    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
     funcs, args, cons_equal, cons_unequal, x_0 = f2m(funcs), a2m(args), f2m(cons_equal), f2m(cons_unequal), p2t(x_0)
-    search = eval(kernel(method))
-    point = []
-    f = []
+    search, point, f = eval(kernel(method)), [], []
     while 1:
         point.append(np.array(x_0))
         f.append(get_value(funcs, args, x_0))
         reps = dict(zip(args, x_0))
         consv_unequal = np.array(cons_unequal.subs(reps)).astype(DataType)
         consv_unequal = np.where(consv_unequal <= 0, consv_unequal, 1)
         consv_unequal = np.where(consv_unequal > 0, consv_unequal, 0)
@@ -170,16 +164,15 @@
             point.append(np.array(x_0))
             f.append(get_value(funcs, args, x_0))
             break
         sigma = p * sigma
     plot_iteration(f, draw, "penalty_L1")
     return (x_0, k, f) if output_f is True else (x_0, k)
 
-# 增广拉格朗日函数法（混合约束）
-def lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType:
+def lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -238,19 +231,18 @@
         
     '''
     assert sigma > 0
     assert p > 1
     assert alpha > 0 
     assert alpha <= beta
     assert beta < 1
-    from .._kernel import kernel, barzilar_borwein, CG, L_BFGS, steihaug_CG
+    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
     from .._drive import cons_unequal_L, v_k, renew_mu_k
     funcs, args, cons_equal, cons_unequal, x_0 = f2m(funcs), a2m(args), f2m(cons_equal), f2m(cons_unequal), p2t(x_0)
-    search = eval(kernel(method))
-    f = []
+    search, f = eval(kernel(method)), []
     lamk = np.array([lamk for i in range(cons_equal.shape[0])]).reshape(cons_equal.shape[0], 1)
     muk = np.array([muk for i in range(cons_unequal.shape[0])]).reshape(cons_unequal.shape[0], 1)
     while 1:
         etak = 1 / sigma
         epsilonk = 1 / sigma**alpha
         cons_uneuqal_modifyed = cons_unequal_L(cons_unequal, args, muk, sigma, x_0)
         L = sp.Matrix([funcs + (sigma / 2) * (cons_equal.T * cons_equal + cons_uneuqal_modifyed) + cons_equal.T * lamk])
@@ -262,19 +254,17 @@
             res = L.jacobian(args)
             if (vkx <= epsilon) and (np.linalg.norm(np.array(res.subs(dict(zip(args, x_0)))).astype(DataType)) <= eta):
                 f.append(get_value(funcs, args, x_0))
                 break
             else:
                 lamk = lamk + sigma * np.array(cons_equal.subs(dict(zip(args, x_0)))).astype(DataType)
                 muk = renew_mu_k(cons_unequal, args, muk, sigma, x_0)
-                sigma = sigma
                 etak = etak / sigma
                 epsilonk = epsilonk / sigma**beta
         else:
-            lamk = lamk
             sigma = p * sigma
             etak = 1 / sigma
             epsilonk  = 1 / sigma**alpha
     plot_iteration(f, draw, "lagrange_augmented_mixequal")
     return (x_0, k, f) if output_f is True else (x_0, k)
 
 __all__ = [penalty_quadraticm, penalty_L1, lagrange_augmentedm]
```

### Comparing `optimtool-2.4.1/optimtool/constrain/unequal.py` & `optimtool-2.4.2/optimtool/constrain/unequal.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 import sympy as sp
 import numpy as np
 from .._utils import get_value, plot_iteration
 from .._convert import f2m, a2m, p2t
 
 from .._typing import FuncArray, ArgArray, PointArray, OutputType, DataType
 
-# 二次罚函数法（不等式约束）
-def penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=10, p: float=0.4, epsilon: float=1e-10, k: int=0) -> OutputType:
+def penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.4, epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -69,19 +68,17 @@
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     assert sigma > 0
     assert p > 0
     assert p < 1
-    from .._kernel import kernel, barzilar_borwein, CG, L_BFGS, steihaug_CG
+    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
     funcs, args, x_0, cons = f2m(funcs), a2m(args), p2t(x_0), f2m(cons)
-    search = eval(kernel(method))
-    point = []
-    f = []
+    search, point, f = eval(kernel(method)), [], []
     while 1:
         point.append(np.array(x_0))
         f.append(get_value(funcs, args, x_0))
         reps = dict(zip(args, x_0))
         consv = np.array(cons.subs(reps)).astype(DataType)
         consv = np.where(consv <= 0, consv, 1)
         consv = np.where(consv > 0, consv, 0)
@@ -92,21 +89,18 @@
             point.append(np.array(x_0))
             f.append(get_value(funcs, args, x_0))
             break
         sigma = p * sigma
     plot_iteration(f, draw, "penalty_quadratic_unequal") 
     return (x_0, k, f) if output_f is True else (x_0, k)
 
-# 内点罚函数法（不等式约束）
 '''
 保证点在定义域内
 '''
-
-# 分式
-def penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k: int=0) -> OutputType:
+def penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -145,19 +139,17 @@
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     assert sigma > 0
     assert p > 0
     assert p < 1
-    from .._kernel import kernel, barzilar_borwein, CG, L_BFGS, steihaug_CG
+    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
     funcs, args, x_0, cons = f2m(funcs), a2m(args), p2t(x_0), f2m(cons)
-    search = eval(kernel(method))
-    point = []
-    f = []
+    search, point, f = eval(kernel(method)), [], []
     sub_pe = 0
     for i in cons:
         sub_pe += 1 / i
     sub_pe = sp.Matrix([sub_pe])
     while 1:
         point.append(np.array(x_0))
         f.append(get_value(funcs, args, x_0))
@@ -167,17 +159,16 @@
         sigma = p * sigma
         if np.linalg.norm(x_0 - point[k - 1]) < epsilon:
             point.append(np.array(x_0))
             f.append(get_value(funcs, args, x_0))
             break
     plot_iteration(f, draw, "penalty_interior_fraction")
     return (x_0, k, f) if output_f is True else (x_0, k)
-    
-# 增广拉格朗日函数法（不等式约束）
-def lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType:
+
+def lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -230,20 +221,19 @@
         
     '''
     assert sigma > 0
     assert p > 1
     assert alpha > 0 
     assert alpha <= beta
     assert beta < 1
-    from .._kernel import kernel, barzilar_borwein, CG, L_BFGS, steihaug_CG
+    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
     from .._drive import cons_unequal_L, renew_mu_k, v_k
     funcs, args, x_0, cons = f2m(funcs), a2m(args), p2t(x_0), f2m(cons)
-    search = eval(kernel(method))
-    f = []
-    muk = np.array([muk for i in range(cons.shape[0])]).reshape(cons.shape[0], 1)
+    search, f = eval(kernel(method)), []
+    muk = np.array([muk for _ in range(cons.shape[0])]).reshape(cons.shape[0], 1)
     while 1:
         etak = 1 / sigma
         epsilonk = 1 / sigma**alpha
         cons_uneuqal_modifyed = cons_unequal_L(cons, args, muk, sigma, x_0)
         L = sp.Matrix([funcs + (sigma / 2) * cons_uneuqal_modifyed])
         f.append(get_value(funcs, args, x_0))
         x_0, _ = search(L, args, x_0, draw=False, epsilon=epsilonk)
@@ -252,15 +242,14 @@
         if vkx <= epsilonk:
             res = L.jacobian(args)
             if (vkx <= epsilon) and (np.linalg.norm(np.array(res.subs(dict(zip(args, x_0)))).astype(DataType)) <= eta):
                 f.append(get_value(funcs, args, x_0))
                 break
             else:
                 muk = renew_mu_k(cons, args, muk, sigma, x_0)
-                sigma = sigma
                 etak = etak / sigma
                 epsilonk = epsilonk / sigma**beta
         else:
             sigma = p * sigma
             etak = 1 / sigma
             epsilonk  = 1 / sigma**alpha
     plot_iteration(f, draw, "lagrange_augmented_unequal")
```

### Comparing `optimtool-2.4.1/optimtool/example/Lasso.py` & `optimtool-2.4.2/optimtool/example/Lasso.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,16 +70,15 @@
         
     '''
     from .._drive import get_f_delta_gradient
     args = a2m(args)
     funcs = sp.Matrix([0.5*((A*args - b).T)*(A*args - b)])
     res = funcs.jacobian(args)
     L = np.linalg.norm((A.T).dot(A)) + mu / delta
-    point = []
-    f = []
+    point, f = [], []
     while 1:
         reps = dict(zip(args, x_0))
         point.append(np.array(x_0))
         f.append(get_value(funcs, args, x_0, mu))
         resv = np.array(res.subs(reps)).astype(DataType)
         argsv = np.array(args.subs(reps)).astype(DataType)
         g = get_f_delta_gradient(resv, argsv, mu, delta)
@@ -138,16 +137,15 @@
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     from .._drive import get_subgradient
     args = a2m(args)
     funcs = sp.Matrix([0.5*((A*args - b).T)*(A*args - b)])
     res = funcs.jacobian(args)
-    point = []
-    f = []
+    point, f = [], []
     while 1:
         reps = dict(zip(args, x_0))
         point.append(np.array(x_0))
         f.append(get_value(funcs, args, x_0, mu))
         resv = np.array(res.subs(reps)).astype(DataType)
         argsv = np.array(args.subs(reps)).astype(DataType)
         g = get_subgradient(resv, argsv, mu)
@@ -201,19 +199,18 @@
 
     Returns
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
-    assert gamma < 1
     assert gamma > 0
+    assert gamma < 1
     args = a2m(args)
-    funcs = sp.Matrix([0.5*((A*args - b).T)*(A*args - b)])
-    f = []
+    funcs, f = sp.Matrix([0.5*((A*args - b).T)*(A*args - b)]), []
     while mu >= epsilon:
         f.append(get_value(funcs, args, x_0, mu))
         x_0, _ = subgradient(A, b, mu, args, x_0, False)
         if mu > epsilon:
             mu = max(epsilon, gamma * mu)
             k = k + 1
         else:
@@ -261,22 +258,18 @@
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     args = a2m(args)
     values, _ = np.linalg.eig((A.T).dot(A))
     lambda_ma = max(values)
-    if isinstance(lambda_ma, complex):
-        tk = 1 / np.real(lambda_ma)
-    else:
-        tk = 1 / lambda_ma
+    tk = 1 / np.real(lambda_ma) if isinstance(lambda_ma, complex) else 1 / lambda_ma
     funcs = sp.Matrix([0.5*((A*args - b).T)*(A*args - b)])
     res = funcs.jacobian(args)
-    f = []
-    point = []
+    point, f = [], []
     while 1:
         reps = dict(zip(args, x_0))
         f.append(get_value(funcs, args, x_0, mu))
         point.append(x_0)
         grad = np.array(res.subs(reps)).astype(DataType)
         x_0 = np.sign(x_0 - tk * grad[0]) * [max(i, 0) for i in np.abs(x_0 - tk * grad[0]) - tk * mu]
         k = k + 1
```

### Comparing `optimtool-2.4.1/optimtool/example/WanYuan.py` & `optimtool-2.4.2/optimtool/example/WanYuan.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,15 +309,15 @@
         plt.annotate(r'$(x_3, y_3)$', xy=(x3, y3), xycoords='data', xytext=(+10, -10), textcoords='offset points', fontsize=10, arrowprops=dict(arrowstyle="->", connectionstyle="arc3,rad=.2"))
         plt.axis("equal")
         plt.show()
         return None
     
     final = []
     funcr, args = maker_data(m, n, a, b, c, x3, y3)
-    fin, k = gauss_newton(funcr, args, x_0, False, epsilon=eps)
+    fin, _ = gauss_newton(funcr, args, x_0, False, epsilon=eps)
     for i in fin: # for i in map(round, fin):
         final.append(round(i, 2)) # final.append(i)
     print("(x0, y0)=",(final[0], final[1]),"\n(x1, y1)=",(final[2], final[3]),"\n(x2, y2)=",(final[4], final[5]))
     if draw is True: # 绘图
         plot_solve(final, x_0, m, n, a, b, c, x3, y3)
     return None
```

### Comparing `optimtool-2.4.1/optimtool/example/__init__.py` & `optimtool-2.4.2/optimtool/example/__init__.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.1/optimtool/hybrid/__init__.py` & `optimtool-2.4.2/optimtool/hybrid/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from . import approximate_point_gradient
+from . import approximate_point_gradient 
+# will be updated in the future
```

### Comparing `optimtool-2.4.1/optimtool/hybrid/approximate_point_gradient.py` & `optimtool-2.4.2/optimtool/hybrid/approximate_point_gradient.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.1/optimtool/unconstrain/__init__.py` & `optimtool-2.4.2/optimtool/unconstrain/__init__.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.1/optimtool/unconstrain/gradient_descent.py` & `optimtool-2.4.2/optimtool/unconstrain/newton.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,22 +15,20 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import numpy as np
-import sympy as sp
 from .._utils import get_value, plot_iteration
-from .._convert import f2m, a2m, p2t
+from .._convert import f2m, a2m, p2t, h2h
 
-from .._typing import FuncArray, ArgArray, PointArray, DataType, OutputType
+from .._typing import FuncArray, ArgArray, PointArray, OutputType, DataType
 
-# 梯度下降法
-def solve(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10, k: int=0) -> OutputType:
+def classic(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -56,35 +54,31 @@
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
     res = funcs.jacobian(args)
-    m = sp.symbols("m")
-    arg = sp.Matrix([m])
-    fx = []
+    hes = res.jacobian(args)
+    f = []
     while 1:
         reps = dict(zip(args, x_0))
-        fx.append(get_value(funcs, args, x_0))
-        dk = -np.array(res.subs(reps)).astype(DataType)
+        f.append(get_value(funcs, args, x_0))
+        hessian = np.array(hes.subs(reps)).astype(DataType)
+        gradient = np.array(res.subs(reps)).astype(DataType)
+        dk = - np.linalg.inv(hessian).dot(gradient.T).reshape(1, -1)
         if np.linalg.norm(dk) >= epsilon:
-            xt = x_0 + m * dk[0]
-            f = funcs.subs(dict(zip(args, xt)))
-            h = f.jacobian(arg)
-            mt = sp.solve(h)
-            x_0 = (x_0 + mt[m] * dk[0]).astype(DataType)
+            x_0 = x_0 + dk[0]
             k = k + 1
         else:
             break
-    plot_iteration(fx, draw, "gradient_descent_solve")
-    return (x_0, k, fx) if output_f is True else (x_0, k)
+    plot_iteration(f, draw, "newton_classic")        
+    return (x_0, k, f) if output_f is True else (x_0, k)
 
-# 最速下降法
-def steepest(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType:
+def modified(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: int=20, epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -94,17 +88,17 @@
         初始迭代点
         
     draw : bool
         绘图接口参数
         
     output_f : bool
         输出迭代函数值列表
-        
+
     method : str
-        非精确线搜索方法
+        单调线搜索方法："armijo", "goldstein", "wolfe"
         
     epsilon : float
         迭代停机准则
         
     k : int
         迭代次数
         
@@ -112,33 +106,35 @@
     Returns
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     from .._search import armijo, goldstein, wolfe
-    search = eval(method)
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
+    search, f = eval(method), []
     res = funcs.jacobian(args)
-    fx = []
+    hes = res.jacobian(args)
     while 1:
         reps = dict(zip(args, x_0))
-        fx.append(get_value(funcs, args, x_0))
-        dk = -np.array(res.subs(reps)).astype(DataType)
+        f.append(get_value(funcs, args, x_0))
+        gradient = np.array(res.subs(reps)).astype(DataType)
+        hessian = np.array(hes.subs(reps)).astype(DataType)
+        hessian = h2h(hessian)
+        dk = -np.linalg.inv(hessian).dot(gradient.T).reshape(1, -1)
         if np.linalg.norm(dk) >= epsilon:
             alpha = search(funcs, args, x_0, dk)
             x_0 = x_0 + alpha * dk[0]
             k = k + 1
         else:
             break
-    plot_iteration(fx, draw, "gradient_descent_steepest")
-    return (x_0, k, fx) if output_f is True else (x_0, k)
-    
-# Barzilar Borwein梯度下降法
-def barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta: float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType:
+    plot_iteration(f, draw, "newton_modified_" + method)
+    return (x_0, k, f) if output_f is True else (x_0, k)
+
+def CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-6, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -148,66 +144,47 @@
         初始迭代点
         
     draw : bool
         绘图接口参数
         
     output_f : bool
         输出迭代函数值列表
-        
+
     method : str
-        非单调线搜索方法："Grippo"与"ZhangHanger"
-        
-    M : int
-        阈值
-        
-    c1 : float
-        常数
-        
-    beta : float
-        常数
-        
-    alpha : float
-        初始步长
+        单调线搜索方法："armijo", "goldstein", "wolfe"
         
     epsilon : float
         迭代停机准则
         
     k : int
         迭代次数
         
 
     Returns
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
-    assert alpha > 0
-    assert c1 > 0
-    assert c1 < 1
-    assert beta > 0
-    assert beta < 1
-    from .._search import Grippo, ZhangHanger
-    search = eval(method)
+    from .._search import armijo, goldstein, wolfe
+    from .._drive import CG_gradient
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
+    search, f = eval(method), []
     res = funcs.jacobian(args)
-    point, f = [], []
+    hes = res.jacobian(args)
+    dk0 = np.zeros((args.shape[0], 1))
     while 1:
-        point.append(x_0)
         reps = dict(zip(args, x_0))
         f.append(get_value(funcs, args, x_0))
-        dk = - np.array(res.subs(reps)).astype(DataType)
+        gradient = np.array(res.subs(reps)).astype(DataType)
+        hess = np.array(hes.subs(reps)).astype(DataType)
+        dk, _ = CG_gradient(hess, -gradient, dk0)
         if np.linalg.norm(dk) >= epsilon:
-            alpha = search(funcs, args, x_0, dk, k, point, c1, beta, alpha)
-            delta = alpha * dk[0]
-            x_0 = x_0 + delta
-            sk = delta
-            yk = np.array(res.subs(dict(zip(args, x_0)))).astype(DataType) + dk
-            if sk.dot(yk.T) != 0:
-                alpha = sk.dot(sk.T) / sk.dot(yk.T)
+            alpha = search(funcs, args, x_0, dk)
+            x_0 = x_0 + alpha * dk[0]
             k = k + 1
         else:
             break
-    plot_iteration(f, draw, "gradient_descent_barzilar_borwein_" + method)
+    plot_iteration(f, draw, "newton_CG_" + method)
     return (x_0, k, f) if output_f is True else (x_0, k)
 
-__all__ = [solve, steepest, barzilar_borwein]
+__all__ = [classic, modified, CG]
```

### Comparing `optimtool-2.4.1/optimtool/unconstrain/newton.py` & `optimtool-2.4.2/optimtool/unconstrain/gradient_descent.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import numpy as np
+import sympy as sp # replace with `from .._base import np, sp` in the future version
 from .._utils import get_value, plot_iteration
-from .._convert import f2m, a2m, p2t, h2h
+from .._convert import f2m, a2m, p2t
 
-from .._typing import FuncArray, ArgArray, PointArray, OutputType, DataType
+from .._typing import FuncArray, ArgArray, PointArray, DataType, OutputType
 
-# 经典牛顿法
-def classic(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10, k: int=0) -> OutputType:
+def solve(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -55,33 +55,33 @@
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
     res = funcs.jacobian(args)
-    hes = res.jacobian(args)
+    m = sp.symbols("m")
+    arg = sp.Matrix([m])
     f = []
     while 1:
         reps = dict(zip(args, x_0))
         f.append(get_value(funcs, args, x_0))
-        hessian = np.array(hes.subs(reps)).astype(DataType)
-        gradient = np.array(res.subs(reps)).astype(DataType)
-        dk = - np.linalg.inv(hessian).dot(gradient.T)
-        dk = dk.reshape(1, -1)
+        dk = -np.array(res.subs(reps)).astype(DataType)
         if np.linalg.norm(dk) >= epsilon:
-            x_0 = x_0 + dk[0]
+            xt = x_0 + m * dk[0]
+            h = funcs.subs(dict(zip(args, xt))).jacobian(arg)
+            mt = sp.solve(h)
+            x_0 = (x_0 + mt[m] * dk[0]).astype(DataType)
             k = k + 1
         else:
             break
-    plot_iteration(f, draw, "newton_classic")        
+    plot_iteration(f, draw, "gradient_descent_solve")
     return (x_0, k, f) if output_f is True else (x_0, k)
-    
-# 修正牛顿法
-def modified(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: int=20, epsilon: float=1e-10, k: int=0) -> OutputType:
+
+def steepest(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -91,20 +91,17 @@
         初始迭代点
         
     draw : bool
         绘图接口参数
         
     output_f : bool
         输出迭代函数值列表
-
-    method : str
-        单调线搜索方法："armijo", "goldstein", "wolfe"
         
-    m : float
-        海瑟矩阵条件数阈值
+    method : str
+        非精确线搜索方法
         
     epsilon : float
         迭代停机准则
         
     k : int
         迭代次数
         
@@ -112,38 +109,32 @@
     Returns
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     from .._search import armijo, goldstein, wolfe
+    search, f = eval(method), []
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
-    search = eval(method)
     res = funcs.jacobian(args)
-    hes = res.jacobian(args)
-    f = []
     while 1:
         reps = dict(zip(args, x_0))
         f.append(get_value(funcs, args, x_0))
-        gradient = np.array(res.subs(reps)).astype(DataType)
-        hess = np.array(hes.subs(reps)).astype(DataType)
-        hessian = h2h(hess, m)
-        dk = - np.linalg.inv(hessian).dot(gradient.T)
-        dk = dk.reshape(1, -1)
+        dk = -np.array(res.subs(reps)).astype(DataType)
         if np.linalg.norm(dk) >= epsilon:
             alpha = search(funcs, args, x_0, dk)
             x_0 = x_0 + alpha * dk[0]
             k = k + 1
         else:
             break
-    plot_iteration(f, draw, "newton_modified_" + method)
+    plot_iteration(f, draw, "gradient_descent_steepest")
     return (x_0, k, f) if output_f is True else (x_0, k)
-
-# 非精确牛顿法
-def CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-6, k: int=0) -> OutputType:
+    
+# Barzilar Borwein梯度下降法
+def barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta: float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -153,49 +144,66 @@
         初始迭代点
         
     draw : bool
         绘图接口参数
         
     output_f : bool
         输出迭代函数值列表
-
+        
     method : str
-        单调线搜索方法："armijo", "goldstein", "wolfe"
+        非单调线搜索方法："Grippo"与"ZhangHanger"
+        
+    M : int
+        阈值
+        
+    c1 : float
+        常数
+        
+    beta : float
+        常数
+        
+    alpha : float
+        初始步长
         
     epsilon : float
         迭代停机准则
         
     k : int
         迭代次数
         
 
     Returns
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
-    from .._search import armijo, goldstein, wolfe
-    from .._drive import CG_gradient
+    assert alpha > 0
+    assert c1 > 0
+    assert c1 < 1
+    assert beta > 0
+    assert beta < 1
+    from .._search import Grippo, ZhangHanger
+    search, point, f = eval(method), [], []
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
-    search = eval(method)
     res = funcs.jacobian(args)
-    hes = res.jacobian(args)
-    dk0 = np.zeros((args.shape[0], 1))
-    f = []
     while 1:
+        point.append(x_0)
         reps = dict(zip(args, x_0))
         f.append(get_value(funcs, args, x_0))
-        gradient = np.array(res.subs(reps)).astype(DataType)
-        hess = np.array(hes.subs(reps)).astype(DataType)
-        # 采用共轭梯度法求解梯度
-        dk, _ = CG_gradient(hess, -gradient, dk0)
+        dk = - np.array(res.subs(reps)).astype(DataType)
         if np.linalg.norm(dk) >= epsilon:
-            alpha = search(funcs, args, x_0, dk)
-            x_0 = x_0 + alpha * dk[0]
+            alpha = search(funcs, args, x_0, dk, k, point, c1, beta, alpha)
+            delta = alpha * dk[0]
+            x_0 = x_0 + delta
+            yk = np.array(res.subs(dict(zip(args, x_0)))).astype(DataType) + dk
+            alpha_up = delta.dot(delta.T)
+            alpha_down = delta.dot(yk.T)
+            if alpha_down != 0:
+                alpha = alpha_up / alpha_down
             k = k + 1
         else:
             break
-    plot_iteration(f, draw, "newton_CG_" + method)
+    plot_iteration(f, draw, "gradient_descent_barzilar_borwein_" + method)
     return (x_0, k, f) if output_f is True else (x_0, k)
 
-__all__ = [classic, modified, CG]
+__all__ = [solve, steepest, barzilar_borwein]
```

### Comparing `optimtool-2.4.1/optimtool/unconstrain/newton_quasi.py` & `optimtool-2.4.2/optimtool/unconstrain/newton_quasi.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,17 +43,14 @@
         
     output_f : bool
         输出迭代函数值列表
         
     method : str
         单调线搜索方法："armijo", "goldstein", "wolfe"
         
-    m : float
-        海瑟矩阵条件数阈值
-        
     epsilon : float
         迭代停机准则
         
     k : int
         迭代次数
         
 
@@ -61,20 +58,19 @@
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     from .._search import armijo, goldstein, wolfe
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
-    search = eval(method)
+    search, f = eval(method), []
     res = funcs.jacobian(args)
     hes = res.jacobian(args)
     hess = np.array(hes.subs(dict(zip(args, x_0)))).astype(DataType)
-    hess = h2h(hess, m)
-    f = []
+    hess = h2h(hess)
     while 1:
         reps = dict(zip(args, x_0))
         f.append(get_value(funcs, args, x_0))
         gradient = np.array(res.subs(reps)).astype(DataType)
         dk = - np.linalg.inv(hess).dot(gradient.T)
         dk = dk.reshape(1, -1)
         if np.linalg.norm(dk) >= epsilon:
@@ -110,17 +106,14 @@
         
     output_f : bool
         输出迭代函数值列表
         
     method : str
         单调线搜索方法："armijo", "goldstein", "wolfe"
         
-    m : float
-        海瑟矩阵条件数阈值
-        
     epsilon : float
         迭代停机准则
         
     k : int
         迭代次数
         
 
@@ -128,21 +121,20 @@
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     from .._search import armijo, goldstein, wolfe
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
-    search = eval(method)
+    search, f = eval(method), []
     res = funcs.jacobian(args)
     hes = res.jacobian(args)
     hess = np.array(hes.subs(dict(zip(args, x_0)))).astype(DataType)
-    hess = h2h(hess, m)
+    hess = h2h(hess)
     hessi = np.linalg.inv(hess)
-    f = []
     while 1:
         reps = dict(zip(args, x_0))
         f.append(get_value(funcs, args, x_0))
         gradient = np.array(res.subs(reps)).astype(DataType)
         dk = - hessi.dot(gradient.T)
         dk = dk.reshape(1, -1)
         if np.linalg.norm(dk) >= epsilon:
@@ -155,15 +147,15 @@
                 hessi = hessi - (hessi.dot(yk.T)).dot((hessi.dot(yk.T)).T) / yk.dot(hessi.dot(yk.T)) + (sk.T).dot(sk) / yk.dot(sk.T)
             k = k + 1
         else:
             break
     plot_iteration(f, draw, "newton_quasi_dfp_" + method)
     return (x_0, k, f) if output_f is True else (x_0, k)
 
-# L_BFGS方法
+# will be updated in the future
 def L_BFGS(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: float=6, epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
@@ -179,15 +171,15 @@
     output_f : bool
         输出迭代函数值列表
         
     method : str
         单调线搜索方法："armijo", "goldstein", "wolfe"
         
     m : float
-        海瑟矩阵条件数阈值
+        阈值
         
     epsilon : float
         迭代停机准则
         
     k : int
         迭代次数
```

### Comparing `optimtool-2.4.1/optimtool/unconstrain/nonlinear_least_square.py` & `optimtool-2.4.2/optimtool/unconstrain/nonlinear_least_square.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import numpy as np
 import sympy as sp
 from .._convert import f2m, a2m, p2t, h2h
 from .._utils import get_value, plot_iteration
 
 from .._typing import FuncArray, ArgArray, PointArray, OutputType, DataType
 
-# 高斯-牛顿法（非线性最小二乘问题）
 def gauss_newton(funcr: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
@@ -59,18 +58,18 @@
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     from .._search import armijo, goldstein, wolfe
     funcr, args, x_0 = f2m(funcr), a2m(args), p2t(x_0)
-    search = eval(method)
+    assert funcr.shape[0] > 1 and funcr.shape[1] ==1 and args.shape[0] == len(x_0)
+    search, f = eval(method), []
     res = funcr.jacobian(args)
     funcs = sp.Matrix([(1/2)*funcr.T*funcr])
-    f = []
     while 1:
         reps = dict(zip(args, x_0))
         rk = np.array(funcr.subs(reps)).astype(DataType)
         f.append(get_value(funcs, args, x_0))
         jk = np.array(res.subs(reps)).astype(DataType)
         q, r = np.linalg.qr(jk)
         dk = np.linalg.inv(r).dot(-(q.T).dot(rk)).reshape(1,-1)
@@ -79,16 +78,15 @@
             x_0 = x_0 + alpha * dk[0]
             k = k + 1
         else:
             break
     plot_iteration(f, draw, "nonlinear_least_square_gauss_newton_" + method)
     return (x_0, k, f) if output_f is True else (x_0, k)
 
-# levenberg marquardt方法
-def levenberg_marquardt(funcr: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, m: float=100, lamk: float=1, eta: float=0.2, p1: float=0.4, p2: float=0.9, gamma1: float=0.7, gamma2: float=1.3, epsilon: float=1e-10, k: int=0) -> OutputType:
+def levenberg_marquardt(funcr: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, lamk: float=1, eta: float=0.2, p1: float=0.4, p2: float=0.9, gamma1: float=0.7, gamma2: float=1.3, epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -98,17 +96,14 @@
         初始迭代点
         
     draw : bool
         绘图接口参数
         
     output_f : bool
         输出迭代函数值列表
-
-    m : float
-        海瑟矩阵条件数阈值
         
     lamk : float
         修正常数
         
     eta : float
         常数
         
@@ -141,14 +136,15 @@
     assert eta < p1
     assert p1 < p2
     assert p2 < 1
     assert gamma1 < 1
     assert gamma2 > 1
     from .._drive import CG_gradient
     funcr, args, x_0 = f2m(funcr), a2m(args), p2t(x_0)
+    assert funcr.shape[0] > 1 and funcr.shape[1] ==1 and args.shape[0] == len(x_0)
     res = funcr.jacobian(args)
     funcs = sp.Matrix([(1/2)*funcr.T*funcr])
     resf = funcs.jacobian(args)
     hess = resf.jacobian(args)
     dk0 = np.zeros((args.shape[0], 1))
     f = []
     while 1:
@@ -156,29 +152,25 @@
         rk = np.array(funcr.subs(reps)).astype(DataType)
         f.append(get_value(funcs, args, x_0))
         jk = np.array(res.subs(reps)).astype(DataType)
         dk, _ = CG_gradient((jk.T).dot(jk) + lamk, -((jk.T).dot(rk)).reshape(1, -1), dk0)
         pk_up = np.array(funcs.subs(reps)).astype(DataType) - np.array(funcs.subs(dict(zip(args, x_0 + dk[0])))).astype(DataType)
         grad_f = np.array(resf.subs(reps)).astype(DataType)
         hess_f = np.array(hess.subs(reps)).astype(DataType)
-        hess_f = h2h(hess_f, m)
-        pk_down = - (grad_f.dot(dk.T) + 0.5*((dk.dot(hess_f)).dot(dk.T)))
+        hess_f = h2h(hess_f)
+        pk_down = -(grad_f.dot(dk.T) + 0.5*((dk.dot(hess_f)).dot(dk.T)))
         pk = pk_up / pk_down
         if np.linalg.norm(dk) >= epsilon:
             if pk < p1:
                 lamk = gamma2 * lamk
             else:
                 if pk > p2:
                     lamk = gamma1 * lamk
-                else:
-                    lamk = lamk
             if pk > eta:
                 x_0 = x_0 + dk[0]
-            else:
-                x_0 = x_0
             k = k + 1
         else:
             break
     plot_iteration(f, draw, "nonlinear_least_square_levenberg_marquardt")        
     return (x_0, k, f) if output_f is True else (x_0, k)
 
 __all__ = [gauss_newton, levenberg_marquardt]
```

### Comparing `optimtool-2.4.1/optimtool/unconstrain/trust_region.py` & `optimtool-2.4.2/optimtool/unconstrain/trust_region.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import numpy as np
 from .._utils import plot_iteration
 from .._convert import f2m, a2m, p2t, h2h
 
 from .._typing import FuncArray, ArgArray, PointArray, OutputType, DataType
 
 # 信赖域算法
-def steihaug_CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, m: float=100, r0: float=1, rmax: float=2, eta: float=0.2, p1: float=0.4, p2: float=0.6, gamma1: float=0.5, gamma2: float=1.5, epsilon: float=1e-6, k: int=0) -> OutputType:
+def steihaug_CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, r0: float=1, rmax: float=2, eta: float=0.2, p1: float=0.4, p2: float=0.6, gamma1: float=0.5, gamma2: float=1.5, epsilon: float=1e-6, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -40,17 +40,14 @@
         
     draw : bool
         绘图接口参数
         
     output_f : bool
         输出迭代函数值列表
         
-    m : float
-        海瑟矩阵条件数阈值
-        
     r0 : float
         搜索半径起点
         
     rmax : float
         搜索最大半径
         
     eta : float
@@ -88,38 +85,33 @@
     assert p2 < 1
     assert gamma1 < 1
     assert gamma2 > 1
     from .._drive import steihaug
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
     res = funcs.jacobian(args)
     hes = res.jacobian(args)
-    s0 = [0 for i in range(args.shape[0])]
-    f = []
+    s0, f = [0 for _ in range(args.shape[0])], []
     while 1:
         reps = dict(zip(args, x_0))
         funv = np.array(funcs.subs(reps)).astype(DataType)
         f.append(funv[0][0])
         grad = np.array(res.subs(reps)).astype(DataType)
         hessi = np.array(hes.subs(reps)).astype(DataType)
-        hessi = h2h(hessi, m)
+        hessi = h2h(hessi)
         dk, _ = steihaug(s0, grad, -grad, hessi, r0)
         if np.linalg.norm(dk) >= epsilon:
             funvk = np.array(funcs.subs(dict(zip(args, x_0 + dk[0])))).astype(DataType)
             pk = (funv - funvk) / -(grad.dot(dk.T) + 0.5*((dk.dot(hessi)).dot(dk.T)))
             if pk < p1:
                 r0 = gamma1 * r0
             else:
-                if (pk > p2) | (np.linalg.norm(dk) == r0):
+                if (pk > p2) or (np.linalg.norm(dk) == r0):
                     r0 = min(gamma2 * r0, rmax)
-                else:
-                    r0 = r0
             if pk > eta:
                 x_0 = x_0 + dk[0]
-            else:
-                x_0 = x_0
-            k = k + 1
+            k += 1
         else:
             break
     plot_iteration(f, draw, "trust_region_steihaug_CG")
     return (x_0, k, f) if output_f is True else (x_0, k)
 
 __all__ = [steihaug_CG]
```

### Comparing `optimtool-2.4.1/optimtool.egg-info/PKG-INFO` & `optimtool-2.4.2/optimtool.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimtool
-Version: 2.4.1
+Version: 2.4.2
 Summary: The fundamental package for scientific research in optimization.
 Home-page: https://github.com/linjing-lab/optimtool
 Download-URL: https://github.com/linjing-lab/optimtool/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: MIT
 Project-URL: Source, https://github.com/linjing-lab/optimtool/tree/master/optimtool/
@@ -13,14 +13,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
@@ -38,29 +39,45 @@
     </a>
     <a href='https://pepy.tech/project/optimtool'>
         <img src="https://pepy.tech/badge/optimtool" alt="Total Downloads" height="20"/>
     </a>
     <a href='https://pepy.tech/project/optimtool'>
         <img src="https://pepy.tech/badge/optimtool/month" alt="Monthly Downloads" height="20"/> 
     </a>
-    <a href='https://code.visualstudio.com/'>
+    <a href='https://pepy.tech/project/optimtool'>
         <img src="https://pepy.tech/badge/optimtool/week" alt="Weekly Downloads" height="20"/> 
     </a>
 </p>
 
 If you want to participate in the development, please follow the [baseline](./baseline.md).
 
 如果你想参与开发，请遵循[baseline](./baseline.md)。
 
 简体中文 | [English](./README_en.md)
 
 ## 项目介绍
 
 &emsp;&emsp;optimtool采用了北京大学出版的《最优化：建模、算法与理论》这本书中的部分理论方法框架，运用了 [`Numpy`](https://github.com/numpy/numpy) 包高效处理数组间运算等的特性，巧妙地应用了 [`Sympy`](https://github.com/sympy/sympy) 内部支持的 .jacobian 等方法，并结合 Python 内置函数 dict 与 zip 实现了 Sympy 矩阵到 Numpy 矩阵的转换，最终设计了一个用于最优化科学研究领域的Python工具包。 研究人员可以通过简单的 [`pip`](https://github.com/pypa/pip) 指令进行下载与使用。
 
+如果你在研究中使用 **optimtool**，欢迎引用它在你的参考资料中（按照下面的格式）。
+
+```text
+林景. optimtool: The fundamental package for scientific research in optimization. 2021. https://pypi.org/project/optimtool/.
+```
+
+下载最新版：
+```text
+git clone https://github.com/linjing-lab/optimtool.git
+cd optimtool
+pip install -e . --verbose
+```
+下载稳定版：
+```text
+pip install optimtool --upgrade
+```
 ## 项目结构
 
 ```textile
 |- optimtool
     |-- constrain
         |-- __init__.py
         |-- equal.py
@@ -87,15 +104,15 @@
     |-- _search.py
     |-- _typing.py
     |-- _utils.py
     |-- _version.py
 ```
 &emsp;&emsp;因为在求解不同的目标函数的全局或局部收敛点时，不同的求取收敛点的方法会有不同的收敛效率以及不同的适用范围，而且在研究过程中不同领域的研究方法被不断地提出、修改、完善、扩充，所以这些方法成了现在人们口中的`最优化方法`。 此项目中的所有内部支持的算法，都是在范数、导数、凸集、凸函数、共轭函数、次梯度和最优化理论等基础方法论的基础上进行设计与完善的。
 
-&emsp;&emsp;optimtool内置了诸如Barzilar Borwein非单调梯度下降法、修正牛顿法、有限内存BFGS方法、截断共轭梯度法-信赖域方法、高斯-牛顿法等无约束优化领域收敛效率与性质较好的算法，以及用于解决约束优化问题的二次罚函数法、增广拉格朗日法等算法。
+&emsp;&emsp;optimtool内置了诸如Barzilar Borwein非单调梯度下降法、修正牛顿法、有限内存BFGS方法、截断共轭梯度法-信赖域方法、高斯-牛顿法等无约束优化领域收敛效率与性质好的算法，以及用于解决约束优化问题的二次罚函数法、增广拉格朗日法等算法。
 
 ## 开始使用
 
 ### 无约束优化算法（unconstrain）
 
 ```python
 import optimtool.unconstrain as ou
@@ -110,58 +127,58 @@
 
 | 方法头                                                                                                                                 | 解释                                   |
 | ----------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
 | solve(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10, k: int=0) -> OutputType                                                             | 通过解方程的方式来求解精确步长                      |
 | steepest(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType                                           | 使用线搜索方法求解非精确步长（默认使用wolfe线搜索）         |
 | barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta: float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType | 使用Grippo与ZhangHanger提出的非单调线搜索方法更新步长 |
 
-#### 牛顿法（newton)
+#### 牛顿法（newton）
 
 ```python
 ou.newton.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
 | 方法头                                                                                             | 解释                                |
 | ----------------------------------------------------------------------------------------------- | --------------------------------- |
 | classic(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10, k: int=0) -> OutputType                        | 通过直接对目标函数二阶导矩阵（海瑟矩阵）进行求逆来获取下一步的步长 |
-| modified(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: int=20, epsilon: float=1e-10, k: int=0) -> OutputType | 修正当前海瑟矩阵保证其正定性（目前只接入了一种修正方法）      |
+| modified(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType | 修正当前海瑟矩阵保证其正定性（目前只接入了一种修正方法）      |
 | CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-6, k: int=0) -> OutputType              | 采用牛顿-共轭梯度法求解梯度（非精确牛顿法的一种）         |
 
 #### 拟牛顿法（newton_quasi）
 
 ```python
 ou.newton_quasi.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
 | 方法头                                                                                          | 解释              |
 | -------------------------------------------------------------------------------------------- | --------------- |
-| bfgs(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: float=20, epsilon: float=1e-10, k: int=0) -> OutputType  | BFGS方法更新海瑟矩阵    |
-| dfp(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: float=20, epsilon: float=1e-4, k: int=0) -> OutputType    | DFP方法更新海瑟矩阵     |
+| bfgs(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType  | BFGS方法更新海瑟矩阵    |
+| dfp(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-4, k: int=0) -> OutputType    | DFP方法更新海瑟矩阵     |
 | L_BFGS(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: float=6, epsilon: float=1e-10, k: int=0) -> OutputType | 双循环方法更新BFGS海瑟矩阵 |
 
 #### 非线性最小二乘法（nonlinear_least_square）
 
 ```python
 ou.nonlinear_least_square.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                  | 解释                         |
 | ---------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------- |
 | gauss_newton(funcr: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType                                                        | 高斯-牛顿提出的方法框架，包括OR分解等操作     |
-| levenberg_marquardt(funcr: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, m: float=100, lamk: float=1, eta: float=0.2, p1: float=0.4, p2: float=0.9, gamma1: float=0.7, gamma2: float=1.3, epsilon: float=1e-10, k: int=0) -> OutputType | Levenberg Marquardt提出的方法框架 |
+| levenberg_marquardt(funcr: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, lamk: float=1, eta: float=0.2, p1: float=0.4, p2: float=0.9, gamma1: float=0.7, gamma2: float=1.3, epsilon: float=1e-10, k: int=0) -> OutputType | Levenberg Marquardt提出的方法框架 |
 
 #### 信赖域方法（trust_region）
 
 ```python
 ou.trust_region.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                               | 解释                  |
 | ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------- |
-| steihaug_CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, m: float=100, r0: float=1, rmax: float=2, eta: float=0.2, p1: float=0.4, p2: float=0.6, gamma1: float=0.5, gamma2: float=1.5, epsilon: float=1e-6, k: int=0) -> OutputType | 截断共轭梯度法在此方法中被用于搜索步长 |
+| steihaug_CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, r0: float=1, rmax: float=2, eta: float=0.2, p1: float=0.4, p2: float=0.6, gamma1: float=0.5, gamma2: float=1.5, epsilon: float=1e-6, k: int=0) -> OutputType | 截断共轭梯度法在此方法中被用于搜索步长 |
 
 ### 约束优化算法（constrain）
 
 ```python
 import optimtool.constrain as oc
 oc.[方法名].[函数名]([目标函数], [参数表], [等式约束表], [不等式约数表], [初始迭代点])
 ```
@@ -170,40 +187,40 @@
 
 ```python
 oc.equal.[函数名]([目标函数], [参数表], [等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                   | 解释        |
 | ----------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
-| penalty_quadratice(funcs: FuncArray, args: FuncArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=10, p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType                     | 增加二次罚项    |
-| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadratice(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType                     | 增加二次罚项    |
+| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 #### 不等式约束（unequal）
 
 ```python
 oc.unequal.[函数名]([目标函数], [参数表], [不等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                                      | 解释        |
 | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------- |
-| penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=10, p: float=0.4, epsilon: float=1e-10, k: int=0) -> OutputType                                     | 增加二次罚项    |
-| penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k: int=0) -> OutputType                              | 增加分式函数罚项  |
-| lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.4, epsilon: float=1e-10, k: int=0) -> OutputType                                     | 增加二次罚项    |
+| penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k: int=0) -> OutputType                              | 增加分式函数罚项  |
+| lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 #### 混合等式约束（mixequal）
 
 ```python
 oc.mixequal.[函数名]([目标函数], [参数表], [等式约束表], [不等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                                                                  | 解释        |
 | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
-| penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=10, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                             | 增加二次罚项    |
-| penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", sigma: float=1, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                                     | L1精确罚函数法  |
-| lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="gradient_descent", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                             | 增加二次罚项    |
+| penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=1, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                                     | L1精确罚函数法  |
+| lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 ### 方法的应用（example）
 
 ```python
 import optimtool.example as oe
 ```
```

#### html2text {}

```diff
@@ -1,52 +1,58 @@
-Metadata-Version: 2.1 Name: optimtool Version: 2.4.1 Summary: The fundamental
+Metadata-Version: 2.1 Name: optimtool Version: 2.4.2 Summary: The fundamental
 package for scientific research in optimization. Home-page: https://github.com/
 linjing-lab/optimtool Download-URL: https://github.com/linjing-lab/optimtool/
 tags Author: ææ¯ Author-email: linjing010729@163.com License: MIT Project-
 URL: Source, https://github.com/linjing-lab/optimtool/tree/master/optimtool/
 Project-URL: Tracker, https://github.com/linjing-lab/optimtool/issues
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License Classifier: Topic ::
-Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
-Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Description-Content-Type: text/markdown License-
-File: LICENSE
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: MIT License Classifier: Topic :: Scientific/Engineering Classifier:
+Topic :: Scientific/Engineering :: Mathematics Classifier: Topic :: Software
+Development Classifier: Topic :: Software Development :: Libraries Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Description-
+Content-Type: text/markdown License-File: LICENSE
                             ****** optimtool ******
       The fundamental package for scientific research in optimization.[?]
     [OSCS_Status] [Total_Downloads] [Monthly_Downloads] [Weekly_Downloads]
 If you want to participate in the development, please follow the [baseline](./
 baseline.md). å¦æä½ æ³åä¸å¼åï¼è¯·éµå¾ª[baseline](./baseline.md)ã
 ç®ä½ä¸­æ | [English](./README_en.md) ## é¡¹ç®ä»ç»
 &emsp;&emsp;optimtooléç¨äºåäº¬å¤§å­¦åºççãæä¼åï¼å»ºæ¨¡ãç®æ³ä¸çè®ºãè¿æ¬ä¹¦ä¸­çé¨åçè®ºæ¹æ³æ¡æ¶ï¼è¿ç¨äº
 [`Numpy`](https://github.com/numpy/numpy)
 åé«æå¤çæ°ç»é´è¿ç®ç­çç¹æ§ï¼å·§å¦å°åºç¨äº [`Sympy`]
 (https://github.com/sympy/sympy) åé¨æ¯æç .jacobian
 ç­æ¹æ³ï¼å¹¶ç»å Python åç½®å½æ° dict ä¸ zip å®ç°äº Sympy
 ç©éµå° Numpy
 ç©éµçè½¬æ¢ï¼æç»è®¾è®¡äºä¸ä¸ªç¨äºæä¼åç§å­¦ç ç©¶é¢åçPythonå·¥å·åã
 ç ç©¶äººåå¯ä»¥éè¿ç®åç [`pip`](https://github.com/pypa/pip)
-æä»¤è¿è¡ä¸è½½ä¸ä½¿ç¨ã ## é¡¹ç®ç»æ ```textile |- optimtool |-
-- constrain |-- __init__.py |-- equal.py |-- mixequal.py |-- unequal.py |-
-- example |-- __init__.py |-- Lasso.py |-- WanYuan.py |-- hybrid |-
-- __init__.py |-- approximate_point_gradient.py |-- unconstrain |-- __init__.py
-|-- gradient_descent.py |-- newton.py |-- newton_quasi.py |-
+æä»¤è¿è¡ä¸è½½ä¸ä½¿ç¨ã å¦æä½ å¨ç ç©¶ä¸­ä½¿ç¨
+**optimtool**ï¼æ¬¢è¿å¼ç¨å®å¨ä½ çåèèµæä¸­ï¼æç§ä¸é¢çæ ¼å¼ï¼ã
+```text ææ¯. optimtool: The fundamental package for scientific research in
+optimization. 2021. https://pypi.org/project/optimtool/. ``` ä¸è½½ææ°çï¼
+```text git clone https://github.com/linjing-lab/optimtool.git cd optimtool pip
+install -e . --verbose ``` ä¸è½½ç¨³å®çï¼ ```text pip install optimtool --
+upgrade ``` ## é¡¹ç®ç»æ ```textile |- optimtool |-- constrain |-
+- __init__.py |-- equal.py |-- mixequal.py |-- unequal.py |-- example |-
+- __init__.py |-- Lasso.py |-- WanYuan.py |-- hybrid |-- __init__.py |-
+- approximate_point_gradient.py |-- unconstrain |-- __init__.py |-
+- gradient_descent.py |-- newton.py |-- newton_quasi.py |-
 - nonlinear_least_square.py |-- trust_region.py |-- __init__.py |-- _convert.py
 |-- _drive.py |-- _kernel.py |-- _search.py |-- _typing.py |-- _utils.py |-
 - _version.py ```
 &emsp;&emsp;å ä¸ºå¨æ±è§£ä¸åçç®æ å½æ°çå¨å±æå±é¨æ¶æç¹æ¶ï¼ä¸åçæ±åæ¶æç¹çæ¹æ³ä¼æä¸åçæ¶ææçä»¥åä¸åçéç¨èå´ï¼èä¸å¨ç ç©¶è¿ç¨ä¸­ä¸åé¢åçç ç©¶æ¹æ³è¢«ä¸æ­å°æåºãä¿®æ¹ãå®åãæ©åï¼æä»¥è¿äºæ¹æ³æäºç°å¨äººä»¬å£ä¸­ç`æä¼åæ¹æ³`ã
 æ­¤é¡¹ç®ä¸­çææåé¨æ¯æçç®æ³ï¼é½æ¯å¨èæ°ãå¯¼æ°ãå¸éãå¸å½æ°ãå±è½­å½æ°ãæ¬¡æ¢¯åº¦åæä¼åçè®ºç­åºç¡æ¹æ³è®ºçåºç¡ä¸è¿è¡è®¾è®¡ä¸å®åçã
 &emsp;&emsp;optimtoolåç½®äºè¯¸å¦Barzilar
 Borweinéåè°æ¢¯åº¦ä¸éæ³ãä¿®æ­£çé¡¿æ³ãæéåå­BFGSæ¹æ³ãæªæ­å±è½­æ¢¯åº¦æ³-
 ä¿¡èµåæ¹æ³ãé«æ¯-
-çé¡¿æ³ç­æ çº¦æä¼åé¢åæ¶ææçä¸æ§è´¨è¾å¥½çç®æ³ï¼ä»¥åç¨äºè§£å³çº¦æä¼åé®é¢çäºæ¬¡ç½å½æ°æ³ãå¢å¹¿ææ ¼ææ¥æ³ç­ç®æ³ã
+çé¡¿æ³ç­æ çº¦æä¼åé¢åæ¶ææçä¸æ§è´¨å¥½çç®æ³ï¼ä»¥åç¨äºè§£å³çº¦æä¼åé®é¢çäºæ¬¡ç½å½æ°æ³ãå¢å¹¿ææ ¼ææ¥æ³ç­ç®æ³ã
 ## å¼å§ä½¿ç¨ ### æ çº¦æä¼åç®æ³ï¼unconstrainï¼ ```python import
 optimtool.unconstrain as ou ou.[æ¹æ³å].[å½æ°å]([ç®æ å½æ°],
 [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` #### æ¢¯åº¦ä¸éæ³ï¼gradient_descentï¼
 ```python ou.gradient_descent.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 --------------------- | ------------------------------------ | | solve(funcs:
@@ -56,112 +62,110 @@
 args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method:
 str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType |
 ä½¿ç¨çº¿æç´¢æ¹æ³æ±è§£éç²¾ç¡®æ­¥é¿ï¼é»è®¤ä½¿ç¨wolfeçº¿æç´¢ï¼ | |
 barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw:
 bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta:
 float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType |
 ä½¿ç¨Grippoä¸ZhangHangeræåºçéåè°çº¿æç´¢æ¹æ³æ´æ°æ­¥é¿ | ####
-çé¡¿æ³ï¼newton) ```python ou.newton.[å½æ°å]([ç®æ å½æ°],
+çé¡¿æ³ï¼newtonï¼ ```python ou.newton.[å½æ°å]([ç®æ å½æ°],
 [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | ------------------
 ----------------------------------------------------------------------------- |
 --------------------------------- | | classic(funcs: FuncArray, args: ArgArray,
 x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10,
 k: int=0) -> OutputType |
 éè¿ç´æ¥å¯¹ç®æ å½æ°äºé¶å¯¼ç©éµï¼æµ·çç©éµï¼è¿è¡æ±éæ¥è·åä¸ä¸æ­¥çæ­¥é¿
 | | modified(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw:
-bool=True, output_f: bool=False, method: str="wolfe", m: int=20, epsilon:
-float=1e-10, k: int=0) -> OutputType |
+bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k:
+int=0) -> OutputType |
 ä¿®æ­£å½åæµ·çç©éµä¿è¯å¶æ­£å®æ§ï¼ç®ååªæ¥å¥äºä¸ç§ä¿®æ­£æ¹æ³ï¼
 | | CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True,
 output_f: bool=False, method: str="wolfe", epsilon: float=1e-6, k: int=0) -
 > OutputType | éç¨çé¡¿-
 å±è½­æ¢¯åº¦æ³æ±è§£æ¢¯åº¦ï¼éç²¾ç¡®çé¡¿æ³çä¸ç§ï¼ | ####
 æçé¡¿æ³ï¼newton_quasiï¼ ```python ou.newton_quasi.[å½æ°å](
 [ç®æ å½æ°], [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | --
 -------------------------------------------------------------------------------
 ----------- | --------------- | | bfgs(funcs: FuncArray, args: ArgArray, x_0:
-PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m:
-float=20, epsilon: float=1e-10, k: int=0) -> OutputType |
-BFGSæ¹æ³æ´æ°æµ·çç©éµ | | dfp(funcs: FuncArray, args: ArgArray, x_0:
-PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m:
-float=20, epsilon: float=1e-4, k: int=0) -> OutputType |
-DFPæ¹æ³æ´æ°æµ·çç©éµ | | L_BFGS(funcs: FuncArray, args: ArgArray, x_0:
-PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m:
-float=6, epsilon: float=1e-10, k: int=0) -> OutputType |
+PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe",
+epsilon: float=1e-10, k: int=0) -> OutputType | BFGSæ¹æ³æ´æ°æµ·çç©éµ |
+| dfp(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True,
+output_f: bool=False, method: str="wolfe", epsilon: float=1e-4, k: int=0) -
+> OutputType | DFPæ¹æ³æ´æ°æµ·çç©éµ | | L_BFGS(funcs: FuncArray, args:
+ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method:
+str="wolfe", m: float=6, epsilon: float=1e-10, k: int=0) -> OutputType |
 åå¾ªç¯æ¹æ³æ´æ°BFGSæµ·çç©éµ | ####
 éçº¿æ§æå°äºä¹æ³ï¼nonlinear_least_squareï¼ ```python
 ou.nonlinear_least_square.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------- | -------------------------- | |
 gauss_newton(funcr: FuncArray, args: ArgArray, x_0: PointArray, draw:
 bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k:
 int=0) -> OutputType | é«æ¯-
 çé¡¿æåºçæ¹æ³æ¡æ¶ï¼åæ¬ORåè§£ç­æä½ | | levenberg_marquardt
 (funcr: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, m: float=100, lamk: float=1, eta: float=0.2, p1: float=0.4, p2:
-float=0.9, gamma1: float=0.7, gamma2: float=1.3, epsilon: float=1e-10, k:
-int=0) -> OutputType | Levenberg Marquardtæåºçæ¹æ³æ¡æ¶ | ####
+bool=False, lamk: float=1, eta: float=0.2, p1: float=0.4, p2: float=0.9,
+gamma1: float=0.7, gamma2: float=1.3, epsilon: float=1e-10, k: int=0) -
+> OutputType | Levenberg Marquardtæåºçæ¹æ³æ¡æ¶ | ####
 ä¿¡èµåæ¹æ³ï¼trust_regionï¼ ```python ou.trust_region.[å½æ°å](
 [ç®æ å½æ°], [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | --
 -------------------------------------------------------------------------------
 ---------------------------------------------------------------- | ------------
 ------- | | steihaug_CG(funcs: FuncArray, args: ArgArray, x_0: PointArray,
-draw: bool=True, output_f: bool=False, m: float=100, r0: float=1, rmax:
-float=2, eta: float=0.2, p1: float=0.4, p2: float=0.6, gamma1: float=0.5,
-gamma2: float=1.5, epsilon: float=1e-6, k: int=0) -> OutputType |
+draw: bool=True, output_f: bool=False, r0: float=1, rmax: float=2, eta:
+float=0.2, p1: float=0.4, p2: float=0.6, gamma1: float=0.5, gamma2: float=1.5,
+epsilon: float=1e-6, k: int=0) -> OutputType |
 æªæ­å±è½­æ¢¯åº¦æ³å¨æ­¤æ¹æ³ä¸­è¢«ç¨äºæç´¢æ­¥é¿ | ###
 çº¦æä¼åç®æ³ï¼constrainï¼ ```python import optimtool.constrain as oc
 oc.[æ¹æ³å].[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨],
 [ä¸ç­å¼çº¦æ°è¡¨], [åå§è¿­ä»£ç¹]) ``` #### ç­å¼çº¦æï¼equalï¼
 ```python oc.equal.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------- | --------- | | penalty_quadratice
-(funcs: FuncArray, args: FuncArray, cons: FuncArray, x_0: PointArray, draw:
-bool=True, output_f: bool=False, method: str="gradient_descent", sigma:
-float=10, p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType |
-å¢å äºæ¬¡ç½é¡¹ | | lagrange_augmentede(funcs: FuncArray, args: ArgArray,
-cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False,
-method: str="gradient_descent", lamk: float=6, sigma: float=10, p: float=2,
-etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType |
-å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | #### ä¸ç­å¼çº¦æï¼unequalï¼ ```python
-oc.unequal.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ä¸ç­å¼çº¦æè¡¨],
-[åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
+(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw:
+bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10,
+p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType | å¢å äºæ¬¡ç½é¡¹ |
+| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0:
+PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region",
+lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon:
+float=1e-6, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | ####
+ä¸ç­å¼çº¦æï¼unequalï¼ ```python oc.unequal.[å½æ°å]([ç®æ å½æ°],
+[åæ°è¡¨], [ä¸ç­å¼çº¦æè¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é
+| | ---------------------------------------------------------------------------
 -------------------------------------------------------------------------------
----------------------------------------------------------- | --------- | |
-penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0:
-PointArray, draw: bool=True, output_f: bool=False, method:
-str="gradient_descent", sigma: float=10, p: float=0.4, epsilon: float=1e-10, k:
-int=0) -> OutputType | å¢å äºæ¬¡ç½é¡¹ | | penalty_interior_fraction(funcs:
-FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True,
-output_f: bool=False, method: str="gradient_descent", sigma: float=12, p:
-float=0.6, epsilon: float=1e-6, k: int=0) -> OutputType |
-å¢å åå¼å½æ°ç½é¡¹ | | lagrange_augmentedu(funcs: FuncArray, args:
+-------------- | --------- | | penalty_quadraticu(funcs: FuncArray, args:
 ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="gradient_descent", muk: float=10, sigma: float=8,
-alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon:
-float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | ####
-æ··åç­å¼çº¦æï¼mixequalï¼ ```python oc.mixequal.[å½æ°å](
+bool=False, method: str="trust_region", sigma: float=10, p: float=0.4, epsilon:
+float=1e-10, k: int=0) -> OutputType | å¢å äºæ¬¡ç½é¡¹ | |
+penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray,
+x_0: PointArray, draw: bool=True, output_f: bool=False, method:
+str="trust_region", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k:
+int=0) -> OutputType | å¢å åå¼å½æ°ç½é¡¹ | | lagrange_augmentedu(funcs:
+FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True,
+output_f: bool=False, method: str="trust_region", muk: float=10, sigma:
+float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1,
+epsilon: float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ |
+#### æ··åç­å¼çº¦æï¼mixequalï¼ ```python oc.mixequal.[å½æ°å](
 [ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨], [ä¸ç­å¼çº¦æè¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 ------- | --------- | | penalty_quadraticm(funcs: FuncArray, args: ArgArray,
 cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw:
-bool=True, output_f: bool=False, method: str="gradient_descent", sigma:
-float=10, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType |
+bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10,
+p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType |
 å¢å äºæ¬¡ç½é¡¹ | | penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal:
 FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="gradient_descent", sigma: float=1, p: float=0.6,
-epsilon: float=1e-10, k: int=0) -> OutputType | L1ç²¾ç¡®ç½å½æ°æ³ | |
+bool=False, method: str="trust_region", sigma: float=1, p: float=0.6, epsilon:
+float=1e-10, k: int=0) -> OutputType | L1ç²¾ç¡®ç½å½æ°æ³ | |
 lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray,
 cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="gradient_descent", lamk: float=6, muk: float=10,
-sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3,
+bool=False, method: str="trust_region", lamk: float=6, muk: float=10, sigma:
+float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3,
 epsilon: float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ |
 ### æ¹æ³çåºç¨ï¼exampleï¼ ```python import optimtool.example as oe ```
 #### Lassoé®é¢ï¼Lassoï¼ ```python oe.Lasso.[å½æ°å]([ç©éµA],
 [ç©éµb], [å å­mu], [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é
 | | ---------------------------------------------------------------------------
 ---------------------------- | ---------------- | | gradient(A: NDArray, b:
 NDArray, mu: float, args: ArgArray, x_0: PointArray, draw: bool=True, output_f:
```

### Comparing `optimtool-2.4.1/optimtool.egg-info/SOURCES.txt` & `optimtool-2.4.2/optimtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.1/setup.py` & `optimtool-2.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,20 +65,22 @@
             'Intended Audience :: Developers',
             'Intended Audience :: Education',
             'Intended Audience :: Science/Research',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
             'License :: OSI Approved :: MIT License',
             'Topic :: Scientific/Engineering',
             'Topic :: Scientific/Engineering :: Mathematics',
             'Topic :: Software Development',
             'Topic :: Software Development :: Libraries',
             'Topic :: Software Development :: Libraries :: Python Modules',
       ],
       install_requires = [
-            'numpy>=1.18.5', 
+            'numpy>=1.21.0', 
             'sympy>=1.9',
             'matplotlib>=3.2.0'
       ],
+      # extras_require = []
 )
```

