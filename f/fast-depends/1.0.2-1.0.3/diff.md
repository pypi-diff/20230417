# Comparing `tmp/fast_depends-1.0.2.tar.gz` & `tmp/fast_depends-1.0.3.tar.gz`

## Comparing `fast_depends-1.0.2.tar` & `fast_depends-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.0.2/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.0.2/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 fast_depends-1.0.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/__about__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/__init__.py
--rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/construct.py
--rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/injector.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/model.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/provider.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/types.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/usage.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 fast_depends-1.0.2/fast_depends/utils.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fast_depends-1.0.2/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.0.2/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.0.2/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.0.2/scripts/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 fast_depends-1.0.2/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.0.2/LICENSE
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 fast_depends-1.0.2/README.md
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 fast_depends-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 fast_depends-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-1.0.3/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.0.3/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.0.3/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 fast_depends-1.0.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/__about__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/__init__.py
+-rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/construct.py
+-rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/injector.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/model.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/provider.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/types.py
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/usage.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/utils.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fast_depends-1.0.3/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.0.3/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.0.3/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.0.3/scripts/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 fast_depends-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 fast_depends-1.0.3/README.md
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 fast_depends-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 fast_depends-1.0.3/PKG-INFO
```

### Comparing `fast_depends-1.0.2/CONTRIBUTING.md` & `fast_depends-1.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.2/.github/workflows/publish_coverage.yml` & `fast_depends-1.0.3/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.2/.github/workflows/publish_pypi.yml` & `fast_depends-1.0.3/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.2/.github/workflows/tests.yml` & `fast_depends-1.0.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.2/fast_depends/construct.py` & `fast_depends-1.0.3/fast_depends/construct.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.2/fast_depends/model.py` & `fast_depends-1.0.3/fast_depends/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, List, Optional, Tuple
 
+from pydantic import create_model
 from pydantic.error_wrappers import ErrorList
 from pydantic.fields import ModelField
 
 from fast_depends.types import AnyCallable
 
 RETURN_FIELD = "custom_return"
 
@@ -27,14 +28,15 @@
         self.use_cache = use_cache
         # Parent argument name at subdependency
         self.name = name
         # Store the path to be able to re-generate a dependable from it in overrides
         self.path = path
         # Save the cache key at creation to optimize performance
         self.cache_key = (self.call,)
+        self.error_model = create_model(getattr(call, "__name__", str(call)))
 
     def cast_response(self, response: Any) -> Tuple[Optional[Any], Optional[ErrorList]]:
         if self.return_field is None:
             return response, []
         return self.return_field.validate(response, {}, loc=RETURN_FIELD)
```

### Comparing `fast_depends-1.0.2/fast_depends/usage.py` & `fast_depends-1.0.3/fast_depends/usage.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,86 +21,89 @@
 
 def Depends(  # noqa: N802
     dependency: Optional[AnyCallable] = None, *, use_cache: bool = True
 ) -> Any:
     return model.Depends(dependency=dependency, use_cache=use_cache)
 
 
+def wrap_dependant(dependant: model.Dependant) -> model.Dependant:
+    return dependant
+
+
 def inject(
     func: Callable[P, T],
     *,
     dependency_overrides_provider: Optional[Any] = dependency_provider,
+    wrap_dependant: Callable[[model.Dependant], model.Dependant] = wrap_dependant,
 ) -> Callable[P, T]:
     dependant = get_dependant(call=func, path=func.__name__)
-    error_model = create_model(func.__name__)
+
+    dependant = wrap_dependant(dependant)
 
     if is_coroutine_callable(func) is True:
         f = async_typed_wrapper
     else:
         f = sync_typed_wrapper
 
     return wraps(func)(
         partial(
             f,
             dependant=dependant,
-            error_model=error_model,
             dependency_overrides_provider=dependency_overrides_provider,
         )
     )
 
 
 async def async_typed_wrapper(
     *args: P.args,
     dependant: model.Dependant,
-    error_model: BaseModel,
     dependency_overrides_provider: Optional[Any],
     **kwargs: P.kwargs,
 ) -> Any:
     kwargs = args_to_kwargs((x.name for x in dependant.params), *args, **kwargs)
 
     async with AsyncExitStack() as stack:
         solved_result, errors, _ = await solve_dependencies_async(
             body=kwargs,
             dependant=dependant,
             stack=stack,
             dependency_overrides_provider=dependency_overrides_provider,
         )
 
         if errors:
-            raise ValidationError(errors, error_model)
+            raise ValidationError(errors, dependant.error_model)
 
         v, errors = dependant.cast_response(
-            await run_async(dependant=dependant, values=solved_result)
+            await run_async(dependant.call, **solved_result)
         )
 
         if errors:
-            raise ValidationError(errors, error_model)
+            raise ValidationError(errors, dependant.error_model)
 
         return v
 
 
 def sync_typed_wrapper(
     *args: P.args,
     dependant: model.Dependant,
-    error_model: BaseModel,
     dependency_overrides_provider: Optional[Any],
     **kwargs: P.kwargs,
 ) -> Any:
     kwargs = args_to_kwargs((x.name for x in dependant.params), *args, **kwargs)
 
     with ExitStack() as stack:
         solved_result, errors, _ = solve_dependencies_sync(
             body=kwargs,
             dependant=dependant,
             stack=stack,
             dependency_overrides_provider=dependency_overrides_provider,
         )
 
         if errors:
-            raise ValidationError(errors, error_model)
+            raise ValidationError(errors, dependant.error_model)
 
         v, errors = dependant.cast_response(dependant.call(**solved_result))
 
         if errors:
-            raise ValidationError(errors, error_model)
+            raise ValidationError(errors, dependant.error_model)
 
         return v
```

### Comparing `fast_depends-1.0.2/LICENSE` & `fast_depends-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.2/README.md` & `fast_depends-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.2/pyproject.toml` & `fast_depends-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.2/PKG-INFO` & `fast_depends-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 1.0.2
+Version: 1.0.3
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fast-depends Version: 1.0.2 Summary: FastDepends -
+Metadata-Version: 2.1 Name: fast-depends Version: 1.0.3 Summary: FastDepends -
 extracted and cleared from HTTP domain logic FastAPI Dependency Injection
 System. Async and sync are both supported. Project-URL: Homepage, https://
 lancetnik.github.io/FastDepends/ Project-URL: Documentation, https://
 lancetnik.github.io/FastDepends/ Project-URL: Tracker, https://github.com/
 Lancetnik/FastDepends/issues Project-URL: Source, https://github.com/Lancetnik/
 FastDepends Author-email: Pastukhov Nikita
 yandex.ru> License-File: LICENSE Keywords: dependency injection,fastapi
```

