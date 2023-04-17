# Comparing `tmp/fast_depends-1.0.1.tar.gz` & `tmp/fast_depends-1.0.2.tar.gz`

## Comparing `fast_depends-1.0.1.tar` & `fast_depends-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.0.1/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.0.1/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 fast_depends-1.0.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/__about__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/__init__.py
--rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/construct.py
--rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/injector.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/model.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/provider.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/types.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/usage.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 fast_depends-1.0.1/fast_depends/utils.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fast_depends-1.0.1/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.0.1/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.0.1/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.0.1/scripts/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 fast_depends-1.0.1/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.0.1/LICENSE
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 fast_depends-1.0.1/README.md
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 fast_depends-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5803 2020-02-02 00:00:00.000000 fast_depends-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.0.2/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.0.2/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 fast_depends-1.0.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/__about__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/__init__.py
+-rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/construct.py
+-rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/injector.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/model.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/provider.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/types.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/usage.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/utils.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fast_depends-1.0.2/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.0.2/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.0.2/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.0.2/scripts/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 fast_depends-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 fast_depends-1.0.2/README.md
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 fast_depends-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 fast_depends-1.0.2/PKG-INFO
```

### Comparing `fast_depends-1.0.1/.github/workflows/publish_coverage.yml` & `fast_depends-1.0.2/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.1/.github/workflows/publish_pypi.yml` & `fast_depends-1.0.2/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.1/.github/workflows/tests.yml` & `fast_depends-1.0.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.1/fast_depends/construct.py` & `fast_depends-1.0.2/fast_depends/construct.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.1/fast_depends/injector.py` & `fast_depends-1.0.2/fast_depends/injector.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.1/fast_depends/model.py` & `fast_depends-1.0.2/fast_depends/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.1/fast_depends/usage.py` & `fast_depends-1.0.2/fast_depends/usage.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.1/LICENSE` & `fast_depends-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.1/README.md` & `fast_depends-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/lancetnik/fastdepends" target="_blank">
         <img src="https://coverage-badge.samuelcolvin.workers.dev/lancetnik/fastdepends.svg" alt="Coverage">
     </a>
     <a href="https://pypi.org/project/fast-depends" target="_blank">
         <img src="https://img.shields.io/pypi/v/fast-depends?label=pypi%20package" alt="Package version">
     </a>
     <a href="https://pepy.tech/project/fast-depends" target="_blank">
-        <img src="https://static.pepy.tech/personalized-badge/fast-depend?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="downloads"/>
+        <img src="https://static.pepy.tech/personalized-badge/fast-depends?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="downloads"/>
     </a>
     <br/>
     <a href="https://pypi.org/project/fast-depend" target="_blank">
         <img src="https://img.shields.io/pypi/pyversions/fast-depends.svg" alt="Supported Python versions">
     </a>
     <a href="https://github.com/Lancetnik/FastDepends/blob/main/LICENSE" target="_blank">
         <img alt="GitHub" src="https://img.shields.io/github/license/Lancetnik/FastDepends?color=%23007ec6">
@@ -24,34 +24,34 @@
 
 ---
 
 Documentation: https://lancetnik.github.io/FastDepends/
 
 ---
 
