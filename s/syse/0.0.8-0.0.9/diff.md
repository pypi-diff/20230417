# Comparing `tmp/syse-0.0.8.tar.gz` & `tmp/syse-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syse-0.0.8.tar", last modified: Thu Mar 23 23:35:27 2023, max compression
+gzip compressed data, was "syse-0.0.9.tar", last modified: Mon Apr 17 18:15:40 2023, max compression
```

## Comparing `syse-0.0.8.tar` & `syse-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 23:35:27.866953 syse-0.0.8/
--rw-rw-rw-   0        0        0     1098 2023-03-20 01:15:09.000000 syse-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2760 2023-03-23 23:35:27.865953 syse-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      810 2023-03-23 23:34:07.000000 syse-0.0.8/README.md
--rw-rw-rw-   0        0        0      751 2023-03-23 23:32:07.000000 syse-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-23 23:35:27.866953 syse-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1076 2023-03-23 23:32:07.000000 syse-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-23 23:35:27.850252 syse-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-03-23 23:35:27.857890 syse-0.0.8/src/syse/
--rw-rw-rw-   0        0        0       47 2023-03-20 22:23:59.000000 syse-0.0.8/src/syse/__init__.py
--rw-rw-rw-   0        0        0    49011 2023-03-23 23:24:23.000000 syse-0.0.8/src/syse/_syse.py
-drwxrwxrwx   0        0        0        0 2023-03-23 23:35:27.864953 syse-0.0.8/src/syse.egg-info/
--rw-rw-rw-   0        0        0     2760 2023-03-23 23:35:27.000000 syse-0.0.8/src/syse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-03-23 23:35:27.000000 syse-0.0.8/src/syse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 23:35:27.000000 syse-0.0.8/src/syse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-03-23 23:35:27.000000 syse-0.0.8/src/syse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-23 23:35:27.000000 syse-0.0.8/src/syse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 18:15:40.476316 syse-0.0.9/
+-rw-rw-rw-   0        0        0     1098 2023-03-20 01:15:09.000000 syse-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3006 2023-04-17 18:15:40.475316 syse-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1056 2023-04-17 16:57:47.000000 syse-0.0.9/README.md
+-rw-rw-rw-   0        0        0      751 2023-04-17 16:58:23.000000 syse-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 18:15:40.476316 syse-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1076 2023-04-17 16:58:23.000000 syse-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:15:40.460905 syse-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 18:15:40.468317 syse-0.0.9/src/syse/
+-rw-rw-rw-   0        0        0       47 2023-03-20 22:23:59.000000 syse-0.0.9/src/syse/__init__.py
+-rw-rw-rw-   0        0        0    49035 2023-04-17 18:08:26.000000 syse-0.0.9/src/syse/_syse.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:15:40.474316 syse-0.0.9/src/syse.egg-info/
+-rw-rw-rw-   0        0        0     3006 2023-04-17 18:15:40.000000 syse-0.0.9/src/syse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-04-17 18:15:40.000000 syse-0.0.9/src/syse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 18:15:40.000000 syse-0.0.9/src/syse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-17 18:15:40.000000 syse-0.0.9/src/syse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-17 18:15:40.000000 syse-0.0.9/src/syse.egg-info/top_level.txt
```

### Comparing `syse-0.0.8/LICENSE` & `syse-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `syse-0.0.8/PKG-INFO` & `syse-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syse
-Version: 0.0.8
+Version: 0.0.9
 Summary: Systems & Industrial Engineering Python Package
 Home-page: https://github.com/apexpromgt/SysE
 Author: Jonathon Nicholson
 Author-email: Jonathon Nicholson <Jonathon@apexpromgt.com>
 License: MIT License
         
         Copyright (c) [2023] [Jonathon Nicholson]
@@ -37,28 +37,28 @@
 License-File: LICENSE
 
 # Welcome to the SysE Python Package!
 
 [![Documentation Status](https://readthedocs.org/projects/syse/badge/?version=latest)](https://syse.readthedocs.io/en/latest/?badge=latest)
 
 
-SysE (/Sis'y/) is a Python library for Systems Engineering.
+SysE is a Python library for Industrial and Systems Engineering.
 
 SysE covers common Industrial & Systems Engineering topics such as:
 * Engineering Economics 
 * Probability & Statistics
 * Modeling & Quantitative Analysis
 * Engineering Management
 
-Some use cases include:
-*
-*
 
 To get started, check out the docs for further information, including how to install SysE and common use cases.
 
 **Links:**
 * **Documentation:** [SysE Docs](https://syse.readthedocs.io/en/latest/)
 * **Repository:** [SysE Repo](https://github.com/Apex-Engineering-Management/SysE)
 
-**Note:**
+**Notes:**
 
-This project is under active development.
+* This project is being worked on, but I am very busy. 
+* The declining depreciation functions will be fixed.
+* The linear optimization function is extremely limited, and will be worked on.
+* For the few functions that can't be called with scalars, arrays, or other sequences, there are plans to update them.
```

