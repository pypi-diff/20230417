# Comparing `tmp/pymathematics-2023.4.16.1.tar.gz` & `tmp/pymathematics-2023.4.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.4.16.1.tar", last modified: Sun Apr 16 06:29:55 2023, max compression
+gzip compressed data, was "pymathematics-2023.4.17.tar", last modified: Mon Apr 17 16:55:06 2023, max compression
```

## Comparing `pymathematics-2023.4.16.1.tar` & `pymathematics-2023.4.17.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-16 06:29:55.952398 pymathematics-2023.4.16.1/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.16.1/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-16 06:29:55.924712 pymathematics-2023.4.16.1/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       30 2023-04-16 06:28:23.000000 pymathematics-2023.4.16.1/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-16 06:29:55.669618 pymathematics-2023.4.16.1/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     7996 2023-04-16 06:28:36.000000 pymathematics-2023.4.16.1/pymathematics/__init__.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      112 2023-04-16 06:00:49.000000 pymathematics-2023.4.16.1/pymathematics/info.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-16 06:29:55.869623 pymathematics-2023.4.16.1/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-16 06:29:55.000000 pymathematics-2023.4.16.1/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-16 06:29:55.000000 pymathematics-2023.4.16.1/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-16 06:29:55.000000 pymathematics-2023.4.16.1/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-16 06:29:55.000000 pymathematics-2023.4.16.1/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-16 06:29:55.955387 pymathematics-2023.4.16.1/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      692 2023-04-16 06:23:12.000000 pymathematics-2023.4.16.1/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-17 16:55:06.913364 pymathematics-2023.4.17/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.17/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-17 16:55:06.900365 pymathematics-2023.4.17/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       30 2023-04-16 06:28:23.000000 pymathematics-2023.4.17/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-17 16:55:06.643919 pymathematics-2023.4.17/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    11933 2023-04-17 16:36:03.000000 pymathematics-2023.4.17/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-17 16:36:43.000000 pymathematics-2023.4.17/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-17 16:55:06.830918 pymathematics-2023.4.17/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-17 16:55:04.000000 pymathematics-2023.4.17/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-17 16:55:04.000000 pymathematics-2023.4.17/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-17 16:55:04.000000 pymathematics-2023.4.17/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-17 16:55:04.000000 pymathematics-2023.4.17/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-17 16:55:06.916367 pymathematics-2023.4.17/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      689 2023-04-17 16:36:31.000000 pymathematics-2023.4.17/setup.py
```

### Comparing `pymathematics-2023.4.16.1/LICENSE` & `pymathematics-2023.4.17/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.4.16.1/pymathematics/__init__.py` & `pymathematics-2023.4.17/pymathematics/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,34 @@
 
 author = author
 version = version
 homepage = homepage
 
 class constants:
     pi = 3.1415926535897932384626433832795
-    exp = 2.7182818284590452353602874713527
+    e = 2.7182818284590452353602874713527
+
+class vector:
+    def cross_product(vector1:list,vector2:list) -> int|float:
+        return [vector1[1]*vector2[2]-vector2[1]*vector1[2],-(vector1[0]*vector2[2]-vector2[0]*vector1[2]),vector1[0]*vector2[1]-vector2[0]*vector1[1]]
+
+    def dot_product(vector1:list,vector2:list) -> int|float:
+        return vector1[0]*vector2[0]+vector1[1]*vector2[1]+vector1[2]*vector2[2]
+
+    def magnitude(vector) -> int|float:
+        return sqrt(vector[0]**2+vector[1]**2+vector[2]**2)
+
+    def projection(vector1:list,vector2:list) -> int|float:
+        """
+        `projection of vector1 to vector2`
+        """
+        return vector.dot_product(vector1,vector2)/vector.magnitude(vector2)
+
+    def angle_of_projection(vector1:list,vector2:list) -> float:
+        return f"arccos({vector.dot_product(vector1,vector2)}/{(vector.magnitude(vector1)*vector.magnitude(vector2))})"
 
 def factorial(number: int) -> int:
     if number == 0:
         return 1
     elif number < 0:
         raise ValueError("number can't be negative!")
     return number*factorial(number-1)
@@ -27,14 +46,26 @@
         return seq[1]
     else:
         for i in range(2,number):
             next_int = seq[i-1]+seq[i-2]
             seq.append(next_int)
     return seq
 
+def reciprocal(number:int|float) -> int|float:
+    return 1/number
+
+def accuracy(actual:list,predicted:list,tolerance:float = 0.01) -> list:
+    if len(actual) != len(predicted):
+        raise ValueError("length of actual and predicted aren't the same")
+    score = 0
+    for x in range(len(actual)):
+        if (actual[x] - predicted[x]) <= tolerance:
+            score += 1
+    return score/len(actual)
+
 def exp(number:int) -> float:
     return summation([(number**n)/factorial(n) for n in range(0,100)])
 
 def absolute(number:int|float) -> int|float:
     if number < 0:
         return -1*number
     return number
@@ -43,15 +74,15 @@
     if number < 0:
         return "undefined"
     elif number == 0:
         return 0
     flag = number/2
     while absolute(flag*flag - number) > 0.00001:
         flag = (flag + number/flag)/2
-    return flag
+    return round(flag,5)
 
 def quadratic_roots(a:int|float,b:int|float,c:int|float) -> int|float:
     D = b*b-4*a*c
     if D < 0:
         x1 = f"{-b} + {sqrt(absolute(D))}i"
         x2 = f"{-b} - {sqrt(absolute(D))}i"
         raise Warning(f"discriminant was negative! {[x1,x2]}")
@@ -84,15 +115,18 @@
             return n+left
 
 
 def ln(number:int|float) -> int|float:
     return 2.303*log(number)
 
 def summation(array:list) -> list:
