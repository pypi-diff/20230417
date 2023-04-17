# Comparing `tmp/uxu-0.0.1.tar.gz` & `tmp/uxu-0.0.2.tar.gz`

## Comparing `uxu-0.0.1.tar` & `uxu-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,76 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 uxu-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 uxu-0.0.1/tests/test_listdiff.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 uxu-0.0.1/uxu/__about__.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 uxu-0.0.1/uxu/__init__.py
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 uxu-0.0.1/uxu/element.py
--rw-r--r--   0        0        0     9770 2020-02-02 00:00:00.000000 uxu-0.0.1/uxu/fiber.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 uxu-0.0.1/uxu/html.py
--rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 uxu-0.0.1/uxu/listdiff.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 uxu-0.0.1/uxu/manager.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 uxu-0.0.1/uxu/patch.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 uxu-0.0.1/uxu/proxy_reactor.py
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 uxu-0.0.1/uxu/rendering.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 uxu-0.0.1/uxu/textnode.py
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 uxu-0.0.1/uxu/vdom.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 uxu-0.0.1/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 uxu-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 uxu-0.0.1/README.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 uxu-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 uxu-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 uxu-0.0.2/.env
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 uxu-0.0.2/pyrightconfig.json
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/0a1237d725462fae/352387855ee8c379
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/0a1237d725462fae/cd6bd1dcfebeffe9
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/1e4bdf158bd9b9e5/394341b7182cd227
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/1e4bdf158bd9b9e5/7d0fdd8cd1d85fd3
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/476fb78351979deb/1dd6f7b457ad880d
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/476fb78351979deb/c32bb284c4a9bfae
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/77d3df0ea028b111/352387855ee8c379
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/77d3df0ea028b111/5ac597c988feda25
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/77d3df0ea028b111/7089cef4b92d73cc
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/77d3df0ea028b111/cd6bd1dcfebeffe9
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/a1b87770545a8882/1dd6f7b457ad880d
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/a1b87770545a8882/c32bb284c4a9bfae
+-rw-r--r--   0        0        0    20988 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/unicode_data/13.0.0/charmap.json.gz
+-rw-r--r--   0        0        0    21505 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/unicode_data/14.0.0/charmap.json.gz
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 uxu-0.0.2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 uxu-0.0.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 uxu-0.0.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 uxu-0.0.2/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 uxu-0.0.2/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 uxu-0.0.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 uxu-0.0.2/.vscode/launch.json
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 uxu-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 uxu-0.0.2/tests/test_listdiff.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 uxu-0.0.2/tests/test_patch.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/__about__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/__init__.py
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/element.py
+-rw-r--r--   0        0        0    11760 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/fiber.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/html.py
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/listdiff.py
+-rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/manager.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/patch.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/persistence.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/proxy_reactor.py
+-rw-r--r--   0        0        0     6046 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/rendering.py
+-rw-r--r--   0        0        0     9102 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/serve.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/textnode.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/util.py
+-rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/vdom.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/lsp/README.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/lsp/__init__.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/lsp/server.py
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/lsp/types.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/rpc/__init__.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/rpc/io_transport.py
+-rw-r--r--   0        0        0    18290 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/rpc/jsonrpc.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/rpc/starlette_ws_transport.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/rpc/transport.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/rpc/websocket_transport.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 uxu-0.0.2/web/.gitignore
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 uxu-0.0.2/web/build.mjs
+-rw-r--r--   0        0        0    14308 2020-02-02 00:00:00.000000 uxu-0.0.2/web/package-lock.json
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 uxu-0.0.2/web/package.json
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 uxu-0.0.2/web/server.mjs
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/.package-lock.json
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/.bin/esbuild -> ../esbuild/bin/esbuild
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/@esbuild/darwin-arm64/README.md
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/@esbuild/darwin-arm64/package.json
+-rwxr-xr-x   0        0        0  8858802 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/@esbuild/darwin-arm64/bin/esbuild
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/esbuild/LICENSE.md
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/esbuild/README.md
+-rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/esbuild/install.js
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/esbuild/package.json
+hrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/esbuild/bin/esbuild
+-rw-r--r--   0        0        0    18934 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/esbuild/lib/main.d.ts
+-rw-r--r--   0        0        0    86013 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/esbuild/lib/main.js
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 uxu-0.0.2/web/src/app.ts
+-rw-r--r--   0        0        0    13701 2020-02-02 00:00:00.000000 uxu-0.0.2/web/src/reactor.ts
+-rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 uxu-0.0.2/web/src/rpc.ts
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 uxu-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 uxu-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 uxu-0.0.2/README.md
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 uxu-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 uxu-0.0.2/PKG-INFO
```

### Comparing `uxu-0.0.1/tests/test_listdiff.py` & `uxu-0.0.2/tests/test_listdiff.py`

 * *Files identical despite different names*

### Comparing `uxu-0.0.1/uxu/fiber.py` & `uxu-0.0.2/uxu/fiber.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,36 +4,39 @@
 from typing import (
     Any,
     Callable,
     ClassVar,
     Coroutine,
     Generic,
     Optional,
-    ParamSpec,
     Protocol,
     TypeVar,
     Union,
     overload,
 )