### Comparing `syse-0.0.8/README.md` & `syse-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Welcome to the SysE Python Package!
 
 [![Documentation Status](https://readthedocs.org/projects/syse/badge/?version=latest)](https://syse.readthedocs.io/en/latest/?badge=latest)
 
 
-SysE (/Sis'y/) is a Python library for Systems Engineering.
+SysE is a Python library for Industrial and Systems Engineering.
 
 SysE covers common Industrial & Systems Engineering topics such as:
 * Engineering Economics 
 * Probability & Statistics
 * Modeling & Quantitative Analysis
 * Engineering Management
 
-Some use cases include:
-*
-*
 
 To get started, check out the docs for further information, including how to install SysE and common use cases.
 
 **Links:**
 * **Documentation:** [SysE Docs](https://syse.readthedocs.io/en/latest/)
 * **Repository:** [SysE Repo](https://github.com/Apex-Engineering-Management/SysE)
 
-**Note:**
+**Notes:**
 
-This project is under active development.
+* This project is being worked on, but I am very busy. 
+* The declining depreciation functions will be fixed.
+* The linear optimization function is extremely limited, and will be worked on.
+* For the few functions that can't be called with scalars, arrays, or other sequences, there are plans to update them.
```

### Comparing `syse-0.0.8/pyproject.toml` & `syse-0.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "syse"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Jonathon Nicholson", email="Jonathon@apexpromgt.com" },
 ]
 description = "Systems & Industrial Engineering Python Package"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `syse-0.0.8/setup.py` & `syse-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "syse",
-    version = "0.0.8",
+    version = "0.0.9",
     author = "Jonathon Nicholson",
     author_email = "Jonathon@apexpromgt.com",
     description = "Systems & Industrial Engineering Python Package",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/apexpromgt/SysE",
     project_urls = {
```

### Comparing `syse-0.0.8/src/syse/_syse.py` & `syse-0.0.9/src/syse/_syse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-"""Some simple financial calculations
-patterned after spreadsheet computations.
-There is some complexity in each function
-so that the functions behave like ufuncs with
+"""Systems & Industrial Engineering functions
+
+functions behave like ufuncs with
 broadcasting and being able to be called with scalars
 or arrays (or other sequences).
+
 Functions support the :class:`decimal.Decimal` type unless
 otherwise stated.
 """
 from __future__ import division, absolute_import, print_function
 
 from decimal import Decimal
 
@@ -43,41 +43,49 @@
 
 
 # Future Value (FV)
 
 def fv(rate, nper, pmt, pv, when='end'):
     """
     Compute the future value.
+
     Given:
      * a present value, `pv`
      * an interest `rate` compounded once per period, of which
        there are
      * `nper` total
      * a (fixed) payment, `pmt`, paid either
      * at the beginning (`when` = {'begin', 1}) or the end
        (`when` = {'end', 0}) of each period
     Return:
        the value at the end of the `nper` periods
+
     Parameters:
         rate (scalar or array_like of shape(M, )): Rate of interest as decimal (not per cent) per period
         nper (scalar or array_like of shape(M, )): Number of compounding periods
         pmt (scalar or array_like of shape(M, )): Payment
         pv (scalar or array_like of shape(M, )): Present value
         when ({{'begin', 1}, {'end', 0}}, {string, int}, optional): When payments are due ('begin' (1) or 'end' (0)).
             Defaults to {'end', 0}.
+
     Returns:
         ndarray: Future values. If all input is scalar, returns a scalar float. If any input is array_like, returns
         future values for each input element. If multiple inputs are array_like, they all must have the same shape.
+
+
     .. Note::
-        The future value is computed by solving the equation::
-            fv +
-            pv*(1+rate)**nper +
-            pmt*(1 + rate*when)/rate*((1 + rate)**nper - 1) == 0
-        or, when ``rate == 0``::
-            fv + pv + pmt * nper == 0
+           The future value is computed by solving the equation::
+                      fv +
+                      pv*(1+rate)**nper +
+                      pmt*(1 + rate*when)/rate*((1 + rate)**nper - 1) == 0
+           or, when ``rate == 0``::
+                      fv + pv + pmt * nper == 0
+
+
+
     Examples:
     ---------
     What is the future value after 10 years of saving $100 now, with
     an additional monthly savings of $100.  Assume the interest rate is
     5% (annually) compounded monthly?
     ::
         import numpy as np
@@ -118,50 +126,55 @@
 
 
 # Payment Against Loan Principal Plus Interest
 
 def pmt(rate, nper, pv, fv=0, when='end'):
     """
     Compute the payment against loan principal plus interest.
+
     Given:
      * a present value, `pv` (e.g., an amount borrowed)
      * a future value, `fv` (e.g., 0)
      * an interest `rate` compounded once per period, of which
        there are
      * `nper` total
      * and (optional) specification of whether payment is made
        at the beginning (`when` = {'begin', 1}) or the end
        (`when` = {'end', 0}) of each period
     Return:
        the (fixed) periodic payment.
+
     Parameters:
         rate (array_like): Rate of interest (per period)
         nper (array_like): Number of compounding periods
         pv (array_like): Present value
         fv (array_like, optional): Future value (default = 0)
         when ({{'begin', 1}, {'end', 0}}, {string, int}): When payments are due ('begin' (1) or 'end' (0))
+
     Returns:
     --------
         ndarray: Payment against loan plus interest. If all input is scalar, returns a scalar float. If any input is
         array_like, returns payment for each input element. If multiple inputs are array_like, they all must have
         the same shape.
+
     .. Note::
         The payment is computed by solving the equation::
             fv +
             pv*(1 + rate)**nper +
             pmt*(1 + rate*when)/rate*((1 + rate)**nper - 1) == 0
         or, when ``rate == 0``::
             fv + pv + pmt * nper == 0
         for ``pmt``.
         Note that computing a monthly mortgage payment is only
         one use for this function.  For example, pmt returns the
         periodic deposit one must make to achieve a specified
         future balance given an initial deposit, a fixed,
         periodically compounded interest rate, and the total
         number of periods.
+
     Examples:
     ---------
     What is the monthly payment needed to pay off a $200,000 loan in 15
     years at an annual interest rate of 7.5%?
     ::
         import syse as syse
         syse.pmt(0.075/12, 12*15, 200000)
@@ -181,26 +194,30 @@
 
 
 # Number of Periodic Payments
 
 def nper(rate, pmt, pv, fv=0, when='end'):
     """
     Compute the number of periodic payments.
+
     :class:`decimal.Decimal` type is not supported.
+
     Parameters:
         rate (array_like): Rate of interest (per period)
         pmt (array_like): Payment
         pv (array_like): Present value
         fv (array_like, optional): Future value
         when ({{'begin', 1}, {'end', 0}}, {string, int}, optional): When payments are due ('begin' (1) or 'end' (0))
+
     .. Note::
         The number of periods ``nper`` is computed by solving the equation::
             fv + pv*(1+rate)**nper + pmt*(1+rate*when)/rate*((1+rate)**nper-1) = 0
         but if ``rate = 0`` then::
             fv + pv + pmt*nper = 0
+
     Examples:
     ---------
     If you only had $150/month to pay towards the loan, how long would it take
     to pay-off a loan of $8,000 at 7% annual interest?
     ::
         import numpy as np
         import syse as syse
@@ -248,71 +265,80 @@
 
 
 # Interest Portion of Payment
 
 def ipmt(rate, per, nper, pv, fv=0, when='end'):
     """
     Compute the interest portion of a payment.
+
     Parameters:
         rate (scalar or array_like of shape(M, )): Rate of interest as decimal (not per cent) per period
         per (scalar or array_like of shape(M, )): Interest paid against the loan changes during the life or the loan.
             The `per` is the payment period to calculate the interest amount.
         nper (scalar or array_like of shape(M, )): Number of compounding periods
         pv (scalar or array_like of shape(M, )): Present value
         fv (scalar or array_like of shape(M, ), optional): Future value
         when ({{'begin', 1}, {'end', 0}}, {string, int}, optional): When payments are due ('begin' (1) or 'end' (0)).
             Defaults to {'end', 0}.
+
     Returns:
         ndarray: Interest portion of payment. If all input is scalar, returns a scalar float. If any input is
         array_like, returns interest payment for each input element. If multiple inputs are array_like,
         they all must have the same shape.
+
+
     See Also
     --------
     ppmt, pmt, pv
+
+
+
+
     .. Note::
         The total payment is made up of payment against principal plus interest.
         ``pmt = ppmt + ipmt``
+
+
+
     Examples:
     ---------
     What is the amortization schedule for a 1 year loan of $2500 at
     8.24% interest per year compounded monthly?
     ::
         import numpy as np
         import syse as syse
         principal = 2500.00
-    The 'per' variable represents the periods of the loan.  Remember that
-    financial equations start the period count at 1!
+    The 'per' variable represents the periods of the loan. Remember that financial equations start the period count at 1!
     ::
         per = np.arange(1*12) + 1
         ipmt = syse.ipmt(0.0824/12, per, 1*12, principal)
         ppmt = syse.ppmt(0.0824/12, per, 1*12, principal)
-    Each element of the sum of the 'ipmt' and 'ppmt' arrays should equal
-    'pmt'.
+    Each element of the sum of the 'ipmt' and 'ppmt' arrays should equal 'pmt'.
     ::
         pmt = syse.pmt(0.0824/12, 1*12, principal)
         np.allclose(ipmt + ppmt, pmt)
         True
     ::
         fmt = '{0:2d} {1:8.2f} {2:8.2f} {3:8.2f}'
         for payment in per:
-            index = payment - 1
-            principal = principal + ppmt[index]
-            print(fmt.format(payment, ppmt[index], ipmt[index], principal))
-            1  -200.58   -17.17  2299.42
-            2  -201.96   -15.79  2097.46
-            3  -203.35   -14.40  1894.11
-            4  -204.74   -13.01  1689.37
-            5  -206.15   -11.60  1483.22
-            6  -207.56   -10.18  1275.66
-            7  -208.99    -8.76  1066.67
-            8  -210.42    -7.32   856.25
-            9  -211.87    -5.88   644.38
-            10  -213.32    -4.42   431.05
-            11  -214.79    -2.96   216.26
-            12  -216.26    -1.49    -0.00
+        index = payment - 1
+        principal = principal + ppmt[index]
+        print(fmt.format(payment, ppmt[index], ipmt[index], principal))
+        1  -200.58   -17.17  2299.42
+        2  -201.96   -15.79  2097.46
+        3  -203.35   -14.40  1894.11
+        4  -204.74   -13.01  1689.37
+        5  -206.15   -11.60  1483.22
+        6  -207.56   -10.18  1275.66
+        7  -208.99    -8.76  1066.67
+        8  -210.42    -7.32   856.25
+        9  -211.87    -5.88   644.38
+        10  -213.32    -4.42   431.05
+        11  -214.79    -2.96   216.26
+        12  -216.26    -1.49    -0.00
         interestpd = np.sum(ipmt)
         np.round(interestpd, 2)
         -112.98
     """
     when = _convert_when(when)
     rate, per, nper, pv, fv, when = np.broadcast_arrays(rate, per, nper,
                                                         pv, fv, when)
@@ -351,14 +377,15 @@
 
 
 # Payment Against Loan Principal
 
 def ppmt(rate, per, nper, pv, fv=0, when='end'):
     """
     Compute the payment against loan principal.
+
     Parameters:
         rate (array_like): Rate of interest (per period)
         per (array_like, int): Amount paid against the loan changes. The `per` is the period of interest.
         nper (array_like): Number of compounding periods
         pv (array_like): Present value
         fv (array_like, optional): Future value
         when ({{'begin', 1}, {'end', 0}}, {string, int}): When payments are due ('begin' (1) or 'end' (0))
@@ -371,38 +398,44 @@
 
 
 # Present Value
 
 def pv(rate, nper, pmt, fv=0, when='end'):
     """
     Compute the present value.
+
     Given:
      * a future value, `fv`
      * an interest `rate` compounded once per period, of which
        there are
      * `nper` total
      * a (fixed) payment, `pmt`, paid either
      * at the beginning (`when` = {'begin', 1}) or the end
        (`when` = {'end', 0}) of each period
+
     Return:
        the value now
+
     Parameters:
         rate (array_like): Rate of interest (per period)
         nper (array_like): Number of compounding periods
         pmt (array_like): Payment
         fv (array_like, optional): Future value
         when ({{'begin', 1}, {'end', 0}}, {string, int}, optional): When payments are due ('begin' (1) or 'end' (0))
+
     Returns:
         ndarray, float: Present value of a series of payments or investments.
+
     .. Note::
         The present value is computed by solving the equation::
             fv + pv*(1 + rate)**nper + pmt*(1 + rate*when)/rate*((1 + rate)**nper - 1) = 0
         or, when ``rate = 0``::
             fv + pv + pmt * nper = 0
         for `pv`, which is then returned.
+
     Examples:
     ---------
     What is the present value (e.g., the initial investment)
     of an investment that needs to total $15692.93
     after 10 years of saving $100 every month?  Assume the
     interest rate is 5% (annually) compounded monthly::
         import numpy as np
@@ -456,23 +489,25 @@
 
 
 # Rate of Interest
 
 def rate(nper, pmt, pv, fv, when='end', guess=None, tol=None, maxiter=100):
     """
     Compute the rate of interest per period.
+
     Parameters:
         nper (array_like): Number of compounding periods
         pmt (array_like): Payment
         pv (array_like): Present value
         fv (array_like): Future value
         when ({{'begin', 1}, {'end', 0}}, {string, int}, optional): When payments are due ('begin' (1) or 'end' (0))
         guess (Number, optional): Starting guess for solving the rate of interest, default 0.1
         tol (Number, optional): Required tolerance for the solution, default 1e-6
         maxiter (int, optional): Maximum iterations in finding the solution
+
     .. Note::
         The rate of interest is computed by iteratively solving the
         (non-linear) equation::
             fv + pv*(1+rate)**nper + pmt*(1+rate*when)/rate * ((1+rate)**nper - 1) = 0
         for ``rate``.
     """
     when = _convert_when(when)
@@ -512,25 +547,29 @@
 
 def irr(values, guess=0.1, tol=1e-12, maxiter=100):
     """
     Return the Internal Rate of Return (IRR).
     This is the "average" periodically compounded rate of return
     that gives a net present value of 0.0; for a more complete explanation,
     see Notes below.
+
     :class:`decimal.Decimal` type is not supported.
+
     Parameters:
         values (array_like, shape(N,)): Input cash flows per time period. By convention, net "deposits" are negative
             and net "withdrawals" are positive. Thus, for example, at least the first element of `values`, which
             represents the initial investment, will typically be negative.
         guess (float, optional): Initial guess of the IRR for the iterative solver. If no guess is given an initial
             guess of 0.1 (i.e. 10%) is assumed instead.
         tol (float, optional): Required tolerance to accept solution. Default is 1e-12.
         maxiter (int, optional): Maximum iterations to perform in finding a solution. Default is 100.
+
     Returns:
         float: Internal Rate of Return for periodic input values.
+
     .. Note::
         The IRR is perhaps best understood through an example (illustrated
         using np.irr in the Examples section below). Suppose one invests 100
         units and then makes the following withdrawals at regular (fixed)
         intervals: 39, 59, 55, 20.  Assuming the ending value is 0, one's 100
         unit investment yields 173 units; however, due to the combination of
         compounding and the periodic withdrawals, the "average" rate of return
@@ -540,14 +579,15 @@
         -100 + \\frac{39}{1+r} + \\frac{59}{(1+r)^2} + \\frac{55}{(1+r)^3} + \\frac{20}{(1+r)^4} = 0
     .. code::
        -100 + (39/1+r) = 0
     In general, for `values` :math:`= [v_0, v_1, ... v_M]`,
     irr is the solution of the equation: [G]_
     .. math::
         \\sum_{t=0}^M{\\frac{v_t}{(1+irr)^{t}}} = 0
+
     Examples:
     ---------
     ::
         import syse as syse
         round(syse.irr([-100, 39, 59, 55, 20]), 5)
         0.28095
         round(syse.irr([-100, 0, 0, 74]), 5)
@@ -596,35 +636,40 @@
 
 
 # Net Present Value (NPV)
 
 def npv(rate, values):
     """
     Returns the NPV (Net Present Value) of a cash flow series.
+
     Parameters:
         rate (scalar): The discount rate.
         values (array_like, shape(M, )): The values of the time series of cash flows. The (fixed) time interval
             between cash flow "events" must be the same as that for which `rate` is given (i.e., if `rate` is per year,
             then precise a year is understood to elapse between each cash flow event). By convention, investments or
             "deposits" are negative, income or "withdrawals" are positive; `values` must begin with the initial
             investment, thus `values[0]` will typically be negative.
+
     Returns:
         float: The NPV of the input cash flow series `values` at the discount `rate`.
+
     Warnings
     --------
     ``npv`` considers a series of cashflows starting in the present (t = 0).
     NPV can also be defined with a series of future cashflows, paid at the
     end, rather than the start, of each period. If future cashflows are used,
     the first cashflow `values[0]` must be zeroed and added to the net
     present value of the future cashflows. This is demonstrated in the
     examples.
+
     Notes
     -----
     Returns the result of: [G]_
     .. math:: \\sum_{t=0}^{M-1}{\\frac{values_t}{(1+rate)^{t}}}
+
     Examples:
     ---------
     Consider a potential project with an initial investment of $40 000 and
     projected cashflows of $5 000, $8 000, $12 000 and $30 000 at the end of
     each period discounted at a rate of 8% per period. To find the project's
     net present value::
         import numpy as np
@@ -653,19 +698,21 @@
 
 
 # Modified Internal Rate of Return
 
 def mirr(values, finance_rate, reinvest_rate):
     """
     Modified internal rate of return.
+
     Parameters:
         values (array_like): Cash flows (must contain at least one positive and one negative value) or nan is returned.
             The first value is considered a sunk cost at time zero.
         finance_rate (scalar): Interest rate paid on the cash flows
         reinvest_rate (scalar): Interest rate received on the cash flows upon reinvestment
+
     Returns:
         float: Modified internal rate of return
     """
     values = np.asarray(values)
     n = values.size
 
     # Without this explicit cast the 1/(n - 1) computation below
@@ -686,99 +733,114 @@
 
 
 # Straight-Line Depreciation
 
 def depreciate(cost, salvage, life):
     """
     Calculate the straight-line depreciation of an asset over time.
+
     Parameters:
         cost: initial cost of the asset
         salvage: salvage value of the asset at the end of its useful life
         life: life of the asset in years
+
     Returns:
         float: depreciation amount
+
     .. Note::
-        The depreciation amount for each full year is the same amount: the original value of the asset B minus the
-        salvage value S all divided by the number of years N:
+        The depreciation amount for each full year is the same amount:
+           the original value of the asset B minus the salvage value S all divided by the number of years N
+
     Examples:
     ---------
     A company purchased a machine for $100,000 with an estimated salvage value of $10,000 after 5 years::
         cost = 100000
         salvage = 10000
         life = 5
         syse.depreciate(cost, salvage, life)
         print("The straight-line depreciation for the machine is ${} per year.".format(depreciate))
         Output = The straight-line depreciation for the machine is $18,000 per year.
+
     .. jupyter-execute::
         :hide-code:
         cost = 100000
         salvage = 10000
         life = 5
         depreciation = (cost - salvage) / life
         print("The straight-line depreciation for the machine is ${} per year.".format(depreciation))
     """
     depreciation = (cost - salvage) / life
     return depreciation
 
 
 # Sum-of-Years-Digits Method:
 
-def digits(cost: float, salvage_value: float, useful_life: int) -> float:
+def digits(cost: np.ndarray, salvage_value: np.ndarray, useful_life: int) -> np.ndarray:
     """
     Compute the depreciation for an asset using the sum-of-years-digits method.
+
     Parameters:
-        cost (float): The cost of the asset.
-        salvage_value (float): The salvage value of the asset.
+        cost (np.ndarray): The cost of the asset.
+        salvage_value (np.ndarray): The salvage value of the asset.
         useful_life (int): The useful life of the asset.
+
     Returns:
-        float: The depreciation for the asset.
+        np.ndarray: The depreciation for the asset.
+
     .. Note::
         The function takes as input the cost of the asset, the salvage_value of the asset at the end of its useful
         life, and the useful_life of the asset in years. It computes the depreciation for the asset using the
         sum-of-years-digits method, which assumes that the asset depreciates more rapidly in the earlier years of
         its life.
+
     Examples:
     ---------
     Suppose a company purchases a machine for $60,000, with an expected salvage value of $6,000 after 6 years.
-    The company expects to use the machine for 6 years. We can compute the depreciation for the machine using the
-    digits function::
-        depreciation = syse.digits(cost=60000, salvage_value=6000, useful_life=6)
-        print(f"The annual depreciation for the machine is ${depreciation/6:.2f}.")
-        Output = The annual depreciation for the machine is $10333.33.
-    This means that the company can deduct $10,333.33 each year for 6 years as a depreciation expense for tax purposes.
-    At the end of 6 years, the book value of the machine will be $6,000, which is the expected salvage value.
-    """
-    years = [i + 1 for i in range(useful_life)]
-    total_years = sum(years)
-    accumulated_depreciation = 0.0
+    The company expects to use the machine for 6 years. We can compute the accumulated depreciation for the machine
+    using the digits function::
+        cost= 60000
+        salvage_value= 6000
+        useful_life= 6
+        syse.digits(cost, salvage_value, useful_life)
+        Output = 54000
+    This means that the accumulated depreciation is $54,000 and the book value of the machine will be $6,000,
+    which is the expected salvage value.
+    """
+    years = np.array([i + 1 for i in range(useful_life)], dtype=np.float64)
+    total_years = np.sum(years)
+    accumulated_depreciation = np.zeros_like(cost, dtype=np.float64)
 
     for year in years:
         depreciation = (cost - salvage_value) * (useful_life - year + 1) / total_years
-        accumulated_depreciation += depreciation
+        accumulated_depreciation += depreciation.astype(np.float64)
 
     return accumulated_depreciation
 
 
 # Declining Balance Method:
 
 def decline(cost: float, salvage_value: float, useful_life: int, rate: float) -> float:
     """
     Compute the depreciation for an asset using the declining balance method.
+
     Parameters:
         cost (float): The cost of the asset.
         salvage_value (float): The salvage value of the asset.
         useful_life (int): The useful life of the asset.
         rate (float): The depreciation rate, expressed as a fraction of 1.
+
     Returns:
         float: The depreciation for the asset.
+
     .. Note::
         The function takes as input the cost of the asset, the salvage_value of the asset at the end of its useful
         life, the useful_life of the asset in years, and the rate of depreciation as a fraction of 1. It computes the
         depreciation for the asset using the declining balance method, which assumes that the asset depreciates by a
         fixed percentage of its remaining book value each year.
+
     Examples:
     ---------
     Suppose a company purchases a delivery truck for $50,000, with an expected salvage value of $5,000 after 5 years.
     The company expects to use the truck for 5 years. The depreciation rate for the truck is 30% per year using the
     declining balance method. We can compute the depreciation for the truck using the
     decline function::
         depreciation = syse.decline(cost=50000, salvage_value=5000, useful_life=5, rate=0.3)
@@ -801,26 +863,30 @@
 
 
 # Double Declining Balance Method:
 
 def double(cost: float, salvage_value: float, useful_life: int, rate: float) -> float:
     """
     Compute the depreciation for an asset using the double declining balance method.
+
     Parameters:
         cost (float): The cost of the asset.
         salvage_value (float): The salvage value of the asset.
         useful_life (int): The useful life of the asset.
         rate (float): The depreciation rate, expressed as a fraction of 1.
+
     Returns:
         float: The depreciation for the asset.
+
     .. Note::
         The function takes the same inputs as the declining_balance_method function, but computes the depreciation
         using the double declining balance method. The double declining balance method assumes that the asset
         depreciates by a fixed percentage of its remaining book value each year, but that the rate of depreciation is
         twice the straight-line rate.
+
     Examples:
     ---------
     Suppose a company purchases a printing press for $100,000, with an expected salvage value of $10,000 after 4 years.
     The company expects to use the printing press for 4 years. The depreciation rate for the printing press is 50% per
     year using the double declining balance method. We can compute the depreciation for the printing press using the
     double function::
         depreciation = syse.double(cost=100000, salvage_value=10000, useful_life=4, rate=0.5)
@@ -841,98 +907,112 @@
         book_value -= depreciation
 
     return accumulated_depreciation
 
 
 # Units of Production Method:
 
-def units(cost: float, salvage_value: float, useful_life: int, units_produced: int) -> float:
+def units(cost, salvage, expected_units_lifetime, production_t, t):
     """
-    Compute the depreciation for an asset using the units-of-production method.
+    Calculate the units-of-production depreciation and book value at the end of year t.
+
     Parameters:
-        cost (float): The cost of the asset.
-        salvage_value (float): The salvage value of the asset.
-        useful_life (int): The useful life of the asset.
-        units_produced (int): The total units produced by the asset during its useful life.
+        cost (float): The original cost of the asset
+        salvage (float): The estimated salvage value of the asset at the end of its useful life
+        expected_units_lifetime (float): The total expected number of units produced over the asset's lifetime
+        production_t (numpy array): A numpy array of units produced per year for t years
+        t (int): Number of years
+
     Returns:
-        float: The depreciation for the asset.
-    .. Note::
-        The function takes as input the cost of the asset, the salvage_value of the asset at the end of its useful life,
-        the useful_life of the asset in years, and the total units_produced by the asset during its useful life.
-        It computes the depreciation for the asset using the units-of-production method, which assumes that the asset
-        depreciates in proportion to the number of units produced by the asset.
+        float: Depreciation expense in year t
+        float: Book value at the end of year t
+
     Examples:
     ---------
-    Suppose a company purchases a printing press for $200,000, with an expected salvage value of $20,000 after
-    producing 1,000,000 pages. The company expects to produce 2,000,000 pages over the life of the printing press.
-    The company plans to use the printing press for 5 years. We can compute the depreciation for the printing press
-    using the units function::
-        depreciation = syse.units(cost=200000, salvage_value=20000, useful_life=5, units_produced=2000000)
-        print(f"The annual depreciation for the printing press is ${depreciation/5:.2f}.")
-        Output = The annual depreciation for the printing press is $32000.00.
-    This means that the company can deduct $32,000 each year for 5 years as a depreciation expense for tax purposes.
-    At the end of 5 years, the book value of the printing press will be $20,000, which is the expected salvage value.
-    """
-    total_units = units_produced
-    accumulated_depreciation = 0.0
+    On January 1, Miners, Inc. bought a backhoe for $500,000. They expect to use it for 5,000 hours, about 1,000 per
+    year for 5 years, before selling it for $100,000. What is the depreciation expense for the first year if they opt
+    for units-of-production method and used it for 1,500 hours?::
+        cost = 500000
+        salvage = 100000
+        expected_units_lifetime = 5000
+        production_t = np.array([1500])  # Only the first year's usage is given, so the array has one element
+        t = 1
+        # Calculate depreciation expense and book value for the first year
+        syse.units(cost, salvage, expected_units_lifetime, production_t, t)
+        Output = 120000.0
 
-    for year in range(1, useful_life + 1):
-        depreciation = (cost - salvage_value) * (units_produced / total_units)
-        accumulated_depreciation += depreciation
-        units_produced -= (units_produced / total_units)
 
-    return accumulated_depreciation
+    """
+    # Calculate Depreciation per Unit
+    depreciation_per_unit = (cost - salvage) / expected_units_lifetime
+    # Calculate Depreciation Expense for each year
+    depreciation_expense_t = production_t * depreciation_per_unit
+    # Calculate accumulated depreciation
+    accumulated_depreciation = np.sum(depreciation_expense_t[:t])
+    # Calculate book value at the end of year t
+    book_value_t = cost - accumulated_depreciation
+
+    return depreciation_expense_t[t-1]
 
 
 # Probability & Statistics
 
 
 # Simple Moving Average
 
 def sma(data, n):
     """
     Calculate the simple moving average of a list of data points for the most recent n periods.
+
     Parameters:
         data (list): A list of data points.
         n (int): The number of most recent observations to be used.
+
     Returns:
         float: The simple moving average.
+
     Examples:
     ---------
-    Suppose you are the owner of a retail store and you want to analyze the sales performance of your store for the
+    Suppose you are the owner of a retail store, and you want to analyze the sales performance of your store for the
     last 10 days. You have a list of the daily sales figures for the past 10 days. You can use the above Python
     function to calculate the simple moving average of the sales figures over the past 10 days to get an idea of the
     store's overall sales trend. This information can be useful in determining whether you need to adjust your
     inventory or marketing strategies to improve sales.
+
+
     """
     if len(data) < n:
         return None
     else:
         return sum(data[-n:]) / n
 
 
 # Weighted Moving Average
 
 def wma(data, weights):
     """
     Calculate the weighted moving average of a list of data points using a list of weights.
+
     Parameters:
         data (list): A list of data points.
         weights (list): A list of weights to be applied to each data point.
+
     Returns:
         float: The weighted moving average.
+
     Examples:
     ---------
-        Suppose you are a financial analyst and you want to analyze the stock price of a company over the
+        Suppose you are a financial analyst, and you want to analyze the stock price of a company over the
         past 5 days. You have a list of the daily closing prices for the past 5 days, and you believe that the
         most recent day's price should be given a higher weight than the previous days. You can use the above
         Python function to calculate the weighted moving average of the stock prices over the past 5 days,
         where the weight of the most recent day's price is 0.5 and the weights of the previous days are 0.3, 0.1,
         and 0.1 respectively. This information can be useful in determining whether the stock price is trending up or
         down and making investment decisions accordingly.
+
     """
     if len(data) != len(weights):
         return None
     else:
         return sum([data[i] * weights[i] for i in range(len(data))]) / sum(weights)
 
 
@@ -959,21 +1039,25 @@
 
 
 # Simple Linear Regression
 
 def line(x, y):
     """
     Calculate slope and intercept of the linear regression line that best fits the data.
+
     Parameters:
         x: list of x-values
         y: list of y-values
+
     Returns:
         tuple: (slope, intercept)
+
     Notes
     -----
+
     Examples:
     ---------
     """
     # Calculate the mean of x and y
     x_mean = sum(x) / len(x)
     y_mean = sum(y) / len(y)
     # Calculate the slope
@@ -993,24 +1077,28 @@
 
 
 # Maximize - Linear Programming
 
 def linear_pro(costs, budget):
     """
     A Python function for linear programming. (Placeholder for a better function)
+
     Parameters:
         costs : A list of costs associated with a project.
         budget : The total budget allocated to the project.
+
     Returns:
         float: A list of the maximum values that can be allocated to each cost while staying within the budget.
+
     .. Caution::
         This function seeks to **maximize** the values.
+
     Examples:
     ---------
-    ::
+      ::
         costs = [1000, 2000, 3000]
         budget = 5000
         solution = syse.linear_pro(costs, budget)
         print(solution)
         Output= [1000.0, 2000.0, 1000.0]
     """
     # Initialize the solution list
@@ -1033,49 +1121,52 @@
 
 
 # Engineering Management
 
 
 # Program Evaluation Review Technique (PERT)
 
-def pert(tasks):
+def pert(*tasks):
     """
-    Calculate the amount of time it will take to realistically finish a project
-    :param tasks:
-    :return: optimistic, most likely, & pessimistic time
+    Calculate the expected time and standard deviation it will take to realistically finish a project using the PERT
+    estimate formula: (O +4M + P)/6
+
+    Parameters:
+           tasks: np.ndarray or list of estimated times for each task
+
+    Returns:
+           float: expected time
+           float: standard deviation
+
     Examples:
     ---------
     You are working on a project to build a new office building.
     You need to estimate the time required to complete the project.
-    You have identified the following tasks:
-    **1.** Design the building\n
-    **2.** Purchase materials\n
-    **3.** Construct the building\n
-    **4.** Finish the interior
-    Using the PERT method, you can estimate the time required to complete the project::
-        tasks = [DesignBuilding(), PurchaseMaterials(), ConstructBuilding(), FinishInterior()]
-        optimistic_time, most_likely_time, pessimistic_time = pert(tasks)
-        print('Optimistic Time:', optimistic_time)
-        print('Most Likely Time:', most_likely_time)
-        print('Pessimistic Time:', pessimistic_time)
-    """
-    # Create a list to store the estimated times for each task
-    estimated_time = []
-    # Loop through each task
-    for task in tasks:
-        # Estimate the time required for the task
-        estimated_time.append(task.estimate_time())
-        # Calculate the optimistic time
-        optimistic_time = min(estimated_time)
-        # Calculate the most likely time
-        most_likely_time = sum(estimated_time) / len(estimated_time)
-        # Calculate the pessimistic time
-        pessimistic_time = max(estimated_time)
-        # Return the PERT values
-        return optimistic_time, most_likely_time, pessimistic_time
+    You have identified the following tasks: **1.** Design the building, **2.** Purchase materials, **3.** Construct the building,
+    and **4.** Finish the interior. You can estimate the time required to complete the project using the PERT function::
+           # Define the tasks for each stage of the project
+           DesignBuilding = [60, 70, 100]
+           PurchaseMaterials = [60, 70, 100]
+           ConstructBuilding = [60, 70, 100]
+           FinishInterior = [60, 70, 100]
+           Output = ([73.33333333, 73.33333333, 73.33333333, 73.33333333]),
+                    [6.66666667, 6.66666667, 6.66666667, 6.66666667]))
+    """
+    # Convert input to NumPy arrays
+    tasks = [np.array(task) for task in tasks]
+    # Extract the optimistic, most likely, and pessimistic times for each set of tasks
+    optimistic_time = [task[0] for task in tasks]
+    most_likely_time = [task[1] for task in tasks]
+    pessimistic_time = [task[2] for task in tasks]
+    # Calculate the expected time using the PERT formula
+    expected_time = (np.array(optimistic_time) + 4 * np.array(most_likely_time) + np.array(pessimistic_time)) / 6
+    # Calculate the standard deviation using the PERT formula
+    standard_deviation = (np.array(pessimistic_time) - np.array(optimistic_time)) / 6
+    # Return the expected time and standard deviation
+    return expected_time, standard_deviation
 
 
 # Network Analysis
 
 # def network():
 #     """
 #
@@ -1115,20 +1206,23 @@
 
 
 # Economic Order Quantity (EOQ)
 
 def eoq(a: float, d: float, h: float) -> float:
     """
     Calculate the economic order quantity (EOQ) for an instantaneous replenishment inventory model.
+
     Parameters:
         A (float): The cost to place one order.
         D (float): The number of units used per year.
         h (float): The holding cost per unit per year.
+
     Returns:
         float: The EOQ that minimizes the total annual inventory cost.
+
     Examples:
     ---------
     Let's say that a small business that sells specialty coffee beans uses an instantaneous replenishment
     inventory model to manage its inventory of beans. The business purchases its coffee beans from a supplier and
     pays a fixed cost of $50 to place an order, regardless of the quantity ordered. The business uses 500 bags of
     coffee beans per year, and the holding cost per bag per year is $5.
     To determine the optimal order quantity, we can use the eoq function::
@@ -1152,24 +1246,26 @@
         A (float): The cost to place one order.
         D (float): The number of units used per year.
         h (float): The holding cost per unit per year.
         R (float): The replenishment rate.
 
     Returns:
         float: The EMQ that minimizes the total annual inventory cost.
+
     .. Note::
         The EMQ formula assumes the same conditions as the EOQ formula
         (i.e., constant and known demand, no stockouts, constant and known ordering
         costs and holding costs), but also assumes that the replenishment rate is
         finite. The EMQ represents the optimal production quantity that minimizes
         the total annual inventory cost, including both holding costs and ordering
         costs, when production is constrained by a finite rate of replenishment.
         Note that the formula assumes that the replenishment rate is given in
         units per day, and that the annual demand is normalized to units per
         day by dividing by 365.
+
     Examples:
     ---------
     Let's say that a manufacturer produces widgets using a finite replenishment rate inventory model to manage its
     inventory of raw materials. The manufacturer purchases a raw material from a supplier and pays a fixed cost of
     $100 to place an order, regardless of the quantity ordered. The manufacturer uses 10,000 units of the raw material
     per year, and the holding cost per unit per year is $8. The supplier has a limited production capacity and can only
     replenish the manufacturer's inventory at a maximum rate of 500 units per day.
@@ -1177,15 +1273,16 @@
         A = 100
         D = 10000
         h = 8
         R = 500
         emq = syse.emq(A, D, h, R)
         print(emq)
         Output = 514.29
+
     .. Important::
         Again, note that this example is simplified and does not take into account other factors that could
         influence the manufacturer's decision-making, such as variability in demand and lead times, stockout costs, and
         other costs associated with ordering and holding inventory. Nonetheless, the EMQ model provides a useful starting
         point for inventory management decisions in a constrained production environment.
     """
     emq = math.sqrt((2 * a * d) / (h * (1 - (d / (r * 365)))))
-    return emq
+    return emq
```

### Comparing `syse-0.0.8/src/syse.egg-info/PKG-INFO` & `syse-0.0.9/src/syse.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syse
-Version: 0.0.8
+Version: 0.0.9
 Summary: Systems & Industrial Engineering Python Package
 Home-page: https://github.com/apexpromgt/SysE
 Author: Jonathon Nicholson
 Author-email: Jonathon Nicholson <Jonathon@apexpromgt.com>
 License: MIT License
         
         Copyright (c) [2023] [Jonathon Nicholson]
@@ -37,28 +37,28 @@
 License-File: LICENSE
 
 # Welcome to the SysE Python Package!
 
 [![Documentation Status](https://readthedocs.org/projects/syse/badge/?version=latest)](https://syse.readthedocs.io/en/latest/?badge=latest)
 
 
-SysE (/Sis'y/) is a Python library for Systems Engineering.
+SysE is a Python library for Industrial and Systems Engineering.
 
 SysE covers common Industrial & Systems Engineering topics such as:
 * Engineering Economics 
 * Probability & Statistics
 * Modeling & Quantitative Analysis
 * Engineering Management
 
-Some use cases include:
-*
-*
 
 To get started, check out the docs for further information, including how to install SysE and common use cases.
 
 **Links:**
 * **Documentation:** [SysE Docs](https://syse.readthedocs.io/en/latest/)
 * **Repository:** [SysE Repo](https://github.com/Apex-Engineering-Management/SysE)
 
-**Note:**
+**Notes:**
 
-This project is under active development.
+* This project is being worked on, but I am very busy. 
+* The declining depreciation functions will be fixed.
+* The linear optimization function is extremely limited, and will be worked on.
+* For the few functions that can't be called with scalars, arrays, or other sequences, there are plans to update them.
```

