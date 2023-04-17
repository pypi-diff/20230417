# Comparing `tmp/jsonnet-v0.8.7-pre5.tar.gz` & `tmp/jsonnet-v0.8.7-pre6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jsonnet-v0.8.7-pre5.tar", last modified: Tue Mar  1 01:25:20 2016, max compression
+gzip compressed data, was "dist/jsonnet-v0.8.7-pre6.tar", last modified: Tue Mar 22 04:57:16 2016, max compression
```

## Comparing `jsonnet-v0.8.7-pre5.tar` & `jsonnet-v0.8.7-pre6.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-x---   0 dcunnin  (216460) eng       (5000)        0 2016-03-01 01:25:20.000000 jsonnet-v0.8.7-pre5/
--rw-r-----   0 dcunnin  (216460) eng       (5000)     4158 2016-03-01 00:39:53.000000 jsonnet-v0.8.7-pre5/Makefile
--rw-r-----   0 dcunnin  (216460) eng       (5000)      155 2015-10-27 02:40:26.000000 jsonnet-v0.8.7-pre5/MANIFEST.in
-drwxr-x---   0 dcunnin  (216460) eng       (5000)        0 2016-03-01 01:25:20.000000 jsonnet-v0.8.7-pre5/jsonnet.egg-info/
--rw-r-----   0 dcunnin  (216460) eng       (5000)        1 2016-03-01 01:25:20.000000 jsonnet-v0.8.7-pre5/jsonnet.egg-info/dependency_links.txt
--rw-r-----   0 dcunnin  (216460) eng       (5000)      271 2016-03-01 01:25:20.000000 jsonnet-v0.8.7-pre5/jsonnet.egg-info/PKG-INFO
--rw-r-----   0 dcunnin  (216460) eng       (5000)        9 2016-03-01 01:25:20.000000 jsonnet-v0.8.7-pre5/jsonnet.egg-info/top_level.txt
--rw-r-----   0 dcunnin  (216460) eng       (5000)      540 2016-03-01 01:25:20.000000 jsonnet-v0.8.7-pre5/jsonnet.egg-info/SOURCES.txt
--rw-r-----   0 dcunnin  (216460) eng       (5000)      271 2016-03-01 01:25:20.000000 jsonnet-v0.8.7-pre5/PKG-INFO
--rw-r-----   0 dcunnin  (216460) eng       (5000)     2116 2016-03-01 01:25:07.000000 jsonnet-v0.8.7-pre5/setup.py
-drwxr-x---   0 dcunnin  (216460) eng       (5000)        0 2016-03-01 01:25:20.000000 jsonnet-v0.8.7-pre5/core/
--rw-r-----   0 dcunnin  (216460) eng       (5000)     1592 2016-03-01 00:39:53.000000 jsonnet-v0.8.7-pre5/core/parser.h
--rw-r-----   0 dcunnin  (216460) eng       (5000)   105349 2016-03-01 00:39:53.000000 jsonnet-v0.8.7-pre5/core/vm.cpp
--rw-r-----   0 dcunnin  (216460) eng       (5000)     5268 2015-10-27 02:40:26.000000 jsonnet-v0.8.7-pre5/core/unicode.h
--rw-r-----   0 dcunnin  (216460) eng       (5000)     5035 2016-03-01 00:39:53.000000 jsonnet-v0.8.7-pre5/core/string_utils.cpp
--rw-r-----   0 dcunnin  (216460) eng       (5000)    14023 2016-03-01 00:39:53.000000 jsonnet-v0.8.7-pre5/core/libjsonnet.cpp
--rw-r-----   0 dcunnin  (216460) eng       (5000)     6856 2016-03-01 00:39:53.000000 jsonnet-v0.8.7-pre5/core/lexer.h
--rw-r-----   0 dcunnin  (216460) eng       (5000)    27787 2016-03-01 00:39:53.000000 jsonnet-v0.8.7-pre5/core/ast.h
--rw-r-----   0 dcunnin  (216460) eng       (5000)     2748 2015-10-20 16:54:22.000000 jsonnet-v0.8.7-pre5/core/static_error.h
--rw-r-----   0 dcunnin  (216460) eng       (5000)    40403 2016-03-01 00:39:53.000000 jsonnet-v0.8.7-pre5/core/parser.cpp
--rw-r-----   0 dcunnin  (216460) eng       (5000)    26925 2016-03-01 00:39:53.000000 jsonnet-v0.8.7-pre5/core/desugarer.cpp
--rw-r-----   0 dcunnin  (216460) eng       (5000)      969 2016-03-01 00:39:53.000000 jsonnet-v0.8.7-pre5/core/string_utils.h
--rw-r-----   0 dcunnin  (216460) eng       (5000)     3907 2015-10-27 02:40:26.000000 jsonnet-v0.8.7-pre5/core/vm.h
--rw-r-----   0 dcunnin  (216460) eng       (5000)     5937 2016-03-01 00:39:53.000000 jsonnet-v0.8.7-pre5/core/static_analysis.cpp
--rw-r-----   0 dcunnin  (216460) eng       (5000)    25973 2016-03-01 00:39:53.000000 jsonnet-v0.8.7-pre5/core/lexer.cpp
--rw-r-----   0 dcunnin  (216460) eng       (5000)      878 2015-10-27 02:40:26.000000 jsonnet-v0.8.7-pre5/core/static_analysis.h
--rw-r--r--   0 dcunnin  (216460) eng       (5000)    15272 2015-10-30 02:07:04.000000 jsonnet-v0.8.7-pre5/core/state.h
--rw-r-----   0 dcunnin  (216460) eng       (5000)    67865 2016-03-01 00:39:53.000000 jsonnet-v0.8.7-pre5/core/formatter.cpp
--rw-r-----   0 dcunnin  (216460) eng       (5000)      766 2016-03-01 00:39:53.000000 jsonnet-v0.8.7-pre5/core/desugarer.h
--rw-r-----   0 dcunnin  (216460) eng       (5000)     1368 2016-03-01 00:39:53.000000 jsonnet-v0.8.7-pre5/core/formatter.h
--rw-r-----   0 dcunnin  (216460) eng       (5000)       59 2016-03-01 01:25:20.000000 jsonnet-v0.8.7-pre5/setup.cfg
-drwxr-x---   0 dcunnin  (216460) eng       (5000)        0 2016-03-01 01:25:20.000000 jsonnet-v0.8.7-pre5/stdlib/
--rw-r-----   0 dcunnin  (216460) eng       (5000)    39121 2016-02-29 20:24:10.000000 jsonnet-v0.8.7-pre5/stdlib/std.jsonnet
-drwxr-x---   0 dcunnin  (216460) eng       (5000)        0 2016-03-01 01:25:20.000000 jsonnet-v0.8.7-pre5/python/
--rw-r-----   0 dcunnin  (216460) eng       (5000)     7110 2016-03-01 01:08:17.000000 jsonnet-v0.8.7-pre5/python/_jsonnet.c
--rw-r-----   0 dcunnin  (216460) eng       (5000)    11358 2015-03-13 15:30:37.000000 jsonnet-v0.8.7-pre5/LICENSE
-drwxr-x---   0 dcunnin  (216460) eng       (5000)        0 2016-03-01 01:25:20.000000 jsonnet-v0.8.7-pre5/include/
--rw-r-----   0 dcunnin  (216460) eng       (5000)     8711 2016-03-01 01:25:19.000000 jsonnet-v0.8.7-pre5/include/libjsonnet.h
+drwxr-x---   0 dcunnin  (216460) eng       (5000)        0 2016-03-22 04:57:16.000000 jsonnet-v0.8.7-pre6/
+-rw-r-----   0 dcunnin  (216460) eng       (5000)     4496 2016-03-22 04:54:20.000000 jsonnet-v0.8.7-pre6/Makefile
+-rw-r-----   0 dcunnin  (216460) eng       (5000)      155 2015-10-27 02:40:26.000000 jsonnet-v0.8.7-pre6/MANIFEST.in
+drwxr-x---   0 dcunnin  (216460) eng       (5000)        0 2016-03-22 04:57:16.000000 jsonnet-v0.8.7-pre6/jsonnet.egg-info/
+-rw-r-----   0 dcunnin  (216460) eng       (5000)        1 2016-03-22 04:57:16.000000 jsonnet-v0.8.7-pre6/jsonnet.egg-info/dependency_links.txt
+-rw-r-----   0 dcunnin  (216460) eng       (5000)      271 2016-03-22 04:57:16.000000 jsonnet-v0.8.7-pre6/jsonnet.egg-info/PKG-INFO
+-rw-r-----   0 dcunnin  (216460) eng       (5000)        9 2016-03-22 04:57:16.000000 jsonnet-v0.8.7-pre6/jsonnet.egg-info/top_level.txt
+-rw-r-----   0 dcunnin  (216460) eng       (5000)      582 2016-03-22 04:57:16.000000 jsonnet-v0.8.7-pre6/jsonnet.egg-info/SOURCES.txt
+-rw-r-----   0 dcunnin  (216460) eng       (5000)      271 2016-03-22 04:57:16.000000 jsonnet-v0.8.7-pre6/PKG-INFO
+-rw-r-----   0 dcunnin  (216460) eng       (5000)     2116 2016-03-09 04:53:43.000000 jsonnet-v0.8.7-pre6/setup.py
+drwxr-x---   0 dcunnin  (216460) eng       (5000)        0 2016-03-22 04:57:16.000000 jsonnet-v0.8.7-pre6/core/
+-rw-r-----   0 dcunnin  (216460) eng       (5000)     1592 2016-03-09 04:53:43.000000 jsonnet-v0.8.7-pre6/core/parser.h
+-rw-r-----   0 dcunnin  (216460) eng       (5000)   107413 2016-03-09 04:53:43.000000 jsonnet-v0.8.7-pre6/core/vm.cpp
+-rw-r-----   0 dcunnin  (216460) eng       (5000)     5268 2015-10-27 02:40:26.000000 jsonnet-v0.8.7-pre6/core/unicode.h
+-rw-r-----   0 dcunnin  (216460) eng       (5000)     5035 2016-03-09 04:53:43.000000 jsonnet-v0.8.7-pre6/core/string_utils.cpp
+-rw-r-----   0 dcunnin  (216460) eng       (5000)    15788 2016-03-22 04:54:20.000000 jsonnet-v0.8.7-pre6/core/libjsonnet.cpp
+-rw-r-----   0 dcunnin  (216460) eng       (5000)     6860 2016-03-22 04:54:20.000000 jsonnet-v0.8.7-pre6/core/lexer.h
+-rw-r-----   0 dcunnin  (216460) eng       (5000)    27787 2016-03-09 04:53:43.000000 jsonnet-v0.8.7-pre6/core/ast.h
+-rw-r-----   0 dcunnin  (216460) eng       (5000)     2920 2016-03-22 04:54:20.000000 jsonnet-v0.8.7-pre6/core/static_error.h
+-rw-r-----   0 dcunnin  (216460) eng       (5000)    40950 2016-03-12 07:58:42.000000 jsonnet-v0.8.7-pre6/core/parser.cpp
+-rw-r-----   0 dcunnin  (216460) eng       (5000)    28357 2016-03-12 01:55:42.000000 jsonnet-v0.8.7-pre6/core/desugarer.cpp
+-rw-r-----   0 dcunnin  (216460) eng       (5000)      969 2016-03-09 04:53:43.000000 jsonnet-v0.8.7-pre6/core/string_utils.h
+-rw-r-----   0 dcunnin  (216460) eng       (5000)     5092 2016-03-09 04:53:43.000000 jsonnet-v0.8.7-pre6/core/vm.h
+-rw-r-----   0 dcunnin  (216460) eng       (5000)     5937 2016-03-09 04:53:43.000000 jsonnet-v0.8.7-pre6/core/static_analysis.cpp
+-rw-r-----   0 dcunnin  (216460) eng       (5000)   131144 2016-03-10 18:46:41.000000 jsonnet-v0.8.7-pre6/core/std.jsonnet.h
+-rw-r-----   0 dcunnin  (216460) eng       (5000)    25882 2016-03-13 22:01:46.000000 jsonnet-v0.8.7-pre6/core/lexer.cpp
+-rw-r-----   0 dcunnin  (216460) eng       (5000)      878 2015-10-27 02:40:26.000000 jsonnet-v0.8.7-pre6/core/static_analysis.h
+-rw-r--r--   0 dcunnin  (216460) eng       (5000)    15272 2015-10-30 02:07:04.000000 jsonnet-v0.8.7-pre6/core/state.h
+-rw-r-----   0 dcunnin  (216460) eng       (5000)    67865 2016-03-09 04:53:43.000000 jsonnet-v0.8.7-pre6/core/formatter.cpp
+-rw-r-----   0 dcunnin  (216460) eng       (5000)      766 2016-03-09 04:53:43.000000 jsonnet-v0.8.7-pre6/core/desugarer.h
+-rw-r-----   0 dcunnin  (216460) eng       (5000)     1368 2016-03-09 04:53:43.000000 jsonnet-v0.8.7-pre6/core/formatter.h
+-rw-r-----   0 dcunnin  (216460) eng       (5000)       59 2016-03-22 04:57:16.000000 jsonnet-v0.8.7-pre6/setup.cfg
+drwxr-x---   0 dcunnin  (216460) eng       (5000)        0 2016-03-22 04:57:16.000000 jsonnet-v0.8.7-pre6/stdlib/
+-rw-r-----   0 dcunnin  (216460) eng       (5000)    38676 2016-03-22 04:54:20.000000 jsonnet-v0.8.7-pre6/stdlib/std.jsonnet
+drwxr-x---   0 dcunnin  (216460) eng       (5000)        0 2016-03-22 04:57:16.000000 jsonnet-v0.8.7-pre6/python/
+-rw-r-----   0 dcunnin  (216460) eng       (5000)     7110 2016-03-09 04:53:43.000000 jsonnet-v0.8.7-pre6/python/_jsonnet.c
+-rw-r-----   0 dcunnin  (216460) eng       (5000)    11358 2015-03-13 15:30:37.000000 jsonnet-v0.8.7-pre6/LICENSE
+drwxr-x---   0 dcunnin  (216460) eng       (5000)        0 2016-03-22 04:57:16.000000 jsonnet-v0.8.7-pre6/include/
+-rw-r-----   0 dcunnin  (216460) eng       (5000)    10021 2016-03-22 04:57:15.000000 jsonnet-v0.8.7-pre6/include/libjsonnet.h
+-rw-r-----   0 dcunnin  (216460) eng       (5000)     5233 2016-03-22 04:54:20.000000 jsonnet-v0.8.7-pre6/include/libjsonnet++.h
```

### Comparing `jsonnet-v0.8.7-pre5/Makefile` & `jsonnet-v0.8.7-pre6/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -46,37 +46,46 @@
 	core/formatter.cpp \
 	core/lexer.cpp \
 	core/libjsonnet.cpp \
 	core/parser.cpp \
 	core/static_analysis.cpp \
 	core/string_utils.cpp \
 	core/vm.cpp