+import warnings
 from .rendering import RenderedFragment, Rendering
-from .patch import ModifyChildrenPatch
+from .patch import ModifyChildrenPatch, ReplaceElementPatch
 from .vdom import (
     Html,
     NormSpec,
     Vdom,
     VdomContext,
     create,
     dispose,
     fresh_id,
+    hydrate,
+    hydrate_lists,
     normalise_html,
     patch,
     vdom_context,
     reconcile_lists,
 )
 import logging
+from .util import ParamSpec
 
 logger = logging.getLogger("uxu")
 
 
 S = TypeVar("S")
 
 SetterFn = Callable[[Union[S, Callable[[S], S]]], None]
@@ -112,19 +115,24 @@
 
     def initialize(self):
         self.evaluate()
 
     def evaluate(self):
         callback = self.callback
         assert callable(callback)
-        self.dispose()
-        if asyncio.iscoroutinefunction(callback):
-            self.task = asyncio.create_task(callback())
+        if vdom_context.get().is_static:
+            logging.debug(
+                f"skipping effect call because vdom context is in static mode"
+            )
         else:
-            callback()
+            self.dispose()
+            if asyncio.iscoroutinefunction(callback):
+                self.task = asyncio.create_task(callback())
+            else:
+                callback()
 
     def reconcile(self, new_hook: "EffectHook"):
         assert type(new_hook) == type(self)
 
         def update():
             self.deps = new_hook.deps
             self.callback = new_hook.callback
@@ -161,14 +169,17 @@
     @property
     def name(self):
         return getattr(self.component, "__name__", "unknown")
 
     def create(self):
         return Fiber.create(self)
 
+    def hydrate(self, r: Rendering) -> "Fiber":
+        return Fiber.hydrate(r, self)
+
     def __str__(self):
         return self.name
 
 
 H = TypeVar("H", bound="AbstractHook")
 
 
@@ -190,57 +201,90 @@
     @property
     def name(self) -> str:
         return getattr(self.component, "__name__")
 
     def __str__(self) -> str:
         return f"<{self.name} {self.id}>"
 
-    def __init__(self, spec: "FiberSpec"):
+    def _hydrate(self, render: Rendering) -> None:
+        if not isinstance(render, RenderedFragment):
+            logger.debug(f"expected RenderedFragment, got {type(render)}")
+            self._create()
+            patch(ReplaceElementPatch(element_id=render.id, new_element=self.render()))
+            return
+        self.id = render.id
+        with self:
+            s = self.component(*self.props_args, **self.props_kwargs)
+            children, reorder = hydrate_lists(render.children, normalise_html(s))
+            patch(ModifyChildrenPatch(self.id, reorder))
+            self.rendered = children
+
+    def _create(self):
+        if hasattr(self, "rendered"):
+            raise RuntimeError("fiber is already initialized")
         self.id = fresh_id()
-        self.key = spec.key  # type: ignore
+        with self:
+            s = self.component(*self.props_args, **self.props_kwargs)
+            self.rendered = create(normalise_html(s))
+
+    def start(self):
+        if hasattr(self, "update_loop_task"):
+            raise RuntimeError("fiber is already running")
         self.invalidated_event = asyncio.Event()
-        component = spec.component
-        if not hasattr(component, "__name__"):
-            logger.warning(f"Please name component {component}.")
-        self.component = component
+        self.update_loop_task = asyncio.create_task(self._update_loop())
+
+    def __init__(self, spec: "FiberSpec"):
+        # [todo] enforce this shouldn't be called directly, use Fiber.create or Fiber.hydrate
+        self.key = spec.key  # type: ignore
+        self.component = spec.component
         self.props_args = spec.props_args
         self.props_kwargs = spec.props_kwargs