-    return sum(array)
+    sigma = 0
+    for x in array:
+        sigma += x
+    return sigma
 
 def product(array:list) -> list:
     result = 1
     for x in array:
         result *= x
     return result
 
@@ -141,14 +175,24 @@
     if cos(theta) == 0:
         raise ValueError(f"sec({theta}) isn't defined at rad({theta})")
     return 1/cos(theta)
 
 def mean(array:list) -> int|float:
     return sum(array)/len(array)
 
+def median(array:list) -> list:
+    sorted_array = quick_sort(array)
+    if len(sorted_array)%2 == 0:
+        mid1 = int(len(sorted_array)/2)
+        mid2 = mid1 - 1
+        return mean([mid1,mid2])
+    else:
+        mid = int(len(sorted_array)/2)
+        return sorted_array[mid]
+
 def standard_deviation(array:list,kind:str = "population") -> list:
     if kind == "sample":
         d = len(array)-1
     elif kind == "population":
         d = len(array)
     else:
         raise ValueError(f"invalid input {kind}! input should be whether 'population' or 'sample'")
@@ -211,45 +255,117 @@
         raise ValueError(f"steps must be greater than zero {steps} < {0}")
     if len(array) < steps:
         raise ValueError(f"invalid input {steps} > {len(array)}! array must have atleast as many elements as the number of steps!")
     avgs = []
     for i in range(len(array)-steps+1):
         subset = array[i:i+steps]
         avgs.append(sum(subset)/steps)
-    return avgs    
+    return avgs
 
 def exponential_moving_average(array:list,alpha:float) -> list:
     if 0 <= alpha <= 1:
         ema = [array[0]]
         for x in range(1,len(array)):
             ema.append(alpha*array[x]+(1-alpha)*ema[x-1])
         return ema
     else:
         raise ValueError("invalid input! the value of alpha should lie between 0 and 1 included")
 
+def bubble_sort(array:list) -> list:
+    for i in range(len(array)):
+        for j in range(0,len(array)-i-1):
+            if array[j] > array[j+1]:
+                array[j],array[j+1] = array[j+1],array[j]
+    return array
+
+def quick_sort(array:list) -> list:
+    if len(array) <= 1:
+        return array
+    pivot = array[len(array)//2]
+    left = [x for x in array if x < pivot]
+    middle = [x for x in array if x == pivot]
+    right = [x for x in array if x > pivot]
+    return quick_sort(left)+middle+quick_sort(right)
+
+def descending_sort(array:list) -> list:
+    for i in range(len(array)):
+        for j in range(i+1,len(array)):
+            if array[j] > array[i]:
+                array[i],array[j] = array[j],array[i]
+    return array
+
 def correlation_coefficient(x:list,y:list) -> list:
     if len(x) != len(y):
         raise ValueError("length of x and y aren't the same!")
     xsum = summation(x)
     ysum = summation(y)
     xysum = summation([x[i]*y[i] for i in range(len(x))])
     xsqrsum = summation([x[i]**2 for i in range(len(x))])
     ysqrsum = summation([y[i]**2 for i in range(len(y))])
     n = len(x)*xysum-xsum*ysum
     d = sqrt((len(x)*xsqrsum-xsum**2)*(len(x)*ysqrsum-ysum**2))
     if d == 0:
         return 0
     return n/d
 
+def slope_intercept(array1:list,array2:list) -> list:
+    if len(array1) != len(array2):
+        raise ValueError("the size of array aren't the same!")
+    xmean = mean(array1)
+    ymean = mean(array2)
+    xdiff = [x-xmean for x in array1]
+    ydiff = [y-ymean for y in array2]
+    slope = summation([xdiff[i]*ydiff[i] for i in range(len(array1))])/summation([d**2 for d in xdiff])
+    intercept = ymean-slope*xmean
+    return [slope,intercept]
+
+def min_max(array):
+    sorted_array = quick_sort(array)
+    return [sorted_array[0],sorted_array[len(sorted_array)-1]]
+
 def mean_sqrd_error(actual:list,predicted:list) -> int|float:
     if len(actual) != len(predicted):
         raise ValueError("length of actual and predicted data aren't equal!")
     errors = [(actual[i]-predicted[i])**2 for i in range(len(actual))]
     return summation(errors)/len(actual)
 
+def mean_error(actual:list,expected:list) -> list:
+    pass
+
+def power(base:int|float,exponent:int|float) -> int|float:
+    return base**exponent
+
+def power_sum(array:list,exponent:int|float) -> list:
+    return summation(power_array(array,exponent))
+
+def power_array(array:list,exponent:int|float) -> list:
+    return [x**exponent for x in array]
+
+def primes(limit:int) -> list:
+    if limit <= 0:
+        raise ValueError("limit must be greater than zero")
+    primes = []
+    for x in range(2,limit):
+        is_prime = True
+        for i in range(2,int(sqrt(x))+1):
+            if x%i == 0:
+                is_prime = False
+                break
+        if is_prime:
+            primes.append(x)
+    return primes
+
+def isprime(number:int) -> bool:
+    if number < 2:
+        return False
+    for x in range(2,int(sqrt(number))+1):
+        if number%x == 0:
+            return False
+    return True
+
 def root_mean_sqrd_error(actual:list,predicted:list) -> int|float:
     if len(actual) != len(predicted):
         raise ValueError("length of actual and predicted data aren't equal!")
     return sqrt(mean_sqrd_error(actual,predicted))
 
 def cost_function(actual:list, predicted:list) -> int|float:
     if len(actual) != len(predicted):
```

### Comparing `pymathematics-2023.4.16.1/setup.py` & `pymathematics-2023.4.17/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.04.16.1",
+    version = "2023.4.17",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
```