+
 LIB_OBJ = $(LIB_SRC:.cpp=.o)
 
+LIB_CPP_SRC = \
+	cpp/libjsonnet++.cc
+
+LIB_CPP_OBJ = $(LIB_OBJ) $(LIB_CPP_SRC:.cc=.o)
+
 ALL = \
 	jsonnet \
 	libjsonnet.so \
+	libjsonnet++.so \
 	libjsonnet_test_snippet \
 	libjsonnet_test_file \
 	libjsonnet.js \
 	doc/js/libjsonnet.js \
 	$(LIB_OBJ)
+
 ALL_HEADERS = \
 	core/ast.h \
 	core/desugarer.h \
 	core/formatter.h \
 	core/lexer.h \
 	core/parser.h \
 	core/state.h \
 	core/static_analysis.h \
 	core/static_error.h \
 	core/string_utils.h \
 	core/vm.h \
 	core/std.jsonnet.h \
-	include/libjsonnet.h
+	include/libjsonnet.h \
+	include/libjsonnet++.h
 
 default: jsonnet
 
 all: $(ALL)
 
 TEST_SNIPPET = "std.assertEqual(({ x: 1, y: self.x } { x: 2 }).y, 2)"
 test: jsonnet libjsonnet.so libjsonnet_test_snippet libjsonnet_test_file
