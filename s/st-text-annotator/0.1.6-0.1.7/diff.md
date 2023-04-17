# Comparing `tmp/st_text_annotator-0.1.6.tar.gz` & `tmp/st_text_annotator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_text_annotator-0.1.6.tar", max compression
+gzip compressed data, was "st_text_annotator-0.1.7.tar", max compression
```

## Comparing `st_text_annotator-0.1.6.tar` & `st_text_annotator-0.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1075 2023-04-14 18:30:17.965925 st_text_annotator-0.1.6/LICENSE
--rw-r--r--   0        0        0      971 2023-04-14 22:26:10.101353 st_text_annotator-0.1.6/README.md
--rw-r--r--   0        0        0      702 2023-04-16 14:19:25.824988 st_text_annotator-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2309 2023-04-15 21:13:21.432502 st_text_annotator-0.1.6/src/st_text_annotator/__init__.py
--rw-r--r--   0        0        0      180 2023-04-14 17:24:02.791373 st_text_annotator-0.1.6/src/st_text_annotator/frontend/.env
--rw-r--r--   0        0        0       67 2023-04-14 17:24:02.792164 st_text_annotator-0.1.6/src/st_text_annotator/frontend/.prettierrc
--rw-r--r--   0        0        0      961 2023-04-14 22:08:31.587769 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0   197459 2023-04-14 22:08:17.378178 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/bootstrap.min.css
--rw-r--r--   0        0        0     2097 2023-04-14 22:08:31.587571 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/index.html
--rw-r--r--   0        0        0      685 2023-04-14 22:08:31.587640 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/precache-manifest.e1f4d7e39016325d19b80487326d9754.js
--rw-r--r--   0        0        0     1183 2023-04-14 22:08:31.587724 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/service-worker.js
--rw-r--r--   0        0        0   594301 2023-04-14 22:08:31.594107 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js
--rw-r--r--   0        0        0     1803 2023-04-14 22:08:31.593423 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0  1813945 2023-04-14 22:08:31.593928 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.map
--rw-r--r--   0        0        0    11817 2023-04-14 22:08:31.593385 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/main.c60fd880.chunk.js
--rw-r--r--   0        0        0      149 2023-04-14 22:08:31.594561 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/main.c60fd880.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0    22907 2023-04-14 22:08:31.593496 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/main.c60fd880.chunk.js.map
--rw-r--r--   0        0        0     1594 2023-04-14 22:08:31.593462 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js
--rw-r--r--   0        0        0     8307 2023-04-14 22:08:31.594489 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js.map
--rw-r--r--   0        0        0      846 2023-04-14 21:50:22.684911 st_text_annotator-0.1.6/src/st_text_annotator/frontend/package.json
--rw-r--r--   0        0        0   197459 2023-04-14 17:24:02.785648 st_text_annotator-0.1.6/src/st_text_annotator/frontend/public/bootstrap.min.css
--rw-r--r--   0        0        0      894 2023-04-14 17:24:02.786098 st_text_annotator-0.1.6/src/st_text_annotator/frontend/public/index.html
--rw-r--r--   0        0        0     7490 2023-04-14 21:49:47.302144 st_text_annotator-0.1.6/src/st_text_annotator/frontend/src/Annotation.tsx
--rw-r--r--   0        0        0     7490 2023-04-15 21:14:06.072822 st_text_annotator-0.1.6/src/st_text_annotator/frontend/src/AnnotationNew.tsx
--rw-r--r--   0        0        0      219 2023-04-15 21:23:26.959735 st_text_annotator-0.1.6/src/st_text_annotator/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2023-04-14 17:24:02.814143 st_text_annotator-0.1.6/src/st_text_annotator/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      459 2023-04-14 17:24:02.792820 st_text_annotator-0.1.6/src/st_text_annotator/frontend/tsconfig.json
--rw-r--r--   0        0        0     1521 1970-01-01 00:00:00.000000 st_text_annotator-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-14 18:30:17.965925 st_text_annotator-0.1.7/LICENSE
+-rw-r--r--   0        0        0      971 2023-04-14 22:26:10.101353 st_text_annotator-0.1.7/README.md
+-rw-r--r--   0        0        0      713 2023-04-16 18:38:17.296216 st_text_annotator-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2308 2023-04-16 18:16:49.394296 st_text_annotator-0.1.7/src/st_text_annotator/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-14 17:24:02.791373 st_text_annotator-0.1.7/src/st_text_annotator/frontend/.env
+-rw-r--r--   0        0        0       67 2023-04-14 17:24:02.792164 st_text_annotator-0.1.7/src/st_text_annotator/frontend/.prettierrc
+-rw-r--r--   0        0        0      961 2023-04-16 18:17:20.106557 st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0   197459 2023-04-16 18:17:00.578609 st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/bootstrap.min.css
+-rw-r--r--   0        0        0     2097 2023-04-16 18:17:20.106481 st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/index.html
+-rw-r--r--   0        0        0      685 2023-04-16 18:17:20.106175 st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/precache-manifest.b83f8cda23e89b45d1bce2e70668eace.js
+-rw-r--r--   0        0        0     1183 2023-04-16 18:17:20.106326 st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/service-worker.js
+-rw-r--r--   0        0        0   594301 2023-04-16 18:17:20.115612 st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js
+-rw-r--r--   0        0        0     1803 2023-04-16 18:17:20.113847 st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0  1813945 2023-04-16 18:17:20.114381 st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.map
+-rw-r--r--   0        0        0    11817 2023-04-16 18:17:20.107357 st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/static/js/main.185866dc.chunk.js
+-rw-r--r--   0        0        0      149 2023-04-16 18:17:20.113813 st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/static/js/main.185866dc.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0    22913 2023-04-16 18:17:20.114480 st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/static/js/main.185866dc.chunk.js.map
+-rw-r--r--   0        0        0     1594 2023-04-16 18:17:20.113768 st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js
+-rw-r--r--   0        0        0     8307 2023-04-16 18:17:20.115460 st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js.map
+-rw-r--r--   0        0        0      846 2023-04-16 18:09:54.163942 st_text_annotator-0.1.7/src/st_text_annotator/frontend/package.json
+-rw-r--r--   0        0        0   197459 2023-04-14 17:24:02.785648 st_text_annotator-0.1.7/src/st_text_annotator/frontend/public/bootstrap.min.css
+-rw-r--r--   0        0        0      894 2023-04-14 17:24:02.786098 st_text_annotator-0.1.7/src/st_text_annotator/frontend/public/index.html
+-rw-r--r--   0        0        0     7490 2023-04-14 21:49:47.302144 st_text_annotator-0.1.7/src/st_text_annotator/frontend/src/Annotation.tsx
+-rw-r--r--   0        0        0     7490 2023-04-15 21:14:06.072822 st_text_annotator-0.1.7/src/st_text_annotator/frontend/src/AnnotationNew.tsx
+-rw-r--r--   0        0        0      219 2023-04-15 21:23:26.959735 st_text_annotator-0.1.7/src/st_text_annotator/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-04-14 17:24:02.814143 st_text_annotator-0.1.7/src/st_text_annotator/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2023-04-14 17:24:02.792820 st_text_annotator-0.1.7/src/st_text_annotator/frontend/tsconfig.json
+-rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 st_text_annotator-0.1.7/PKG-INFO
```

### Comparing `st_text_annotator-0.1.6/LICENSE` & `st_text_annotator-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.6/README.md` & `st_text_annotator-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/__init__.py` & `st_text_annotator-0.1.7/src/st_text_annotator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import streamlit.components.v1 as components
 