-        assert not hasattr(self, "rendered") and not hasattr(
-            self, "hooks"
-        ), "already created"
+        if not hasattr(self.component, "__name__"):
+            logger.warning(f"Please name component {self.component}.")
         self.hooks = []
         self.hook_idx = 0
-        t = fiber_context.set(self)
-        s = self.component(*self.props_args, **self.props_kwargs)
-        self.rendered = create(normalise_html(s))
-        fiber_context.reset(t)
-        self.update_loop_task = asyncio.create_task(self.update_loop())
+        # now you need to run either _create() or _hydrate()
+
+    def __enter__(self):
+        self._reset_ticket = fiber_context.set(self)
+        return self
 
-    async def update_loop(self):
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        fiber_context.reset(self._reset_ticket)
+
+    async def _update_loop(self):
         while True:
             await self.invalidated_event.wait()
             logger.debug(f"{str(self)} rerendering.")
             self.invalidated_event.clear()
             try:
                 self.reconcile_core()
             except Exception as e:
                 logger.exception("failure in update loop")
 
     def dispose(self):
         # [todo] can I just use GC?
         assert hasattr(self, "hooks")
-        assert hasattr(self, "rendered"), "fiber is not rendered"
-        dispose(self.rendered)
+        assert hasattr(
+            self, "rendered"
+        ), "Fiber not initialized with _create or _hydrate"
+        if hasattr(self, "rendered"):
+            dispose(self.rendered)
         for hook in reversed(self.hooks):
             hook.dispose()
-        self.update_loop_task.cancel()
+        if hasattr(self, "update_loop_task"):
+            self.update_loop_task.cancel()
 
     def invalidate(self):
         """Called when a hook's callback is invoked, means that a re-render must occur."""
-        logger.debug(f"{str(self)} invalidated.")
+        logger.debug(f"{str(self)} invalidated")
+        if vdom_context.get().is_static:
+            warnings.warn(
+                "fiber was invalidated but vdom context is in static mode, so fiber update loop is not running"
+            )
         self.invalidated_event.set()
 
     def reconcile_hook(self, hook: H) -> H:
         if self.hook_idx >= len(self.hooks):
             # initialisation case
             self.hooks.append(hook)
             self.hook_idx += 1
@@ -281,32 +325,27 @@
         children, reorder = reconcile_lists(self.rendered, spec)
         self.rendered = children
         l = self.hook_idx + 1
         old_hooks = self.hooks[l:]
         self.hooks = self.hooks[:l]
         for hook in reversed(old_hooks):
             hook.dispose()
-        patch(
-            ModifyChildrenPatch(
-                element_id=self.id,
-                remove_these=reorder.remove_these,
-                then_insert_these=reorder.then_insert_these,
-                children_length_start=reorder.l1_len,
-            )
-        )
+        patch(ModifyChildrenPatch(self.id, reorder))
         return
 
     def reconcile(self, new_spec: "FiberSpec") -> "Fiber":
         assert isinstance(new_spec, FiberSpec)
         assert hasattr(self, "hooks") and hasattr(self, "rendered"), "not created"
         # if the identity of the component function has changed that
         # means we should rerender.
         if new_spec.name != self.name or self.component is not new_spec.component:
             self.dispose()
-            new_fiber = Fiber(new_spec)
+            new_fiber = Fiber.create(new_spec)
+            new_render: Rendering = new_fiber.render()
+            patch(ReplaceElementPatch(element_id=self.id, new_element=new_render))
             return new_fiber
         # [todo] check whether the props have changed here
         if (
             self.props_args == new_spec.props_args
             and self.props_kwargs == new_spec.props_kwargs
             and not self.invalidated_event.is_set()
         ):
@@ -319,16 +358,28 @@
 
     def render(self) -> Rendering:
         return RenderedFragment(
             id=self.id, children=[x.render() for x in self.rendered]
         )
 
     @classmethod
-    def create(cls, spec: FiberSpec):
-        return cls(spec)
+    def create(cls, spec: FiberSpec) -> "Fiber":
+        f = cls(spec)
+        f._create()
+        if not vdom_context.get().is_static:
+            f.start()
+        return f
+
+    @classmethod
+    def hydrate(cls, render: Rendering, spec: FiberSpec) -> "Fiber":
+        f = cls(spec)
+        f._hydrate(render)
+        if not vdom_context.get().is_static:
+            f.start()
+        return f
 
 
 fiber_context: ContextVar[Fiber] = ContextVar("fiber_context")
 
 
 class StateVar(Protocol[S]):
     @property