@@ -87,33 +96,41 @@
 	cd examples/terraform ; ./check.sh
 	cd test_suite ; ./run_tests.sh
 	cd test_suite ; ./run_fmt_tests.sh
 
 MAKEDEPEND_SRCS = \
 	cmd/jsonnet.cpp \
 	core/libjsonnet_test_snippet.c \
-	core/libjsonnet_test_file.c
+	core/libjsonnet_test_file.c \
+	cpp/libjsonnet_cpp_test_snippet.c \
+	cpp/libjsonnet_cpp_test_file.c
 
 depend:
 	makedepend -f- $(LIB_SRC) $(MAKEDEPEND_SRCS) > Makefile.depend
 
 core/desugarer.cpp: core/std.jsonnet.h
 
 # Object files
 %.o: %.cpp
 	$(CXX) -c $(CXXFLAGS) $< -o $@
 
+%.o: %.cc
+	$(CXX) -c $(CXXFLAGS) $< -o $@
+
 # Commandline executable.
 jsonnet: cmd/jsonnet.cpp $(LIB_OBJ)
 	$(CXX) $(CXXFLAGS) $(LDFLAGS) $< $(LIB_SRC:.cpp=.o) -o $@
 
 # C binding.
 libjsonnet.so: $(LIB_OBJ)
 	$(CXX) $(LDFLAGS) $(LIB_OBJ) $(SHARED_LDFLAGS) -o $@
 
+libjsonnet++.so: $(LIB_CPP_OBJ)
+	$(CXX) $(LDFLAGS) $(LIB_CPP_OBJ) $(SHARED_LDFLAGS) -o $@
+
 # Javascript build of C binding
 JS_EXPORTED_FUNCTIONS = 'EXPORTED_FUNCTIONS=["_jsonnet_make", "_jsonnet_evaluate_snippet", "_jsonnet_realloc", "_jsonnet_destroy"]'
 
 libjsonnet.js: $(LIB_SRC) $(ALL_HEADERS)
 	$(EMCXX) -s $(JS_EXPORTED_FUNCTIONS) $(EMCXXFLAGS) $(LDFLAGS) $(LIB_SRC) -o $@
 
 # Copy javascript build to doc directory
```

### Comparing `jsonnet-v0.8.7-pre5/jsonnet.egg-info/SOURCES.txt` & `jsonnet-v0.8.7-pre6/jsonnet.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 core/libjsonnet.cpp
 core/parser.cpp
 core/parser.h
 core/state.h
 core/static_analysis.cpp
 core/static_analysis.h
 core/static_error.h
+core/std.jsonnet.h
 core/string_utils.cpp
 core/string_utils.h
 core/unicode.h
 core/vm.cpp
 core/vm.h
+include/libjsonnet++.h
 include/libjsonnet.h
 jsonnet.egg-info/PKG-INFO
 jsonnet.egg-info/SOURCES.txt
 jsonnet.egg-info/dependency_links.txt
 jsonnet.egg-info/top_level.txt
 python/_jsonnet.c
 stdlib/std.jsonnet
```

### Comparing `jsonnet-v0.8.7-pre5/setup.py` & `jsonnet-v0.8.7-pre6/setup.py`

 * *Files identical despite different names*

### Comparing `jsonnet-v0.8.7-pre5/core/parser.h` & `jsonnet-v0.8.7-pre6/core/parser.h`

 * *Files identical despite different names*

### Comparing `jsonnet-v0.8.7-pre5/core/vm.cpp` & `jsonnet-v0.8.7-pre6/core/vm.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -2288,14 +2288,50 @@
                 scratch = stack.top().val;
                 stack.pop();
                 r[encode_utf8(f.first)] = encode_utf8(vstr);
             }
             return r;
         }
 