-RELEASE = False
+RELEASE = True
 
 if not RELEASE:
     _component_func = components.declare_component("st_text_annotator", url="http://localhost:3001")
 else:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component("StTextAnnotator", path=build_dir)
```

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/asset-manifest.json` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/asset-manifest.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7788461538461539%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/main.185866dc.chunk.js')], delete: [2]}",*

 * * "'files'": "{'main.js': './static/js/main.185866dc.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.185866dc.chunk.js.map', "*

 * *            "'precache-manifest.b83f8cda23e89b45d1bce2e70668eace.js': "*

 * *            "'./precache-manifest.b83f8cda23e89b45d1bce2e70668eace.js', "*

 * *            "'static/js/main.185866dc.chunk.js.LICENSE.txt': "*

 * *            "'./static/js/main.185866dc.chunk.js.LICENSE.txt', delete: "*

 * *        […]*

```diff
@@ -1,20 +1,20 @@
 {
     "entrypoints": [
         "static/js/runtime-main.d5954658.js",
         "static/js/2.0d16c425.chunk.js",
-        "static/js/main.c60fd880.chunk.js"
+        "static/js/main.185866dc.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.c60fd880.chunk.js",
-        "main.js.map": "./static/js/main.c60fd880.chunk.js.map",
-        "precache-manifest.e1f4d7e39016325d19b80487326d9754.js": "./precache-manifest.e1f4d7e39016325d19b80487326d9754.js",
+        "main.js": "./static/js/main.185866dc.chunk.js",
+        "main.js.map": "./static/js/main.185866dc.chunk.js.map",
+        "precache-manifest.b83f8cda23e89b45d1bce2e70668eace.js": "./precache-manifest.b83f8cda23e89b45d1bce2e70668eace.js",
         "runtime-main.js": "./static/js/runtime-main.d5954658.js",
         "runtime-main.js.map": "./static/js/runtime-main.d5954658.js.map",
         "service-worker.js": "./service-worker.js",
         "static/js/2.0d16c425.chunk.js": "./static/js/2.0d16c425.chunk.js",
         "static/js/2.0d16c425.chunk.js.LICENSE.txt": "./static/js/2.0d16c425.chunk.js.LICENSE.txt",
         "static/js/2.0d16c425.chunk.js.map": "./static/js/2.0d16c425.chunk.js.map",
-        "static/js/main.c60fd880.chunk.js.LICENSE.txt": "./static/js/main.c60fd880.chunk.js.LICENSE.txt"
+        "static/js/main.185866dc.chunk.js.LICENSE.txt": "./static/js/main.185866dc.chunk.js.LICENSE.txt"
     }
 }
```

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/bootstrap.min.css` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/index.html` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(t){function e(e){for(var n,a,l=e[0],i=e[1],f=e[2],c=0,s=[];c<l.length;c++)a=l[c],Object.prototype.hasOwnProperty.call(o,a)&&o[a]&&s.push(o[a][0]),o[a]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(t[n]=i[n]);for(p&&p(e);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var t,e=0;e<u.length;e++){for(var r=u[e],n=!0,l=1;l<r.length;l++){var i=r[l];0!==o[i]&&(n=!1)}n&&(u.splice(e--,1),t=a(a.s=r[0]))}return t}var n={},o={1:0},u=[];function a(e){if(n[e])return n[e].exports;var r=n[e]={i:e,l:!1,exports:{}};return t[e].call(r.exports,r,r.exports,a),r.l=!0,r.exports}a.m=t,a.c=n,a.d=function(t,e,r){a.o(t,e)||Object.defineProperty(t,e,{enumerable:!0,get:r})},a.r=function(t){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(t,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(t,"__esModule",{value:!0})},a.t=function(t,e){if(1&e&&(t=a(t)),8&e)return t;if(4&e&&"object"==typeof t&&t&&t.__esModule)return t;var r=Object.create(null);if(a.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:t}),2&e&&"string"!=typeof t)for(var n in t)a.d(r,n,function(e){return t[e]}.bind(null,n));return r},a.n=function(t){var e=t&&t.__esModule?function(){return t.default}:function(){return t};return a.d(e,"a",e),e},a.o=function(t,e){return Object.prototype.hasOwnProperty.call(t,e)},a.p="./";var l=this["webpackJsonpsteamlit-text-annotator"]=this["webpackJsonpsteamlit-text-annotator"]||[],i=l.push.bind(l);l.push=e,l=l.slice();for(var f=0;f<l.length;f++)e(l[f]);var p=i;r()}([])</script><script src="./static/js/2.0d16c425.chunk.js"></script><script src="./static/js/main.c60fd880.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(t){function e(e){for(var n,a,l=e[0],i=e[1],f=e[2],c=0,s=[];c<l.length;c++)a=l[c],Object.prototype.hasOwnProperty.call(o,a)&&o[a]&&s.push(o[a][0]),o[a]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(t[n]=i[n]);for(p&&p(e);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var t,e=0;e<u.length;e++){for(var r=u[e],n=!0,l=1;l<r.length;l++){var i=r[l];0!==o[i]&&(n=!1)}n&&(u.splice(e--,1),t=a(a.s=r[0]))}return t}var n={},o={1:0},u=[];function a(e){if(n[e])return n[e].exports;var r=n[e]={i:e,l:!1,exports:{}};return t[e].call(r.exports,r,r.exports,a),r.l=!0,r.exports}a.m=t,a.c=n,a.d=function(t,e,r){a.o(t,e)||Object.defineProperty(t,e,{enumerable:!0,get:r})},a.r=function(t){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(t,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(t,"__esModule",{value:!0})},a.t=function(t,e){if(1&e&&(t=a(t)),8&e)return t;if(4&e&&"object"==typeof t&&t&&t.__esModule)return t;var r=Object.create(null);if(a.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:t}),2&e&&"string"!=typeof t)for(var n in t)a.d(r,n,function(e){return t[e]}.bind(null,n));return r},a.n=function(t){var e=t&&t.__esModule?function(){return t.default}:function(){return t};return a.d(e,"a",e),e},a.o=function(t,e){return Object.prototype.hasOwnProperty.call(t,e)},a.p="./";var l=this["webpackJsonpsteamlit-text-annotator"]=this["webpackJsonpsteamlit-text-annotator"]||[],i=l.push.bind(l);l.push=e,l=l.slice();for(var f=0;f<l.length;f++)e(l[f]);var p=i;r()}([])</script><script src="./static/js/2.0d16c425.chunk.js"></script><script src="./static/js/main.185866dc.chunk.js"></script></body></html>
```

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/precache-manifest.e1f4d7e39016325d19b80487326d9754.js` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/precache-manifest.b83f8cda23e89b45d1bce2e70668eace.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 self.__precacheManifest = (self.__precacheManifest || []).concat([{
-    "revision": "8e14c2683e875562d7b6e58ef892eab2",
+    "revision": "e8a817de21b648283a45140d001b57fc",
     "url": "./index.html"
 }, {
     "revision": "a3e3442fe61845021c19",
     "url": "./static/js/2.0d16c425.chunk.js"
 }, {
     "revision": "3dc2da520b7611f998bec3f8b32ee24e",
     "url": "./static/js/2.0d16c425.chunk.js.LICENSE.txt"
 }, {
-    "revision": "d87b8e1d32402b5daa52",
-    "url": "./static/js/main.c60fd880.chunk.js"
+    "revision": "4207c7b8adbe5a2f92c2",
+    "url": "./static/js/main.185866dc.chunk.js"
 }, {
     "revision": "4e0e34f265fae8f33b01b27ae29d9d6f",
-    "url": "./static/js/main.c60fd880.chunk.js.LICENSE.txt"
+    "url": "./static/js/main.185866dc.chunk.js.LICENSE.txt"
 }, {
     "revision": "befa42638fa391b5bfa2",
     "url": "./static/js/runtime-main.d5954658.js"
 }]);