```

### Comparing `uxu-0.0.1/uxu/html.py` & `uxu-0.0.2/uxu/html.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from functools import partial, singledispatch
-from typing import Any, Literal, Optional, ParamSpec, Sequence, TypeVar, Union, overload
+from typing import Any, Literal, Optional, Sequence, TypeVar, Union, overload
 
 from .textnode import TextNodeSpec
 from .vdom import Html, NormSpec, normalise_html
 from .element import ElementSpec
 from .fiber import Component, FiberSpec
-
+from .util import ParamSpec
 
 P = ParamSpec("P")
 
+"""
+[todo] use the https://github.com/Knio/dominate libarary.
+or at least mimick it.
+ """
+
 
 @overload
 def h(tag: str, attrs: dict, *children: Html, key: Optional[str] = None) -> ElementSpec:
     ...
 
 
 @overload
-def h(tag: Component[P], *args: P.args, **kwargs: P.kwargs) -> FiberSpec[P]:
+def h(tag: Component[P], *args: P.args, **kwargs: P.kwargs) -> FiberSpec:
     ...
 
 
 def h(tag, attrs, *children: Html, key=None, **kwargs) -> Union[ElementSpec, FiberSpec]:  # type: ignore
     if type(tag) == str:
         if not isinstance(attrs, dict):
             raise TypeError("attrs must be a dict")
@@ -36,11 +41,21 @@
     else:
         raise TypeError(f"unrecognised tag: {tag}")
 
 
 # [todo] type-safe html elements.
 # [todo] type-safe CSS inline styles.
 
-div = partial(h, tag="div")
-p = partial(h, tag="p")
-h1 = partial(h, tag="h1")
-h2 = partial(h, tag="h2")
+
+def alias(tag):
+    def core(*children, **attrs):
+        return h(tag, attrs, *children)
+
+    return core
+
+
+def img(src: str, alt="image"):
+    return h("img", dict(src=src, alt=alt))
+
+
+div = alias("div")
+p = alias("p")
```

### Comparing `uxu-0.0.1/uxu/listdiff.py` & `uxu-0.0.2/uxu/listdiff.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,14 +223,18 @@
         )
 
     @classmethod
     def identity(cls, length: int) -> "Reorder[Any]":
         return cls(l1_len=length, l2_len=length, remove_these={}, then_insert_these={})
 
     @property
+    def is_identity(self):
+        return len(self.remove_these) == 0 and len(self.then_insert_these) == 0
+
+    @property
     def deletions(self):
         """Get the indices of items in the first list that are deleted."""
         for i in self.remove_these.keys():
             if self.remove_these[i] is None:
                 yield i
 
     @property
```

### Comparing `uxu-0.0.1/uxu/proxy_reactor.py` & `uxu-0.0.2/uxu/proxy_reactor.py`

 * *Files identical despite different names*

### Comparing `uxu-0.0.1/uxu/rendering.py` & `uxu-0.0.2/uxu/patch.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,89 +1,101 @@
-from dataclasses import dataclass, field, replace
-from typing import Any, Callable, Union
+from dataclasses import dataclass, field, is_dataclass, replace
+from typing import Any, Union
 
-""" A rendering is the thing that we actually send over the wire to Javascript. """
+from .rendering import Rendering, RenderedElement, RenderedAttrVal, RootRendering
+from .listdiff import Reorder
 
 
-@dataclass
-class EventHandler:
-    handler_id: Any
+from abc import ABC, abstractmethod
+
+"""
+[todo] ABC
+[todo] serialisation
+[todo] patch application
+"""
 
-    def __eq__(self, other):
-        if not isinstance(other, EventHandler):
-            return False
-        return self.handler_id == other.handler_id
 
-    def __todict__(self):
-        return {"__handler__": self.handler_id}
+class Patch(ABC):
+    kind: str
 
-    @classmethod
-    def __ofdict__(cls, d: dict):
-        return EventHandler(d["__handler__"])
+    @property
+    def is_empty(self):
+        return False
 
+    @abstractmethod
+    def apply(self, root: RootRendering):
+        """Apply the given patch to the given rendering.
 
-RenderedAttrVal = Union[EventHandler, str, dict]
+        raises:
+            RuntimeError: When trying to apply an InvalidatePatch.
+        """
+        raise NotImplementedError()
 
 
 @dataclass