+        std::vector<std::string> manifestStream(void)
+        {
+            std::vector<std::string> r;
+            LocationRange loc("During manifestation");
+            if (scratch.t != Value::ARRAY) {
+                std::stringstream ss;
+                ss << "Stream mode: Top-level object was a " << type_str(scratch.t) << ", "
+                   << "should be an array whose elements hold "
+                   << "the JSON for each document in the stream.";
+                throw makeError(loc, ss.str());
+            }
+            auto *arr = static_cast<HeapArray*>(scratch.v.h);
+            for (auto *thunk : arr->elements) {
+                LocationRange tloc = thunk->body == nullptr
+                                   ? loc
+                                   : thunk->body->location;
+                if (thunk->filled) {
+                    stack.newCall(loc, thunk, nullptr, 0, BindingFrame{});
+                    // Keep arr alive when scratch is overwritten
+                    stack.top().val = scratch;
+                    scratch = thunk->content;
+                } else {
+                    stack.newCall(loc, thunk,
+                                  thunk->self, thunk->offset, thunk->upValues);
+                    // Keep arr alive when scratch is overwritten
+                    stack.top().val = scratch;
+                    evaluate(thunk->body, stack.size());
+                }
+                String element = manifestJson(tloc, true, U"");
+                scratch = stack.top().val;
+                stack.pop();
+                r.push_back(encode_utf8(element));
+            }
+            return r;
+        }
+
     };
 
 }
 
 std::string jsonnet_vm_execute(Allocator *alloc, const AST *ast,
                                const ExtMap &ext_vars,
                                unsigned max_stack, double gc_min_objects,
@@ -2320,7 +2356,18 @@
 {
     Interpreter vm(alloc, ext_vars, max_stack, gc_min_objects, gc_growth_trigger,
                    import_callback, ctx);
     vm.evaluate(ast, 0);
     return vm.manifestMulti(string_output);
 }
 
+std::vector<std::string> jsonnet_vm_execute_stream(
+  Allocator *alloc, const AST *ast, const ExtMap &ext_vars, unsigned max_stack,
+  double gc_min_objects, double gc_growth_trigger, JsonnetImportCallback *import_callback,
+  void *ctx)
+{
+    Interpreter vm(alloc, ext_vars, max_stack, gc_min_objects, gc_growth_trigger,
+                   import_callback, ctx);
+    vm.evaluate(ast, 0);
+    return vm.manifestStream();
+}
+
```

### Comparing `jsonnet-v0.8.7-pre5/core/unicode.h` & `jsonnet-v0.8.7-pre6/core/unicode.h`

 * *Files identical despite different names*

### Comparing `jsonnet-v0.8.7-pre5/core/string_utils.cpp` & `jsonnet-v0.8.7-pre6/core/string_utils.cpp`

 * *Files identical despite different names*

### Comparing `jsonnet-v0.8.7-pre5/core/libjsonnet.cpp` & `jsonnet-v0.8.7-pre6/core/libjsonnet.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     JsonnetImportCallback *importCallback;
     void *importCallbackContext;
     bool stringOutput;
     std::vector<std::string> jpaths;
 
     FmtOpts fmtOpts;
     bool fmtDebugDesugaring;
-    
+
     JsonnetVm(void)
       : gcGrowthTrigger(2.0), maxStack(500), gcMinObjects(1000), maxTrace(20),
         importCallback(default_import_callback), importCallbackContext(this), stringOutput(false),
         fmtDebugDesugaring(false)
     {
         jpaths.emplace_back("/usr/share/" + std::string(jsonnet_version()) + "/");
         jpaths.emplace_back("/usr/local/share/" + std::string(jsonnet_version()) + "/");
@@ -337,67 +337,98 @@
     TRY
         return jsonnet_fmt_snippet_aux(vm, filename, snippet, error);
     CATCH("jsonnet_fmt_snippet")
     return nullptr;  // Never happens.
 }
 
 
+namespace {
+  enum EvalKind { REGULAR, MULTI, STREAM };
+}
+
 static char *jsonnet_evaluate_snippet_aux(JsonnetVm *vm, const char *filename,
-                                          const char *snippet, int *error, bool multi)
+                                          const char *snippet, int *error, EvalKind kind)
 {
     try {
         Allocator alloc;
-        std::string json_str;
         AST *expr;
-        std::map<std::string, std::string> files;
         Tokens tokens = jsonnet_lex(filename, snippet);
 
         expr = jsonnet_parse(&alloc, tokens);
 
         jsonnet_desugar(&alloc, expr);
 
         jsonnet_static_analysis(expr);
-        if (multi) {
-            files = jsonnet_vm_execute_multi(&alloc, expr, vm->ext, vm->maxStack,
-                                             vm->gcMinObjects, vm->gcGrowthTrigger,
-                                             vm->importCallback, vm->importCallbackContext,
-                                             vm->stringOutput);
-        } else {
-            json_str = jsonnet_vm_execute(&alloc, expr, vm->ext, vm->maxStack,
-                                          vm->gcMinObjects, vm->gcGrowthTrigger,
-                                          vm->importCallback, vm->importCallbackContext,
-                                          vm->stringOutput);
-            json_str += "\n";
-        }
+        switch (kind) {
+            case REGULAR: {
+                std::string json_str = jsonnet_vm_execute(
+                    &alloc, expr, vm->ext, vm->maxStack, vm->gcMinObjects, vm->gcGrowthTrigger,
+                    vm->importCallback, vm->importCallbackContext, vm->stringOutput);
+                json_str += "\n";
+                *error = false;
+                return from_string(vm, json_str);
+            }
+            break;
 
-        if (multi) {
-            size_t sz = 1; // final sentinel
-            for (const auto &pair : files) {
-                sz += pair.first.length() + 1; // include sentinel
-                sz += pair.second.length() + 2; // Add a '\n' as well as sentinel
+            case MULTI: {
+                std::map<std::string, std::string> files = jsonnet_vm_execute_multi(
+                    &alloc, expr, vm->ext, vm->maxStack, vm->gcMinObjects, vm->gcGrowthTrigger,
+                    vm->importCallback, vm->importCallbackContext, vm->stringOutput);
+                size_t sz = 1; // final sentinel
+                for (const auto &pair : files) {
+                    sz += pair.first.length() + 1; // include sentinel
+                    sz += pair.second.length() + 2; // Add a '\n' as well as sentinel
+                }
+                char *buf = (char*)::malloc(sz);
+                if (buf == nullptr) memory_panic();
+                std::ptrdiff_t i = 0;
+                for (const auto &pair : files) {
+                    memcpy(&buf[i], pair.first.c_str(), pair.first.length() + 1);
+                    i += pair.first.length() + 1;
+                    memcpy(&buf[i], pair.second.c_str(), pair.second.length());
+                    i += pair.second.length();
+                    buf[i] = '\n';
+                    i++;
+                    buf[i] = '\0';
+                    i++;
+                }
+                buf[i] = '\0'; // final sentinel
+                *error = false;
+                return buf;
             }
-            char *buf = (char*)::malloc(sz);
-            if (buf == nullptr) memory_panic();
-            std::ptrdiff_t i = 0;
-            for (const auto &pair : files) {
-                memcpy(&buf[i], pair.first.c_str(), pair.first.length() + 1);
-                i += pair.first.length() + 1;
-                memcpy(&buf[i], pair.second.c_str(), pair.second.length());
-                i += pair.second.length();
-                buf[i] = '\n';
-                i++;
-                buf[i] = '\0';
-                i++;
+            break;
+
+            case STREAM: {
+                std::vector<std::string> documents = jsonnet_vm_execute_stream(
+                    &alloc, expr, vm->ext, vm->maxStack, vm->gcMinObjects, vm->gcGrowthTrigger,
+                    vm->importCallback, vm->importCallbackContext);
+                size_t sz = 1; // final sentinel
+                for (const auto &doc : documents) {
+                    sz += doc.length() + 2; // Add a '\n' as well as sentinel
+                }
+                char *buf = (char*)::malloc(sz);
+                if (buf == nullptr) memory_panic();
+                std::ptrdiff_t i = 0;
+                for (const auto &doc : documents) {
+                    memcpy(&buf[i], doc.c_str(), doc.length());
+                    i += doc.length();
+                    buf[i] = '\n';
+                    i++;
+                    buf[i] = '\0';
+                    i++;
+                }
+                buf[i] = '\0'; // final sentinel
+                *error = false;
+                return buf;
             }
-            buf[i] = '\0'; // final sentinel
-            *error = false;
-            return buf;
-        } else {
-            *error = false;
-            return from_string(vm, json_str);
+            break;
+
+            default:
+            fputs("INTERNAL ERROR: bad value of 'kind', probably memory corruption.\n", stderr);
+            abort();
         }
 
     } catch (StaticError &e) {
         std::stringstream ss;
         ss << "STATIC ERROR: " << e << std::endl;
         *error = true;
         return from_string(vm, ss.str());
@@ -419,64 +450,81 @@
         }
         *error = true;
         return from_string(vm, ss.str());
     }
 
 }
 
-static char *jsonnet_evaluate_file_aux(JsonnetVm *vm, const char *filename, int *error, bool multi)
+static char *jsonnet_evaluate_file_aux(JsonnetVm *vm, const char *filename, int *error, EvalKind kind)
 {
     std::ifstream f;
     f.open(filename);
     if (!f.good()) {
         std::stringstream ss;
         ss << "Opening input file: " << filename << ": " << strerror(errno);
         *error = true;
         return from_string(vm, ss.str());
     }
     std::string input;
     input.assign(std::istreambuf_iterator<char>(f),
                  std::istreambuf_iterator<char>());
 
-    return jsonnet_evaluate_snippet_aux(vm, filename, input.c_str(), error, multi);
+    return jsonnet_evaluate_snippet_aux(vm, filename, input.c_str(), error, kind);
 }
 
 char *jsonnet_evaluate_file(JsonnetVm *vm, const char *filename, int *error)
 {
     TRY
-    return jsonnet_evaluate_file_aux(vm, filename, error, false);
+    return jsonnet_evaluate_file_aux(vm, filename, error, REGULAR);
     CATCH("jsonnet_evaluate_file")
     return nullptr;  // Never happens.
 }
 
 char *jsonnet_evaluate_file_multi(JsonnetVm *vm, const char *filename, int *error)
 {
     TRY
-    return jsonnet_evaluate_file_aux(vm, filename, error, true);
+    return jsonnet_evaluate_file_aux(vm, filename, error, MULTI);
     CATCH("jsonnet_evaluate_file_multi")
     return nullptr;  // Never happens.
 }
 
+char *jsonnet_evaluate_file_stream(JsonnetVm *vm, const char *filename, int *error)
+{
+    TRY
+    return jsonnet_evaluate_file_aux(vm, filename, error, STREAM);
+    CATCH("jsonnet_evaluate_file_stream")
+    return nullptr;  // Never happens.
+}
+
 char *jsonnet_evaluate_snippet(JsonnetVm *vm, const char *filename, const char *snippet, int *error)
 {
     TRY
-    return jsonnet_evaluate_snippet_aux(vm, filename, snippet, error, false);
+    return jsonnet_evaluate_snippet_aux(vm, filename, snippet, error, REGULAR);
     CATCH("jsonnet_evaluate_snippet")
     return nullptr;  // Never happens.
 }
 
 char *jsonnet_evaluate_snippet_multi(JsonnetVm *vm, const char *filename,
                                      const char *snippet, int *error)
 {
     TRY
-    return jsonnet_evaluate_snippet_aux(vm, filename, snippet, error, true);
+    return jsonnet_evaluate_snippet_aux(vm, filename, snippet, error, MULTI);
     CATCH("jsonnet_evaluate_snippet_multi")
     return nullptr;  // Never happens.
 }
 
+char *jsonnet_evaluate_snippet_stream(JsonnetVm *vm, const char *filename,
+                                     const char *snippet, int *error)
+{
+    TRY
+    return jsonnet_evaluate_snippet_aux(vm, filename, snippet, error, STREAM);
+    CATCH("jsonnet_evaluate_snippet_stream")
+    return nullptr;  // Never happens.
+}
+
 char *jsonnet_realloc(JsonnetVm *vm, char *str, size_t sz)
 {
     (void) vm;
     if (str == nullptr) {
         if (sz == 0) return nullptr;
         auto *r = static_cast<char*>(::malloc(sz));
         if (r == nullptr) memory_panic();
```

### Comparing `jsonnet-v0.8.7-pre5/core/lexer.h` & `jsonnet-v0.8.7-pre6/core/lexer.h`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     /** Content of the token if it wasn't a keyword. */
     std::string data;
 
     /** If kind == STRING_BLOCK then stores the sequence of whitespace that indented the block. */
     std::string stringBlockIndent;
 
     /** If kind == STRING_BLOCK then stores the sequence of whitespace that indented the end of
-     * the block. 
+     * the block.
      *
      * This is always fewer whitespace characters than in stringBlockIndent.
      */
     std::string stringBlockTermIndent;
 
     String data32(void) { return decode_utf8(data); }
 
@@ -149,15 +149,16 @@
     Token(Kind kind, const Fodder &fodder, const std::string &data,
           const std::string &string_block_indent, const std::string &string_block_term_indent,
           const LocationRange &location)
       : kind(kind), fodder(fodder), data(data), stringBlockIndent(string_block_indent),
         stringBlockTermIndent(string_block_term_indent), location(location)
     { }
 
-    //Token(Kind kind, const std::string &data="") : kind(kind), data(data) { }
+    Token(Kind kind, const std::string &data="")
+        : kind(kind), data(data) { }
 
     static const char *toString(Kind v)
     {
         switch (v) {
             case BRACE_L: return "\"{\"";
             case BRACE_R: return "\"}\"";
             case BRACKET_L: return "\"[\"";
@@ -200,15 +201,15 @@
             std::cerr << "INTERNAL ERROR: Unknown token kind: " << v << std::endl;
             std::abort();
         }
     }
 };
 
 /** The result of lexing.
- * 
+ *
  * Because of the EOF token, this will always contain at least one token.  So element 0 can be used
  * to get the filename.
  */
 typedef std::list<Token> Tokens;
 
 static inline bool operator==(const Token &a, const Token &b)
 {
```

### Comparing `jsonnet-v0.8.7-pre5/core/ast.h` & `jsonnet-v0.8.7-pre6/core/ast.h`

 * *Files identical despite different names*

### Comparing `jsonnet-v0.8.7-pre5/core/static_error.h` & `jsonnet-v0.8.7-pre6/core/static_error.h`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 */
 
 #ifndef JSONNET_STATIC_ERROR_H
 #define JSONNET_STATIC_ERROR_H
 
+#include <iostream>
+#include <sstream>
+
 struct Location {
     unsigned long line;
     unsigned long column;
     Location(void)
       : line(0), column(0)
     { }
     Location(unsigned long line_number, unsigned long column)
@@ -87,19 +90,26 @@
       : location(filename, location, location), msg(msg)
     {
     }
     StaticError(const LocationRange &location, const std::string &msg)
       : location(location), msg(msg)
     {
     }
+
+    std::string toString() const
+    {
+        std::stringstream ss;
+        if (location.isSet()) {
+            ss << location << ":";
+        }
+        ss << " " << msg;
+        return ss.str();
+    }
 };
 
 static inline std::ostream &operator<<(std::ostream &o, const StaticError &err)
 {
-    if (err.location.isSet()) {
-        o << err.location << ":";
-    }
-    o << " " << err.msg;
+    o << err.toString();
     return o;
 }
 
 #endif  // JSONNET_ERROR_H
```

### Comparing `jsonnet-v0.8.7-pre5/core/parser.cpp` & `jsonnet-v0.8.7-pre6/core/parser.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -183,17 +183,16 @@
             Token paren_r = parseCommaList(exprs, Token::PAREN_R, element_kind, got_comma);
 
             // Check they're all identifiers
             Params ret;
             for (const auto &p_ast_fodder : exprs) {
                 auto *p = dynamic_cast<Var*>(p_ast_fodder.first);
                 if (p == nullptr) {
-                    std::stringstream ss;
-                    ss << "Not an identifier: " << p_ast_fodder.first;
-                    throw StaticError(p_ast_fodder.first->location, ss.str());
+                    throw StaticError(p_ast_fodder.first->location,
+                                      "Expected an identifier but got a complex expression.");
                 }
                 ret.emplace_back(p->openFodder, p->id, p_ast_fodder.second);
             }
 
             close_fodder = paren_r.fodder;
 
             return ret;
@@ -850,20 +849,30 @@
                         AST *second = nullptr;
                         Fodder third_fodder;
                         AST *third = nullptr;
 
                         if (peek().kind == Token::BRACKET_R)
                             throw unexpected(pop(), "parsing index");
 
+                        // break up "::" into ":", ":" before we start parsing.
+                        if (peek().kind == Token::OPERATOR && peek().data == "::") {
+                            Token joined = pop();
+                            push(Token(Token::OPERATOR, joined.fodder, ":", "", "",
+                                       joined.location));
+                            push(Token(Token::OPERATOR, Fodder{}, ":", "", "", joined.location));
+                        }
+
+                        Token first_token = pop();
                         if (peek().kind == Token::OPERATOR && peek().data == "::") {
                             Token joined = pop();
                             push(Token(Token::OPERATOR, joined.fodder, ":", "", "",
                                        joined.location));
                             push(Token(Token::OPERATOR, Fodder{}, ":", "", "", joined.location));
                         }
+                        push(first_token);
 
                         if (peek().data != ":")
                             first = parse(MAX_PRECEDENCE);
 
                         if (peek().kind != Token::BRACKET_R) {
                             is_slice = true;
                             Token delim = pop();
```

### Comparing `jsonnet-v0.8.7-pre5/core/desugarer.cpp` & `jsonnet-v0.8.7-pre6/core/desugarer.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,17 @@
 
     const Identifier *id(const String &s)
     { return alloc->makeIdentifier(s); }
 
     LiteralString *str(const String &s)
     { return make<LiteralString>(E, EF, s, LiteralString::DOUBLE, "", ""); }
 
+    LiteralString *str(const LocationRange &loc, const String &s)
+    { return make<LiteralString>(loc, EF, s, LiteralString::DOUBLE, "", ""); }
+
     Var *var(const Identifier *ident)
     { return make<Var>(E, EF, ident); }
 
     Var *std(void)
     { return var(id(U"std")); }
 
     
@@ -107,29 +110,69 @@
 
     Array *singleton(AST *body)
     {
         return make<Array>(body->location, EF, Array::Elements{Array::Element(body, EF)},
                            false, EF);
     }
 
-    Apply *length(AST *v)
+    Apply *stdFunc(const String &name, AST *v)
     {
         return make<Apply>(
             v->location, 
             EF,
-            make<Index>(E, EF, std(), EF, false, str(U"length"), EF, nullptr, EF, nullptr, EF),
+            make<Index>(E, EF, std(), EF, false, str(name), EF, nullptr, EF, nullptr, EF),
             EF,
             Apply::Args{{v, EF}},
             false,  // trailingComma
             EF,
             EF,
             true  // tailstrict
         );
     }
 
+    Apply *stdFunc(const LocationRange &loc, const String &name, AST *a, AST *b)
+    {
+        return make<Apply>(
+            loc, 
+            EF,
+            make<Index>(E, EF, std(), EF, false, str(name), EF, nullptr, EF, nullptr, EF),
+            EF,
+            Apply::Args{{a, EF}, {b, EF}},
+            false,  // trailingComma
+            EF,
+            EF,
+            true  // tailstrict
+        );
+    }
+
+    Apply *length(AST *v)
+    {
+        return stdFunc(U"length", v);
+    }
+
+    Apply *type(AST *v)
+    {
+        return stdFunc(U"type", v);
+    }
+
+    Apply *equals(const LocationRange &loc, AST *a, AST *b)
+    {
+        return stdFunc(loc, U"equals", a, b);
+    }
+
+    Error *error(AST *msg)
+    {
+        return alloc->make<Error>(msg->location, EF, msg);
+    }
+
+    Error *error(const LocationRange &loc, const String &msg)
+    {
+        return error(str(loc, msg));
+    }
+
     public:
     Desugarer(Allocator *alloc)
       : alloc(alloc)
     { }
 
     void desugarFields(AST *ast, ObjectFields &fields, unsigned obj_level)
     {
@@ -155,15 +198,15 @@
             field.expr2 = alloc->make<Conditional>(
                 ast->location,
                 EF,
                 field.expr2,
                 EF,
                 alloc->make<LiteralBoolean>(E, EF, true),
                 EF,
-                alloc->make<Error>(msg->location, EF, msg));
+                error(msg));
         }
 
         // Remove methods
         for (auto &field : fields) {
             if (!field.methodSugar) continue;
             field.expr2 = alloc->make<Function>(
                 field.expr2->location, EF, field.fodderL, field.params, field.trailingComma,
@@ -328,28 +371,31 @@
                             EF,
                             in,  // True branch.
                             EF,
                             out);  // False branch.
                     } break;
                     case ComprehensionSpec::FOR: {
                         /*
-                            local $l = [[[...array...]]];
-                            local aux_{i}(i_{i}, r) =
-                                if i_{i} >= std.length(l) then
+                            local $l = [[[...array...]]]
+                                  aux_{i}(i_{i}, r) =
+                                if i_{i} >= std.length($l) then
                                     [[[...out...]]]
                                 else
-                                    local [[[...var...]]] = l[i_{i}];
-                                    [[[...in...]]]
-                            aux_{i}(0, r) tailstrict;
+                                    local [[[...var...]]] = $l[i_{i}];
+                                    [[[...in...]]];`
+                            if std.type($l) != "array" then
+                                error "In comprehension, can only iterate over array.."
+                            else
+                                aux_{i}(0, r) tailstrict;
                         */
                         in = make<Local>(
                             ast->location,
                             EF,
                             Local::Binds {
-                                bind(_l, spec.expr),
+                                bind(_l, spec.expr),  // Need to check expr is an array
                                 bind(_aux[i], make<Function>(
                                     ast->location,
                                     EF,
                                     EF,
                                     std::vector<Param>{Param(EF, _i[i], EF), Param(EF, _r, EF)},
                                     false,  // trailingComma
                                     EF,
@@ -368,31 +414,40 @@
                                                 spec.var,
                                                 make<Index>(E, EF, var(_l), EF, false, var(_i[i]),
                                                             EF, nullptr, EF, nullptr, EF)
                                             ),
                                             in)
                                     )
                                 ))},
-                            make<Apply>(
-                                E,
+                            make<Conditional>(
+                                ast->location, 
                                 EF,
-                                var(_aux[i]),
-                                EF,
-                                Apply::Args {
-                                    {zero, EF},
-                                    {
-                                        i == 0 ? make<Array>(E, EF, Array::Elements{}, false, EF)
-                                               : static_cast<AST*>(var(_r)),
-                                        EF,
-                                    }
-                                },
-                                false,  // trailingComma
+                                equals(ast->location, type(var(_l)), str(U"array")),
                                 EF,
+                                make<Apply>(
+                                    E,
+                                    EF,
+                                    var(_aux[i]),
+                                    EF,
+                                    Apply::Args {
+                                        {zero, EF},
+                                        {
+                                            i == 0
+                                            ? make<Array>(E, EF, Array::Elements{}, false, EF)
+                                            : static_cast<AST*>(var(_r)),
+                                            EF,
+                                        }
+                                    },
+                                    false,  // trailingComma
+                                    EF,
+                                    EF,
+                                    true),  // tailstrict
                                 EF,
-                                true));  // tailstrict
+                                error(ast->location,
+                                      U"In comprehension, can only iterate over array.")));
                     } break;
                 }
             }
 
             ast_ = in;
 
         } else if (auto *ast = dynamic_cast<Assert*>(ast_)) {
@@ -422,19 +477,15 @@
                     ast_ = alloc->make<Apply>(ast->location, ast->openFodder, f_mod, EF, args,
                                               false, EF, EF, false);
                 } break;
 
                 case BOP_MANIFEST_UNEQUAL:
                 invert = true;
                 case BOP_MANIFEST_EQUAL: {
-                    AST *f_equals = alloc->make<Index>(E, EF, std(), EF, false, str(U"equals"), EF,
-                                                       nullptr, EF, nullptr, EF);
-                    Apply::Args args = {{ast->left, EF}, {ast->right, EF}};
-                    ast_ = alloc->make<Apply>(ast->location, ast->openFodder,
-                                              f_equals, EF, args, false, EF, EF, false);
+                    ast_ = equals(ast->location, ast->left, ast->right);
                     if (invert)
                         ast_ = alloc->make<Unary>(ast->location, ast->openFodder, UOP_NOT, ast_);
                 }
                 break;
 
                 default:;
                 // Otherwise don't change it.