-FastDepends - extracted and cleared from HTTP domain logic Fastapi Dependency Injection System.
-This is a little library, providing you ability to use lovely Fastapi interfaces at your own
+FastDepends - FastAPI Dependency Injection system extracted from FastAPI and cleared of all HTTP logic.
+This is a small library which provides you with the ability to use lovely Fastapi interfaces in your own
 projects or tools.
 
 Thanks to [*fastapi*](https://fastapi.tiangolo.com/) and [*pydantic*](https://docs.pydantic.dev/) projects for this
-greate functional. This package just a little change Fasapi sources to provide DI functionality pyre-python way.
+greate functionality. This package is just a small change of the original Fastapi sources to provide DI functionality in a pyre-Python way.
 
-Async and sync code supported as well.
+Async and sync modes are both supported.
 
 ## Installation
 
 ```bash
 pip install fast-depends
 ```
 
 ## Usage
 
 There is no way to make Dependency Injection easier
 
-You can use this library without any frameworks at **sync** and **async** code both
+You can use this library without any frameworks in both **sync** and **async** code.
 
 ### Async code
 ```python
 import asyncio
 
 from fast_depends import inject, Depends
 
@@ -83,29 +83,29 @@
     c: int = Depends(dependency)
 ) -> float:
     return a + b + c
 
 assert main("1", 2) == 4.0
 ```
 
-`@inject` decorator playing multiple roles at the same time:
+`@inject` decorator plays multiple roles at the same time:
 
 * resolve *Depends* classes
-* cast types according python annotation
+* cast types according to Python annotation
 * validate incoming parameters using *pydantic*
 
 ---
 
 ### Features
-Syncronous code is fully supported at this package: without any `async_to_sync`, `run_sync`, `syncify` or any other tricks.
+Synchronous code is fully supported in this package: without any `async_to_sync`, `run_sync`, `syncify` or any other tricks.
 
-Also, *FastDepends* casts function return the same way, it can be very felpfull to build your own tools.
+Also, *FastDepends* casts functions' return values the same way, it can be very helpful in building your own tools.
 
-There is two main defferences from native Fastapi DI System.
+These are two main defferences from native Fastapi DI System.
 
 ---
 
 ### Note
-Library was build by actual **0.95.0 FastAPI** version.
+Library was based on **0.95.0 FastAPI** version.
 
-If we'll be too far behind, please, contact [me](mailto:diementros@yandex.ru)
+If we are too far behind, please, contact [me](mailto:diementros@yandex.ru)
 or contubute yourself. Really appreciate your help.
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
 # FastDepends
           [Tests_coverage] [Coverage] [Package_version] [downloads]
                      [Supported_Python_versions] [GitHub]
 --- Documentation: https://lancetnik.github.io/FastDepends/ --- FastDepends -
-extracted and cleared from HTTP domain logic Fastapi Dependency Injection
-System. This is a little library, providing you ability to use lovely Fastapi
-interfaces at your own projects or tools. Thanks to [*fastapi*](https://
-fastapi.tiangolo.com/) and [*pydantic*](https://docs.pydantic.dev/) projects
-for this greate functional. This package just a little change Fasapi sources to
-provide DI functionality pyre-python way. Async and sync code supported as
-well. ## Installation ```bash pip install fast-depends ``` ## Usage There is no
-way to make Dependency Injection easier You can use this library without any
-frameworks at **sync** and **async** code both ### Async code ```python import
-asyncio from fast_depends import inject, Depends async def dependency(a: int) -
-> int: return a @inject async def main( a: int, b: int, c: int = Depends
-(dependency) ) -> float: return a + b + c assert asyncio.run(main("1", 2)) ==
-4.0 ``` ### Sync code ```python from fast_depends import inject, Depends def
-dependency(a: int) -> int: return a @inject def main( a: int, b: int, c: int =
-Depends(dependency) ) -> float: return a + b + c assert main("1", 2) == 4.0 ```
-`@inject` decorator playing multiple roles at the same time: * resolve
-*Depends* classes * cast types according python annotation * validate incoming
-parameters using *pydantic* --- ### Features Syncronous code is fully supported
-at this package: without any `async_to_sync`, `run_sync`, `syncify` or any
-other tricks. Also, *FastDepends* casts function return the same way, it can be
-very felpfull to build your own tools. There is two main defferences from
-native Fastapi DI System. --- ### Note Library was build by actual **0.95.0
-FastAPI** version. If we'll be too far behind, please, contact [me](mailto:
+FastAPI Dependency Injection system extracted from FastAPI and cleared of all
+HTTP logic. This is a small library which provides you with the ability to use
+lovely Fastapi interfaces in your own projects or tools. Thanks to [*fastapi*]
+(https://fastapi.tiangolo.com/) and [*pydantic*](https://docs.pydantic.dev/
+) projects for this greate functionality. This package is just a small change
+of the original Fastapi sources to provide DI functionality in a pyre-Python
+way. Async and sync modes are both supported. ## Installation ```bash pip
+install fast-depends ``` ## Usage There is no way to make Dependency Injection
+easier You can use this library without any frameworks in both **sync** and
+**async** code. ### Async code ```python import asyncio from fast_depends
+import inject, Depends async def dependency(a: int) -> int: return a @inject
+async def main( a: int, b: int, c: int = Depends(dependency) ) -> float: return
+a + b + c assert asyncio.run(main("1", 2)) == 4.0 ``` ### Sync code ```python
+from fast_depends import inject, Depends def dependency(a: int) -> int: return
+a @inject def main( a: int, b: int, c: int = Depends(dependency) ) -> float:
+return a + b + c assert main("1", 2) == 4.0 ``` `@inject` decorator plays
+multiple roles at the same time: * resolve *Depends* classes * cast types
+according to Python annotation * validate incoming parameters using *pydantic*
+--- ### Features Synchronous code is fully supported in this package: without
+any `async_to_sync`, `run_sync`, `syncify` or any other tricks. Also,
+*FastDepends* casts functions' return values the same way, it can be very
+helpful in building your own tools. These are two main defferences from native
+Fastapi DI System. --- ### Note Library was based on **0.95.0 FastAPI**
+version. If we are too far behind, please, contact [me](mailto:
 diementros@yandex.ru) or contubute yourself. Really appreciate your help.
```

### Comparing `fast_depends-1.0.1/pyproject.toml` & `fast_depends-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.1/PKG-INFO` & `fast_depends-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 1.0.1
+Version: 1.0.2
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -60,15 +60,15 @@
     <a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/lancetnik/fastdepends" target="_blank">
         <img src="https://coverage-badge.samuelcolvin.workers.dev/lancetnik/fastdepends.svg" alt="Coverage">
     </a>
     <a href="https://pypi.org/project/fast-depends" target="_blank">
         <img src="https://img.shields.io/pypi/v/fast-depends?label=pypi%20package" alt="Package version">
     </a>
     <a href="https://pepy.tech/project/fast-depends" target="_blank">
-        <img src="https://static.pepy.tech/personalized-badge/fast-depend?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="downloads"/>
+        <img src="https://static.pepy.tech/personalized-badge/fast-depends?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="downloads"/>
     </a>
     <br/>
     <a href="https://pypi.org/project/fast-depend" target="_blank">
         <img src="https://img.shields.io/pypi/pyversions/fast-depends.svg" alt="Supported Python versions">
     </a>
     <a href="https://github.com/Lancetnik/FastDepends/blob/main/LICENSE" target="_blank">
         <img alt="GitHub" src="https://img.shields.io/github/license/Lancetnik/FastDepends?color=%23007ec6">
@@ -77,34 +77,34 @@
 
 ---
 
 Documentation: https://lancetnik.github.io/FastDepends/
 
 ---
 
-FastDepends - extracted and cleared from HTTP domain logic Fastapi Dependency Injection System.
-This is a little library, providing you ability to use lovely Fastapi interfaces at your own
+FastDepends - FastAPI Dependency Injection system extracted from FastAPI and cleared of all HTTP logic.
+This is a small library which provides you with the ability to use lovely Fastapi interfaces in your own
 projects or tools.
 
 Thanks to [*fastapi*](https://fastapi.tiangolo.com/) and [*pydantic*](https://docs.pydantic.dev/) projects for this
-greate functional. This package just a little change Fasapi sources to provide DI functionality pyre-python way.
+greate functionality. This package is just a small change of the original Fastapi sources to provide DI functionality in a pyre-Python way.
 
-Async and sync code supported as well.
+Async and sync modes are both supported.
 
 ## Installation
 
 ```bash
 pip install fast-depends
 ```
 
 ## Usage
 
 There is no way to make Dependency Injection easier
 
-You can use this library without any frameworks at **sync** and **async** code both
+You can use this library without any frameworks in both **sync** and **async** code.
 
 ### Async code
 ```python
 import asyncio
 
 from fast_depends import inject, Depends
 
@@ -136,29 +136,29 @@
     c: int = Depends(dependency)
 ) -> float:
     return a + b + c
 
 assert main("1", 2) == 4.0
 ```
 
-`@inject` decorator playing multiple roles at the same time:
+`@inject` decorator plays multiple roles at the same time:
 
 * resolve *Depends* classes
-* cast types according python annotation
+* cast types according to Python annotation
 * validate incoming parameters using *pydantic*
 
 ---
 
 ### Features
-Syncronous code is fully supported at this package: without any `async_to_sync`, `run_sync`, `syncify` or any other tricks.
+Synchronous code is fully supported in this package: without any `async_to_sync`, `run_sync`, `syncify` or any other tricks.
 
-Also, *FastDepends* casts function return the same way, it can be very felpfull to build your own tools.
+Also, *FastDepends* casts functions' return values the same way, it can be very helpful in building your own tools.
 
-There is two main defferences from native Fastapi DI System.
+These are two main defferences from native Fastapi DI System.
 
 ---
 
 ### Note
-Library was build by actual **0.95.0 FastAPI** version.
+Library was based on **0.95.0 FastAPI** version.
 
-If we'll be too far behind, please, contact [me](mailto:diementros@yandex.ru)
+If we are too far behind, please, contact [me](mailto:diementros@yandex.ru)
 or contubute yourself. Really appreciate your help.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fast-depends Version: 1.0.1 Summary: FastDepends -
+Metadata-Version: 2.1 Name: fast-depends Version: 1.0.2 Summary: FastDepends -
 extracted and cleared from HTTP domain logic FastAPI Dependency Injection
 System. Async and sync are both supported. Project-URL: Homepage, https://
 lancetnik.github.io/FastDepends/ Project-URL: Documentation, https://
 lancetnik.github.io/FastDepends/ Project-URL: Tracker, https://github.com/
 Lancetnik/FastDepends/issues Project-URL: Source, https://github.com/Lancetnik/
 FastDepends Author-email: Pastukhov Nikita
 yandex.ru> License-File: LICENSE Keywords: dependency injection,fastapi
@@ -31,31 +31,32 @@
 [toml]>=7.2; extra == 'test' Requires-Dist: pytest-asyncio>=0.21; extra ==
 'test' Requires-Dist: pytest-xdist[psutil]; extra == 'test' Requires-Dist:
 pytest>=7; extra == 'test' Description-Content-Type: text/markdown #
 FastDepends
           [Tests_coverage] [Coverage] [Package_version] [downloads]
                      [Supported_Python_versions] [GitHub]
 --- Documentation: https://lancetnik.github.io/FastDepends/ --- FastDepends -
-extracted and cleared from HTTP domain logic Fastapi Dependency Injection
-System. This is a little library, providing you ability to use lovely Fastapi
-interfaces at your own projects or tools. Thanks to [*fastapi*](https://
-fastapi.tiangolo.com/) and [*pydantic*](https://docs.pydantic.dev/) projects
-for this greate functional. This package just a little change Fasapi sources to
-provide DI functionality pyre-python way. Async and sync code supported as
-well. ## Installation ```bash pip install fast-depends ``` ## Usage There is no
-way to make Dependency Injection easier You can use this library without any
-frameworks at **sync** and **async** code both ### Async code ```python import
-asyncio from fast_depends import inject, Depends async def dependency(a: int) -
-> int: return a @inject async def main( a: int, b: int, c: int = Depends
-(dependency) ) -> float: return a + b + c assert asyncio.run(main("1", 2)) ==
-4.0 ``` ### Sync code ```python from fast_depends import inject, Depends def
-dependency(a: int) -> int: return a @inject def main( a: int, b: int, c: int =
-Depends(dependency) ) -> float: return a + b + c assert main("1", 2) == 4.0 ```
-`@inject` decorator playing multiple roles at the same time: * resolve
-*Depends* classes * cast types according python annotation * validate incoming
-parameters using *pydantic* --- ### Features Syncronous code is fully supported
-at this package: without any `async_to_sync`, `run_sync`, `syncify` or any
-other tricks. Also, *FastDepends* casts function return the same way, it can be
-very felpfull to build your own tools. There is two main defferences from
-native Fastapi DI System. --- ### Note Library was build by actual **0.95.0
-FastAPI** version. If we'll be too far behind, please, contact [me](mailto:
+FastAPI Dependency Injection system extracted from FastAPI and cleared of all
+HTTP logic. This is a small library which provides you with the ability to use
+lovely Fastapi interfaces in your own projects or tools. Thanks to [*fastapi*]
+(https://fastapi.tiangolo.com/) and [*pydantic*](https://docs.pydantic.dev/
+) projects for this greate functionality. This package is just a small change
+of the original Fastapi sources to provide DI functionality in a pyre-Python
+way. Async and sync modes are both supported. ## Installation ```bash pip
+install fast-depends ``` ## Usage There is no way to make Dependency Injection
+easier You can use this library without any frameworks in both **sync** and
+**async** code. ### Async code ```python import asyncio from fast_depends
+import inject, Depends async def dependency(a: int) -> int: return a @inject
+async def main( a: int, b: int, c: int = Depends(dependency) ) -> float: return
+a + b + c assert asyncio.run(main("1", 2)) == 4.0 ``` ### Sync code ```python
+from fast_depends import inject, Depends def dependency(a: int) -> int: return
+a @inject def main( a: int, b: int, c: int = Depends(dependency) ) -> float:
+return a + b + c assert main("1", 2) == 4.0 ``` `@inject` decorator plays
+multiple roles at the same time: * resolve *Depends* classes * cast types
+according to Python annotation * validate incoming parameters using *pydantic*
+--- ### Features Synchronous code is fully supported in this package: without
+any `async_to_sync`, `run_sync`, `syncify` or any other tricks. Also,
+*FastDepends* casts functions' return values the same way, it can be very
+helpful in building your own tools. These are two main defferences from native
+Fastapi DI System. --- ### Note Library was based on **0.95.0 FastAPI**
+version. If we are too far behind, please, contact [me](mailto:
 diementros@yandex.ru) or contubute yourself. Really appreciate your help.
```