-class RenderedText:
-    value: str
-    id: Any
-    kind: str = field(default="text")
+class InvalidatePatch(Patch):
+    """Used to trigger a re-render of entire tree. Avoid."""
+
+    kind: str = field(default="invalidate")
+
+    def apply(self, root: Rendering):
+        raise RuntimeError("Can't apply an invalidation patch, please rerender.")
 
 
 @dataclass
-class RenderedElement:
-    id: Any
-    tag: str
-    attrs: dict[str, RenderedAttrVal]
-    children: list["Rendering"]
-    kind: str = field(default="element")
+class ModifyAttributesPatch(Patch):
+    remove: list[str]
+    add: dict[str, RenderedAttrVal]
+    element_id: str
+    kind: str = field(default="modify-attrs")
+
+    @property
+    def is_empty(self) -> bool:
+        return len(self.remove) == 0 and len(self.add) == 0
+
+    def apply(self, root: RootRendering):
+        def visit(r: Rendering):
+            assert isinstance(r, RenderedElement), "invalid id"
+            attrs = {k: v for k, v in r.attrs.items() if k not in self.remove}
+            attrs.update(self.add)
+            return replace(r, attrs=attrs)
+
+        return root.lens_id(self.element_id, visit)
 
 
 @dataclass
-class RenderedFragment:
-    id: Any
-    children: list["Rendering"]
-    kind: str = field(default="fragment")
+class ModifyChildrenPatch(Patch):
+    element_id: str
+    reorder: Reorder[Rendering]
+    kind: str = field(default="modify-children")
+
+    @property
+    def is_empty(self) -> bool:
+        return self.reorder.is_identity
+
+    def apply(self, root: RootRendering):
+        def visit(r: Rendering):
+            cs: list[Rendering] = getattr(r, "children")
+            cs2 = self.reorder.apply(cs)
+            assert is_dataclass(r)
+            return replace(r, children=cs2)
+
+        return root.lens_id(self.element_id, visit)
 
 
 @dataclass
-class RenderedWidget:
-    """This is used to hook into JavaScript code."""
+class ReplaceElementPatch(Patch):
+    element_id: str
+    new_element: Rendering  # output of render
+    kind: str = field(default="replace-element")
+
+    def apply(self, root: Rendering):
+        return root.lens_id(self.element_id, lambda r: self.new_element)
 
-    id: Any
-    name: str
-    props: Any
-    kind: str = field(default="widget")
-
-
-Rendering = Union[RenderedElement, RenderedText, RenderedFragment]
-
-
-def iter_event_handlers(x: "Rendering"):
-    if isinstance(x, RenderedElement):
-        for name, v in x.attrs.items():
-            if isinstance(v, EventHandler):
-                yield name, v
-    children = getattr(x, "children", [])
-    for child in children:
-        yield from iter_event_handlers(child)
-
-
-def map_event_handlers(modify: Callable[[EventHandler], EventHandler]):
-    def rec(x: Rendering) -> Rendering:
-        if isinstance(x, RenderedElement):
-            attrs = {
-                k: modify(v) if isinstance(v, EventHandler) else v
-                for k, v in x.attrs.items()
-            }
-            children = list(map(rec, x.children))
-            return replace(x, attrs=attrs, children=children)
-        elif isinstance(x, RenderedText):
-            return x
-        elif isinstance(x, RenderedFragment):
-            return replace(x, children=list(map(rec, x.children)))
-        else:
-            raise TypeError()
 
-    return rec
+@dataclass
+class ReplaceRootPatch(Patch):
+    root : RootRendering
+    kind: str = field(default="replace-root")
+
+    def apply(self, root: RootRendering):
+        return self.root
```

### Comparing `uxu-0.0.1/uxu/vdom.py` & `uxu-0.0.2/uxu/vdom.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 
     def _register_event(self, k: str, handler: Callable):
         ...
 
     def _unregister_event(self, k: str):
         ...
 
+    @property
+    def is_static(self) -> bool:
+        ...
+
 
 vdom_context: ContextVar[VdomContext] = ContextVar("vdom_context")
 
 
 @contextmanager
 def set_vdom_context(r: VdomContext):
     t = vdom_context.set(r)
@@ -73,14 +77,18 @@
     def __str__(self):
         ...
 
     @abstractmethod
     def create(self) -> Vdom:
         ...
 