@@ -465,14 +516,15 @@
         } else if (dynamic_cast<const Import*>(ast_)) {
             // Nothing to do.
 
         } else if (dynamic_cast<const Importstr*>(ast_)) {
             // Nothing to do.
 
         } else if (auto *ast = dynamic_cast<Index*>(ast_)) {
+            desugar(ast->target, obj_level);
             if (ast->isSlice) {
                 if (ast->index == nullptr)
                     ast->index = make<LiteralNull>(ast->location, EF);
                 desugar(ast->index, obj_level);
 
                 if (ast->end == nullptr)
                     ast->end = make<LiteralNull>(ast->location, EF);
@@ -496,15 +548,14 @@
                     },
                     false,  // trailing comma
                     EF,
                     EF,
                     false  // tailstrict
                 );
             } else {
-                desugar(ast->target, obj_level);
                 if (ast->id != nullptr) {
                     assert(ast->index == nullptr);
                     ast->index = str(ast->id->name);
                     ast->id = nullptr;
                 }
                 desugar(ast->index, obj_level);
             }
```

### Comparing `jsonnet-v0.8.7-pre5/core/string_utils.h` & `jsonnet-v0.8.7-pre6/core/string_utils.h`

 * *Files identical despite different names*

### Comparing `jsonnet-v0.8.7-pre5/core/vm.h` & `jsonnet-v0.8.7-pre6/core/vm.h`

 * *Files 15% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 std::string jsonnet_vm_execute(Allocator *alloc, const AST *ast,
                                const std::map<std::string, VmExt> &ext,
                                unsigned max_stack, double gc_min_objects,
                                double gc_growth_trigger,
                                JsonnetImportCallback *import_callback, void *import_callback_ctx,
                                bool string_output);
 
-/** Execute the program and return the value as a number of JSON files.
+/** Execute the program and return the value as a number of named JSON files.
  *
  * This assumes the given program yields an object whose keys are filenames.
  *
  * \param alloc The allocator used to create the ast.
  * \param ast The program to execute.
  * \param ext The external vars / code.
  * \param max_stack Recursion beyond this level gives an error.
@@ -91,8 +91,30 @@
  */
 std::map<std::string, std::string> jsonnet_vm_execute_multi(
     Allocator *alloc, const AST *ast, const std::map<std::string, VmExt> &ext,
     unsigned max_stack, double gc_min_objects, double gc_growth_trigger,
     JsonnetImportCallback *import_callback, void *import_callback_ctx,
     bool string_output);
 
+/** Execute the program and return the value as a stream of JSON files.
+ *
+ * This assumes the given program yields an array whose elements are individual
+ * JSON files.
+ *
+ * \param alloc The allocator used to create the ast.
+ * \param ast The program to execute.
+ * \param ext The external vars / code.
+ * \param max_stack Recursion beyond this level gives an error.
+ * \param gc_min_objects The garbage collector does not run when the heap is this small.
+ * \param gc_growth_trigger Growth since last garbage collection cycle to trigger a new cycle.
+ * \param import_callback A callback to handle imports
+ * \param import_callback_ctx Context param for the import callback.
+ * \param output_string Whether to expect a string and output it without JSON encoding
+ * \throws RuntimeError reports runtime errors in the program.
+ * \returns A mapping from filename to the JSON strings for that file.
+ */
+std::vector<std::string> jsonnet_vm_execute_stream(
+    Allocator *alloc, const AST *ast, const std::map<std::string, VmExt> &ext,
+    unsigned max_stack, double gc_min_objects, double gc_growth_trigger,
+    JsonnetImportCallback *import_callback, void *import_callback_ctx);
+
 #endif
```

