# Comparing `tmp/buildbot-www-react-3.7.0.tar.gz` & `tmp/buildbot-www-react-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/buildbot-www-react-3.7.0.tar", last modified: Sun Dec  4 11:52:39 2022, max compression
+gzip compressed data, was "dist/buildbot-www-react-3.8.0.tar", last modified: Mon Apr 17 01:21:06 2023, max compression
```

## Comparing `buildbot-www-react-3.7.0.tar` & `buildbot-www-react-3.8.0.tar`

### file list

```diff
@@ -1,39 +1,23 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      314 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2113 2022-12-04 11:48:49.000000 buildbot-www-react-3.7.0/README.md
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      855 2022-12-04 11:48:49.000000 buildbot-www-react-3.7.0/buildbot_www_react/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1100 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/asset-manifest.json
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      755 2022-12-04 11:51:52.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/browser-warning-list.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1108 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/browser-warning.css
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2244 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/browser-warning.css.map
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    30881 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/browser-warning.js
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/css/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   201314 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/css/main.5d5c294a.chunk.css
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   423983 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/css/main.5d5c294a.chunk.css.map
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21460 2022-12-04 11:51:52.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/icon.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1180 2022-12-04 11:51:52.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/icon.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3163 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/index.html
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/js/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   760401 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/js/2.cfcdd80c.chunk.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3708 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/js/2.cfcdd80c.chunk.js.LICENSE.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)  3165689 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/js/2.cfcdd80c.chunk.js.map
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4649 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/js/3.e65a7642.chunk.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10273 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/js/3.e65a7642.chunk.js.map
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   143200 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/js/main.31f9f031.chunk.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   482104 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/js/main.31f9f031.chunk.js.map
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2361 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/js/runtime-main.30b8d22a.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12459 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/js/runtime-main.30b8d22a.js.map
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      393 2022-12-04 11:51:52.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/manifest.json
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       67 2022-12-04 11:51:52.000000 buildbot-www-react-3.7.0/buildbot_www_react/static/robots.txt
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      314 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1358 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       71 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        9 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react.egg-info/requires.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       19 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/buildbot_www_react.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2022-12-04 11:52:39.000000 buildbot-www-react-3.7.0/setup.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1714 2022-12-04 11:48:49.000000 buildbot-www-react-3.7.0/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      258 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/PKG-INFO
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/buildbot_www_react/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/buildbot_www_react/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      855 2023-04-17 01:17:21.000000 buildbot-www-react-3.8.0/buildbot_www_react/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/buildbot_www_react/static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      755 2023-04-17 01:21:05.000000 buildbot-www-react-3.8.0/buildbot_www_react/static/browser-warning-list.js
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1411 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/buildbot_www_react/static/browser-warning.css
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    28827 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/buildbot_www_react/static/browser-warning.js
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21460 2023-04-17 01:21:05.000000 buildbot-www-react-3.8.0/buildbot_www_react/static/icon.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1180 2023-04-17 01:21:05.000000 buildbot-www-react-3.8.0/buildbot_www_react/static/icon.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      953 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/buildbot_www_react/static/index.html
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      393 2023-04-17 01:21:05.000000 buildbot-www-react-3.8.0/buildbot_www_react/static/manifest.json
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       67 2023-04-17 01:21:05.000000 buildbot-www-react-3.8.0/buildbot_www_react/static/robots.txt
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/buildbot_www_react.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      258 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/buildbot_www_react.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      655 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/buildbot_www_react.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/buildbot_www_react.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       50 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/buildbot_www_react.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        9 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/buildbot_www_react.egg-info/requires.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       19 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/buildbot_www_react.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-04-17 01:21:06.000000 buildbot-www-react-3.8.0/setup.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1714 2023-04-17 01:17:21.000000 buildbot-www-react-3.8.0/setup.py
```

### Comparing `buildbot-www-react-3.7.0/buildbot_www_react/__init__.py` & `buildbot-www-react-3.8.0/buildbot_www_react/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-www-react-3.7.0/buildbot_www_react/static/browser-warning-list.js` & `buildbot-www-react-3.8.0/buildbot_www_react/static/browser-warning-list.js`

 * *Files identical despite different names*

### Comparing `buildbot-www-react-3.7.0/buildbot_www_react/static/browser-warning.js` & `buildbot-www-react-3.8.0/buildbot_www_react/static/browser-warning.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,251 +1,256 @@
 ! function(e) {
     "object" == typeof exports && "undefined" != typeof module ? module.exports = e() : "function" == typeof define && define.amd ? define([], e) : ("undefined" != typeof window ? window : "undefined" != typeof global ? global : "undefined" != typeof self ? self : this).outdatedBrowserRework = e()
-}((function() {
-    return function e(o, r, i) {
-        function a(t, l) {
-            if (!r[t]) {
-                if (!o[t]) {
-                    var n = "function" == typeof require && require;
-                    if (!l && n) return n(t, !0);
-                    if (s) return s(t, !0);
-                    throw (n = new Error("Cannot find module '" + t + "'")).code = "MODULE_NOT_FOUND", n
+}(function() {
+    return function n(i, a, s) {
+        function t(o, e) {
+            if (!a[o]) {
+                if (!i[o]) {
+                    var r = "function" == typeof require && require;
+                    if (!e && r) return r(o, !0);
+                    if (l) return l(o, !0);
+                    throw (r = new Error("Cannot find module '" + o + "'")).code = "MODULE_NOT_FOUND", r
                 }
-                n = r[t] = {
+                r = a[o] = {
                     exports: {}
-                }, o[t][0].call(n.exports, (function(e) {
-                    return a(o[t][1][e] || e)
-                }), n, n.exports, e, o, r, i)
+                }, i[o][0].call(r.exports, function(e) {
+                    return t(i[o][1][e] || e)
+                }, r, r.exports, n, i, a, s)
             }
-            return r[t].exports
+            return a[o].exports
         }
-        for (var s = "function" == typeof require && require, t = 0; t < i.length; t++) a(i[t]);
-        return a
+        for (var l = "function" == typeof require && require, e = 0; e < s.length; e++) t(s[e]);
+        return t
     }({
         1: [function(e, o, r) {
-            var i = {
+            var a = {
                     Chrome: 57,
                     Edge: 39,
                     Safari: 10,
                     "Mobile Safari": 10,
                     Opera: 50,
                     Firefox: 50,
                     Vivaldi: 1,
                     IE: !1
                 },
-                a = {
+                d = {
                     12: .1,
                     13: 21,
                     14: 31,
                     15: 39,
                     16: 41,
                     17: 42,
                     18: 44
                 };
-            o.exports = function(e, o) {
-                var r, s = o.browserSupport ? function(e, o) {
+            o.exports = function(t, e) {
+                var o, l = e.browserSupport ? function(e, o) {
                         for (var r in o) e[r] = o[r];
                         return e
-                    }(i, o.browserSupport) : i,
-                    t = o.requiredCssProperty || !1,
-                    l = e.browser.name;
-                o.requireChromeOnAndroid && (r = "Android" === e.os.name && "Chrome" !== e.browser.name);
-                var n, u = (n = !1, l in s ? s[l] || (n = !0) : o.isUnknownBrowserOK || (n = !0), n);
+                    }(a, e.browserSupport) : a,
+                    r = e.requiredCssProperty || !1,
+                    n = t.browser.name;
+                e.requireChromeOnAndroid && (o = "Android" === t.os.name && "Chrome" !== t.browser.name);
+                var i, u = (i = !1, n in l ? l[n] || (i = !0) : e.isUnknownBrowserOK || (i = !0), i);
                 return {
-                    isAndroidButNotChrome: r,
+                    isAndroidButNotChrome: o,
                     isBrowserOutOfDate: function() {
-                        var o = e.browser.version,
-                            r = e.browser.major,
-                            i = e.os.name,
-                            t = e.os.version;
-                        "Edge" === l && r <= 18 && (r = a[r]), "Firefox" === l && "iOS" === i && (l = "Mobile Safari", r = (o = t).substring(0, t.indexOf(".")));
-                        var n, d = !1;
-                        return u ? d = !0 : l in s && ("object" == typeof(n = s[l]) ? (i = n.major, t = n.minor, (r < i || r == i && o.replace(/[^\d.]/g, "").split(".")[1] < t) && (d = !0)) : r < n && (d = !0)), d
+                        var e = t.browser.version,
+                            o = t.browser.major,
+                            r = t.os.name,
+                            i = t.os.version;
+                        "Edge" === n && o <= 18 && (o = d[o]), "Firefox" === n && "iOS" === r && (n = "Mobile Safari", o = (e = i).substring(0, i.indexOf(".")));
+                        var a, s = !1;
+                        return u ? s = !0 : n in l && ("object" == typeof(a = l[n]) ? (r = a.major, i = a.minor, (o < r || o == r && e.replace(/[^\d.]/g, "").split(".")[1] < i) && (s = !0)) : o < a && (s = !0)), s
                     }(),
                     isBrowserUnsupported: u,
                     isPropertySupported: function(e) {
                         if (!e) return !0;
                         var o = document.createElement("div"),
                             r = ["khtml", "ms", "o", "moz", "webkit"],
                             i = r.length;
                         if (e in o.style) return !0;
-                        for (e = e.replace(/^[a-z]/, (function(e) {
+                        for (e = e.replace(/^[a-z]/, function(e) {
                                 return e.toUpperCase()
-                            })); i--;)
-                            if (r[i] + e in o.style) return !0;
+                            }); i--;) {
+                            if (r[i] + e in o.style) return !0
+                        }
                         return !1
-                    }(t)
+                    }(r)
                 }
             }
         }, {}],
         2: [function(e, o, r) {
-            o.exports = function e() {
+            o.exports = function t() {
                 if (arguments.length < 1 || "object" != typeof arguments[0]) return !1;
                 if (arguments.length < 2) return arguments[0];
-                for (var o = arguments[0], r = 1; r < arguments.length; r++) {
-                    var i, a = arguments[r];
-                    for (i in a) {
-                        var s = o[i],
-                            t = a[i];
-                        o[i] = "object" != typeof t || null === t ? t : e("object" != typeof s || null === s ? {} : s, t)
+                for (var e = arguments[0], o = 1; o < arguments.length; o++) {
+                    var r, i = arguments[o];
+                    for (r in i) {
+                        var a = e[r],
+                            s = i[r];
+                        e[r] = "object" != typeof s || null === s ? s : t("object" != typeof a || null === a ? {} : a, s)
                     }
                 }
-                return o
+                return e
             }
         }, {}],
         3: [function(e, o, r) {
-            var i = e("./evaluateBrowser"),
-                a = e("./languages.json"),
-                s = e("./extend"),
-                t = e("ua-parser-js");
-            o.exports = function(e) {
-                var o = function() {
-                        var o = new t(navigator.userAgent).getResult(),
+            var f = e("./evaluateBrowser"),
+                v = e("./languages.json"),
+                y = e("./extend"),
+                S = e("ua-parser-js"),
+                k = "#f25648",
+                A = "white";
+            o.exports = function(h) {
+                var e = function() {
+                        var e = new S(navigator.userAgent).getResult(),
                             r = document.getElementById("outdated");
-                        e = e || {};
-                        var l = window.navigator.language || window.navigator.userLanguage,
-                            n = e.backgroundColor || "#f25648",
-                            u = e.textColor || "white",
-                            d = e.fullscreen || !1,
-                            p = e.language || l.slice(0, 2),
-                            w = "web";
-                        "Android" === o.os.name ? w = "googlePlay" : "iOS" === o.os.name && (w = "appStore");
-                        var c, g, m, b, h, f = !1,
-                            v = !0,
-                            y = function(e) {
+                        h = h || {};
+                        var o = window.navigator.language || window.navigator.userLanguage,
+                            i = h.backgroundColor || k,
+                            a = h.textColor || A,
+                            s = h.fullscreen || !1,
+                            t = h.language || o.slice(0, 2),
+                            l = "web";
+                        "Android" === e.os.name ? l = "googlePlay" : "iOS" === e.os.name && (l = "appStore");
+                        var n, u, d, p, w, c = !1,
+                            g = !0,
+                            m = function(e) {
                                 var o;
-                                o = e, r.style.opacity = o / 100, r.style.filter = "alpha(opacity=" + o + ")", 1 === e && (r.style.display = "table"), 100 === e && (v = !0)
-                            };
-                        if ((o = i(o, e)).isAndroidButNotChrome || o.isBrowserOutOfDate || !o.isPropertySupported) {
-                            if (f = o.isBrowserUnsupported, v && "1" !== r.style.opacity) {
-                                v = !1;
-                                for (var S = 1; S <= 100; S++) setTimeout(function(e) {
+                                o = e, r.style.opacity = o / 100, r.style.filter = "alpha(opacity=" + o + ")", 1 === e && (r.style.display = "table"), 100 === e && (g = !0)
+                            },
+                            e = f(e, h);
+                        if (e.isAndroidButNotChrome || e.isBrowserOutOfDate || !e.isPropertySupported) {
+                            if (c = e.isBrowserUnsupported, g && "1" !== r.style.opacity) {
+                                g = !1;
+                                for (var b = 1; b <= 100; b++) setTimeout(function(e) {
                                     return function() {
-                                        y(e)
+                                        m(e)
                                     }
-                                }(S), 8 * S)
+                                }(b), 8 * b)
                             }
-                            o = document.getElementById("outdated"), d && o.classList.add("fullscreen"), o.innerHTML = (b = a[m = p] || a.en, h = e.messages && e.messages[m], b = {
-                                web: "<p>" + (m = s({}, b, h)).update.web + (m.url ? '<a id="buttonUpdateBrowser" rel="nofollow" href="' + m.url + '">' + m.callToAction + "</a>" : "") + "</p>",
-                                googlePlay: "<p>" + m.update.googlePlay + '<a id="buttonUpdateBrowser" rel="nofollow" href="https://play.google.com/store/apps/details?id=com.android.chrome">' + m.callToAction + "</a></p>",
-                                appStore: "<p>" + m.update[w] + "</p>"
-                            } [w], h = m.outOfDate, f && m.unsupported && (h = m.unsupported), '<div class="vertical-center"><h6>' + h + "</h6>" + b + '<p class="last"><a href="#" id="buttonCloseUpdateBrowser" title="' + m.close + '">&times;</a></p></div>'), c = document.getElementById("buttonCloseUpdateBrowser"), g = document.getElementById("buttonUpdateBrowser"), r.style.backgroundColor = n, r.style.color = u, r.children[0].children[0].style.color = u, r.children[0].children[1].style.color = u, g && (g.style.color = u, g.style.borderColor && (g.style.borderColor = u), g.onmouseover = function() {
-                                this.style.color = n, this.style.backgroundColor = u
-                            }, g.onmouseout = function() {
-                                this.style.color = u, this.style.backgroundColor = n
-                            }), c.style.color = u, c.onmousedown = function() {
+                            e = document.getElementById("outdated");
+                            s && e.classList.add("fullscreen"), e.innerHTML = (p = v[d = t] || v.en, w = h.messages && h.messages[d], d = y({}, p, w), p = {
+                                web: "<p>" + d.update.web + (d.url ? '<a id="buttonUpdateBrowser" rel="nofollow" href="' + d.url + '">' + d.callToAction + "</a>" : "") + "</p>",
+                                googlePlay: "<p>" + d.update.googlePlay + '<a id="buttonUpdateBrowser" rel="nofollow" href="https://play.google.com/store/apps/details?id=com.android.chrome">' + d.callToAction + "</a></p>",
+                                appStore: "<p>" + d.update[l] + "</p>"
+                            } [l], w = d.outOfDate, c && d.unsupported && (w = d.unsupported), '<div class="vertical-center"><h6>' + w + "</h6>" + p + '<p class="last"><a href="#" id="buttonCloseUpdateBrowser" title="' + d.close + '">&times;</a></p></div>'), n = document.getElementById("buttonCloseUpdateBrowser"), u = document.getElementById("buttonUpdateBrowser"), r.style.backgroundColor = i, r.style.color = a, r.children[0].children[0].style.color = a, r.children[0].children[1].style.color = a, u && (u.style.color = a, u.style.borderColor && (u.style.borderColor = a), u.onmouseover = function() {
+                                this.style.color = i, this.style.backgroundColor = a
+                            }, u.onmouseout = function() {
+                                this.style.color = a, this.style.backgroundColor = i
+                            }), n.style.color = a, n.onmousedown = function() {
                                 return !(r.style.display = "none")
                             }
                         }
                     },
-                    r = window.onload;
-                "function" != typeof window.onload ? window.onload = o : window.onload = function() {
-                    r && r(), o()
+                    o = window.onload;
+                "function" != typeof window.onload ? window.onload = e : window.onload = function() {
+                    o && o(), e()
                 }
             }
         }, {
             "./evaluateBrowser": 1,
             "./extend": 2,
             "./languages.json": 4,
             "ua-parser-js": 5
         }],
         4: [function(e, o, r) {
             o.exports = {
                 ko: {
-                    outOfDate: "\ucd5c\uc2e0 \ube0c\ub77c\uc6b0\uc800\uac00 \uc544\ub2d9\ub2c8\ub2e4!",
+                    outOfDate: "최신 브라우저가 아닙니다!",
                     update: {
-                        web: "\uc6f9\uc0ac\uc774\ud2b8\ub97c \uc81c\ub300\ub85c \ubcf4\ub824\uba74 \ube0c\ub77c\uc6b0\uc800\ub97c \uc5c5\ub370\uc774\ud2b8\ud558\uc138\uc694.",
-                        googlePlay: "Google Play\uc5d0\uc11c Chrome\uc744 \uc124\uce58\ud558\uc138\uc694",
-                        appStore: "\uc124\uc815 \uc571\uc5d0\uc11c iOS\ub97c \uc5c5\ub370\uc774\ud2b8\ud558\uc138\uc694"
+                        web: "웹사이트를 제대로 보려면 브라우저를 업데이트하세요.",
+                        googlePlay: "Google Play에서 Chrome을 설치하세요",
+                        appStore: "설정 앱에서 iOS를 업데이트하세요"
                     },
                     url: "https://browser-update.org/update-browser.html",
-                    callToAction: "\uc9c0\uae08 \ube0c\ub77c\uc6b0\uc800 \uc5c5\ub370\uc774\ud2b8\ud558\uae30",
-                    close: "\ub2eb\uae30"
+                    callToAction: "지금 브라우저 업데이트하기",
+                    close: "닫기"
                 },
                 ja: {
-                    outOfDate: "\u53e4\u3044\u30d6\u30e9\u30a6\u30b6\u3092\u304a\u4f7f\u3044\u306e\u3088\u3046\u3067\u3059\u3002",
+                    outOfDate: "古いブラウザをお使いのようです。",
                     update: {
-                        web: "\u30a6\u30a7\u30d6\u30b5\u30a4\u30c8\u3092\u6b63\u3057\u304f\u8868\u793a\u3067\u304d\u308b\u3088\u3046\u306b\u3001\u30d6\u30e9\u30a6\u30b6\u3092\u30a2\u30c3\u30d7\u30c7\u30fc\u30c8\u3057\u3066\u304f\u3060\u3055\u3044\u3002",
-                        googlePlay: "Google Play\u304b\u3089Chrome\u3092\u30a4\u30f3\u30b9\u30c8\u30fc\u30eb\u3057\u3066\u304f\u3060\u3055\u3044",
-                        appStore: "\u8a2d\u5b9a\u304b\u3089iOS\u3092\u30a2\u30c3\u30d7\u30c7\u30fc\u30c8\u3057\u3066\u304f\u3060\u3055\u3044"
+                        web: "ウェブサイトを正しく表示できるように、ブラウザをアップデートしてください。",
+                        googlePlay: "Google PlayからChromeをインストールしてください",
+                        appStore: "設定からiOSをアップデートしてください"
                     },
                     url: "https://browser-update.org/update-browser.html",
-                    callToAction: "\u4eca\u3059\u3050\u30d6\u30e9\u30a6\u30b6\u3092\u30a2\u30c3\u30d7\u30c7\u30fc\u30c8\u3059\u308b",
-                    close: "\u9589\u3058\u308b"
+                    callToAction: "今すぐブラウザをアップデートする",
+                    close: "閉じる"
                 },
                 br: {
                     outOfDate: "O seu navegador est&aacute; desatualizado!",
                     update: {
                         web: "Atualize o seu navegador para ter uma melhor experi&ecirc;ncia e visualiza&ccedil;&atilde;o deste site. ",
                         googlePlay: "Please install Chrome from Google Play",
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
                     callToAction: "Atualize o seu navegador agora",
                     close: "Fechar"
                 },
                 ca: {
-                    outOfDate: "El vostre navegador no est\xe0 actualitzat!",
+                    outOfDate: "El vostre navegador no està actualitzat!",
                     update: {
                         web: "Actualitzeu el vostre navegador per veure correctament aquest lloc web. ",
-                        googlePlay: "Instal\xb7leu Chrome des de Google Play",
-                        appStore: "Actualitzeu iOS des de l'aplicaci\xf3 Configuraci\xf3"
+                        googlePlay: "Instal·leu Chrome des de Google Play",
+                        appStore: "Actualitzeu iOS des de l'aplicació Configuració"
                     },
                     url: "https://browser-update.org/update-browser.html",
                     callToAction: "Actualitzar el meu navegador ara",
                     close: "Tancar"
                 },
                 zh: {
-                    outOfDate: "\u60a8\u7684\u6d4f\u89c8\u5668\u5df2\u8fc7\u65f6",
+                    outOfDate: "您的浏览器已过时",
                     update: {
-                        web: "\u8981\u6b63\u5e38\u6d4f\u89c8\u672c\u7f51\u7ad9\u8bf7\u5347\u7ea7\u60a8\u7684\u6d4f\u89c8\u5668\u3002",
+                        web: "要正常浏览本网站请升级您的浏览器。",
                         googlePlay: "Please install Chrome from Google Play",
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
-                    callToAction: "\u73b0\u5728\u5347\u7ea7",
-                    close: "\u5173\u95ed"
+                    callToAction: "现在升级",
+                    close: "关闭"
                 },
                 cz: {
-                    outOfDate: "V\xe1\u0161 prohl\xed\u017ee\u010d je zastaral\xfd!",
+                    outOfDate: "Váš prohlížeč je zastaralý!",
                     update: {
-                        web: "Pro spr\xe1vn\xe9 zobrazen\xed t\u011bchto str\xe1nek aktualizujte sv\u016fj prohl\xed\u017ee\u010d. ",
+                        web: "Pro správné zobrazení těchto stránek aktualizujte svůj prohlížeč. ",
                         googlePlay: "Nainstalujte si Chrome z Google Play",
-                        appStore: "Aktualizujte si syst\xe9m iOS"
+                        appStore: "Aktualizujte si systém iOS"
                     },
                     url: "https://browser-update.org/update-browser.html",
-                    callToAction: "Aktualizovat nyn\xed sv\u016fj prohl\xed\u017ee\u010d",
-                    close: "Zav\u0159\xedt"
+                    callToAction: "Aktualizovat nyní svůj prohlížeč",
+                    close: "Zavřít"
                 },
                 da: {
-                    outOfDate: "Din browser er for\xe6ldet!",
+                    outOfDate: "Din browser er forældet!",
                     update: {
-                        web: "Opdat\xe9r din browser for at f\xe5 vist denne hjemmeside korrekt. ",
-                        googlePlay: "Install\xe9r venligst Chrome fra Google Play",
-                        appStore: "Opdat\xe9r venligst iOS"
+                        web: "Opdatér din browser for at få vist denne hjemmeside korrekt. ",
+                        googlePlay: "Installér venligst Chrome fra Google Play",
+                        appStore: "Opdatér venligst iOS"
                     },
                     url: "https://browser-update.org/update-browser.html",
-                    callToAction: "Opdat\xe9r din browser nu",
+                    callToAction: "Opdatér din browser nu",
                     close: "Luk"
                 },
                 de: {
                     outOfDate: "Ihr Browser ist veraltet!",
                     update: {
                         web: "Bitte aktualisieren Sie Ihren Browser, um diese Website korrekt darzustellen. ",
                         googlePlay: "Please install Chrome from Google Play",
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
                     callToAction: "Den Browser jetzt aktualisieren ",
-                    close: "Schlie\xdfen"
+                    close: "Schließen"
                 },
                 ee: {
                     outOfDate: "Sinu veebilehitseja on vananenud!",
                     update: {
-                        web: "Palun uuenda oma veebilehitsejat, et n\xe4ha lehek\xfclge korrektselt. ",
+                        web: "Palun uuenda oma veebilehitsejat, et näha lehekülge korrektselt. ",
                         googlePlay: "Please install Chrome from Google Play",
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
                     callToAction: "Uuenda oma veebilehitsejat kohe",
                     close: "Sulge"
                 },
@@ -257,67 +262,67 @@
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
                     callToAction: "Update my browser now",
                     close: "Close"
                 },
                 es: {
-                    outOfDate: "\xa1Tu navegador est\xe1 anticuado!",
+                    outOfDate: "¡Tu navegador está anticuado!",
                     update: {
-                        web: "Actualiza tu navegador para ver esta p\xe1gina correctamente. ",
+                        web: "Actualiza tu navegador para ver esta página correctamente. ",
                         googlePlay: "Please install Chrome from Google Play",
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
                     callToAction: "Actualizar mi navegador ahora",
                     close: "Cerrar"
                 },
                 fa: {
                     rightToLeft: !0,
-                    outOfDate: "\u0645\u0631\u0648\u0631\u06af\u0631 \u0634\u0645\u0627 \u0645\u0646\u0633\u0648\u062e \u0634\u062f\u0647 \u0627\u0633\u062a!",
+                    outOfDate: "مرورگر شما منسوخ شده است!",
                     update: {
-                        web: "\u062c\u0647\u062a \u0645\u0634\u0627\u0647\u062f\u0647 \u0635\u062d\u06cc\u062d \u0627\u06cc\u0646 \u0648\u0628\u0633\u0627\u06cc\u062a\u060c \u0645\u0631\u0648\u0631\u06af\u0631\u062a\u0627\u0646 \u0631\u0627 \u0628\u0631\u0648\u0632 \u0631\u0633\u0627\u0646\u06cc \u0646\u0645\u0627\u06cc\u06cc\u062f. ",
+                        web: "جهت مشاهده صحیح این وبسایت، مرورگرتان را بروز رسانی نمایید. ",
                         googlePlay: "Please install Chrome from Google Play",
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
-                    callToAction: "\u0647\u0645\u06cc\u0646 \u062d\u0627\u0644\u0627 \u0645\u0631\u0648\u0631\u06af\u0631\u0645 \u0631\u0627 \u0628\u0631\u0648\u0632 \u06a9\u0646",
+                    callToAction: "همین حالا مرورگرم را بروز کن",
                     close: "Close"
                 },
                 fi: {
                     outOfDate: "Selaimesi on vanhentunut!",
                     update: {
                         web: "Lataa ajantasainen selain n&auml;hd&auml;ksesi t&auml;m&auml;n sivun oikein. ",
                         googlePlay: "Asenna uusin Chrome Google Play -kaupasta",
-                        appStore: "P\xe4ivit\xe4 iOS puhelimesi asetuksista"
+                        appStore: "Päivitä iOS puhelimesi asetuksista"
                     },
                     url: "https://browser-update.org/update-browser.html",
                     callToAction: "P&auml;ivit&auml; selaimeni nyt ",
                     close: "Sulje"
                 },
                 fr: {
                     outOfDate: "Votre navigateur n'est plus compatible !",
                     update: {
-                        web: "Mettez \xe0 jour votre navigateur pour afficher correctement ce site Web. ",
+                        web: "Mettez à jour votre navigateur pour afficher correctement ce site Web. ",
                         googlePlay: "Merci d'installer Chrome depuis le Google Play Store",
-                        appStore: "Merci de mettre \xe0 jour iOS depuis l'application R\xe9glages"
+                        appStore: "Merci de mettre à jour iOS depuis l'application Réglages"
                     },
                     url: "https://browser-update.org/update-browser.html",
-                    callToAction: "Mettre \xe0 jour maintenant ",
+                    callToAction: "Mettre à jour maintenant ",
                     close: "Fermer"
                 },
                 hu: {
-                    outOfDate: "A b\xf6ng\xe9sz\u0151je elavult!",
+                    outOfDate: "A böngészője elavult!",
                     update: {
-                        web: "Firss\xedtse vagy cser\xe9lje le a b\xf6ng\xe9sz\u0151j\xe9t. ",
+                        web: "Firssítse vagy cserélje le a böngészőjét. ",
                         googlePlay: "Please install Chrome from Google Play",
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
-                    callToAction: "A b\xf6ng\xe9sz\u0151m friss\xedt\xe9se ",
+                    callToAction: "A böngészőm frissítése ",
                     close: "Close"
                 },
                 id: {
                     outOfDate: "Browser yang Anda gunakan sudah ketinggalan zaman!",
                     update: {
                         web: "Perbaharuilah browser Anda agar bisa menjelajahi website ini dengan nyaman. ",
                         googlePlay: "Please install Chrome from Google Play",
@@ -335,168 +340,168 @@
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
                     callToAction: "Aggiorna ora",
                     close: "Chiudi"
                 },
                 lt: {
-                    outOfDate: "J\u016bs\u0173 nar\u0161ykl\u0117s versija yra pasenusi!",
+                    outOfDate: "Jūsų naršyklės versija yra pasenusi!",
                     update: {
-                        web: "Atnaujinkite savo nar\u0161ykl\u0119, kad gal\u0117tum\u0117te per\u017ei\u016br\u0117ti \u0161i\u0105 svetain\u0119 tinkamai. ",
+                        web: "Atnaujinkite savo naršyklę, kad galėtumėte peržiūrėti šią svetainę tinkamai. ",
                         googlePlay: "Please install Chrome from Google Play",
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
-                    callToAction: "Atnaujinti nar\u0161ykl\u0119 ",
+                    callToAction: "Atnaujinti naršyklę ",
                     close: "Close"
                 },
                 nl: {
                     outOfDate: "Je gebruikt een oude browser!",
                     update: {
                         web: "Update je browser om deze website correct te bekijken. ",
                         googlePlay: "Please install Chrome from Google Play",
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
                     callToAction: "Update mijn browser nu ",
                     close: "Sluiten"
                 },
                 pl: {
-                    outOfDate: "Twoja przegl\u0105darka jest przestarza\u0142a!",
+                    outOfDate: "Twoja przeglądarka jest przestarzała!",
                     update: {
-                        web: "Zaktualizuj swoj\u0105 przegl\u0105dark\u0119, aby poprawnie wy\u015bwietli\u0107 t\u0119 stron\u0119. ",
-                        googlePlay: "Prosz\u0119 zainstalowa\u0107 przegl\u0105dark\u0119 Chrome ze sklepu Google Play",
-                        appStore: "Prosz\u0119 zaktualizowa\u0107 iOS z Ustawie\u0144"
+                        web: "Zaktualizuj swoją przeglądarkę, aby poprawnie wyświetlić tę stronę. ",
+                        googlePlay: "Proszę zainstalować przeglądarkę Chrome ze sklepu Google Play",
+                        appStore: "Proszę zaktualizować iOS z Ustawień"
                     },
                     url: "https://browser-update.org/update-browser.html",
-                    callToAction: "Zaktualizuj przegl\u0105dark\u0119 ju\u017c teraz",
+                    callToAction: "Zaktualizuj przeglądarkę już teraz",
                     close: "Zamknij"
                 },
                 pt: {
                     outOfDate: "O seu browser est&aacute; desatualizado!",
                     update: {
                         web: "Atualize o seu browser para ter uma melhor experi&ecirc;ncia e visualiza&ccedil;&atilde;o deste site. ",
                         googlePlay: "Please install Chrome from Google Play",
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
                     callToAction: "Atualize o seu browser agora",
                     close: "Fechar"
                 },
                 ro: {
-                    outOfDate: "Browserul este \xeenvechit!",
+                    outOfDate: "Browserul este învechit!",
                     update: {
-                        web: "Actualiza\u021bi browserul pentru a vizualiza corect acest site. ",
+                        web: "Actualizați browserul pentru a vizualiza corect acest site. ",
                         googlePlay: "Please install Chrome from Google Play",
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
-                    callToAction: "Actualiza\u021bi browserul acum!",
+                    callToAction: "Actualizați browserul acum!",
                     close: "Close"
                 },
                 ru: {
-                    outOfDate: "\u0412\u0430\u0448 \u0431\u0440\u0430\u0443\u0437\u0435\u0440 \u0443\u0441\u0442\u0430\u0440\u0435\u043b!",
+                    outOfDate: "Ваш браузер устарел!",
                     update: {
-                        web: "\u041e\u0431\u043d\u043e\u0432\u0438\u0442\u0435 \u0432\u0430\u0448 \u0431\u0440\u0430\u0443\u0437\u0435\u0440 \u0434\u043b\u044f \u043f\u0440\u0430\u0432\u0438\u043b\u044c\u043d\u043e\u0433\u043e \u043e\u0442\u043e\u0431\u0440\u0430\u0436\u0435\u043d\u0438\u044f \u044d\u0442\u043e\u0433\u043e \u0441\u0430\u0439\u0442\u0430. ",
+                        web: "Обновите ваш браузер для правильного отображения этого сайта. ",
                         googlePlay: "Please install Chrome from Google Play",
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
-                    callToAction: "\u041e\u0431\u043d\u043e\u0432\u0438\u0442\u044c \u043c\u043e\u0439 \u0431\u0440\u0430\u0443\u0437\u0435\u0440 ",
-                    close: "\u0417\u0430\u043a\u0440\u044b\u0442\u044c"
+                    callToAction: "Обновить мой браузер ",
+                    close: "Закрыть"
                 },
                 si: {
-                    outOfDate: "Va\u0161 brskalnik je zastarel!",
+                    outOfDate: "Vaš brskalnik je zastarel!",
                     update: {
-                        web: "Za pravilen prikaz spletne strani posodobite va\u0161 brskalnik. ",
+                        web: "Za pravilen prikaz spletne strani posodobite vaš brskalnik. ",
                         googlePlay: "Please install Chrome from Google Play",
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
                     callToAction: "Posodobi brskalnik ",
                     close: "Zapri"
                 },
                 sv: {
-                    outOfDate: "Din webbl\xe4sare st\xf6djs ej l\xe4ngre!",
+                    outOfDate: "Din webbläsare stödjs ej längre!",
                     update: {
-                        web: "Uppdatera din webbl\xe4sare f\xf6r att webbplatsen ska visas korrekt. ",
+                        web: "Uppdatera din webbläsare för att webbplatsen ska visas korrekt. ",
                         googlePlay: "Please install Chrome from Google Play",
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
-                    callToAction: "Uppdatera min webbl\xe4sare nu",
-                    close: "St\xe4ng"
+                    callToAction: "Uppdatera min webbläsare nu",
+                    close: "Stäng"
                 },
                 ua: {
-                    outOfDate: "\u0412\u0430\u0448 \u0431\u0440\u0430\u0443\u0437\u0435\u0440 \u0437\u0430\u0441\u0442\u0430\u0440\u0456\u0432!",
+                    outOfDate: "Ваш браузер застарів!",
                     update: {
-                        web: "\u041e\u043d\u043e\u0432\u0456\u0442\u044c \u0432\u0430\u0448 \u0431\u0440\u0430\u0443\u0437\u0435\u0440 \u0434\u043b\u044f \u043f\u0440\u0430\u0432\u0438\u043b\u044c\u043d\u043e\u0433\u043e \u0432\u0456\u0434\u043e\u0431\u0440\u0430\u0436\u0435\u043d\u043d\u044f \u0446\u044c\u043e\u0433\u043e \u0441\u0430\u0439\u0442\u0430. ",
+                        web: "Оновіть ваш браузер для правильного відображення цього сайта. ",
                         googlePlay: "Please install Chrome from Google Play",
                         appStore: "Please update iOS from the Settings App"
                     },
                     url: "https://browser-update.org/update-browser.html",
-                    callToAction: "\u041e\u043d\u043e\u0432\u0438\u0442\u0438 \u043c\u0456\u0439 \u0431\u0440\u0430\u0443\u0437\u0435\u0440 ",
-                    close: "\u0417\u0430\u043a\u0440\u0438\u0442\u0438"
+                    callToAction: "Оновити мій браузер ",
+                    close: "Закрити"
                 }
             }
         }, {}],
-        5: [function(e, o, r) {
-            ! function(e, i) {
+        5: [function(e, k, A) {
+            ! function(a, p) {
                 "use strict";
-                var a = "function",
-                    s = "undefined",
-                    t = "model",
-                    l = "name",
-                    n = "type",
-                    u = "vendor",
-                    d = "version",
-                    p = "architecture",
-                    w = "console",
-                    c = "mobile",
-                    g = "tablet",
-                    m = "smarttv",
-                    b = "wearable",
-                    h = {
+                var w = "function",
+                    e = "undefined",
+                    o = "model",
+                    r = "name",
+                    i = "type",
+                    s = "vendor",
+                    t = "version",
+                    l = "architecture",
+                    n = "console",
+                    u = "mobile",
+                    d = "tablet",
+                    c = "smarttv",
+                    g = "wearable",
+                    m = {
                         extend: function(e, o) {
                             var r, i = {};
                             for (r in e) o[r] && o[r].length % 2 == 0 ? i[r] = o[r].concat(e[r]) : i[r] = e[r];
                             return i
                         },
                         has: function(e, o) {
                             return "string" == typeof e && -1 !== o.toLowerCase().indexOf(e.toLowerCase())
                         },
                         lowerize: function(e) {
                             return e.toLowerCase()
                         },
                         major: function(e) {
-                            return "string" == typeof e ? e.replace(/[^\d\.]/g, "").split(".")[0] : i
+                            return "string" == typeof e ? e.replace(/[^\d\.]/g, "").split(".")[0] : p
                         },
                         trim: function(e) {
                             return e.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, "")
                         }
                     },
-                    f = {
+                    b = {
                         rgx: function(e, o) {
-                            for (var r, s, t, l, n, u = 0; u < o.length && !l;) {
-                                for (var d = o[u], p = o[u + 1], w = r = 0; w < d.length && !l;)
-                                    if (l = d[w++].exec(e))
-                                        for (s = 0; s < p.length; s++) n = l[++r], "object" == typeof(t = p[s]) && 0 < t.length ? 2 == t.length ? typeof t[1] == a ? this[t[0]] = t[1].call(this, n) : this[t[0]] = t[1] : 3 == t.length ? typeof t[1] != a || t[1].exec && t[1].test ? this[t[0]] = n ? n.replace(t[1], t[2]) : i : this[t[0]] = n ? t[1].call(this, n, t[2]) : i : 4 == t.length && (this[t[0]] = n ? t[3].call(this, n.replace(t[1], t[2])) : i) : this[t] = n || i;
-                                u += 2
+                            for (var r, i, a, s, t, l = 0; l < o.length && !s;) {
+                                for (var n = o[l], u = o[l + 1], d = r = 0; d < n.length && !s;)
+                                    if (s = n[d++].exec(e))
+                                        for (i = 0; i < u.length; i++) t = s[++r], "object" == typeof(a = u[i]) && 0 < a.length ? 2 == a.length ? typeof a[1] == w ? this[a[0]] = a[1].call(this, t) : this[a[0]] = a[1] : 3 == a.length ? typeof a[1] != w || a[1].exec && a[1].test ? this[a[0]] = t ? t.replace(a[1], a[2]) : p : this[a[0]] = t ? a[1].call(this, t, a[2]) : p : 4 == a.length && (this[a[0]] = t ? a[3].call(this, t.replace(a[1], a[2])) : p) : this[a] = t || p;
+                                l += 2
                             }
                         },
                         str: function(e, o) {
                             for (var r in o)
                                 if ("object" == typeof o[r] && 0 < o[r].length) {
-                                    for (var a = 0; a < o[r].length; a++)
-                                        if (h.has(o[r][a], e)) return "?" === r ? i : r
-                                } else if (h.has(o[r], e)) return "?" === r ? i : r;
+                                    for (var i = 0; i < o[r].length; i++)
+                                        if (m.has(o[r][i], e)) return "?" === r ? p : r
+                                } else if (m.has(o[r], e)) return "?" === r ? p : r;
                             return e
                         }
                     },
-                    v = {
+                    h = {
                         browser: {
                             oldsafari: {
                                 version: {
                                     "1.0": "/8",
                                     1.2: "/1",
                                     1.3: "/3",
                                     "2.0": "/412",
@@ -537,638 +542,638 @@
                                     8.1: "NT 6.3",
                                     10: ["NT 6.4", "NT 10.0"],
                                     RT: "ARM"
                                 }
                             }
                         }
                     },
-                    y = {
+                    f = {
                         browser: [
                             [/(opera\smini)\/([\w\.-]+)/i, /(opera\s[mobiletab]+).+version\/([\w\.-]+)/i, /(opera).+version\/([\w\.]+)/i, /(opera)[\/\s]+([\w\.]+)/i],
-                            [l, d],
+                            [r, t],
                             [/(opios)[\/\s]+([\w\.]+)/i],
                             [
-                                [l, "Opera Mini"], d
+                                [r, "Opera Mini"], t
                             ],
                             [/\s(opr)\/([\w\.]+)/i],
                             [
-                                [l, "Opera"], d
+                                [r, "Opera"], t
                             ],
                             [/(kindle)\/([\w\.]+)/i, /(lunascape|maxthon|netfront|jasmine|blazer)[\/\s]?([\w\.]*)/i, /(avant\s|iemobile|slim)(?:browser)?[\/\s]?([\w\.]*)/i, /(bidubrowser|baidubrowser)[\/\s]?([\w\.]+)/i, /(?:ms|\()(ie)\s([\w\.]+)/i, /(rekonq)\/([\w\.]*)/i, /(chromium|flock|rockmelt|midori|epiphany|silk|skyfire|ovibrowser|bolt|iron|vivaldi|iridium|phantomjs|bowser|quark|qupzilla|falkon)\/([\w\.-]+)/i],
-                            [l, d],
+                            [r, t],
                             [/(konqueror)\/([\w\.]+)/i],
                             [
-                                [l, "Konqueror"], d
+                                [r, "Konqueror"], t
                             ],
                             [/(trident).+rv[:\s]([\w\.]+).+like\sgecko/i],
                             [
-                                [l, "IE"], d
+                                [r, "IE"], t
                             ],
                             [/(edge|edgios|edga|edg)\/((\d+)?[\w\.]+)/i],
                             [
-                                [l, "Edge"], d
+                                [r, "Edge"], t
                             ],
                             [/(yabrowser)\/([\w\.]+)/i],
                             [
-                                [l, "Yandex"], d
+                                [r, "Yandex"], t
                             ],
                             [/(Avast)\/([\w\.]+)/i],
                             [
-                                [l, "Avast Secure Browser"], d
+                                [r, "Avast Secure Browser"], t
                             ],
                             [/(AVG)\/([\w\.]+)/i],
                             [
-                                [l, "AVG Secure Browser"], d
+                                [r, "AVG Secure Browser"], t
                             ],
                             [/(puffin)\/([\w\.]+)/i],
                             [
-                                [l, "Puffin"], d
+                                [r, "Puffin"], t
                             ],
                             [/(focus)\/([\w\.]+)/i],
                             [
-                                [l, "Firefox Focus"], d
+                                [r, "Firefox Focus"], t
                             ],
                             [/(opt)\/([\w\.]+)/i],
                             [
-                                [l, "Opera Touch"], d
+                                [r, "Opera Touch"], t
                             ],
                             [/((?:[\s\/])uc?\s?browser|(?:juc.+)ucweb)[\/\s]?([\w\.]+)/i],
                             [
-                                [l, "UCBrowser"], d
+                                [r, "UCBrowser"], t
                             ],
                             [/(comodo_dragon)\/([\w\.]+)/i],
                             [
-                                [l, /_/g, " "], d
+                                [r, /_/g, " "], t
                             ],
                             [/(windowswechat qbcore)\/([\w\.]+)/i],
                             [
-                                [l, "WeChat(Win) Desktop"], d
+                                [r, "WeChat(Win) Desktop"], t
                             ],
                             [/(micromessenger)\/([\w\.]+)/i],
                             [
-                                [l, "WeChat"], d
+                                [r, "WeChat"], t
                             ],
                             [/(brave)\/([\w\.]+)/i],
                             [
-                                [l, "Brave"], d
+                                [r, "Brave"], t
                             ],
                             [/(qqbrowserlite)\/([\w\.]+)/i],
-                            [l, d],
+                            [r, t],
                             [/(QQ)\/([\d\.]+)/i],
-                            [l, d],
+                            [r, t],
                             [/m?(qqbrowser)[\/\s]?([\w\.]+)/i],
-                            [l, d],
+                            [r, t],
                             [/(baiduboxapp)[\/\s]?([\w\.]+)/i],
-                            [l, d],
+                            [r, t],
                             [/(2345Explorer)[\/\s]?([\w\.]+)/i],
-                            [l, d],
+                            [r, t],
                             [/(MetaSr)[\/\s]?([\w\.]+)/i],
-                            [l],
+                            [r],
                             [/(LBBROWSER)/i],
-                            [l],
+                            [r],
                             [/xiaomi\/miuibrowser\/([\w\.]+)/i],
-                            [d, [l, "MIUI Browser"]],
+                            [t, [r, "MIUI Browser"]],
                             [/;fbav\/([\w\.]+);/i],
-                            [d, [l, "Facebook"]],
+                            [t, [r, "Facebook"]],
                             [/safari\s(line)\/([\w\.]+)/i, /android.+(line)\/([\w\.]+)\/iab/i],
-                            [l, d],
+                            [r, t],
                             [/headlesschrome(?:\/([\w\.]+)|\s)/i],
-                            [d, [l, "Chrome Headless"]],
+                            [t, [r, "Chrome Headless"]],
                             [/\swv\).+(chrome)\/([\w\.]+)/i],
                             [
-                                [l, /(.+)/, "$1 WebView"], d
+                                [r, /(.+)/, "$1 WebView"], t
                             ],
                             [/((?:oculus|samsung)browser)\/([\w\.]+)/i],
                             [
-                                [l, /(.+(?:g|us))(.+)/, "$1 $2"], d
+                                [r, /(.+(?:g|us))(.+)/, "$1 $2"], t
                             ],
                             [/android.+version\/([\w\.]+)\s+(?:mobile\s?safari|safari)*/i],
-                            [d, [l, "Android Browser"]],
+                            [t, [r, "Android Browser"]],
                             [/(sailfishbrowser)\/([\w\.]+)/i],
                             [
-                                [l, "Sailfish Browser"], d
+                                [r, "Sailfish Browser"], t
                             ],
                             [/(chrome|omniweb|arora|[tizenoka]{5}\s?browser)\/v?([\w\.]+)/i],
-                            [l, d],
+                            [r, t],
                             [/(dolfin)\/([\w\.]+)/i],
                             [
-                                [l, "Dolphin"], d
+                                [r, "Dolphin"], t
                             ],
                             [/(qihu|qhbrowser|qihoobrowser|360browser)/i],
                             [
-                                [l, "360 Browser"]
+                                [r, "360 Browser"]
                             ],
                             [/((?:android.+)crmo|crios)\/([\w\.]+)/i],
                             [
-                                [l, "Chrome"], d
+                                [r, "Chrome"], t
                             ],
                             [/(coast)\/([\w\.]+)/i],
                             [
-                                [l, "Opera Coast"], d
+                                [r, "Opera Coast"], t
                             ],
                             [/fxios\/([\w\.-]+)/i],
-                            [d, [l, "Firefox"]],
+                            [t, [r, "Firefox"]],
                             [/version\/([\w\.]+).+?mobile\/\w+\s(safari)/i],
-                            [d, [l, "Mobile Safari"]],
+                            [t, [r, "Mobile Safari"]],
                             [/version\/([\w\.]+).+?(mobile\s?safari|safari)/i],
-                            [d, l],
+                            [t, r],
                             [/webkit.+?(gsa)\/([\w\.]+).+?(mobile\s?safari|safari)(\/[\w\.]+)/i],
                             [
-                                [l, "GSA"], d
+                                [r, "GSA"], t
                             ],
                             [/webkit.+?(mobile\s?safari|safari)(\/[\w\.]+)/i],
-                            [l, [d, f.str, v.browser.oldsafari.version]],
+                            [r, [t, b.str, h.browser.oldsafari.version]],
                             [/(webkit|khtml)\/([\w\.]+)/i],
-                            [l, d],
+                            [r, t],
                             [/(navigator|netscape)\/([\w\.-]+)/i],
                             [
-                                [l, "Netscape"], d
+                                [r, "Netscape"], t
                             ],
                             [/(swiftfox)/i, /(icedragon|iceweasel|camino|chimera|fennec|maemo\sbrowser|minimo|conkeror)[\/\s]?([\w\.\+]+)/i, /(firefox|seamonkey|k-meleon|icecat|iceape|firebird|phoenix|palemoon|basilisk|waterfox)\/([\w\.-]+)$/i, /(mozilla)\/([\w\.]+).+rv\:.+gecko\/\d+/i, /(polaris|lynx|dillo|icab|doris|amaya|w3m|netsurf|sleipnir)[\/\s]?([\w\.]+)/i, /(links)\s\(([\w\.]+)/i, /(gobrowser)\/?([\w\.]*)/i, /(ice\s?browser)\/v?([\w\._]+)/i, /(mosaic)[\/\s]([\w\.]+)/i],
-                            [l, d]
+                            [r, t]
                         ],
                         cpu: [
                             [/(?:(amd|x(?:(?:86|64)[_-])?|wow|win)64)[;\)]/i],
                             [
-                                [p, "amd64"]
+                                [l, "amd64"]
                             ],
                             [/(ia32(?=;))/i],
                             [
-                                [p, h.lowerize]
+                                [l, m.lowerize]
                             ],
                             [/((?:i[346]|x)86)[;\)]/i],
                             [
-                                [p, "ia32"]
+                                [l, "ia32"]
                             ],
                             [/windows\s(ce|mobile);\sppc;/i],
                             [
-                                [p, "arm"]
+                                [l, "arm"]
                             ],
                             [/((?:ppc|powerpc)(?:64)?)(?:\smac|;|\))/i],
                             [
-                                [p, /ower/, "", h.lowerize]
+                                [l, /ower/, "", m.lowerize]
                             ],
                             [/(sun4\w)[;\)]/i],
                             [
-                                [p, "sparc"]
+                                [l, "sparc"]
                             ],
                             [/((?:avr32|ia64(?=;))|68k(?=\))|arm(?:64|(?=v\d+[;l]))|(?=atmel\s)avr|(?:irix|mips|sparc)(?:64)?(?=;)|pa-risc)/i],
                             [
-                                [p, h.lowerize]
+                                [l, m.lowerize]
                             ]
                         ],
                         device: [
                             [/\((ipad|playbook);[\w\s\),;-]+(rim|apple)/i],
-                            [t, u, [n, g]],
+                            [o, s, [i, d]],
                             [/applecoremedia\/[\w\.]+ \((ipad)/],
-                            [t, [u, "Apple"],
-                                [n, g]
+                            [o, [s, "Apple"],
+                                [i, d]
                             ],
                             [/(apple\s{0,1}tv)/i],
                             [
-                                [t, "Apple TV"],
-                                [u, "Apple"],
-                                [n, m]
+                                [o, "Apple TV"],
+                                [s, "Apple"],
+                                [i, c]
                             ],
                             [/(archos)\s(gamepad2?)/i, /(hp).+(touchpad)/i, /(hp).+(tablet)/i, /(kindle)\/([\w\.]+)/i, /\s(nook)[\w\s]+build\/(\w+)/i, /(dell)\s(strea[kpr\s\d]*[\dko])/i],
-                            [u, t, [n, g]],
+                            [s, o, [i, d]],
                             [/(kf[A-z]+)\sbuild\/.+silk\//i],
-                            [t, [u, "Amazon"],
-                                [n, g]
+                            [o, [s, "Amazon"],
+                                [i, d]
                             ],
                             [/(sd|kf)[0349hijorstuw]+\sbuild\/.+silk\//i],
                             [
-                                [t, f.str, v.device.amazon.model],
-                                [u, "Amazon"],
-                                [n, c]
+                                [o, b.str, h.device.amazon.model],
+                                [s, "Amazon"],
+                                [i, u]
                             ],
                             [/android.+aft([bms])\sbuild/i],
-                            [t, [u, "Amazon"],
-                                [n, m]
+                            [o, [s, "Amazon"],
+                                [i, c]
                             ],
                             [/\((ip[honed|\s\w*]+);.+(apple)/i],
-                            [t, u, [n, c]],
+                            [o, s, [i, u]],
                             [/\((ip[honed|\s\w*]+);/i],
-                            [t, [u, "Apple"],
-                                [n, c]
+                            [o, [s, "Apple"],
+                                [i, u]
                             ],
                             [/(blackberry)[\s-]?(\w+)/i, /(blackberry|benq|palm(?=\-)|sonyericsson|acer|asus|dell|meizu|motorola|polytron)[\s_-]?([\w-]*)/i, /(hp)\s([\w\s]+\w)/i, /(asus)-?(\w+)/i],
-                            [u, t, [n, c]],
+                            [s, o, [i, u]],
                             [/\(bb10;\s(\w+)/i],
-                            [t, [u, "BlackBerry"],
-                                [n, c]
+                            [o, [s, "BlackBerry"],
+                                [i, u]
                             ],
                             [/android.+(transfo[prime\s]{4,10}\s\w+|eeepc|slider\s\w+|nexus 7|padfone|p00c)/i],
-                            [t, [u, "Asus"],
-                                [n, g]
+                            [o, [s, "Asus"],
+                                [i, d]
                             ],
                             [/(sony)\s(tablet\s[ps])\sbuild\//i, /(sony)?(?:sgp.+)\sbuild\//i],
                             [
-                                [u, "Sony"],
-                                [t, "Xperia Tablet"],
-                                [n, g]
+                                [s, "Sony"],
+                                [o, "Xperia Tablet"],
+                                [i, d]
                             ],
                             [/android.+\s([c-g]\d{4}|so[-l]\w+)(?=\sbuild\/|\).+chrome\/(?![1-6]{0,1}\d\.))/i],
-                            [t, [u, "Sony"],
-                                [n, c]
+                            [o, [s, "Sony"],
+                                [i, u]
                             ],
                             [/\s(ouya)\s/i, /(nintendo)\s([wids3u]+)/i],
-                            [u, t, [n, w]],
+                            [s, o, [i, n]],
                             [/android.+;\s(shield)\sbuild/i],
-                            [t, [u, "Nvidia"],
-                                [n, w]
+                            [o, [s, "Nvidia"],
+                                [i, n]
                             ],
                             [/(playstation\s[34portablevi]+)/i],
-                            [t, [u, "Sony"],
-                                [n, w]
+                            [o, [s, "Sony"],
+                                [i, n]
                             ],
                             [/(sprint\s(\w+))/i],
                             [
-                                [u, f.str, v.device.sprint.vendor],
-                                [t, f.str, v.device.sprint.model],
-                                [n, c]
+                                [s, b.str, h.device.sprint.vendor],
+                                [o, b.str, h.device.sprint.model],
+                                [i, u]
                             ],
                             [/(htc)[;_\s-]+([\w\s]+(?=\)|\sbuild)|\w+)/i, /(zte)-(\w*)/i, /(alcatel|geeksphone|nexian|panasonic|(?=;\s)sony)[_\s-]?([\w-]*)/i],
-                            [u, [t, /_/g, " "],
-                                [n, c]
+                            [s, [o, /_/g, " "],
+                                [i, u]
                             ],
                             [/(nexus\s9)/i],
-                            [t, [u, "HTC"],
-                                [n, g]
+                            [o, [s, "HTC"],
+                                [i, d]
                             ],
                             [/d\/huawei([\w\s-]+)[;\)]/i, /(nexus\s6p|vog-l29|ane-lx1|eml-l29|ele-l29)/i],
-                            [t, [u, "Huawei"],
-                                [n, c]
+                            [o, [s, "Huawei"],
+                                [i, u]
                             ],
                             [/android.+(bah2?-a?[lw]\d{2})/i],
-                            [t, [u, "Huawei"],
-                                [n, g]
+                            [o, [s, "Huawei"],
+                                [i, d]
                             ],
                             [/(microsoft);\s(lumia[\s\w]+)/i],
-                            [u, t, [n, c]],
+                            [s, o, [i, u]],
                             [/[\s\(;](xbox(?:\sone)?)[\s\);]/i],
-                            [t, [u, "Microsoft"],
-                                [n, w]
+                            [o, [s, "Microsoft"],
+                                [i, n]
                             ],
                             [/(kin\.[onetw]{3})/i],
                             [
-                                [t, /\./g, " "],
-                                [u, "Microsoft"],
-                                [n, c]
+                                [o, /\./g, " "],
+                                [s, "Microsoft"],
+                                [i, u]
                             ],
                             [/\s(milestone|droid(?:[2-4x]|\s(?:bionic|x2|pro|razr))?:?(\s4g)?)[\w\s]+build\//i, /mot[\s-]?(\w*)/i, /(XT\d{3,4}) build\//i, /(nexus\s6)/i],
-                            [t, [u, "Motorola"],
-                                [n, c]
+                            [o, [s, "Motorola"],
+                                [i, u]
                             ],
                             [/android.+\s(mz60\d|xoom[\s2]{0,2})\sbuild\//i],
-                            [t, [u, "Motorola"],
-                                [n, g]
+                            [o, [s, "Motorola"],
+                                [i, d]
                             ],
                             [/hbbtv\/\d+\.\d+\.\d+\s+\([\w\s]*;\s*(\w[^;]*);([^;]*)/i],
                             [
-                                [u, h.trim],
-                                [t, h.trim],
-                                [n, m]
+                                [s, m.trim],
+                                [o, m.trim],
+                                [i, c]
                             ],
                             [/hbbtv.+maple;(\d+)/i],
                             [
-                                [t, /^/, "SmartTV"],
-                                [u, "Samsung"],
-                                [n, m]
+                                [o, /^/, "SmartTV"],
+                                [s, "Samsung"],
+                                [i, c]
                             ],
                             [/\(dtv[\);].+(aquos)/i],
-                            [t, [u, "Sharp"],
-                                [n, m]
+                            [o, [s, "Sharp"],
+                                [i, c]
                             ],
                             [/android.+((sch-i[89]0\d|shw-m380s|gt-p\d{4}|gt-n\d+|sgh-t8[56]9|nexus 10))/i, /((SM-T\w+))/i],
                             [
-                                [u, "Samsung"], t, [n, g]
+                                [s, "Samsung"], o, [i, d]
                             ],
                             [/smart-tv.+(samsung)/i],
-                            [u, [n, m], t],
+                            [s, [i, c], o],
                             [/((s[cgp]h-\w+|gt-\w+|galaxy\snexus|sm-\w[\w\d]+))/i, /(sam[sung]*)[\s-]*(\w+-?[\w-]*)/i, /sec-((sgh\w+))/i],
                             [
-                                [u, "Samsung"], t, [n, c]
+                                [s, "Samsung"], o, [i, u]
                             ],
                             [/sie-(\w*)/i],
-                            [t, [u, "Siemens"],
-                                [n, c]
+                            [o, [s, "Siemens"],
+                                [i, u]
                             ],
                             [/(maemo|nokia).*(n900|lumia\s\d+)/i, /(nokia)[\s_-]?([\w-]*)/i],
                             [
-                                [u, "Nokia"], t, [n, c]
+                                [s, "Nokia"], o, [i, u]
                             ],
                             [/android[x\d\.\s;]+\s([ab][1-7]\-?[0178a]\d\d?)/i],
-                            [t, [u, "Acer"],
-                                [n, g]
+                            [o, [s, "Acer"],
+                                [i, d]
                             ],
                             [/android.+([vl]k\-?\d{3})\s+build/i],
-                            [t, [u, "LG"],
-                                [n, g]
+                            [o, [s, "LG"],
+                                [i, d]
                             ],
                             [/android\s3\.[\s\w;-]{10}(lg?)-([06cv9]{3,4})/i],
                             [
-                                [u, "LG"], t, [n, g]
+                                [s, "LG"], o, [i, d]
                             ],
                             [/(lg) netcast\.tv/i],
-                            [u, t, [n, m]],
+                            [s, o, [i, c]],
                             [/(nexus\s[45])/i, /lg[e;\s\/-]+(\w*)/i, /android.+lg(\-?[\d\w]+)\s+build/i],
-                            [t, [u, "LG"],
-                                [n, c]
+                            [o, [s, "LG"],
+                                [i, u]
                             ],
                             [/(lenovo)\s?(s(?:5000|6000)(?:[\w-]+)|tab(?:[\s\w]+))/i],
-                            [u, t, [n, g]],
+                            [s, o, [i, d]],
                             [/android.+(ideatab[a-z0-9\-\s]+)/i],
-                            [t, [u, "Lenovo"],
-                                [n, g]
+                            [o, [s, "Lenovo"],
+                                [i, d]
                             ],
                             [/(lenovo)[_\s-]?([\w-]+)/i],
-                            [u, t, [n, c]],
+                            [s, o, [i, u]],
                             [/linux;.+((jolla));/i],
-                            [u, t, [n, c]],
+                            [s, o, [i, u]],
                             [/((pebble))app\/[\d\.]+\s/i],
-                            [u, t, [n, b]],
+                            [s, o, [i, g]],
                             [/android.+;\s(oppo)\s?([\w\s]+)\sbuild/i],
-                            [u, t, [n, c]],
+                            [s, o, [i, u]],
                             [/crkey/i],
                             [
-                                [t, "Chromecast"],
-                                [u, "Google"],
-                                [n, m]
+                                [o, "Chromecast"],
+                                [s, "Google"],
+                                [i, c]
                             ],
                             [/android.+;\s(glass)\s\d/i],
-                            [t, [u, "Google"],
-                                [n, b]
+                            [o, [s, "Google"],
+                                [i, g]
                             ],
                             [/android.+;\s(pixel c)[\s)]/i],
-                            [t, [u, "Google"],
-                                [n, g]
+                            [o, [s, "Google"],
+                                [i, d]
                             ],
                             [/android.+;\s(pixel( [23])?( xl)?)[\s)]/i],
-                            [t, [u, "Google"],
-                                [n, c]
+                            [o, [s, "Google"],
+                                [i, u]
                             ],
                             [/android.+;\s(\w+)\s+build\/hm\1/i, /android.+(hm[\s\-_]*note?[\s_]*(?:\d\w)?)\s+build/i, /android.+(mi[\s\-_]*(?:a\d|one|one[\s_]plus|note lte)?[\s_]*(?:\d?\w?)[\s_]*(?:plus)?)\s+build/i, /android.+(redmi[\s\-_]*(?:note)?(?:[\s_]?[\w\s]+))\s+build/i],
                             [
-                                [t, /_/g, " "],
-                                [u, "Xiaomi"],
-                                [n, c]
+                                [o, /_/g, " "],
+                                [s, "Xiaomi"],
+                                [i, u]
                             ],
                             [/android.+(mi[\s\-_]*(?:pad)(?:[\s_]?[\w\s]+))\s+build/i],
                             [
-                                [t, /_/g, " "],
-                                [u, "Xiaomi"],
-                                [n, g]
+                                [o, /_/g, " "],
+                                [s, "Xiaomi"],
+                                [i, d]
                             ],
                             [/android.+;\s(m[1-5]\snote)\sbuild/i],
-                            [t, [u, "Meizu"],
-                                [n, c]
+                            [o, [s, "Meizu"],
+                                [i, u]
                             ],
                             [/(mz)-([\w-]{2,})/i],
                             [
-                                [u, "Meizu"], t, [n, c]
+                                [s, "Meizu"], o, [i, u]
                             ],
                             [/android.+a000(1)\s+build/i, /android.+oneplus\s(a\d{4})[\s)]/i],
-                            [t, [u, "OnePlus"],
-                                [n, c]
+                            [o, [s, "OnePlus"],
+                                [i, u]
                             ],
                             [/android.+[;\/]\s*(RCT[\d\w]+)\s+build/i],
-                            [t, [u, "RCA"],
-                                [n, g]
+                            [o, [s, "RCA"],
+                                [i, d]
                             ],
                             [/android.+[;\/\s]+(Venue[\d\s]{2,7})\s+build/i],
-                            [t, [u, "Dell"],
-                                [n, g]
+                            [o, [s, "Dell"],
+                                [i, d]
                             ],
                             [/android.+[;\/]\s*(Q[T|M][\d\w]+)\s+build/i],
-                            [t, [u, "Verizon"],
-                                [n, g]
+                            [o, [s, "Verizon"],
+                                [i, d]
                             ],
                             [/android.+[;\/]\s+(Barnes[&\s]+Noble\s+|BN[RT])(V?.*)\s+build/i],
                             [
-                                [u, "Barnes & Noble"], t, [n, g]
+                                [s, "Barnes & Noble"], o, [i, d]
                             ],
                             [/android.+[;\/]\s+(TM\d{3}.*\b)\s+build/i],
-                            [t, [u, "NuVision"],
-                                [n, g]
+                            [o, [s, "NuVision"],
+                                [i, d]
                             ],
                             [/android.+;\s(k88)\sbuild/i],
-                            [t, [u, "ZTE"],
-                                [n, g]
+                            [o, [s, "ZTE"],
+                                [i, d]
                             ],
                             [/android.+[;\/]\s*(gen\d{3})\s+build.*49h/i],
-                            [t, [u, "Swiss"],
-                                [n, c]
+                            [o, [s, "Swiss"],
+                                [i, u]
                             ],
                             [/android.+[;\/]\s*(zur\d{3})\s+build/i],
-                            [t, [u, "Swiss"],
-                                [n, g]
+                            [o, [s, "Swiss"],
+                                [i, d]
                             ],
                             [/android.+[;\/]\s*((Zeki)?TB.*\b)\s+build/i],
-                            [t, [u, "Zeki"],
-                                [n, g]
+                            [o, [s, "Zeki"],
+                                [i, d]
                             ],
                             [/(android).+[;\/]\s+([YR]\d{2})\s+build/i, /android.+[;\/]\s+(Dragon[\-\s]+Touch\s+|DT)(\w{5})\sbuild/i],
                             [
-                                [u, "Dragon Touch"], t, [n, g]
+                                [s, "Dragon Touch"], o, [i, d]
                             ],
                             [/android.+[;\/]\s*(NS-?\w{0,9})\sbuild/i],
-                            [t, [u, "Insignia"],
-                                [n, g]
+                            [o, [s, "Insignia"],
+                                [i, d]
                             ],
                             [/android.+[;\/]\s*((NX|Next)-?\w{0,9})\s+build/i],
-                            [t, [u, "NextBook"],
-                                [n, g]
+                            [o, [s, "NextBook"],
+                                [i, d]
                             ],
                             [/android.+[;\/]\s*(Xtreme\_)?(V(1[045]|2[015]|30|40|60|7[05]|90))\s+build/i],
                             [
-                                [u, "Voice"], t, [n, c]
+                                [s, "Voice"], o, [i, u]
                             ],
                             [/android.+[;\/]\s*(LVTEL\-)?(V1[12])\s+build/i],
                             [
-                                [u, "LvTel"], t, [n, c]
+                                [s, "LvTel"], o, [i, u]
                             ],
                             [/android.+;\s(PH-1)\s/i],
-                            [t, [u, "Essential"],
-                                [n, c]
+                            [o, [s, "Essential"],
+                                [i, u]
                             ],
                             [/android.+[;\/]\s*(V(100MD|700NA|7011|917G).*\b)\s+build/i],
-                            [t, [u, "Envizen"],
-                                [n, g]
+                            [o, [s, "Envizen"],
+                                [i, d]
                             ],
                             [/android.+[;\/]\s*(Le[\s\-]+Pan)[\s\-]+(\w{1,9})\s+build/i],
-                            [u, t, [n, g]],
+                            [s, o, [i, d]],
                             [/android.+[;\/]\s*(Trio[\s\-]*.*)\s+build/i],
-                            [t, [u, "MachSpeed"],
-                                [n, g]
+                            [o, [s, "MachSpeed"],
+                                [i, d]
                             ],
                             [/android.+[;\/]\s*(Trinity)[\-\s]*(T\d{3})\s+build/i],
-                            [u, t, [n, g]],
+                            [s, o, [i, d]],
                             [/android.+[;\/]\s*TU_(1491)\s+build/i],
-                            [t, [u, "Rotor"],
-                                [n, g]
+                            [o, [s, "Rotor"],
+                                [i, d]
                             ],
                             [/android.+(KS(.+))\s+build/i],
-                            [t, [u, "Amazon"],
-                                [n, g]
+                            [o, [s, "Amazon"],
+                                [i, d]
                             ],
                             [/android.+(Gigaset)[\s\-]+(Q\w{1,9})\s+build/i],
-                            [u, t, [n, g]],
+                            [s, o, [i, d]],
                             [/\s(tablet|tab)[;\/]/i, /\s(mobile)(?:[;\/]|\ssafari)/i],
                             [
-                                [n, h.lowerize], u, t
+                                [i, m.lowerize], s, o
                             ],
                             [/[\s\/\(](smart-?tv)[;\)]/i],
                             [
-                                [n, m]
+                                [i, c]
                             ],
                             [/(android[\w\.\s\-]{0,9});.+build/i],
-                            [t, [u, "Generic"]]
+                            [o, [s, "Generic"]]
                         ],
                         engine: [
                             [/windows.+\sedge\/([\w\.]+)/i],
-                            [d, [l, "EdgeHTML"]],
+                            [t, [r, "EdgeHTML"]],
                             [/webkit\/537\.36.+chrome\/(?!27)([\w\.]+)/i],
-                            [d, [l, "Blink"]],
+                            [t, [r, "Blink"]],
                             [/(presto)\/([\w\.]+)/i, /(webkit|trident|netfront|netsurf|amaya|lynx|w3m|goanna)\/([\w\.]+)/i, /(khtml|tasman|links)[\/\s]\(?([\w\.]+)/i, /(icab)[\/\s]([23]\.[\d\.]+)/i],
-                            [l, d],
+                            [r, t],
                             [/rv\:([\w\.]{1,9}).+(gecko)/i],
-                            [d, l]
+                            [t, r]
                         ],
                         os: [
                             [/microsoft\s(windows)\s(vista|xp)/i],
-                            [l, d],
+                            [r, t],
                             [/(windows)\snt\s6\.2;\s(arm)/i, /(windows\sphone(?:\sos)*)[\s\/]?([\d\.\s\w]*)/i, /(windows\smobile|windows)[\s\/]?([ntce\d\.\s]+\w)/i],
-                            [l, [d, f.str, v.os.windows.version]],
+                            [r, [t, b.str, h.os.windows.version]],
                             [/(win(?=3|9|n)|win\s9x\s)([nt\d\.]+)/i],
                             [
-                                [l, "Windows"],
-                                [d, f.str, v.os.windows.version]
+                                [r, "Windows"],
+                                [t, b.str, h.os.windows.version]
                             ],
                             [/\((bb)(10);/i],
                             [
-                                [l, "BlackBerry"], d
+                                [r, "BlackBerry"], t
                             ],
                             [/(blackberry)\w*\/?([\w\.]*)/i, /(tizen|kaios)[\/\s]([\w\.]+)/i, /(android|webos|palm\sos|qnx|bada|rim\stablet\sos|meego|sailfish|contiki)[\/\s-]?([\w\.]*)/i],
-                            [l, d],
+                            [r, t],
                             [/(symbian\s?os|symbos|s60(?=;))[\/\s-]?([\w\.]*)/i],
                             [
-                                [l, "Symbian"], d
+                                [r, "Symbian"], t
                             ],
                             [/\((series40);/i],
-                            [l],
+                            [r],
                             [/mozilla.+\(mobile;.+gecko.+firefox/i],
                             [
-                                [l, "Firefox OS"], d
+                                [r, "Firefox OS"], t
                             ],
                             [/(nintendo|playstation)\s([wids34portablevu]+)/i, /(mint)[\/\s\(]?(\w*)/i, /(mageia|vectorlinux)[;\s]/i, /(joli|[kxln]?ubuntu|debian|suse|opensuse|gentoo|(?=\s)arch|slackware|fedora|mandriva|centos|pclinuxos|redhat|zenwalk|linpus)[\/\s-]?(?!chrom)([\w\.-]*)/i, /(hurd|linux)\s?([\w\.]*)/i, /(gnu)\s?([\w\.]*)/i],
-                            [l, d],
+                            [r, t],
                             [/(cros)\s[\w]+\s([\w\.]+\w)/i],
                             [
-                                [l, "Chromium OS"], d
+                                [r, "Chromium OS"], t
                             ],
                             [/(sunos)\s?([\w\.\d]*)/i],
                             [
-                                [l, "Solaris"], d
+                                [r, "Solaris"], t
                             ],
                             [/\s([frentopc-]{0,4}bsd|dragonfly)\s?([\w\.]*)/i],
-                            [l, d],
+                            [r, t],
                             [/(haiku)\s(\w+)/i],
-                            [l, d],
+                            [r, t],
                             [/cfnetwork\/.+darwin/i, /ip[honead]{2,4}(?:.*os\s([\w]+)\slike\smac|;\sopera)/i],
                             [
-                                [d, /_/g, "."],
-                                [l, "iOS"]
+                                [t, /_/g, "."],
+                                [r, "iOS"]
                             ],
                             [/(mac\sos\sx)\s?([\w\s\.]*)/i, /(macintosh|mac(?=_powerpc)\s)/i],
                             [
-                                [l, "Mac OS"],
-                                [d, /_/g, "."]
+                                [r, "Mac OS"],
+                                [t, /_/g, "."]
                             ],
                             [/((?:open)?solaris)[\/\s-]?([\w\.]*)/i, /(aix)\s((\d)(?=\.|\)|\s)[\w\.])*/i, /(plan\s9|minix|beos|os\/2|amigaos|morphos|risc\sos|openvms|fuchsia)/i, /(unix)\s?([\w\.]*)/i],
-                            [l, d]
+                            [r, t]
                         ]
                     },
-                    S = function(o, r) {
-                        if ("object" == typeof o && (r = o, o = i), !(this instanceof S)) return new S(o, r).getResult();
-                        var a = o || (e && e.navigator && e.navigator.userAgent ? e.navigator.userAgent : ""),
-                            s = r ? h.extend(y, r) : y;
+                    v = function(e, o) {
+                        if ("object" == typeof e && (o = e, e = p), !(this instanceof v)) return new v(e, o).getResult();
+                        var r = e || (a && a.navigator && a.navigator.userAgent ? a.navigator.userAgent : ""),
+                            i = o ? m.extend(f, o) : f;
                         return this.getBrowser = function() {
                             var e = {
-                                name: i,
-                                version: i
+                                name: p,
+                                version: p
                             };
-                            return f.rgx.call(e, a, s.browser), e.major = h.major(e.version), e
+                            return b.rgx.call(e, r, i.browser), e.major = m.major(e.version), e
                         }, this.getCPU = function() {
                             var e = {
-                                architecture: i
+                                architecture: p
                             };
-                            return f.rgx.call(e, a, s.cpu), e
+                            return b.rgx.call(e, r, i.cpu), e
                         }, this.getDevice = function() {
                             var e = {
-                                vendor: i,
-                                model: i,
-                                type: i
+                                vendor: p,
+                                model: p,
+                                type: p
                             };
-                            return f.rgx.call(e, a, s.device), e
+                            return b.rgx.call(e, r, i.device), e
                         }, this.getEngine = function() {
                             var e = {
-                                name: i,
-                                version: i
+                                name: p,
+                                version: p
                             };
-                            return f.rgx.call(e, a, s.engine), e
+                            return b.rgx.call(e, r, i.engine), e
                         }, this.getOS = function() {
                             var e = {
-                                name: i,
-                                version: i
+                                name: p,
+                                version: p
                             };
-                            return f.rgx.call(e, a, s.os), e
+                            return b.rgx.call(e, r, i.os), e
                         }, this.getResult = function() {
                             return {
                                 ua: this.getUA(),
                                 browser: this.getBrowser(),
                                 engine: this.getEngine(),
                                 os: this.getOS(),
                                 device: this.getDevice(),
                                 cpu: this.getCPU()
                             }
                         }, this.getUA = function() {
-                            return a
+                            return r
                         }, this.setUA = function(e) {
-                            return a = e, this
+                            return r = e, this
                         }, this
                     };
-                S.VERSION = "0.7.22", S.BROWSER = {
-                    NAME: l,
+                v.VERSION = "0.7.22", v.BROWSER = {
+                    NAME: r,
                     MAJOR: "major",
-                    VERSION: d
-                }, S.CPU = {
-                    ARCHITECTURE: p
-                }, S.DEVICE = {
-                    MODEL: t,
-                    VENDOR: u,
-                    TYPE: n,
-                    CONSOLE: w,
-                    MOBILE: c,
-                    SMARTTV: m,
-                    TABLET: g,
-                    WEARABLE: b,
+                    VERSION: t
+                }, v.CPU = {
+                    ARCHITECTURE: l
+                }, v.DEVICE = {
+                    MODEL: o,
+                    VENDOR: s,
+                    TYPE: i,
+                    CONSOLE: n,
+                    MOBILE: u,
+                    SMARTTV: c,
+                    TABLET: d,
+                    WEARABLE: g,
                     EMBEDDED: "embedded"
-                }, S.ENGINE = {
-                    NAME: l,
-                    VERSION: d
-                }, S.OS = {
-                    NAME: l,
-                    VERSION: d
-                }, typeof r != s ? (typeof o != s && o.exports && (r = o.exports = S), r.UAParser = S) : e && (e.UAParser = S);
-                var k, A = e && (e.jQuery || e.Zepto);
-                A && !A.ua && (k = new S, A.ua = k.getResult(), A.ua.get = function() {
-                    return k.getUA()
-                }, A.ua.set = function(e) {
-                    k.setUA(e);
-                    var o, r = k.getResult();
-                    for (o in r) A.ua[o] = r[o]
+                }, v.ENGINE = {
+                    NAME: r,
+                    VERSION: t
+                }, v.OS = {
+                    NAME: r,
+                    VERSION: t
+                }, typeof A != e ? (typeof k != e && k.exports && (A = k.exports = v), A.UAParser = v) : a && (a.UAParser = v);
+                var y, S = a && (a.jQuery || a.Zepto);
+                S && !S.ua && (y = new v, S.ua = y.getResult(), S.ua.get = function() {
+                    return y.getUA()
+                }, S.ua.set = function(e) {
+                    y.setUA(e);
+                    var o, r = y.getResult();
+                    for (o in r) S.ua[o] = r[o]
                 })
             }("object" == typeof window ? window : this)
         }, {}]
     }, {}, [3])(3)
-}));
+});
```

### Comparing `buildbot-www-react-3.7.0/buildbot_www_react/static/icon.png` & `buildbot-www-react-3.8.0/buildbot_www_react/static/icon.png`

 * *Files identical despite different names*

### Comparing `buildbot-www-react-3.7.0/buildbot_www_react/static/icon.svg` & `buildbot-www-react-3.8.0/buildbot_www_react/static/icon.svg`

 * *Files identical despite different names*

### Comparing `buildbot-www-react-3.7.0/setup.py` & `buildbot-www-react-3.8.0/setup.py`

 * *Files identical despite different names*