```

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/service-worker.js` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/service-worker.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.e1f4d7e39016325d19b80487326d9754.js"
+    "./precache-manifest.b83f8cda23e89b45d1bce2e70668eace.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.LICENSE.txt` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.map` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/main.c60fd880.chunk.js` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/static/js/main.185866dc.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.c60fd880.chunk.js.LICENSE.txt */
+/*! For license information please see main.185866dc.chunk.js.LICENSE.txt */
 (this["webpackJsonpsteamlit-text-annotator"] = this["webpackJsonpsteamlit-text-annotator"] || []).push([
     [0], {
         17: function(e, t, n) {
             e.exports = n(24)
         },
         24: function(e, t, n) {
             "use strict";
@@ -541,8 +541,8 @@
             i.a.render(a.a.createElement(a.a.StrictMode, null, a.a.createElement(y, null)), document.getElementById("root"))
         }
     },
     [
         [17, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.c60fd880.chunk.js.map
+//# sourceMappingURL=main.185866dc.chunk.js.map
```

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/main.c60fd880.chunk.js.map` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/static/js/main.185866dc.chunk.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333333%*

 * *Differences: {"'file'": "'static/js/main.185866dc.chunk.js'",*

 * * "'sources'": "{insert: [(0, 'AnnotationNew.tsx')], delete: [0]}",*

 * * "'sourcesContent'": '{insert: [(1, \'import React from "react"\\nimport ReactDOM from '*

 * *                     '"react-dom"\\nimport MyComponent from '*

 * *                     '"./AnnotationNew"\\n\\nReactDOM.render(\\n  <React.StrictMode>\\n    '*

 * *                     '<MyComponent />\\n  </React.StrictMode>,\\n  '*

 * *                     'document.getElementById("root")\\n)\\n\')], delete: [1]}'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "static/js/main.c60fd880.chunk.js",
+    "file": "static/js/main.185866dc.chunk.js",
     "mappings": "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",
     "names": [
         "_regeneratorRuntime",
         "exports",
         "Op",
         "Object",
         "prototype",
@@ -237,16 +237,16 @@
         "ReactDOM",
         "StrictMode",
         "MyComponent",
         "getElementById"
     ],
     "sourceRoot": "",
     "sources": [
-        "Annotation.tsx",
+        "AnnotationNew.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
         "import {\n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\n\ninterface Reference {\n  start: number,\n  end: number,\n  label: string\n}\n\ninterface State {\n  text: string\n  actual_text: JSX.Element[]\n  selectedReference: number\n  annotations: Reference[][]\n}\n\nconst COLOR = \"#fbf8cc\"\n\n\nclass Annotation extends StreamlitComponentBase<State> {\n  public state: State = { text: \"\", actual_text: [], annotations: [], selectedReference: 0 }\n\n  public async componentDidMount() {\n    const { text, annotations } = this.props.args\n\n    await this.setState({ text, annotations })\n\n    let actual_text = [<>{ text }</>]\n\n    if (annotations.length > 0) {\n      actual_text = this.renderHighlightedText()\n    }\n    this.setState({ actual_text })\n    Streamlit.setComponentValue({ annotations: annotations })\n  }\n\n  private checkOverlap = (start: number, end: number, annotations: Reference[]) => {\n    return annotations.some((annotation) => {\n      return (annotation.start < start && annotation.end > start) || (annotation.start < end && annotation.end > end)\n    })\n  }\n\n  private handleMouseUp = () => {\n    const selection = document.getSelection()\n\n    if (selection && selection.toString().length > 0) {\n      const { annotations } = this.state\n\n      const start = selection.anchorOffset < selection.focusOffset ? selection.anchorOffset : selection.focusOffset\n      const end = selection.anchorOffset < selection.focusOffset ? selection.focusOffset : selection.anchorOffset\n\n      const selected_text = this.state.text.slice(start, end)\n\n      if (annotations.length < this.state.selectedReference + 1) {\n        annotations.push([])\n      }\n\n      if (\n        this.checkOverlap(start, end, annotations[this.state.selectedReference]) && annotations[this.state.selectedReference].length === 1\n      ) {\n        annotations.splice(this.state.selectedReference, 1)\n      }\n      // if overlap with other annotation remove the smaller one\n      else if (this.checkOverlap(start, end, annotations[this.state.selectedReference])) {\n        annotations[this.state.selectedReference] = annotations[this.state.selectedReference].filter((annotation) => {\n          return !((annotation.start < start && annotation.end > start) || (annotation.start < end && annotation.end > end))\n        })\n      } else {\n        annotations[this.state.selectedReference].push({\n          start,\n          end,\n          label: selected_text,\n        })\n      }\n\n      Streamlit.setComponentValue({ annotations: annotations })\n    }\n    this.setState({ actual_text: this.renderHighlightedText() })\n  }\n\n  private handleMouseDown = () => {\n    this.setState({ actual_text: [<>{ this.state.text }</>] })\n  }\n\n  private newReference = () => {\n    this.setState({ selectedReference: this.state.annotations.length })\n  }\n\n  private renderHighlightedText = () => {\n    const { annotations, text: total_text } = this.state\n\n    const selectedAnnotations = annotations.map((liStTextAnnotator, index) => {\n      return liStTextAnnotator.map((annotation) => {\n        return {\n          ...annotation,\n          index,\n          color: COLOR,\n          text: total_text.slice(annotation.start, annotation.end),\n        }\n      })\n    }).filter((annotation, index) => index === this.state.selectedReference)\n\n    // flatten array\n    const flattenAnnotations = selectedAnnotations.flat()\n\n    // sort by start\n    const sortedAnnotations = flattenAnnotations.sort((a, b) => a.start - b.start)\n\n    // render text with color\n    let lastEnd = 0\n\n    if (sortedAnnotations.length === 0) {\n      return [<>{ total_text }</>]\n    }\n\n    return sortedAnnotations.map((annotation, index_annotations, array) => {\n      const { start, end, color, text, index } = annotation\n      const textBefore = total_text.slice(lastEnd, start)\n      lastEnd = end\n\n      return (\n        <>\n          { textBefore }\n          <span style={ {\n            backgroundColor: this.state.selectedReference === index ? color : \"transparent\",\n            color: this.state.selectedReference === index ? \"black\" : \"white\",\n          } }>{ text }</span>\n          { index_annotations === array.length - 1 && total_text.slice(end) }\n        </>\n      )\n    })\n  }\n\n  public render = (): ReactNode => {\n    return (\n      <>\n        <div>\n          <button\n            onClick={ this.newReference }\n            style={ { backgroundColor: \"transparent\", color: \"white\", border: \"1px solid white\" } }\n          >\n            New Reference\n          </button>\n          <div style={ { display: \"flex\", flexDirection: \"column\", flexWrap: \"wrap\" } }>\n            { // get selected reference\n              this.state.annotations.map((annotation, index) => {\n                return (\n                  <div\n                    key={ index }\n                    style={ { textAlign: \"start\" } }\n                  >\n                    <button\n                      onClick={ async () => {\n                        await this.setState({ selectedReference: index })\n                        this.setState({ actual_text: this.renderHighlightedText() })\n                      } }\n                      style={ {\n                        backgroundColor: this.state.selectedReference !== index ? \"transparent\" : COLOR,\n                        color: this.state.selectedReference !== index ? \"white\" : \"black\",\n                        fontWeight: this.state.selectedReference === index ? \"bold\" : \"normal\",\n                        border: this.state.selectedReference === index ? \"1px solid white\" : \"1px solid transparent\",\n                        width: \"400px\",\n                        overflow: \"hidden\",\n                        whiteSpace: \"nowrap\",\n                        textAlign: \"start\",\n                      } }>\n                      { annotation[0].label}\n                    </button>\n                    <button\n                      onClick={ async () => {\n                        await this.setState({\n                          annotations: this.state.annotations.filter((_, i) => i !== index),\n                          selectedReference: this.state.selectedReference === index ? 0 : this.state.selectedReference,\n                        })\n                        this.setState({ actual_text: this.renderHighlightedText() })\n                        Streamlit.setComponentValue({ annotations: this.state.annotations.filter((_, i) => i !== index) })\n                      } }\n                      style={ {\n                        backgroundColor: this.state.selectedReference !== index ? \"transparent\" : COLOR,\n                        color: this.state.selectedReference !== index ? \"white\" : \"black\",\n                        fontWeight: this.state.selectedReference === index ? \"bold\" : \"normal\",\n                        border: this.state.selectedReference === index ? \"1px solid white\" : \"1px solid transparent\",\n                      } }>\n                      X\n                    </button>\n                  </div>\n                )\n              })\n            }\n          </div>\n        </div>\n        <br/>\n        <br/>\n        <div>\n          <div\n            id=\"text\" style={ { whiteSpace: \"pre-wrap\" } }\n            onMouseUp={ this.handleMouseUp }\n            onMouseDown={ this.handleMouseDown }\n          >\n            { this.state.actual_text }\n          </div>\n        </div>\n      </>\n    )\n  }\n}\n\nexport default withStreamlitConnection(Annotation)\n",
-        "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport MyComponent from \"./Annotation\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <MyComponent />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
+        "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport MyComponent from \"./AnnotationNew\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <MyComponent />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js.map` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js.map`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/package.json` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/package.json`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/public/bootstrap.min.css` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/public/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/public/index.html` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/src/Annotation.tsx` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/src/Annotation.tsx`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.6/src/st_text_annotator/frontend/src/AnnotationNew.tsx` & `st_text_annotator-0.1.7/src/st_text_annotator/frontend/src/AnnotationNew.tsx`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.6/PKG-INFO` & `st_text_annotator-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: st-text-annotator
-Version: 0.1.6
+Version: 0.1.7
 Summary: Component for annotating text for NLP resolution
 License: MIT
+Keywords: streamlit,text,annotation,nlp
 Author: Robin Marquet
 Author-email: robin.marquet@epitech.eu
 Requires-Python: >=3.8,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