### Comparing `jsonnet-v0.8.7-pre5/core/static_analysis.cpp` & `jsonnet-v0.8.7-pre6/core/static_analysis.cpp`

 * *Files identical despite different names*

### Comparing `jsonnet-v0.8.7-pre5/core/lexer.cpp` & `jsonnet-v0.8.7-pre6/core/lexer.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -371,63 +371,54 @@
         Location begin(line_number, c - line_start + 1);
 
         switch (*c) {
 
             // The following operators should never be combined with subsequent symbols.
             case '{':
             kind = Token::BRACE_L;
-            data = "{";
             c++;
             break;
 
             case '}':
             kind = Token::BRACE_R;
-            data = "}";
             c++;
             break;
 
             case '[':
             kind = Token::BRACKET_L;
-            data = "[";
             c++;
             break;
 
             case ']':
             kind = Token::BRACKET_R;
-            data = "]";
             c++;
             break;
 
             case ',':
             kind = Token::COMMA;
-            data = ",";
             c++;
             break;
 
             case '.':
             kind = Token::DOT;
-            data = ".";
             c++;
             break;
 
             case '(':
             kind = Token::PAREN_L;
-            data = "(";
             c++;
             break;
 
             case ')':
             kind = Token::PAREN_R;
-            data = ")";
             c++;
             break;
 
             case ';':
             kind = Token::SEMICOLON;
-            data = ";";
             c++;
             break;
 
             // Numeric literals.
             case '0': case '1': case '2': case '3': case '4':
             case '5': case '6': case '7': case '8': case '9':
             kind = Token::NUMBER;
@@ -687,15 +678,20 @@
                 // Not allowed to end with a + - ~ ! unless a single char.
                 // So, wind it back if we need to (but not too far).
                 while (c > operator_begin + 1
                        && (*(c-1) == '+' || *(c-1) == '-' || *(c-1) == '~' || *(c-1) == '!')) {
                     c--;
                 }
                 data += std::string(operator_begin, c);
-                kind = data == "$" ? Token::DOLLAR : Token::OPERATOR;
+                if (data == "$") {
+                    kind = Token::DOLLAR;
+                    data = "";
+                } else {
+                    kind = Token::OPERATOR;
+                }
             } else {
                 std::stringstream ss;
                 ss << "Could not lex the character ";
                 auto uc = (unsigned char)(*c);
                 if (*c < 32)
                     ss << "code " << unsigned(uc);
                 else
```

### Comparing `jsonnet-v0.8.7-pre5/core/static_analysis.h` & `jsonnet-v0.8.7-pre6/core/static_analysis.h`

 * *Files identical despite different names*

### Comparing `jsonnet-v0.8.7-pre5/core/state.h` & `jsonnet-v0.8.7-pre6/core/state.h`

 * *Files identical despite different names*

### Comparing `jsonnet-v0.8.7-pre5/core/formatter.cpp` & `jsonnet-v0.8.7-pre6/core/formatter.cpp`

 * *Files identical despite different names*

### Comparing `jsonnet-v0.8.7-pre5/core/desugarer.h` & `jsonnet-v0.8.7-pre6/core/desugarer.h`

 * *Files identical despite different names*

### Comparing `jsonnet-v0.8.7-pre5/core/formatter.h` & `jsonnet-v0.8.7-pre6/core/formatter.h`

 * *Files identical despite different names*

### Comparing `jsonnet-v0.8.7-pre5/stdlib/std.jsonnet` & `jsonnet-v0.8.7-pre6/stdlib/std.jsonnet`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             aux(str, c, 0, [], ""),
 
     range(from, to)::
         std.makeArray(to - from + 1, function(i) i + from),
 
     slice(indexable, index, end, step)::
         if (index != null && index < 0) || (end != null && end < 0) || (step != null && step < 0) then
-            error("got [%s:%s:%s] but negative index, end, and steps are not implemented" % [index, end, step] )
+            error("got [%s:%s:%s] but negative index, end, and steps are not supported" % [index, end, step] )
         else if std.type(indexable) != "string" && std.type(indexable) != "array" then
             error("std.slice accepts a string or an array, but got: %s" % std.type(indexable))
         else
             local invar =
                 // loop invariant with defaults applied
                 {
                     indexable: indexable,
@@ -317,33 +317,26 @@
                         prec: prec.v,
                         ctype: ctype.v,
                         caps: ctype.caps,
                     }
                 };
 
         // Parse a format string (containing none or more % format tags).
-        local parse_codes(str, i, out) = 
+        local parse_codes(str, i, out, cur) =
             if i >= std.length(str) then
-                out
+                out + [cur]
             else
                 local c = str[i];
                 if c == "%" then
                     local r = parse_code(str, i + 1);
-                    parse_codes(str, r.i, out+[r.code]) tailstrict
+                    parse_codes(str, r.i, out + [cur, r.code], "") tailstrict
                 else
-                    local last = out[std.length(out)-1];
-                    local append = std.length(out) > 0 && std.type(last) == "string";
-                    parse_codes(str, i + 1, if append then
-                        std.makeArray(std.length(out),
-                            function(i) if i < std.length(out)-1 then out[i] else last + c) tailstrict
-                    else
-                        std.makeArray(std.length(out) + 1,
-                            function(i) if i < std.length(out) then out[i] else c)) tailstrict;
+                    parse_codes(str, i + 1, out, cur + c) tailstrict;
 
-        local codes = parse_codes(str, 0, []);
+        local codes = parse_codes(str, 0, [], "");
 
 
         ///////////////////////
         // Format the values //
         ///////////////////////
 
         // Useful utilities
```

### Comparing `jsonnet-v0.8.7-pre5/python/_jsonnet.c` & `jsonnet-v0.8.7-pre6/python/_jsonnet.c`

 * *Files identical despite different names*

### Comparing `jsonnet-v0.8.7-pre5/LICENSE` & `jsonnet-v0.8.7-pre6/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonnet-v0.8.7-pre5/include/libjsonnet.h` & `jsonnet-v0.8.7-pre6/include/libjsonnet.h`

 * *Files 12% similar despite different names*

```diff
@@ -13,21 +13,23 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 */
 
 #ifndef LIB_JSONNET_H
 #define LIB_JSONNET_H
 
+#include <stddef.h>
+
 /** \file This file is a library interface for evaluating Jsonnet.  It is written in C++ but exposes
  * a C interface for easier wrapping by other languages.  See \see jsonnet_lib_test.c for an example
  * of using the library.
  */
 
 
-#define LIB_JSONNET_VERSION "v0.8.7-pre5"
+#define LIB_JSONNET_VERSION "v0.8.7-pre6"
 
 
 /** Return the version string of the Jsonnet interpreter.  Conforms to semantic versioning
  * http://semver.org/ If this does not match LIB_JSONNET_VERSION then there is a mismatch between
  * header and compiled library.
  */
 const char *jsonnet_version(void);
@@ -184,39 +186,67 @@
  * \returns Either JSON or the error message.
  */
 char *jsonnet_evaluate_snippet(struct JsonnetVm *vm,
                                const char *filename,
                                const char *snippet,
                                int *error);
 
-/** Evaluate a file containing Jsonnet code, return a number of JSON files.
+/** Evaluate a file containing Jsonnet code, return a number of named JSON files.
  *
  * The returned character buffer contains an even number of strings, the filename and JSON for each
  * JSON file interleaved.  It should be cleaned up with jsonnet_realloc.
  *
  * \param filename Path to a file containing Jsonnet code.
  * \param error Return by reference whether or not there was an error.
  * \returns Either the error, or a sequence of strings separated by \0, terminated with \0\0.
  */
 char *jsonnet_evaluate_file_multi(struct JsonnetVm *vm,
                                   const char *filename,
                                   int *error);
 
-/** Evaluate a string containing Jsonnet code, return a number of JSON files.
+/** Evaluate a string containing Jsonnet code, return a number of named JSON files.
  *
  * The returned character buffer contains an even number of strings, the filename and JSON for each
  * JSON file interleaved.  It should be cleaned up with jsonnet_realloc.
  *
  * \param filename Path to a file containing Jsonnet code.
  * \param snippet Jsonnet code to execute.
  * \param error Return by reference whether or not there was an error.
  * \returns Either the error, or a sequence of strings separated by \0, terminated with \0\0.
  */
 char *jsonnet_evaluate_snippet_multi(struct JsonnetVm *vm,
                                      const char *filename,
                                      const char *snippet,
                                      int *error);
 
+/** Evaluate a file containing Jsonnet code, return a number of JSON files.
+ *
+ * The returned character buffer contains several strings.  It should be cleaned up with
+ * jsonnet_realloc.
+ *
+ * \param filename Path to a file containing Jsonnet code.
+ * \param error Return by reference whether or not there was an error.
+ * \returns Either the error, or a sequence of strings separated by \0, terminated with \0\0.
+ */
+char *jsonnet_evaluate_file_stream(struct JsonnetVm *vm,
+                                   const char *filename,
+                                   int *error);
+
+/** Evaluate a string containing Jsonnet code, return a number of JSON files.
+ *
+ * The returned character buffer contains several strings.  It should be cleaned up with
+ * jsonnet_realloc.
+ *
+ * \param filename Path to a file containing Jsonnet code.
+ * \param snippet Jsonnet code to execute.
+ * \param error Return by reference whether or not there was an error.
+ * \returns Either the error, or a sequence of strings separated by \0, terminated with \0\0.
+ */
+char *jsonnet_evaluate_snippet_stream(struct JsonnetVm *vm,
+                                      const char *filename,
+                                      const char *snippet,
+                                      int *error);
+
 /** Complement of \see jsonnet_vm_make. */
 void jsonnet_destroy(struct JsonnetVm *vm);
 
 #endif  // LIB_JSONNET_H
```