+    @abstractmethod
+    def hydrate(self, r: Rendering) -> Vdom:
+        ...
+
 
 @overload
 def create(s: NormSpec) -> Vdom:
     ...
 
 
 @overload
@@ -93,14 +101,21 @@
         return list(map(create, s))
     elif isinstance(s, NormSpec):
         return s.create()
     else:
         raise TypeError(f"unrecognised spec {s}")
 
 
+def hydrate(r: Rendering, s: NormSpec) -> Vdom:
+    if isinstance(s, NormSpec) and isinstance(r, Rendering):
+        return s.hydrate(r)
+    else:
+        raise TypeError(f"unrecognised {r}, {s}")
+
+
 @overload
 def render(s: Vdom) -> Rendering:
     ...
 
 
 @overload
 def render(s: list[Vdom]) -> list[Rendering]:
@@ -112,30 +127,49 @@
         return list(map(render, s))
     elif isinstance(s, Vdom):
         return s.render()
     else:
         raise TypeError(f"unrecognised spec {s}")
 
 
+def hydrate_lists(
+    old: list[Rendering], new: list[NormSpec]
+) -> tuple[list[Vdom], Reorder[Rendering]]:
+    reorder: Reorder = listdiff([x.key for x in old], [x.key for x in new])
+    for ri in reorder.deletions:
+        pass
+    new_vdom: list[Any] = [None] * len(new)
+    for i, j in reorder.moves:
+        assert new_vdom[j] is None
+        new_vdom[j] = hydrate(old[i], new[j])
+    for j in reorder.creations:
+        assert new_vdom[j] is None
+        new_vdom[j] = new[j].create()
+    assert all(x is not None for x in new_vdom)
+    reorder = reorder.map_inserts(lambda j, _: new_vdom[j].render())
+    # [todo] abstract with reconcile_lists
+    return new_vdom, reorder
+
+
 def reconcile_lists(
     old: list[Vdom], new: list[NormSpec]
-) -> tuple[list[Vdom], Reorder[Vdom]]:
-    r: Reorder = listdiff([x.key for x in old], [x.key for x in new])
-    for ri in r.deletions:
+) -> tuple[list[Vdom], Reorder[Rendering]]:
+    reorder: Reorder = listdiff([x.key for x in old], [x.key for x in new])
+    for ri in reorder.deletions:
         old[ri].dispose()
     new_vdom: list[Any] = [None] * len(new)
-    for i, j in r.moves:
+    for i, j in reorder.moves:
         assert new_vdom[j] is None
         new_vdom[j] = reconcile(old[i], new[j])
-    for j in r.creations:
+    for j in reorder.creations:
         assert new_vdom[j] is None
         new_vdom[j] = new[j].create()
     assert all(x is not None for x in new_vdom)
-    r = r.map_inserts(lambda j, _: new_vdom[j])
-    return new_vdom, r
+    reorder = reorder.map_inserts(lambda j, _: new_vdom[j].render())
+    return new_vdom, reorder
 
 
 def reconcile(old: Vdom, new: NormSpec) -> Vdom:
     if isinstance(new, old.spec_type):
         return old.reconcile(new)  # type: ignore
     old.dispose()
     # [todo] add better patch... this shouldn't really happen because we match on keys.
```

### Comparing `uxu-0.0.1/LICENSE.txt` & `uxu-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uxu-0.0.1/pyproject.toml` & `uxu-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,58 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "uxu"
-description = ''
+description = 'Server-side interactive HTML engine.'
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 license = "MIT"
 keywords = []
 authors = [
   { name = "E.W.Ayers", email = "contact@edayers.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = []
+dependencies = [
+  "miniscutil",
+  "websockets",
+  "html5lib",
+  "dominate",
+
+  # server
+  "pydantic",
+  "pydantic[dotenv]",
+  "python-jose", # for JWTs
+  "starlette",
+
+]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/EdAyers/sss/uxu"
 Issues = "https://github.com/EdAyers/sss/issues"
 Source = "https://github.com/EdAyers/sss/uxu"
 
 [tool.hatch.version]
 path = "uxu/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
+  "miniscutil @ {root:uri}/../miniscutil",
 ]
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=uxu --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["37", "38", "39", "310", "311"]
@@ -55,7 +66,15 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[tool.hatch.envs.test]
+dependencies = [
+  "pytest", "pytest-cov", "hypothesis", "pytest-snapshot",
+  "pytest-asyncio",
+  "numpy",
+  "miniscutil @ {root:uri}/../miniscutil",
+]
```

